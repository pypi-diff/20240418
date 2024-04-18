# Comparing `tmp/hich_restrict-0.1.4-py3-none-any.whl.zip` & `tmp/hich_restrict-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7001 bytes, number of entries: 10
+Zip file size: 7495 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 hich_restrict/__init__.py
--rw-r--r--  2.0 unx     1447 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
+-rw-r--r--  2.0 unx     2508 b- defN 80-Jan-01 00:00 hich_restrict/__main__.py
 -rw-r--r--  2.0 unx     4202 b- defN 80-Jan-01 00:00 hich_restrict/contacts.py
 -rw-r--r--  2.0 unx     4343 b- defN 80-Jan-01 00:00 hich_restrict/fragments.py
 -rw-r--r--  2.0 unx     3942 b- defN 80-Jan-01 00:00 hich_restrict/restrict_manager.py
 -rw-r--r--  2.0 unx     1289 b- defN 80-Jan-01 00:00 hich_restrict/timer.py
--rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.4.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.4.dist-info/RECORD
-10 files, 16635 bytes uncompressed, 5597 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx      445 b- defN 80-Jan-01 00:00 hich_restrict-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 hich_restrict-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 80-Jan-01 00:00 hich_restrict-0.1.5.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      819 b- defN 16-Jan-01 00:00 hich_restrict-0.1.5.dist-info/RECORD
+10 files, 17696 bytes uncompressed, 6091 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: hich_restrict/restrict_manager.py
 Comment: 
 
 Filename: hich_restrict/timer.py
 Comment: 
 
-Filename: hich_restrict-0.1.4.dist-info/METADATA
+Filename: hich_restrict-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: hich_restrict-0.1.4.dist-info/WHEEL
+Filename: hich_restrict-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: hich_restrict-0.1.4.dist-info/entry_points.txt
+Filename: hich_restrict-0.1.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: hich_restrict-0.1.4.dist-info/RECORD
+Filename: hich_restrict-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hich_restrict/__main__.py

```diff
@@ -14,15 +14,15 @@
 @click.option("--output-pairs",
     type=str,
     help="Filename for output .pairs file")
 @click.argument("frag-file")
 @click.argument("input-pairs")
 def cli(frag_file_format, output_pairs, frag_file, input_pairs):
     """
-    hich-restrict v 0.1.3
+    hich-restrict v 0.1.5
     
     frag-file: a non-compressed plaintext file containing fragments. All
     fragments from a particular chromosome must be in one contiguous block,
     with ascending coordinates. All fragments in a chromosome must be
     adjacent (frag_n start = frag_n-1 end + 1).
 
     input-pairs: a text file containing pairs in .pairs format. Can be
@@ -33,10 +33,27 @@
     rm.setup(cmd, frag_file_format, output_pairs, frag_file, input_pairs)
     start = time.time()
     rm.tag()
     end = time.time()
     duration = end - start
     print(f"Tag duration (s): {duration}")
 
+    # My current speed is about 4k reads/s which means a 400M read .pairs file
+    # takes over a day to tag, roughly fitting what we get on exacloud.
+    # The main issue is that loading the restriction fragments into memory
+    # takes 5 Gb, but the runtime is bottlenecked by the search, so
+    # to parallelize that it would require multiprocessing where each process
+    # utilizes 5 Gb of memory, and currently we are achieving that by just
+    # tagging all the files at the same time.
+    # 
+    # Improving performance would require splitting restriction fragments over
+    # multiple processes. One way we could do that is by splitting up the
+    # restriction fragments by chromosomes (or by position within chroms)
+    # and assigning one process per interval. Pairs would be fed into the
+    # appropriate process in batches, multiprocessed, and then rejoined
+    #
+    # However, it is probably not hard for people to just request more memory
+    # and accept an extra day of processing time. So I'm not convinced this
+    # is high-priority yet.
 
 if __name__ == "__main__":
     cli()
```

## Comparing `hich_restrict-0.1.4.dist-info/RECORD` & `hich_restrict-0.1.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 hich_restrict/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-hich_restrict/__main__.py,sha256=UrHTjLbNSw8UQCGW1-PF7BV_6hyg6lF5Kiy7j0Y4GMg,1447
+hich_restrict/__main__.py,sha256=7oznp6nx4_XtON0DAF4sZDxYHTvZL6_rADyNc0831aQ,2508
 hich_restrict/contacts.py,sha256=088NMTKygzd43V2vPlkfj3_Fzybw04YIBInUoVWd0BM,4202
 hich_restrict/fragments.py,sha256=oY7ceSjTIYauV1gElRvKrnF1LCJqwfNr7VqcfIvmNZ8,4343
 hich_restrict/restrict_manager.py,sha256=WaR7n3EtHJAhvN2oHceLstVGBjdWS-62jxCjCdWt_20,3942
 hich_restrict/timer.py,sha256=VhkDub_yc5dQmXwHfKRQjFuFD_S64bpMl9akkSbNrOA,1289
-hich_restrict-0.1.4.dist-info/METADATA,sha256=K4VdyFWs1r6KU0zalWJZbdqW7E1y9bcvrE1_1h57Vn0,445
-hich_restrict-0.1.4.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-hich_restrict-0.1.4.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
-hich_restrict-0.1.4.dist-info/RECORD,,
+hich_restrict-0.1.5.dist-info/METADATA,sha256=ybc20PVjdqPOhOFRNVh4mVZxyX-pMr01Rr8-6MRaZx8,445
+hich_restrict-0.1.5.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+hich_restrict-0.1.5.dist-info/entry_points.txt,sha256=gO9fXm7Uq94XUtbPUFzStNx2VxM8N-JfSK8hBqaBiZU,60
+hich_restrict-0.1.5.dist-info/RECORD,,
```

