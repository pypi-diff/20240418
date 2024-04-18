# Comparing `tmp/pyshared-1.5.4-py3-none-any.whl.zip` & `tmp/pyshared-1.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 12256 bytes, number of entries: 16
+Zip file size: 12251 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      781 b- defN 24-Apr-12 00:41 pyshared/__init__.py
 -rw-r--r--  2.0 unx      124 b- defN 24-Jan-11 01:53 pyshared/consts.py
 -rw-r--r--  2.0 unx     1293 b- defN 24-Jan-12 03:28 pyshared/crypto.py
 -rw-r--r--  2.0 unx     2029 b- defN 24-Apr-03 16:31 pyshared/env.py
 -rw-r--r--  2.0 unx      943 b- defN 24-Mar-31 21:02 pyshared/exceptions.py
 -rw-r--r--  2.0 unx      936 b- defN 24-Apr-12 00:40 pyshared/pytest.py
 -rw-r--r--  2.0 unx     4929 b- defN 24-Apr-03 16:29 pyshared/python.py
 -rw-r--r--  2.0 unx      790 b- defN 24-Jan-11 05:57 pyshared/shell.py
 -rw-r--r--  2.0 unx     2083 b- defN 24-Jan-12 03:45 pyshared/terminal.py
--rw-r--r--  2.0 unx     2793 b- defN 24-Apr-12 01:03 pyshared/test.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-12 01:13 pyshared/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     6829 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1211 b- defN 24-Apr-12 01:16 pyshared-1.5.4.dist-info/RECORD
-16 files, 25932 bytes uncompressed, 10288 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx     2792 b- defN 24-Apr-18 06:32 pyshared/test.py
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-18 06:34 pyshared/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6829 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1211 b- defN 24-Apr-18 06:36 pyshared-1.5.5.dist-info/RECORD
+16 files, 25931 bytes uncompressed, 10283 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyshared/test.py
 Comment: 
 
 Filename: pyshared/version.py
 Comment: 
 
-Filename: pyshared-1.5.4.dist-info/LICENSE
+Filename: pyshared-1.5.5.dist-info/LICENSE
 Comment: 
 
-Filename: pyshared-1.5.4.dist-info/METADATA
+Filename: pyshared-1.5.5.dist-info/METADATA
 Comment: 
 
-Filename: pyshared-1.5.4.dist-info/WHEEL
+Filename: pyshared-1.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyshared-1.5.4.dist-info/top_level.txt
+Filename: pyshared-1.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyshared-1.5.4.dist-info/RECORD
+Filename: pyshared-1.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyshared/test.py

```diff
@@ -100,8 +100,8 @@
     @property
     def memoryview(self) -> memoryview:
         """Generate a random memoryview object."""
         return memoryview(self.bytes)
 
     def __getitem__(self, key: str):
         """Return the random data for the given type."""
-        return eval(f'self.{key}')
+        return getattr(self, key)
```

## pyshared/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.4'
+__version__ = '1.5.5'
```

## Comparing `pyshared-1.5.4.dist-info/LICENSE` & `pyshared-1.5.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyshared-1.5.4.dist-info/METADATA` & `pyshared-1.5.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyshared
-Version: 1.5.4
+Version: 1.5.5
 Summary: A Python library containing common utility functions for use across multiple codebases, filling gaps not covered by the standard Python libraries.
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Cary Carter
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

## Comparing `pyshared-1.5.4.dist-info/RECORD` & `pyshared-1.5.5.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 pyshared/crypto.py,sha256=Ww3uT2xa7g0ewgZzvJthJQ_BRPeHM0sLZPc5c3tad2E,1293
 pyshared/env.py,sha256=sJM9SVUIKVq9n7ugpC81zRhvAlNPur_Q8qUiCasglXQ,2029
 pyshared/exceptions.py,sha256=j7alpB6QyzZcCt9quCWPIKXmSsUw7dZPvs7fdqbYbO4,943
 pyshared/pytest.py,sha256=3coYUTNfSHB7-pQIPlIOWwOjbtjgBoX5uEc90DfH188,936
 pyshared/python.py,sha256=2AsqfdwMGv-ZwXvlaKvaPKmXwq69yFSwKIzQfMblD_E,4929
 pyshared/shell.py,sha256=F2EJdaImnnlxeiONPlzdXcE_JZ1HUAdBWR5_i-WLfSA,790
 pyshared/terminal.py,sha256=6BjoRuUoqU7iKuXhEqU091aOiQWJUcVWXTMeUlNE3MA,2083
-pyshared/test.py,sha256=j7mug9uYsYHq0R6NjrjvJQSIWlOEcKCRTASjejcSJxE,2793
-pyshared/version.py,sha256=J1aSCJ_LeXu9eC8GJfi0qc4dCnumcuDr3J7ga_AZg8g,22
-pyshared-1.5.4.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-pyshared-1.5.4.dist-info/METADATA,sha256=FptX90LNHGBSO2sIL51ggGISuHKZberqBEpbgN7n4wg,6829
-pyshared-1.5.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-pyshared-1.5.4.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
-pyshared-1.5.4.dist-info/RECORD,,
+pyshared/test.py,sha256=Ta4nNuYckDAtay4mltFCrXSHicQyuQvwGrkM0ypvPHQ,2792
+pyshared/version.py,sha256=Zzj2nCH-pedLXQfcBxIuFgiJXSAz9GGJSJ96GFPKLJE,22
+pyshared-1.5.5.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+pyshared-1.5.5.dist-info/METADATA,sha256=CHBR8FbsUpN7sxO59JrQQORWyEpMP_FA7IrVxahAXdU,6829
+pyshared-1.5.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pyshared-1.5.5.dist-info/top_level.txt,sha256=ymmYDwmXcInf2QKo-75Is2v41uN5Wg_n5XnONS5UX0o,9
+pyshared-1.5.5.dist-info/RECORD,,
```

