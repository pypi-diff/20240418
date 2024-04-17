# Comparing `tmp/np-aind-metadata-0.1.1.tar.gz` & `tmp/np_aind_metadata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np-aind-metadata-0.1.1.tar", last modified: Fri Apr 12 23:13:00 2024, max compression
+gzip compressed data, was "np_aind_metadata-0.1.2.tar", last modified: Wed Apr 17 23:36:28 2024, max compression
```

## Comparing `np-aind-metadata-0.1.1.tar` & `np_aind_metadata-0.1.2.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.452252 np-aind-metadata-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-12 23:13:00.452252 np-aind-metadata-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-12 23:12:57.000000 np-aind-metadata-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:13:00.452252 np-aind-metadata-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.448252 np-aind-metadata-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.448252 np-aind-metadata-0.1.1/src/np_aind_metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-12 23:12:53.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-12 23:12:55.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.448252 np-aind-metadata-0.1.1/src/np_aind_metadata/init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-04-12 23:12:55.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/init/dynamic_routing_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.448252 np-aind-metadata-0.1.1/src/np_aind_metadata/np/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/np/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-12 23:12:55.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/np/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.448252 np-aind-metadata-0.1.1/src/np_aind_metadata/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-12 23:12:55.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/scripts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.452252 np-aind-metadata-0.1.1/src/np_aind_metadata/update/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-12 23:12:55.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/update/dynamic_routing_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-12 23:12:55.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/update/dynamic_routing_task_etl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-12 23:12:54.000000 np-aind-metadata-0.1.1/src/np_aind_metadata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.452252 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-12 23:13:00.000000 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-12 23:13:00.000000 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:13:00.000000 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 23:13:00.000000 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 23:13:00.000000 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 23:13:00.000000 np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:13:00.452252 np-aind-metadata-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 23:12:24.000000 np-aind-metadata-0.1.1/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-17 23:36:26.000000 np_aind_metadata-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.964764 np_aind_metadata-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.964764 np_aind_metadata-0.1.2/src/np_aind_metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/src/np_aind_metadata/init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21535 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/init/dynamic_routing_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/src/np_aind_metadata/np/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/np/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/np/dynamic_routing_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-17 23:36:23.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/np_codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/src/np_aind_metadata/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-17 23:36:23.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/src/np_aind_metadata/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5711 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/update/dynamic_routing_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15636 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/update/dynamic_routing_task_etl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/src/np_aind_metadata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-17 23:36:28.000000 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-17 23:36:28.000000 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:36:28.000000 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-17 23:36:28.000000 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-17 23:36:28.000000 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-17 23:36:28.000000 np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:36:28.968764 np_aind_metadata-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-04-17 23:35:50.000000 np_aind_metadata-0.1.2/tests/test_np_codeocean.py
```

### Comparing `np-aind-metadata-0.1.1/LICENSE` & `np_aind_metadata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/PKG-INFO` & `np_aind_metadata-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.1
+Version: 0.1.2
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np-aind-metadata-0.1.1/README.md` & `np_aind_metadata-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/pyproject.toml` & `np_aind_metadata-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dependencies = [
     "h5py>=3.10.0",
     "pyyaml>=6.0.1",
     "np-session>=0.6.40",
     "np-config>=0.4.27",
     "aind-metadata-mapper==0.6.2",
 ]
-version = "0.1.1"
+version = "0.1.2"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
```

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/__init__.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/common.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 # LASER_ASSEMBLY_0 = "Laser Assembly 0"
 # LASER_ASSEMBLY_1 = "Laser Assembly 1"
 # CAMERA_0 = "Camera 0"
 # CAMERA_1 = "Camera 1"
 # CAMERA_2 = "Camera 2"
 
 
+RigName = typing.Literal["NP0", "NP1", "NP2", "NP3"]
+
+
 class NeuropixelsETLContext(pydantic.BaseModel):
     """Base Context for Neuropixels ETL."""
 
     source: pathlib.Path
 
 
 class DynamicRoutingTaskContext(NeuropixelsETLContext):
```

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/init/dynamic_routing_task.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/init/dynamic_routing_task.py`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/np/dynamic_routing_task.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/np/dynamic_routing_task.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,34 +112,25 @@
 
 
 def update_rig_from_session_dir(
     rig_path: pathlib.Path,
     session_dir: pathlib.Path,
     output_dir: pathlib.Path = pathlib.Path("./"),
     include: typing.Optional[list[str]] = None,
-    id_prefix: typing.Optional[str] = None,
-    id_suffix: typing.Optional[str] = None,
 ) -> common.DynamicRoutingTaskUpdateContext:
     context = common.DynamicRoutingTaskUpdateContext(
         source=rig_path,
     )
     context = dynamic_routing_task_update.scrape_update_context(session_dir, context)
     logger.debug("Scraped context: %s" % context.model_dump_json())
-    session = np_session.Session(session_dir.stem)
-    _id = session.date.strftime("%Y-%m-%d")
-    if id_prefix:
-        _id = f"{id_prefix}_{_id}"
-    if id_suffix:
-        _id = f"{_id}_{id_suffix}"
-    logger.debug(f"ID: {_id}")
-    output_path = output_dir / f"{_id}_rig.json"
+    output_path = output_dir / "rig.json"
     updated = dynamic_routing_task_update.update_rig(
         context,
         output_path=output_path,
-        modification_date=session.date,
+        modification_date=datetime.date.today(),
         include=include,
     )
     _fix_modification_date(updated.source, output_path)
     return updated
 
 
 # using typing.Any due to np_session import failing in github actions
```

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/scripts/main.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/scripts/main.py`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/update/dynamic_routing_task.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/update/dynamic_routing_task.py`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/update/dynamic_routing_task_etl.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/update/dynamic_routing_task_etl.py`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata/utils.py` & `np_aind_metadata-0.1.2/src/np_aind_metadata/utils.py`

 * *Files identical despite different names*

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/PKG-INFO` & `np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-aind-metadata
-Version: 0.1.1
+Version: 0.1.2
 Author-email: Christopher Mochizuki <chrism@alleninstitute.org>
 License: MIT
 Project-URL: Repository, https://github.com/AllenInstitute/np-aind-metadata
 Project-URL: Issues, https://github.com/AllenInstitute/np-aind-metadata/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `np-aind-metadata-0.1.1/src/np_aind_metadata.egg-info/SOURCES.txt` & `np_aind_metadata-0.1.2/src/np_aind_metadata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 src/np_aind_metadata/__init__.py
 src/np_aind_metadata/common.py
+src/np_aind_metadata/np_codeocean.py
 src/np_aind_metadata/py.typed
+src/np_aind_metadata/storage.py
 src/np_aind_metadata/utils.py
 src/np_aind_metadata.egg-info/PKG-INFO
 src/np_aind_metadata.egg-info/SOURCES.txt
 src/np_aind_metadata.egg-info/dependency_links.txt
 src/np_aind_metadata.egg-info/entry_points.txt
 src/np_aind_metadata.egg-info/requires.txt
 src/np_aind_metadata.egg-info/top_level.txt
@@ -15,8 +17,9 @@
 src/np_aind_metadata/init/dynamic_routing_task.py
 src/np_aind_metadata/np/__init__.py
 src/np_aind_metadata/np/dynamic_routing_task.py
 src/np_aind_metadata/scripts/main.py
 src/np_aind_metadata/update/__init__.py
 src/np_aind_metadata/update/dynamic_routing_task.py
 src/np_aind_metadata/update/dynamic_routing_task_etl.py
-tests/test_core.py
+tests/test_core.py
+tests/test_np_codeocean.py
```

