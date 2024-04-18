# Comparing `tmp/flap-lite-0.6.8.tar.gz` & `tmp/flap-lite-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flap-lite-0.6.8.tar", last modified: Thu Nov 16 21:13:08 2023, max compression
+gzip compressed data, was "flap-lite-0.6.9.tar", last modified: Thu Nov 16 21:38:36 2023, max compression
```

## Comparing `flap-lite-0.6.8.tar` & `flap-lite-0.6.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1090 2023-10-18 11:42:59.000000 flap-lite-0.6.8/LICENSE
--rw-r--r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1855 2023-11-16 21:13:08.155714 flap-lite-0.6.8/PKG-INFO
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      519 2023-10-19 10:52:19.000000 flap-lite-0.6.8/README.md
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1343 2023-11-16 21:11:58.000000 flap-lite-0.6.8/pyproject.toml
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)       38 2023-11-16 21:13:08.155714 flap-lite-0.6.8/setup.cfg
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:22.000000 flap-lite-0.6.8/src/flap/__init__.py
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/alignment/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/alignment/__init__.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    10131 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/alignment/linear_assignment_alignment.py
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/database/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/database/__init__.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     2078 2023-11-16 21:11:10.000000 flap-lite-0.6.8/src/flap/database/db_build_vocabulary.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     3448 2023-11-16 21:11:10.000000 flap-lite-0.6.8/src/flap/database/db_import.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    15795 2023-11-16 21:11:10.000000 flap-lite-0.6.8/src/flap/database/db_index.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    12995 2023-11-16 21:11:10.000000 flap-lite-0.6.8/src/flap/database/sql.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1438 2023-11-14 13:59:15.000000 flap-lite-0.6.8/src/flap/database/sql_in_memory.py
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/matcher/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/matcher/__init__.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    15351 2023-11-14 13:59:15.000000 flap-lite-0.6.8/src/flap/matcher/sql_matcher.py
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/parser/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/parser/__init__.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)   127118 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/parser/multiplier_index.csv
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)   115040 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/parser/pc1_mappings_region.json
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    13726 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/parser/rule_parser_fast.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      852 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/parser/thoroughfare_patterns.json
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/preprocessing/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     3074 2023-11-14 13:59:15.000000 flap-lite-0.6.8/src/flap/preprocessing/__init__.py
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap/utils/
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     4059 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/utils/__init__.py
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     2441 2023-10-19 16:11:21.000000 flap-lite-0.6.8/src/flap/utils/progress_map.py
-drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:13:08.155714 flap-lite-0.6.8/src/flap_lite.egg-info/
--rw-r--r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1855 2023-11-16 21:13:08.000000 flap-lite-0.6.8/src/flap_lite.egg-info/PKG-INFO
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      849 2023-11-16 21:13:08.000000 flap-lite-0.6.8/src/flap_lite.egg-info/SOURCES.txt
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        1 2023-11-16 21:13:08.000000 flap-lite-0.6.8/src/flap_lite.egg-info/dependency_links.txt
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      415 2023-11-16 21:13:08.000000 flap-lite-0.6.8/src/flap_lite.egg-info/requires.txt
--rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        5 2023-11-16 21:13:08.000000 flap-lite-0.6.8/src/flap_lite.egg-info/top_level.txt
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1090 2023-10-18 11:42:59.000000 flap-lite-0.6.9/LICENSE
+-rw-r--r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1855 2023-11-16 21:38:36.743353 flap-lite-0.6.9/PKG-INFO
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      519 2023-10-19 10:52:19.000000 flap-lite-0.6.9/README.md
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1343 2023-11-16 21:38:19.000000 flap-lite-0.6.9/pyproject.toml
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)       38 2023-11-16 21:38:36.743353 flap-lite-0.6.9/setup.cfg
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:22.000000 flap-lite-0.6.9/src/flap/__init__.py
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/alignment/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/alignment/__init__.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    10131 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/alignment/linear_assignment_alignment.py
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/database/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/database/__init__.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     2078 2023-11-16 21:11:10.000000 flap-lite-0.6.9/src/flap/database/db_build_vocabulary.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     3448 2023-11-16 21:11:10.000000 flap-lite-0.6.9/src/flap/database/db_import.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    15793 2023-11-16 21:37:47.000000 flap-lite-0.6.9/src/flap/database/db_index.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    12995 2023-11-16 21:11:10.000000 flap-lite-0.6.9/src/flap/database/sql.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1438 2023-11-14 13:59:15.000000 flap-lite-0.6.9/src/flap/database/sql_in_memory.py
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/matcher/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/matcher/__init__.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    15351 2023-11-14 13:59:15.000000 flap-lite-0.6.9/src/flap/matcher/sql_matcher.py
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/parser/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/parser/__init__.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)   127118 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/parser/multiplier_index.csv
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)   115040 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/parser/pc1_mappings_region.json
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)    13726 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/parser/rule_parser_fast.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      852 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/parser/thoroughfare_patterns.json
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/preprocessing/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     3074 2023-11-14 13:59:15.000000 flap-lite-0.6.9/src/flap/preprocessing/__init__.py
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap/utils/
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     4059 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/utils/__init__.py
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     2441 2023-10-19 16:11:21.000000 flap-lite-0.6.9/src/flap/utils/progress_map.py
+drwxrwxr-x   0 huayu_ssh  (1001) huayu_ssh  (1001)        0 2023-11-16 21:38:36.743353 flap-lite-0.6.9/src/flap_lite.egg-info/
+-rw-r--r--   0 huayu_ssh  (1001) huayu_ssh  (1001)     1855 2023-11-16 21:38:36.000000 flap-lite-0.6.9/src/flap_lite.egg-info/PKG-INFO
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      849 2023-11-16 21:38:36.000000 flap-lite-0.6.9/src/flap_lite.egg-info/SOURCES.txt
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        1 2023-11-16 21:38:36.000000 flap-lite-0.6.9/src/flap_lite.egg-info/dependency_links.txt
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)      415 2023-11-16 21:38:36.000000 flap-lite-0.6.9/src/flap_lite.egg-info/requires.txt
+-rw-rw-r--   0 huayu_ssh  (1001) huayu_ssh  (1001)        5 2023-11-16 21:38:36.000000 flap-lite-0.6.9/src/flap_lite.egg-info/top_level.txt
```

### Comparing `flap-lite-0.6.8/LICENSE` & `flap-lite-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/PKG-INFO` & `flap-lite-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flap-lite
-Version: 0.6.8
+Version: 0.6.9
 Summary: An open-source tool for linking free-text addresses to UPRN
 Author-email: Huayu Zhang <huayu.zhang@ed.ac.uk>
 Project-URL: Homepage, https://github.com/huayu-zhang/flap_lite
 Project-URL: Bug Tracker, https://github.com/huayu-zhang/flap_lite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `flap-lite-0.6.8/README.md` & `flap-lite-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/pyproject.toml` & `flap-lite-0.6.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flap-lite"
-version = "0.6.8"
+version = "0.6.9"
 authors = [
   { name="Huayu Zhang", email="huayu.zhang@ed.ac.uk"},
 ]
 description = "An open-source tool for linking free-text addresses to UPRN"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flap-lite-0.6.8/src/flap/alignment/linear_assignment_alignment.py` & `flap-lite-0.6.9/src/flap/alignment/linear_assignment_alignment.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/database/db_build_vocabulary.py` & `flap-lite-0.6.9/src/flap/database/db_build_vocabulary.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/database/db_import.py` & `flap-lite-0.6.9/src/flap/database/db_import.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/database/db_index.py` & `flap-lite-0.6.9/src/flap/database/db_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         res_expanded.to_sql(name='expanded', con=conn_temp, if_exists='append', dtype='TEXT', index=False)
 
         range_rows.append(expand_bn(df_chunk))
 
     if len(range_rows):
 
-        df_range_rows = pd.concat([range_rows])
+        df_range_rows = pd.concat(range_rows)
 
         range_indexed = indexing_uprn(df_range_rows)
 
         range_expanded = expand_number_like(range_indexed)
 
         range_expanded.to_sql(name='expanded', con=conn_temp, if_exists='append', dtype='TEXT', index=False)
```

### Comparing `flap-lite-0.6.8/src/flap/database/sql.py` & `flap-lite-0.6.9/src/flap/database/sql.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/database/sql_in_memory.py` & `flap-lite-0.6.9/src/flap/database/sql_in_memory.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/matcher/sql_matcher.py` & `flap-lite-0.6.9/src/flap/matcher/sql_matcher.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/parser/multiplier_index.csv` & `flap-lite-0.6.9/src/flap/parser/multiplier_index.csv`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/parser/pc1_mappings_region.json` & `flap-lite-0.6.9/src/flap/parser/pc1_mappings_region.json`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/parser/rule_parser_fast.py` & `flap-lite-0.6.9/src/flap/parser/rule_parser_fast.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/parser/thoroughfare_patterns.json` & `flap-lite-0.6.9/src/flap/parser/thoroughfare_patterns.json`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/preprocessing/__init__.py` & `flap-lite-0.6.9/src/flap/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/utils/__init__.py` & `flap-lite-0.6.9/src/flap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap/utils/progress_map.py` & `flap-lite-0.6.9/src/flap/utils/progress_map.py`

 * *Files identical despite different names*

### Comparing `flap-lite-0.6.8/src/flap_lite.egg-info/PKG-INFO` & `flap-lite-0.6.9/src/flap_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flap-lite
-Version: 0.6.8
+Version: 0.6.9
 Summary: An open-source tool for linking free-text addresses to UPRN
 Author-email: Huayu Zhang <huayu.zhang@ed.ac.uk>
 Project-URL: Homepage, https://github.com/huayu-zhang/flap_lite
 Project-URL: Bug Tracker, https://github.com/huayu-zhang/flap_lite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `flap-lite-0.6.8/src/flap_lite.egg-info/SOURCES.txt` & `flap-lite-0.6.9/src/flap_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

