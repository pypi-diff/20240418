# Comparing `tmp/hich_restrict-0.1.3-py3-none-any.whl.zip` & `tmp/hich_restrict-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6919 bytes, number of entries: 10
+Zip file size: 7001 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 hich_restrict/__init__.py
--rw-r--r--  2.0 unx     1331 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
+-rw-r--r--  2.0 unx     1447 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
 -rw-r--r--  2.0 unx     4202 b- defN 80-Jan-01 00:00 hich_restrict/contacts.py
 -rw-r--r--  2.0 unx     4343 b- defN 80-Jan-01 00:00 hich_restrict/fragments.py
--rw-r--r--  2.0 unx     3761 b- defN 80-Jan-01 00:00 hich_restrict/restrict_manager.py
+-rw-r--r--  2.0 unx     3942 b- defN 80-Jan-01 00:00 hich_restrict/restrict_manager.py
 -rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 hich_restrict/timer.py
--rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.3.dist-info/RECORD
-10 files, 16338 bytes uncompressed, 5515 bytes compressed:  66.2%
+-rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.4.dist-info/RECORD
+10 files, 16635 bytes uncompressed, 5597 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: hich_restrict/restrict_manager.py
 Comment: 
 
 Filename: hich_restrict/timer.py
 Comment: 
 
-Filename: hich_restrict-0.1.3.dist-info/METADATA
+Filename: hich_restrict-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: hich_restrict-0.1.3.dist-info/WHEEL
+Filename: hich_restrict-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: hich_restrict-0.1.3.dist-info/entry_points.txt
+Filename: hich_restrict-0.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: hich_restrict-0.1.3.dist-info/RECORD
+Filename: hich_restrict-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hich_restrict/__main__.py

```diff
@@ -27,12 +27,16 @@
 
     input-pairs: a text file containing pairs in .pairs format. Can be
     plaintext or compressed with gzip (.gz, .gzip) or lz4 (.lz4).
     """
     cmd = ' '.join(sys.argv)
     rm = RestrictManager()
     rm.setup(cmd, frag_file_format, output_pairs, frag_file, input_pairs)
+    start = time.time()
     rm.tag()
+    end = time.time()
+    duration = end - start
+    print(f"Tag duration (s): {duration}")
 
 
 if __name__ == "__main__":
     cli()
```

## hich_restrict/restrict_manager.py

```diff
@@ -36,14 +36,15 @@
         file = None
         compress = False
         if self.output_pairs:
             file = autodetect_open(self.output_pairs, 'wb')
             compress = detect_compression(self.output_pairs)
         
         buffer = []
+        wrote_first = False
         # Tag contacts and save
         for fields, line in self.contacts:
             if fields is not None:
                 frag1 = self.frag_finder.find(fields['chrom1'], int(fields['pos1']))
                 frag2 = self.frag_finder.find(fields['chrom2'], int(fields['pos2']))
                 frag_tag = "\t".join([str(s) for s in frag1+frag2])
                 new_line = f"{line.strip()}\t{frag_tag}\n"
@@ -51,20 +52,23 @@
                 new_line = line
             if not file:
                 click.echo(new_line.strip())
             else:
                 buffer.append(new_line.strip())
                 if len(buffer) >= buffer_size:
                     out = '\n'.join(buffer)
+                    out = '\n' + out if wrote_first else out
                     out = out.encode('utf-8') if compress else out
                     file.write(out)
                     buffer = []
+                    wrote_first = True
 
         if file:
             out = '\n'.join(buffer)
+            out = '\n' + out if wrote_first else out
             out = out.encode('utf-8') if compress else out
             file.write(out)
             file.close()
             
 
     def frag_reader(self, frag_file_format, frag_file):
         # Determine what reader to use based on user-specified parameters
```

## Comparing `hich_restrict-0.1.3.dist-info/RECORD` & `hich_restrict-0.1.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 hich_restrict/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hich_restrict/__main__.py,sha256=Qy6eE7SYZv7brHAvm-fRzwRqV7vqmxlLRfF9bIDESy4,1331
+hich_restrict/__main__.py,sha256=UrHTjLbNSw8UQCGW1-PF7BV_6hyg6lF5Kiy7j0Y4GMg,1447
 hich_restrict/contacts.py,sha256=088NMTKygzd43V2vPlkfj3_Fzybw04YIBInUoVWd0BM,4202
 hich_restrict/fragments.py,sha256=oY7ceSjTIYauV1gElRvKrnF1LCJqwfNr7VqcfIvmNZ8,4343
-hich_restrict/restrict_manager.py,sha256=M2Ll_VylhjRhUSWcRxibpTnw78__rDc6oVosm3T28go,3761
+hich_restrict/restrict_manager.py,sha256=WaR7n3EtHJAhvN2oHceLstVGBjdWS-62jxCjCdWt_20,3942
 hich_restrict/timer.py,sha256=VhkDub_yc5dQmXwHfKRQjFuFD_S64bpMl9akkSbNrOA,1289
-hich_restrict-0.1.3.dist-info/METADATA,sha256=tpN5yYDZaG3EsuLirJ3wVux6H8U672OsiUwU4xhABD4,445
-hich_restrict-0.1.3.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-hich_restrict-0.1.3.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
-hich_restrict-0.1.3.dist-info/RECORD,,
+hich_restrict-0.1.4.dist-info/METADATA,sha256=K4VdyFWs1r6KU0zalWJZbdqW7E1y9bcvrE1_1h57Vn0,445
+hich_restrict-0.1.4.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+hich_restrict-0.1.4.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
+hich_restrict-0.1.4.dist-info/RECORD,,
```

