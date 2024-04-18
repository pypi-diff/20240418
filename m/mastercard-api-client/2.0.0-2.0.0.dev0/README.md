# Comparing `tmp/mastercard_api_client-2.0.0.tar.gz` & `tmp/mastercard_api_client-2.0.0.dev0.tar.gz`

## Comparing `mastercard_api_client-2.0.0.tar` & `mastercard_api_client-2.0.0.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/_version.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/__init__.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/baseobject.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/config.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/constants.py
--rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/controller.py
--rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/exceptions.py
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/model.py
--rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/core/util.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/security/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/security/authentication.py
--rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/security/oauth.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/mastercardapicore/security/util.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/.gitignore
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/README.md
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/_version.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/__init__.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/baseobject.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/config.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/constants.py
+-rw-r--r--   0        0        0    10082 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/controller.py
+-rw-r--r--   0        0        0     8777 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/exceptions.py
+-rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/model.py
+-rw-r--r--   0        0        0     5385 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/core/util.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/security/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/security/authentication.py
+-rw-r--r--   0        0        0     7242 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/security/oauth.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/mastercardapicore/security/util.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/.gitignore
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/README.md
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mastercard_api_client-2.0.0.dev0/PKG-INFO
```

### Comparing `mastercard_api_client-2.0.0/.github/workflows/publish.yaml` & `mastercard_api_client-2.0.0.dev0/.github/workflows/publish.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -38,8 +38,8 @@
             ./dist/*.tar.gz
           prerelease: ${{ contains(github.ref, '-pre') }}
           generate_release_notes: ${{ !contains(github.ref, '-pre') }}
 
       - name: Publish Distribution Package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
-          password: ${{ secrets.PYPI_TOKEN }}
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/baseobject.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/baseobject.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/config.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/config.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/constants.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/constants.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/controller.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/controller.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/exceptions.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/model.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/model.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/core/util.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/core/util.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/security/authentication.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/security/authentication.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/security/oauth.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/security/oauth.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/mastercardapicore/security/util.py` & `mastercard_api_client-2.0.0.dev0/mastercardapicore/security/util.py`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/.gitignore` & `mastercard_api_client-2.0.0.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/pyproject.toml` & `mastercard_api_client-2.0.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mastercard_api_client-2.0.0/PKG-INFO` & `mastercard_api_client-2.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mastercard-api-client
-Version: 2.0.0
+Version: 2.0.0.dev0
 Summary: MasterCard API Python Core SDK, fork of the mastercard-api-core library.
 Author-email: Twisto Platform <platform@twisto.cz>
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

