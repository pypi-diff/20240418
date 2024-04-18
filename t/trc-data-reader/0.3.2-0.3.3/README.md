# Comparing `tmp/trc_data_reader-0.3.2-py3-none-any.whl.zip` & `tmp/trc_data_reader-0.3.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10364 bytes, number of entries: 6
--rw-r--r--  2.0 unx    15650 b- defN 24-Apr-04 16:48 trc.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-04 16:49 trc_data_reader-0.3.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1453 b- defN 24-Apr-04 16:49 trc_data_reader-0.3.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 16:49 trc_data_reader-0.3.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-04 16:49 trc_data_reader-0.3.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      490 b- defN 24-Apr-04 16:49 trc_data_reader-0.3.2.dist-info/RECORD
-6 files, 29046 bytes uncompressed, 9476 bytes compressed:  67.4%
+Zip file size: 10372 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    15713 b- defN 24-Apr-18 03:32 trc.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1453 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      490 b- defN 24-Apr-18 03:32 trc_data_reader-0.3.3.dist-info/RECORD
+6 files, 29109 bytes uncompressed, 9484 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: trc.py
 Comment: 
 
-Filename: trc_data_reader-0.3.2.dist-info/LICENSE
+Filename: trc_data_reader-0.3.3.dist-info/LICENSE
 Comment: 
 
-Filename: trc_data_reader-0.3.2.dist-info/METADATA
+Filename: trc_data_reader-0.3.3.dist-info/METADATA
 Comment: 
 
-Filename: trc_data_reader-0.3.2.dist-info/WHEEL
+Filename: trc_data_reader-0.3.3.dist-info/WHEEL
 Comment: 
 
-Filename: trc_data_reader-0.3.2.dist-info/top_level.txt
+Filename: trc_data_reader-0.3.3.dist-info/top_level.txt
 Comment: 
 
-Filename: trc_data_reader-0.3.2.dist-info/RECORD
+Filename: trc_data_reader-0.3.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trc.py

```diff
@@ -196,21 +196,21 @@
             self['DataRate'] = reader.header.frame_rate
             self['CameraRate'] = reader.header.frame_rate
             self['NumFrames'] = reader.header.last_frame
             self['NumMarkers'] = reader.get('POINT').get('USED').int16_value
             self['Units'] = reader.get('POINT').get('UNITS').string_value
             self['OrigDataRate'] = reader.header.frame_rate
             self['OrigDataStartFrame'] = reader.header.first_frame
-            self['OrigNumFrames'] = reader.header.last_frame
+            self['OrigNumFrames'] = reader.header.last_frame - reader.header.first_frame + 1
 
             # Set data column labels.
             self['Markers'] = [label.strip() for label in reader.point_labels]
 
             # Set frame numbers.
-            self['Frame#'] = [i for i in range(1, self['NumFrames'] + 1)]
+            self['Frame#'] = [i for i in range(reader.header.first_frame, reader.header.last_frame + 1)]
 
             # Set marker data.
             for i, points, analog in reader.read_frames():
                 time = (i - 1) * (1 / reader.point_rate)
                 self[i] = time, [point[:3].tolist() for point in points]
 
     def import_from(self, filename):
```

## Comparing `trc_data_reader-0.3.2.dist-info/LICENSE` & `trc_data_reader-0.3.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `trc_data_reader-0.3.2.dist-info/METADATA` & `trc_data_reader-0.3.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trc-data-reader
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package for reading track row column (trc) motion capture data.
 Home-page: https://github.com/hsorby/trc-data-reader
 Author: Hugh Sorby
 Author-email: h.sorby@auckland.ac.nz
 License: Apache 2.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

