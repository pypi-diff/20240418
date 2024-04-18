# Comparing `tmp/lense-0.0.2-py3-none-any.whl.zip` & `tmp/lense-0.0.57-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,8 @@
-Zip file size: 7865 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat       24 b- defN 24-Apr-11 09:48 lense/__init__.py
--rw-rw-rw-  2.0 fat      455 b- defN 24-Apr-15 12:02 lense/app.py
--rw-rw-rw-  2.0 fat        0 b- defN 24-Apr-11 06:48 lense/_chat/__init__.py
--rw-rw-rw-  2.0 fat     1173 b- defN 24-Apr-15 11:44 lense/_chat/cglense.py
--rw-rw-rw-  2.0 fat     6653 b- defN 24-Apr-15 11:55 lense/_chat/engine.py
--rw-rw-rw-  2.0 fat     4850 b- defN 24-Apr-15 11:45 lense/_chat/error_handling.py
--rw-rw-rw-  2.0 fat     4179 b- defN 24-Apr-15 11:48 lense/_chat/loader.py
--rw-rw-rw-  2.0 fat      519 b- defN 24-Apr-15 11:45 lense/_chat/replace_file.py
--rw-rw-rw-  2.0 fat      653 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      909 b- defN 24-Apr-16 05:24 lense-0.0.2.dist-info/RECORD
-12 files, 19513 bytes uncompressed, 6347 bytes compressed:  67.5%
+Zip file size: 1726 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-17 09:56 lense/__init__.py
+-rw-rw-rw-  2.0 fat     1075 b- defN 24-Apr-18 10:55 lense/main.py
+-rw-rw-rw-  2.0 fat      103 b- defN 24-Apr-18 10:57 lense-0.0.57.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 10:57 lense-0.0.57.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-18 10:57 lense-0.0.57.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      434 b- defN 24-Apr-18 10:57 lense-0.0.57.dist-info/RECORD
+6 files, 1733 bytes uncompressed, 940 bytes compressed:  45.8%
```

## zipnote {}

```diff
@@ -1,37 +1,19 @@
 Filename: lense/__init__.py
 Comment: 
 
-Filename: lense/app.py
+Filename: lense/main.py
 Comment: 
 
-Filename: lense/_chat/__init__.py
+Filename: lense-0.0.57.dist-info/METADATA
 Comment: 
 
-Filename: lense/_chat/cglense.py
+Filename: lense-0.0.57.dist-info/WHEEL
 Comment: 
 
-Filename: lense/_chat/engine.py
+Filename: lense-0.0.57.dist-info/top_level.txt
 Comment: 
 
-Filename: lense/_chat/error_handling.py
-Comment: 
-
-Filename: lense/_chat/loader.py
-Comment: 
-
-Filename: lense/_chat/replace_file.py
-Comment: 
-
-Filename: lense-0.0.2.dist-info/METADATA
-Comment: 
-
-Filename: lense-0.0.2.dist-info/WHEEL
-Comment: 
-
-Filename: lense-0.0.2.dist-info/top_level.txt
-Comment: 
-
-Filename: lense-0.0.2.dist-info/RECORD
+Filename: lense-0.0.57.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lense/__init__.py

```diff
@@ -1 +1 @@
-from .app import lense
+from .main import start
```

