# Comparing `tmp/slalom_tapdance-0.9.10.dev49.tar.gz` & `tmp/slalom_tapdance-0.9.10.dev50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-0.9.10.dev49.tar", max compression
+gzip compressed data, was "slalom_tapdance-0.9.10.dev50.tar", max compression
```

## Comparing `slalom_tapdance-0.9.10.dev49.tar` & `slalom_tapdance-0.9.10.dev50.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-04-18 20:57:32.751343 slalom_tapdance-0.9.10.dev49/LICENSE
--rw-r--r--   0        0        0     1169 2024-04-18 20:57:51.075407 slalom_tapdance-0.9.10.dev49/pyproject.toml
--rw-r--r--   0        0        0      288 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/__init__.py
--rw-r--r--   0        0        0      696 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/cli.py
--rw-r--r--   0        0        0    15304 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/config.py
--rw-r--r--   0        0        0    13533 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/install_helper.py
--rw-r--r--   0        0        0    37111 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/states.py
--rw-r--r--   0        0        0    11787 2024-04-18 20:57:32.755343 slalom_tapdance-0.9.10.dev49/tapdance/syncs.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev49/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-18 21:05:08.865644 slalom_tapdance-0.9.10.dev50/LICENSE
+-rw-r--r--   0        0        0     1169 2024-04-18 21:05:26.437494 slalom_tapdance-0.9.10.dev50/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/cli.py
+-rw-r--r--   0        0        0    15304 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/config.py
+-rw-r--r--   0        0        0    13533 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/install_helper.py
+-rw-r--r--   0        0        0    37111 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/states.py
+-rw-r--r--   0        0        0    11787 2024-04-18 21:05:08.869644 slalom_tapdance-0.9.10.dev50/tapdance/syncs.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 slalom_tapdance-0.9.10.dev50/PKG-INFO
```

### Comparing `slalom_tapdance-0.9.10.dev49/LICENSE` & `slalom_tapdance-0.9.10.dev50/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/pyproject.toml` & `slalom_tapdance-0.9.10.dev50/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "0.9.10-dev.49"
+version = "0.9.10-dev.50"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["AJ Steers <aj.steers@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/cli.py` & `slalom_tapdance-0.9.10.dev50/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/config.py` & `slalom_tapdance-0.9.10.dev50/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/docker.py` & `slalom_tapdance-0.9.10.dev50/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/install_helper.py` & `slalom_tapdance-0.9.10.dev50/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/plans.py` & `slalom_tapdance-0.9.10.dev50/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/states.py` & `slalom_tapdance-0.9.10.dev50/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/tapdance/syncs.py` & `slalom_tapdance-0.9.10.dev50/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-0.9.10.dev49/PKG-INFO` & `slalom_tapdance-0.9.10.dev50/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 0.9.10.dev49
+Version: 0.9.10.dev50
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: AJ Steers
 Author-email: aj.steers@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

