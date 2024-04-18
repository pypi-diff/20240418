# Comparing `tmp/configextractor-py-1.1.3.tar.gz` & `tmp/configextractor_py-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configextractor-py-1.1.3.tar", last modified: Wed Jan 31 14:58:52 2024, max compression
+gzip compressed data, was "configextractor_py-1.1.4.tar", last modified: Thu Apr 18 13:53:26 2024, max compression
```

## Comparing `configextractor-py-1.1.3.tar` & `configextractor_py-1.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/
--rw-r--r--   0 vsts      (1001) docker     (127)       89 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (127)      671 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/.gitmodules
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.520280 configextractor-py-1.1.3/.vscode/
--rw-r--r--   0 vsts      (1001) docker     (127)      939 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/.vscode/settings.json
--rw-r--r--   0 vsts      (1001) docker     (127)     3914 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     3553 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.520280 configextractor-py-1.1.3/configextractor/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1992 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/cli.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.520280 configextractor-py-1.1.3/configextractor/frameworks/
--rw-r--r--   0 vsts      (1001) docker     (127)      202 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/base.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2450 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/cape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4365 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/maco.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2793 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/malduck.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10364 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/mwcp.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2926 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/frameworks/ratdecoder.py.bak
--rw-r--r--   0 vsts      (1001) docker     (127)    13140 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/configextractor/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/configextractor_py.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     3914 2024-01-31 14:58:52.000000 configextractor-py-1.1.3/configextractor_py.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-01-31 14:58:52.000000 configextractor-py-1.1.3/configextractor_py.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-31 14:58:52.000000 configextractor-py-1.1.3/configextractor_py.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-01-31 14:58:52.000000 configextractor-py-1.1.3/configextractor_py.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-01-31 14:58:52.000000 configextractor-py-1.1.3/configextractor_py.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-01-31 14:58:52.000000 configextractor-py-1.1.3/configextractor_py.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)     1703 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/pipelines/test.yaml
--rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/tests/parsers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/parsers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/parsers/cape_extractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)      280 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/parsers/maco_extractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)      129 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/parsers/mwcp_extractor.py
--rw-r--r--   0 vsts      (1001) docker     (127)        7 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      974 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/test_detection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1677 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/test_run.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:52.524280 configextractor-py-1.1.3/tests/venv_parsers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-31 14:58:40.000000 configextractor-py-1.1.3/tests/venv_parsers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)       89 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (127)      671 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/.gitmodules
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.763631 configextractor_py-1.1.4/.vscode/
+-rw-r--r--   0 vsts      (1001) docker     (127)      939 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/.vscode/settings.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     3914 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     3553 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.763631 configextractor_py-1.1.4/configextractor/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1992 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/cli.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/configextractor/frameworks/
+-rw-r--r--   0 vsts      (1001) docker     (127)      202 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/base.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2450 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/cape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4249 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/maco.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2793 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/malduck.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10364 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/mwcp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2926 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/frameworks/ratdecoder.py.bak
+-rw-r--r--   0 vsts      (1001) docker     (127)    13176 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/configextractor/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/configextractor_py.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3914 2024-04-18 13:53:26.000000 configextractor_py-1.1.4/configextractor_py.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      932 2024-04-18 13:53:26.000000 configextractor_py-1.1.4/configextractor_py.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-18 13:53:26.000000 configextractor_py-1.1.4/configextractor_py.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       91 2024-04-18 13:53:26.000000 configextractor_py-1.1.4/configextractor_py.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-18 13:53:26.000000 configextractor_py-1.1.4/configextractor_py.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       16 2024-04-18 13:53:26.000000 configextractor_py-1.1.4/configextractor_py.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1703 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/pipelines/test.yaml
+-rw-r--r--   0 vsts      (1001) docker     (127)       40 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/tests/parsers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/parsers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      358 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/parsers/cape_extractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      313 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/parsers/maco_extractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      129 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/parsers/mwcp_extractor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        7 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      974 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/test_detection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2096 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/test_run.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:26.767632 configextractor_py-1.1.4/tests/venv_parsers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-18 13:53:15.000000 configextractor_py-1.1.4/tests/venv_parsers/__init__.py
```

### Comparing `configextractor-py-1.1.3/.gitmodules` & `configextractor_py-1.1.4/.gitmodules`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/.vscode/settings.json` & `configextractor_py-1.1.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/PKG-INFO` & `configextractor_py-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configextractor-py
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for extracting malware configurations across multiple frameworks
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Requires-Dist: cart
 Requires-Dist: click
 Requires-Dist: maco
 Requires-Dist: mwcfg
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: configextractor-py Version: 1.1.3 Summary: A
+Metadata-Version: 2.1 Name: configextractor-py Version: 1.1.4 Summary: A
 library for extracting malware configurations across multiple frameworks
 Requires-Python: >=3.8,<3.12 Description-Content-Type: text/markdown Requires-
 Dist: cart Requires-Dist: click Requires-Dist: maco Requires-Dist: mwcfg
 Requires-Dist: mwcp Requires-Dist: plyara Requires-Dist: regex #
 ConfigExtractor _[_L_a_t_e_s_t_ _S_t_a_b_l_e_ _R_e_l_e_a_s_e_]Maintainer: @cccs-rs Python Library for
 performing configuration extraction across multiple extraction frameworks (ie.
 Maco, MWCP, etc.). This tool is actively used in the [Assemblyline](https://
```

### Comparing `configextractor-py-1.1.3/README.md` & `configextractor_py-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/cli.py` & `configextractor_py-1.1.4/configextractor/cli.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/frameworks/base.py` & `configextractor_py-1.1.4/configextractor/frameworks/base.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/frameworks/cape.py` & `configextractor_py-1.1.4/configextractor/frameworks/cape.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/frameworks/maco.py` & `configextractor_py-1.1.4/configextractor/frameworks/maco.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     def result_template(self, extractor: Extractor, yara_matches: List) -> Dict[str, str]:
         template = super().result_template(extractor, yara_matches)
         decoder = extractor.module()
         template.update(
             {
                 "author": decoder.author,
                 "description": decoder.__doc__,
-                "config": {"family": decoder.family if hasattr(decoder, "family") else decoder.__class__.__name__},
             }
         )
         return template
 
     def run(self, sample_path: str, parsers: Dict[Extractor, List[str]]) -> List[dict]:
         results = list()
         for extractor, yara_matches in parsers.items():
```

### Comparing `configextractor-py-1.1.3/configextractor/frameworks/malduck.py` & `configextractor_py-1.1.4/configextractor/frameworks/malduck.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/frameworks/mwcp.py` & `configextractor_py-1.1.4/configextractor/frameworks/mwcp.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/frameworks/ratdecoder.py.bak` & `configextractor_py-1.1.4/configextractor/frameworks/ratdecoder.py.bak`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/configextractor/main.py` & `configextractor_py-1.1.4/configextractor/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,14 +233,15 @@
 
             if cart.is_cart(buf):
                 # Uncart file to temporary location for analysis
                 cart.unpack_file(sample, sample_copy.name)
             else:
                 # Make a copy of the file to the temporary location
                 sample_copy.write(buf)
+                sample_copy.flush()
 
             # Get YARA-dependent parsers that should run based on match
             for yara_match in self.yara.match(sample_copy.name):
                 # Retrieve relevant parser information
                 extractor = self.parsers[yara_match.namespace]
                 if block_regex and block_regex.match(extractor.module.__name__):
                     self.log.info(f"Blocking {extractor.module.__name__} based on passed blocklist regex list")
```

### Comparing `configextractor-py-1.1.3/configextractor_py.egg-info/PKG-INFO` & `configextractor_py-1.1.4/configextractor_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configextractor-py
-Version: 1.1.3
+Version: 1.1.4
 Summary: A library for extracting malware configurations across multiple frameworks
 Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown
 Requires-Dist: cart
 Requires-Dist: click
 Requires-Dist: maco
 Requires-Dist: mwcfg
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: configextractor-py Version: 1.1.3 Summary: A
+Metadata-Version: 2.1 Name: configextractor-py Version: 1.1.4 Summary: A
 library for extracting malware configurations across multiple frameworks
 Requires-Python: >=3.8,<3.12 Description-Content-Type: text/markdown Requires-
 Dist: cart Requires-Dist: click Requires-Dist: maco Requires-Dist: mwcfg
 Requires-Dist: mwcp Requires-Dist: plyara Requires-Dist: regex #
 ConfigExtractor _[_L_a_t_e_s_t_ _S_t_a_b_l_e_ _R_e_l_e_a_s_e_]Maintainer: @cccs-rs Python Library for
 performing configuration extraction across multiple extraction frameworks (ie.
 Maco, MWCP, etc.). This tool is actively used in the [Assemblyline](https://
```

### Comparing `configextractor-py-1.1.3/configextractor_py.egg-info/SOURCES.txt` & `configextractor_py-1.1.4/configextractor_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/pipelines/publish.yaml` & `configextractor_py-1.1.4/pipelines/publish.yaml`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/pipelines/test.yaml` & `configextractor_py-1.1.4/pipelines/test.yaml`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/setup.py` & `configextractor_py-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/tests/test_detection.py` & `configextractor_py-1.1.4/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `configextractor-py-1.1.3/tests/test_run.py` & `configextractor_py-1.1.4/tests/test_run.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,7 +38,19 @@
             assert True
 
         # Test running MACO extractors in venv mode
         assert MACO(logger=None).run_in_venv(sample_path=sample.name, extractor=maco)
 
         # Test running MWCP extractors in venv mode
         assert MWCP(logger=None).run_in_venv(sample_path=sample.name, extractor=mwcp)
+
+
+def test_itty_bitty_file(cx):
+    maco: Extractor = cx.parsers["venv_parsers.maco_extractor.TestMACO"]
+    file_content = b"Hello world"
+
+    # Create a small test file to run with the extractor
+    with NamedTemporaryFile(delete=False) as sample:
+        sample.write(file_content)
+        sample.flush()
+
+        assert cx.run_parsers(sample.name)["MACO"][0]["config"]["decoded_strings"] == [file_content.decode()]
```

