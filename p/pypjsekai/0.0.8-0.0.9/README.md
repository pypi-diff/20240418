# Comparing `tmp/pypjsekai-0.0.8.tar.gz` & `tmp/pypjsekai-0.0.9.tar.gz`

## Comparing `pypjsekai-0.0.8.tar` & `pypjsekai-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/__about__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/__init__.py
--rwxr-xr-x   0        0        0    21855 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/api.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/asset.py
--rwxr-xr-x   0        0        0     1006 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/asset_bundle.py
--rw-r--r--   0        0        0    31218 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/client.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/exceptions.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/live.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/py.typed
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/utilities.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/enums/__init__.py
--rw-r--r--   0        0        0    23054 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/enums/enums.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/enums/information.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/enums/platform.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/enums/tutorial_status.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/enums/unknown.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/__init__.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/asset_bundle_info.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/game_version.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/information.py
--rw-r--r--   0        0        0    69258 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/master_data.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/model.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pjsekai/models/system_info.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pypjsekai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/__about__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/__init__.py
+-rwxr-xr-x   0        0        0    21855 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/api.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/asset.py
+-rwxr-xr-x   0        0        0     1006 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/asset_bundle.py
+-rw-r--r--   0        0        0    31335 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/client.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/exceptions.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/live.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/py.typed
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/utilities.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/enums/__init__.py
+-rw-r--r--   0        0        0    23054 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/enums/enums.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/enums/information.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/enums/platform.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/enums/tutorial_status.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/enums/unknown.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/__init__.py
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/asset_bundle_info.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/game_version.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/information.py
+-rw-r--r--   0        0        0    69258 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/master_data.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/model.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pjsekai/models/system_info.py
+-rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pypjsekai-0.0.9/PKG-INFO
```

### Comparing `pypjsekai-0.0.8/pjsekai/api.py` & `pypjsekai-0.0.9/pjsekai/api.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/asset.py` & `pypjsekai-0.0.9/pjsekai/asset.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,18 @@
         self._asset_bundle_info = new_value
         if self.path is not None and new_value is not None:
             self.path.parent.mkdir(parents=True, exist_ok=True)
             with self.path.joinpath("AssetBundleInfo.json").open("w") as f:
                 dump(new_value,f,indent=2,ensure_ascii=False,default=AssetBundleInfo.encoder)
 
     def __init__(self, version: str, hash: str, asset_directory: Optional[str] = None) -> None:
+        self._path = None
         if asset_directory is not None:
             p = Path(asset_directory)
-            if p.exists and not p.is_dir():
+            if p.exists() and not p.is_dir():
                 raise NotADirectoryError
             self._path = p
 
         self._version = version
         self._hash = hash
 
         if self.path is not None:
```

### Comparing `pypjsekai-0.0.8/pjsekai/asset_bundle.py` & `pypjsekai-0.0.9/pjsekai/asset_bundle.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/client.py` & `pypjsekai-0.0.9/pjsekai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,18 @@
             "data_version": data_version,
             "app_version_status": app_version_status,
         })
         self.api_manager.system_info = self.system_info
 
     @_auto_session_refresh
     def update_asset(self, asset_version: str, asset_hash: str) -> None:
-        self._asset = Asset(asset_version,asset_hash,str(self.asset_directory))
+        if self.asset_directory is None:
+            self._asset = Asset(asset_version,asset_hash)
+        else:
+            self._asset = Asset(asset_version,asset_hash,str(self.asset_directory))
         self._asset.get_asset_bundle_info(self.api_manager)
         self.system_info = self.system_info.copy(update={
             "asset_version": asset_version,
             "asset_hash": asset_hash,
         })
         self.api_manager.system_info = self.system_info
```

### Comparing `pypjsekai-0.0.8/pjsekai/exceptions.py` & `pypjsekai-0.0.9/pjsekai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/live.py` & `pypjsekai-0.0.9/pjsekai/live.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/utilities.py` & `pypjsekai-0.0.9/pjsekai/utilities.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/enums/enums.py` & `pypjsekai-0.0.9/pjsekai/enums/enums.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/enums/information.py` & `pypjsekai-0.0.9/pjsekai/enums/information.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/enums/platform.py` & `pypjsekai-0.0.9/pjsekai/enums/platform.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/enums/tutorial_status.py` & `pypjsekai-0.0.9/pjsekai/enums/tutorial_status.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/enums/unknown.py` & `pypjsekai-0.0.9/pjsekai/enums/unknown.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/models/asset_bundle_info.py` & `pypjsekai-0.0.9/pjsekai/models/asset_bundle_info.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/models/information.py` & `pypjsekai-0.0.9/pjsekai/models/information.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/models/master_data.py` & `pypjsekai-0.0.9/pjsekai/models/master_data.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pjsekai/models/model.py` & `pypjsekai-0.0.9/pjsekai/models/model.py`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/.gitignore` & `pypjsekai-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/LICENSE.txt` & `pypjsekai-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/pyproject.toml` & `pypjsekai-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pypjsekai-0.0.8/PKG-INFO` & `pypjsekai-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypjsekai
-Version: 0.0.8
+Version: 0.0.9
 Summary: Reverse engineered Python client for the mobile rhythm game Project SEKAI COLORFUL STAGE! feat. Hatsune Miku
 Project-URL: Documentation, https://github.com/pjsek-ai/pypjsekai#readme
 Project-URL: Issues, https://github.com/pjsek-ai/pypjsekai/issues
 Project-URL: Source, https://github.com/pjsek-ai/pypjsekai
 Author-email: Erik Chan <erikchan002@gmail.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
```

