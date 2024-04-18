# Comparing `tmp/jupyter_firefly_extensions-4.1.0.tar.gz` & `tmp/jupyter_firefly_extensions-4.1.1.tar.gz`

## Comparing `jupyter_firefly_extensions-4.1.0.tar` & `jupyter_firefly_extensions-4.1.1.tar`

### file list

```diff
@@ -1,46 +1,61 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/.yarnrc.yml
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/License.txt
--rw-r--r--   0        0        0   541440 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/W4 (1).fits
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/conftest.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/install.json
--rwxr-xr-x   0        0        0     2250 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/new-release-procedure.md
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/setup.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/tsconfig.json
--rw-r--r--   0        0        0   188187 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/yarn.lock
--rw-r--r--   0        0        0    12786 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/examples/slate-demo-explicit.ipynb
--rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/examples/slate-demo-explicit2.ipynb
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter-config/server-config/jupyter_firefly_extensions.json
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/_version.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/handlers.py
--rw-r--r--   0        0        0    20800 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/build_log.json
--rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/package.json
--rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/lib_index_js.c1d115cfda38af519d09.js
--rw-r--r--   0        0        0    32908 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/lib_index_js.c1d115cfda38af519d09.js.map
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map
--rw-r--r--   0        0        0    30297 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/remoteEntry.cc1485ece5d30f69b3de.js
--rw-r--r--   0        0        0    29228 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/remoteEntry.cc1485ece5d30f69b3de.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/style.js
--rw-r--r--   0        0        0    19650 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js
--rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map
--rw-r--r--   0        0        0    60655 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js
--rw-r--r--   0        0        0    85321 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/tests/__init__.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/tests/test_handlers.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/src/FireflyCommonUtils.js
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/src/FitsViewerExt.js
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/src/SlateCommandExt.js
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/src/handler.ts
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/src/index.ts
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/src/svg.d.ts
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/style/base.css
--rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/style/fftools-logo.svg
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/style/index.js
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/.gitignore
--rwxr-xr-x   0        0        0     4417 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/README.md
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/.yarnrc.yml
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/License.txt
+-rw-r--r--   0        0        0   541440 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/W4 (1).fits
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/conftest.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/install.json
+-rwxr-xr-x   0        0        0     2995 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/new-release-procedure.md
+-rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/setup.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/tsconfig.json
+-rw-r--r--   0        0        0   188187 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/yarn.lock
+-rw-r--r--   0        0        0    12786 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit2.ipynb
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter-config/server-config/jupyter_firefly_extensions.json
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/_version.py
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/handlers.py
+-rw-r--r--   0        0        0    22079 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/build_log.json
+-rw-r--r--   0        0        0     5978 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/package.json
+-rw-r--r--   0        0        0    67539 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js
+-rw-r--r--   0        0        0    33304 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js.map
+-rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.500e363702a4f528a942.js
+-rw-r--r--   0        0        0    34197 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.500e363702a4f528a942.js.map
+-rw-r--r--   0        0        0    67539 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.7646a236feb88a665a4b.js
+-rw-r--r--   0        0        0    34026 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.7646a236feb88a665a4b.js.map
+-rw-r--r--   0        0        0    68653 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d1c31609190d65e955f6.js
+-rw-r--r--   0        0        0    34277 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d1c31609190d65e955f6.js.map
+-rw-r--r--   0        0        0    68172 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d679203f6e645e4e72b0.js
+-rw-r--r--   0        0        0    33714 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.d679203f6e645e4e72b0.js.map
+-rw-r--r--   0        0        0    68653 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.eebc69299ba593b23ce5.js
+-rw-r--r--   0        0        0    33794 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.eebc69299ba593b23ce5.js.map
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map
+-rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.284b55f4388674029ec0.js.map
+-rw-r--r--   0        0        0    29475 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.53df49ccb005af25f721.js.map
+-rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.a7d5002bd2d65a12a265.js.map
+-rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.bd0f9e95d8cbaf017e34.js.map
+-rw-r--r--   0        0        0    30759 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.d65ffc2462e0ee205d4e.js
+-rw-r--r--   0        0        0    29694 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.d65ffc2462e0ee205d4e.js.map
+-rw-r--r--   0        0        0    29475 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.f552d540a624c45383fa.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style.js
+-rw-r--r--   0        0        0    19650 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js
+-rw-r--r--   0        0        0    15207 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map
+-rw-r--r--   0        0        0    60655 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js
+-rw-r--r--   0        0        0    85321 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/tests/__init__.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/tests/test_handlers.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/FireflyCommonUtils.js
+-rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/FitsViewerExt.js
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/SlateCommandExt.js
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/handler.ts
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/index.ts
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/src/svg.d.ts
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/base.css
+-rw-r--r--   0        0        0    40698 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/fftools-logo.svg
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/style/index.js
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/.gitignore
+-rwxr-xr-x   0        0        0     4954 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/README.md
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 jupyter_firefly_extensions-4.1.1/PKG-INFO
```

### Comparing `jupyter_firefly_extensions-4.1.0/License.txt` & `jupyter_firefly_extensions-4.1.1/License.txt`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/W4 (1).fits` & `jupyter_firefly_extensions-4.1.1/W4 (1).fits`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/new-release-procedure.md` & `jupyter_firefly_extensions-4.1.1/new-release-procedure.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,34 @@
    - From the root directory of package, run:
         ```bash
         pip install --upgrade build
         python -m build
         ```
    - check it: `ls dist` should show two files a `.tar.gz` file and a `.whl` file
 5. _Optional_ - At this point you could do an optional test installation ([see below](#optional-test-installation))
-6. Upload to PYPI  
-    ```bash
-    pip install --upgrade twine
-    twine upload dist/*
-    ```
+
+6. Upload to PYPI
+   1. _One-time-only auth setup:_ Login to pypi and then in your account settings, go to the API tokens section and select "Add API token". Give it any name and select scope to project:jupyter-firefly-extensions and create token. To save this token for later uses, make sure to create a `$HOME/.pypirc` file (or update it if you already have it) with the following:
+      ```ini
+      [distutils]
+      index-servers =
+         jupyter-firefly-extensions
+
+      [jupyter-firefly-extensions]
+      repository = https://upload.pypi.org/legacy/
+      username = __token__
+      password = pypi-token-you-created
+      ```
+
+   2. Upload dist to pypi using twine (with the auth setup in previous step)
+      ```bash
+      pip install --upgrade twine
+      twine upload dist/* --repository jupyter-firefly-extensions
+      ```
+
 7. If any files were edited (i.e `package.json`):
    - `git commit -a`
    - `git push origin master`
 8. Tag
    -  `git tag -a version-#.#.#`  (replace version number with the current version from `package.json`)
 9. Push tags
    - `git push --tags`
```

### Comparing `jupyter_firefly_extensions-4.1.0/package.json` & `jupyter_firefly_extensions-4.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'version'": "'4.1.1'"}*

```diff
@@ -190,12 +190,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.1.0",
+    "version": "4.1.1",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `jupyter_firefly_extensions-4.1.0/tsconfig.json` & `jupyter_firefly_extensions-4.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/yarn.lock` & `jupyter_firefly_extensions-4.1.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -4968,19 +4968,19 @@
     tsserver: bin/tsserver
   checksum: 82b94da3f4604a8946da585f7d6c3025fff8410779e5bde2855ab130d05e4fd08938b9e593b6ebed165bda6ad9292b230984f10952cf82f0a0ca07bbeaa08172
   languageName: node
   linkType: hard
 
 "typescript@patch:typescript@~5.0.2#~builtin<compat/typescript>":
   version: 5.0.4
-  resolution: "typescript@patch:typescript@npm%3A5.0.4#~builtin<compat/typescript>::version=5.0.4&hash=b5f058"
+  resolution: "typescript@patch:typescript@npm%3A5.0.4#~builtin<compat/typescript>::version=5.0.4&hash=85af82"
   bin:
     tsc: bin/tsc
     tsserver: bin/tsserver
-  checksum: d26b6ba97b6d163c55dbdffd9bbb4c211667ebebc743accfeb2c8c0154aace7afd097b51165a72a5bad2cf65a4612259344ff60f8e642362aa1695c760d303ac
+  checksum: bb309d320c59a26565fb3793dba550576ab861018ff3fd1b7fccabbe46ae4a35546bc45f342c0a0b6f265c801ccdf64ffd68f548f117ceb7f0eac4b805cd52a9
   languageName: node
   linkType: hard
 
 "typestyle@npm:^2.0.4":
   version: 2.4.0
   resolution: "typestyle@npm:2.4.0"
   dependencies:
```

### Comparing `jupyter_firefly_extensions-4.1.0/examples/slate-demo-explicit.ipynb` & `jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/examples/slate-demo-explicit2.ipynb` & `jupyter_firefly_extensions-4.1.1/examples/slate-demo-explicit2.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/__init__.py` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/handlers.py` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     Called when the extension is loaded.
 
     Args:
         nb_server_app (NotebookWebApplication): handle to the Notebook webserver instance.
     """
     global firefly_config
     web_app = server_app.web_app
-    config_url = server_app.config.get('Firefly', {}).get('url', '')
+    config_url = server_app.config.get('Firefly', {}).get('url', 'http://localhost:8080/firefly')
     url = None
     if 'FIREFLY_URL' in os.environ:
         url = os.environ['FIREFLY_URL']
     if not url:
         url = config_url
 
     web_app.settings['fireflyURL'] = url
```

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/build_log.json` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/build_log.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998676818094135%*

 * *Differences: {'0': "{'plugins': {1: {'_options': {'shared': {'@jupyterlab/application': {'requiredVersion': "*

 * *      "'^4.1.6'}, '@jupyterlab/application-extension': {'requiredVersion': '^4.1.6'}, "*

 * *      "'@jupyterlab/apputils-extension': {'requiredVersion': '^4.1.6'}, "*

 * *      "'@jupyterlab/cell-toolbar-extension': {'requiredVersion': '^4.1.6'}, "*

 * *      "'@jupyterlab/celltags-extension': {'requiredVersion': '^4.1.6'}, "*

 * *      "'@jupyterlab/codemirror-extension': {'requiredVersion': '^4.1.6'}, "*

 * *      "'@jupyterlab/compl […]*

```diff
@@ -129,418 +129,446 @@
                             "singleton": true
                         },
                         "@codemirror/view": {
                             "import": false,
                             "requiredVersion": "^6.9.6",
                             "singleton": true
                         },
+                        "@jupyter/react-components": {
+                            "import": false,
+                            "requiredVersion": "^0.13.3",
+                            "singleton": true
+                        },
+                        "@jupyter/web-components": {
+                            "import": false,
+                            "requiredVersion": "^0.13.3",
+                            "singleton": true
+                        },
                         "@jupyter/ydoc": {
                             "import": false,
-                            "requiredVersion": "^1.0.2",
+                            "requiredVersion": "^1.1.1",
                             "singleton": true
                         },
                         "@jupyterlab/application": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/application-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/apputils": {
                             "import": false,
-                            "requiredVersion": "^4.1.5",
+                            "requiredVersion": "^4.2.6",
                             "singleton": true
                         },
                         "@jupyterlab/apputils-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/attachments": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/cell-toolbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/cell-toolbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/cells": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/celltags-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/codeeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/codemirror-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/completer": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/completer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/console": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/console-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/coreutils": {
                             "import": false,
-                            "requiredVersion": "^6.0.5",
+                            "requiredVersion": "^6.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/csvviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/csvviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/debugger": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/debugger-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/docmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/docmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/docregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/documentsearch": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/documentsearch-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/extensionmanager": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/extensionmanager-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/filebrowser": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/filebrowser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/fileeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/fileeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/help-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/htmlviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/htmlviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/hub-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/imageviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/imageviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/inspector-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/javascript-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/json-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/launcher": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/launcher-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/logconsole": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/logconsole-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/lsp": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/lsp-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/mainmenu": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/mainmenu-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/markdownviewer": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/markdownviewer-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/markedparser-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/mathjax-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
+                        },
+                        "@jupyterlab/mermaid": {
+                            "import": false,
+                            "requiredVersion": "^4.1.6",
+                            "singleton": true
+                        },
+                        "@jupyterlab/mermaid-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/metadataform": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/metadataform-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/metapackage": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/nbconvert-css": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/nbformat": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/notebook": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/notebook-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/observables": {
                             "import": false,
-                            "requiredVersion": "^5.0.5"
+                            "requiredVersion": "^5.1.6"
                         },
                         "@jupyterlab/outputarea": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/pdf-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
+                        },
+                        "@jupyterlab/pluginmanager": {
+                            "import": false,
+                            "requiredVersion": "^4.1.6",
+                            "singleton": true
+                        },
+                        "@jupyterlab/pluginmanager-extension": {
+                            "import": false,
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/property-inspector": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/rendermime": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/rendermime-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/rendermime-interfaces": {
                             "import": false,
-                            "requiredVersion": "^3.8.5",
+                            "requiredVersion": "^3.9.6",
                             "singleton": true
                         },
                         "@jupyterlab/running": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/running-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/services": {
                             "import": false,
-                            "requiredVersion": "^7.0.5",
+                            "requiredVersion": "^7.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/settingeditor-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/settingregistry": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/shortcuts-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/statedb": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/statusbar-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/terminal": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/terminal-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/theme-dark-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/theme-light-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/toc": {
                             "import": false,
-                            "requiredVersion": "^6.0.5",
+                            "requiredVersion": "^6.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/toc-extension": {
                             "import": false,
-                            "requiredVersion": "^6.0.5"
+                            "requiredVersion": "^6.1.6"
                         },
                         "@jupyterlab/tooltip": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/tooltip-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/translation": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/translation-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/ui-components": {
                             "import": false,
-                            "requiredVersion": "^4.0.5",
+                            "requiredVersion": "^4.1.6",
                             "singleton": true
                         },
                         "@jupyterlab/ui-components-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@jupyterlab/vega5-extension": {
                             "import": false,
-                            "requiredVersion": "^4.0.5"
+                            "requiredVersion": "^4.1.6"
                         },
                         "@lezer/common": {
                             "import": false,
                             "requiredVersion": "^1.0.0",
                             "singleton": true
                         },
                         "@lezer/highlight": {
@@ -551,30 +579,30 @@
                         "@lumino/algorithm": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/application": {
                             "import": false,
-                            "requiredVersion": "^2.0.1",
+                            "requiredVersion": "^2.3.0-alpha.0",
                             "singleton": true
                         },
                         "@lumino/commands": {
                             "import": false,
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "@lumino/coreutils": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/datagrid": {
                             "import": false,
-                            "requiredVersion": "^2.0.1",
+                            "requiredVersion": "^2.3.0-alpha.0",
                             "singleton": true
                         },
                         "@lumino/disposable": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
@@ -616,23 +644,33 @@
                         "@lumino/virtualdom": {
                             "import": false,
                             "requiredVersion": "^2.0.0",
                             "singleton": true
                         },
                         "@lumino/widgets": {
                             "import": false,
-                            "requiredVersion": "^2.0.1",
+                            "requiredVersion": "^2.3.1-alpha.0",
+                            "singleton": true
+                        },
+                        "@microsoft/fast-element": {
+                            "import": false,
+                            "requiredVersion": "^1.12.0",
+                            "singleton": true
+                        },
+                        "@microsoft/fast-foundation": {
+                            "import": false,
+                            "requiredVersion": "^2.49.2",
                             "singleton": true
                         },
                         "b64-to-blob": {},
                         "firefly-api-access": {},
                         "jupyter_firefly_extensions": {
                             "import": "/Users/jsinghal/dev/cm/jupyter_firefly_extensions/lib/index.js",
                             "singleton": true,
-                            "version": "4.0.0"
+                            "version": "4.1.0"
                         },
                         "lodash": {},
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
```

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/package.json` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9795833333333333%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d65ffc2462e0ee205d4e.js'}}",*

 * * "'version'": "'4.1.0'"}*

```diff
@@ -110,15 +110,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/Caltech-IPAC/jupyter_firefly_extensions",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.cc1485ece5d30f69b3de.js",
+            "load": "static/remoteEntry.d65ffc2462e0ee205d4e.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_firefly_extensions"
                 },
@@ -195,12 +195,12 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "4.0.0",
+    "version": "4.1.0",
     "workspaces": [
         "ui-tests"
     ]
 }
```

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/lib_index_js.c1d115cfda38af519d09.js.map` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/lib_index_js.30945f690cca6de2b14f.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8285714285714285%*

 * *Differences: {"'file'": "'lib_index_js.30945f690cca6de2b14f.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;;;;;AAA+C;AAG/C,IAAI,SAAS,CAAC;AACd,IAAI,uBAAuB,CAAC;AAC5B,MAAM,QAAQ,GAAE,eAAe,CAAC,qBAAqB,CAAC,CAAC;AACvD,MAAM,YAAY,GAAE;IAChB,MAAM,EAAE,KAAK;IACb,IAAI,EAAE,MAAM;IACZ,WAAW,EAAE,SAAS;IACtB,KAAK,EAAE,SAAS;IAChB,OAAO,EAAE,EAAE,kBAAkB,EAAE,gBAAgB,EAAE;CACpD,CAAC;AAEF;;;;GAIG;AACI,KAAK,UAAU,WAAW;;IAC7B,IAAI,uBAAuB;QAAE,OAAO,uBAAuB,CAAC;IAE5D,IAAI;QACA,IAAI,CAAC,SAAS;YAAE,SAAS,GAAE,MAAM,CAAC,MAAM,KAAK,CAAC,QAAQ,EAAE,YAAY,CAAC,CAAC […]*

```diff
@@ -1,19 +1,19 @@
 {
-    "file": "lib_index_js.c1d115cfda38af519d09.js",
-    "mappings": "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",
+    "file": "lib_index_js.30945f690cca6de2b14f.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter_firefly_extensions/./src/FireflyCommonUtils.js",
         "webpack://jupyter_firefly_extensions/./src/FitsViewerExt.js",
         "webpack://jupyter_firefly_extensions/./src/SlateCommandExt.js",
         "webpack://jupyter_firefly_extensions/./src/index.ts"
     ],
     "sourcesContent": [
         "import {initFirefly} from 'firefly-api-access';\n\n\nlet cachedLoc;\nlet cachedFindFireflyResult;\nconst ffLocURL= makeLabEndpoint('lab/fireflyLocation');\nconst fetchOptions= {\n    method: 'get',\n    mode: 'cors',\n    credentials: 'include',\n    cache: 'default',\n    headers: { 'X-Requested-With': 'XMLHttpRequest' }\n};\n\n/**\n * Determine where firefly is my calling the lab server extension then load firefly.\n * Results are cache so this function can be call many times.\n * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}\n */\nexport async function findFirefly()  {\n    if (cachedFindFireflyResult) return cachedFindFireflyResult;\n\n    try {\n        if (!cachedLoc) cachedLoc= await (await fetch(ffLocURL, fetchOptions)).json();\n\n        const {fireflyURL='http://localhost:8080/firefly', fireflyChannel:channel}= cachedLoc;\n        if (!window.firefly?.initialized) window.firefly= {...window.firefly, wsch:channel};\n        if (!window.getFireflyAPI) window.getFireflyAPI= initFirefly(fireflyURL);\n        const firefly= await window.getFireflyAPI();\n        cachedFindFireflyResult= {fireflyURL, channel, firefly};\n        return cachedFindFireflyResult;\n    }\n    catch (e) {\n        console.group('Firefly Load Failed');\n        console.log('findFirefly: Could not determine firefly location or load firefly, call failed');\n        console.log(`find firefly url: ${ffLocURL}`);\n        if (cachedLoc) console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.channel}`);\n        console.log(e);\n        console.groupEnd('Firefly Load Failed');\n    }\n\n}\n\n\n\nexport function buildURLErrorHtml(e) {\n    const details= `<br>Set the firefly URL by setting <code>c.Firefly.url</code> in \n                    <code>jupyter_notebook_config.py</code>\n                    <br>or the environment variable <code>FIREFLY_URL</code>`;\n    return `<div style='padding: 30px 0 0 30px'>${e.message}${details}</div>`;\n}\n\n\nexport function makeLabEndpoint(endPoint, searchParams) {\n    const {origin,pathname}= new URL(window.document.location.href);\n    const originURL= origin + pathname;\n    const start= originURL.substring(0, originURL.lastIndexOf('lab'))\n    const slashMaybe= start.endsWith('/') ? '' : '/';\n    return `${start}${slashMaybe}${endPoint}${searchParams?'?'+searchParams.toString():''}`\n}",
         "import b64toBlob from 'b64-to-blob';\nimport {buildURLErrorHtml, findFirefly, makeLabEndpoint} from './FireflyCommonUtils.js';\nimport { Widget } from '@lumino/widgets';\nimport { ABCWidgetFactory, DocumentWidget} from '@jupyterlab/docregistry';\nimport { PageConfig} from '@jupyterlab/coreutils';\n\n\nexport const FITS_MIME_TYPE = 'application/fits';\n\n\n/**\n * The class name added to the extension.\n */\nconst CLASS_NAME = 'jp-OutputWidgetFITS';\n\nlet idCounter=0;\n\nconst FACTORY = 'FITS-IMAGE';\n\n\nconst fitsIFileType= {\n    name: 'FITS',\n    displayName: 'FITS file',\n    fileFormat: 'base64',  // TODO: try putting a null here to keep from loading file, the might be the answer\n                           // will need to check the JL version someway\n    format: 'base64',\n    mimeTypes: [FITS_MIME_TYPE],\n    extensions: ['.fits']\n};\n\n/**\n *\n * @param {JupyterLab} app\n * @param {ILayoutRestorer} restorer\n */\nexport function activateFitsViewerExt(app, restorer) {\n    const namespace = 'firefly-imageviewer-widget';\n    const jlVersion= PageConfig.getOption('appVersion');\n    const vAry= jlVersion?.split('.').map( (x) => Number(x)) ?? [0,0,0];\n\n    // if Jupyter Lab version is 3.1 or greater then clear the fileFormat so it does not load the file on the client\n    // see - https://github.com/jupyterlab/jupyterlab/pull/7596\n    if (vAry[0] >=3 && vAry[1] >= 1) fitsIFileType.fileFormat= null;\n\n    app.docRegistry.addFileType(fitsIFileType);\n    const factory = new ABCWidgetFactory({\n        name: FACTORY,\n        modelName: 'base64',\n        // modelName: 'fits-model',\n        fileTypes: ['FITS'],\n        defaultFor: ['FITS'],\n        readOnly: true\n    });\n    factory.createNewWidget= createNewFitsViewerDocumentWidget;\n    app.docRegistry.addWidgetFactory(factory);\n\n    factory.widgetCreated.connect((sender, widget) => {\n        const types = app.docRegistry.getFileTypesForPath(widget.context.path);\n\n        if (types.length) {\n            widget.title.iconClass = types[0].iconClass || '';\n            widget.title.iconLabel = types[0].iconLabel || '';\n        }\n    });\n}\n\n\n\n\n\nexport function createNewFitsViewerDocumentWidget(context) {\n    // instead of extending DocumentWidget like the example, just use it directly\n    return new DocumentWidget({ content:new FitsViewerWidget(context), context, reveal:true, toolbar:null });\n}\n\n/**\n * A widget for rendering FITS.\n */\nexport class FitsViewerWidget extends Widget {\n    /**\n     * Construct a new output widget.\n     * @param context\n     */\n    constructor(context) {\n        super({ node: createNode(context._path) });\n        const useModel= window.firefly && window.firefly.jlExtUseModel || false;\n        this.addClass(CLASS_NAME);\n        this.filename= context._path;\n        idCounter++;\n        this.plotId= `${this.filename}-${idCounter}`;\n        this.loaded= false;\n        if (this.isDisposed) return;\n        this.renderModel(context,useModel).then(() => {\n        });\n        context.model.contentChanged.connect( this.renderModel, this );\n        context.fileChanged.connect( this.renderModel, this );\n    }\n\n    /**\n     * Render FITS into this widget's node.\n     * @param context\n     * @param useModelFirst\n     * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}\n     */\n    renderModel(context, useModelFirst) {\n\n        if (this.isDisposed) return;\n\n        if (this.loaded) {\n            return findFirefly()\n                .then( (ffConfig) => ffConfig.firefly.action.dispatchChangeActivePlotView(this.plotId) );\n        }\n\n        let firefly, fireflyURL;\n        return findFirefly()\n            .then( (ffConfig) => {\n                firefly= ffConfig.firefly;\n                fireflyURL= ffConfig.fireflyURL;\n                if (useModelFirst) {\n                    return context.ready.then(() => loadFileToServer(context.model.toString(), this.filename, firefly, fireflyURL));\n                }\n                else {\n                    return tellLabToLoadFileToServer(this.filename, firefly);\n                }\n            } )\n            .then( (response) => response.text())\n            .then( (text) => {\n                if (useModelFirst) {\n                    const [, cacheKey] = text.split('::::');\n                    showImage(cacheKey,this.plotId, this.filename, firefly);\n                }\n                else {\n                    if (text && text.length<300 && text.startsWith('${')) {\n                        showImage(text,this.plotId, this.filename, firefly);\n                    }\n                    else {\n                        console.log('Firefly FitsViewExt: Failed to upload from server, ' +\n                                          'falling back to (slower) browser upload.');\n                        context.ready.then(() => loadFileToServer(context.model.toString(), this.filename, firefly, fireflyURL))\n                            .then( (response) => response.text())\n                            .then( (text) => {\n                                const [, cacheKey] = text.split('::::');\n                                showImage(cacheKey, this.plotId, this.filename, firefly);\n                            });\n                    }\n                }\n                this.loaded= true;\n            })\n            .catch( (e) => {\n                const div= document.getElementById(this.filename);\n                if (div) div.innerHTML=buildURLErrorHtml(e);\n            });\n    }\n\n    dispose() {\n        return findFirefly()\n            .then( (ffConfig) => ffConfig.firefly.action.dispatchDeletePlotView({plotId:this.plotId, holdWcsMatch:true}) );\n\n    }\n\n    activate() {\n        super.activate();\n        if (this.loaded) {\n            return findFirefly().then( (ffConfig) => ffConfig.firefly.action.dispatchChangeActivePlotView(this.plotId) );\n        }\n    }\n}\n\n\nfunction tellLabToLoadFileToServer( path, firefly) {\n    const url= makeLabEndpoint('lab/sendToFirefly', new URLSearchParams({'path':path}));\n    return firefly.util.fetchUrl(url,{ method: 'GET' },false, false)\n        .catch( (e) => {\n            console.error('Firefly FitsViewExt: Got Error from upload request',e);\n            return 'FAILED';\n        });\n}\n\n\nfunction loadFileToServer( fileData, filename, firefly, fireflyURL) {\n    const {fetchUrl, ServerParams}= firefly.util;\n    const UL_URL = `${fireflyURL}/sticky/CmdSrv?${ServerParams.COMMAND}=${ServerParams.UPLOAD}&filename=${filename}`;\n    const fitsBlob= b64toBlob(fileData);\n    const options = { method: 'multipart', params: { filename, type:'FITS', file: fitsBlob } };\n    return fetchUrl(UL_URL, options);\n}\n\nfunction showImage(cacheKey, plotId, filename, firefly) {\n    const req= {\n        type     : 'FILE',\n        FILE     : cacheKey,\n        plotId,\n        plotGroupId: 'JUPLAB',\n        title: filename\n    };\n    firefly.action.dispatchApiToolsView(true, false);\n    firefly.setGlobalPref({imageDisplayType: 'encapusulate'});\n    firefly.showImage(filename, req, null, false);\n}\n\nfunction createNode(filename) {\n    const node = document.createElement('div');\n    node.id= filename;\n    return node;\n}\n\n//=========================================================================================================\n//============ Keep code below for reference\n//============ Keep code below for reference\n//============ Keep code below for reference\n\n\n// /**\n//  * A mime renderer factory for FITS data.\n//  */\n// export const fitsViewerRendererFactory = {\n//     safe: true,\n//     mimeTypes: [FITS_MIME_TYPE],\n//     createRenderer: options => {\n//         return new FitsViewerWidget (options);\n//     }\n// };\n\n\n\n// import { ABCWidgetFactory, DocumentRegistry, DocumentWidget, IDocumentWidget } from '@jupyterlab/docregistry';\n// import { PageConfig, URLExt } from '@jupyterlab/coreutils';\n\n\n// const ERROR_MSG_CONT= `Make sure you set the firefly URL in your jupyter_notebook_config.py.\n//                 For example- 'c.Firefly.url= http://some.firefly.url/firefly'`;\n\n// for adding a second extension for a mime type - does not work yet in Jupyter Lab\n// --- https://github.com/jupyterlab/jupyterlab/issues/5381\n// export const fitsViewerRendererFactory2 = {\n//     safe: true,\n//     mimeTypes: [FITS_MIME_TYPE],\n//     createRenderer: options => {\n//         return new FitsViewerWidget (options);\n//     }\n// };\n\n\n// export class FitsViewerDocument extends DocumentWidget {\n//\n//   constructor(context) {\n//       super({ content:new FitsViewerWidget(context), context, reveal:true, toolbar:null });\n//     // const toolbar = Private.createToolbar(content.viewer);\n//     // const reveal = content.ready;\n//   }\n// }\n\n\n// export class FitsViewerFactory extends ABCWidgetFactory {\n//\n//     constructor(options) {\n//         super(options);\n//     }\n//\n//\n//\n//     /**\n//      * Create a new widget given a context.\n//      * @param context DocumentRegistry.IContext<DocumentRegistry.IModel>\n//      * @return DocumentWidget\n//      */\n//     createNewWidget(context) {\n//         // return new FitsViewerDocument(context);\n//         return new DocumentWidget({ content:new FitsViewerWidget(context), context, reveal:true, toolbar:null });\n//     }\n// }\n\n\n// const a= {\n//     name: 'some-name',\n//     fileTypes: ['csv'],\n//     defaultFor: [],\n//     defaultRendered: [],\n//     readOnly: false,\n//     modelName: 'text',\n//     preferKernel: false,\n//     canStartKernel: false,\n//     widgetCreated: new Signal(null),\n// }\n",
-        "import { Widget } from '@lumino/widgets';\nimport { ICommandPalette, IFrame } from '@jupyterlab/apputils';\nimport { JupyterFrontEnd } from '@jupyterlab/application';\nimport { ILauncher } from '@jupyterlab/launcher';\n\nimport { findFirefly } from './FireflyCommonUtils.js';\n\n\nlet widgetId;\nlet widgetCnt= 1;\nlet openWidgets= {};\n\n\n/**\n * Extension can be started in two ways.\n * 1. as a jupyter command\n * 2. firefly_client sending a 'StartLabWindow' action\n * @param {JupyterFrontEnd} app\n * @param {ICommandPalette} palette\n * @param {ILauncher | null} launcher\n */\nexport function activateSlateCommandExt(app, palette, launcher) {\n    findFirefly().then( (ffConfig) => {\n        const {firefly}= ffConfig;\n        firefly.util.addActionListener(['StartLabWindow'], (action,state) => {\n            openSlateMulti(app, action.payload.renderTreeId, false);\n        });\n        firefly.util.addActionListener(['StartBrowserTab'], (action,state) => {\n            firefly.setViewerConfig(firefly.ViewerType.Grid);\n            firefly.getViewer(action.payload.channel).openViewer();\n        });\n\n    });\n\n    // for starting extension as a jupyter command -----------\n    const command = 'firefly:open-slate';\n    const category = 'Firefly';\n\n    app.commands.addCommand(command, {\n        label: 'Open Firefly',\n        caption: 'Open Firefly',\n        isEnabled: () => true,\n        execute: () => {\n            const id= 'slate-'+ widgetCnt;\n            widgetCnt++;\n            openSlateMulti(app, id, true);\n        }\n    });\n\n    palette.addItem({ command, category });\n    if (launcher) launcher.add({ command, category});\n}\n\nfunction openSlateMulti(app, id, activate) {\n    activate= window.document.getElementById(id) || activate;\n    if (!openWidgets[id]) {\n        let widget = new SlateRootWidget(id);\n        if (app.shell.addToMainArea) app.shell.addToMainArea(widget); // --- pre version 1\n        else if (app.shell.add) app.shell.add(widget, 'main');  // version 1\n        else throw Error('Could not add firefly to tab');\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n        openWidgets[id]= widget;\n    }\n    if (activate) app.shell.activateById(id);\n\n}\n\n\n/**\n * Open only one slate tab.  Using this funtion keeps the slate tab as a singleton.\n *\n * Currently not used.\n * @param app\n */\nfunction openSlateSingleOnly(app) {\n    if (!widgetId) {\n        let widget = new SlateRootWidget('slate-1');\n        app.shell.addToMainArea(widget);\n        widgetId= widget.id;\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n    else {\n\n    }\n    app.shell.activateById(widgetId);\n}\n\n\n\nexport class SlateRootWidget extends Widget {\n    /**\n     * Construct a new output widget.\n     */\n    constructor(id) {\n        super({node: createNode(id)});\n        this.id= id;\n        this.title.label= 'Firefly: '+ id;\n        this.title.closable= true;\n        findFirefly().then( (ffConfig) => {\n            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL);\n        } );\n    }\n\n    startViewer(firefly, id, fireflyURL) {\n        const {util,action}= firefly;\n        const props=  {\n            div: id,\n            renderTreeId: id,\n            template: 'FireflySlate',\n            disableDefaultDropDown: true,\n        };\n        const fallbackMenu= [\n            {label:'Images', action:'ImageSelectDropDownSlateCmd'},\n            {label:'TAP Searches', action: 'TAPSearch'},\n            {label:'Catalogs', action:'IrsaCatalogDropDown'},\n            {label:'Charts', action:'ChartSelectDropDownCmd'},\n            {label:'Upload', action: 'FileUploadDropDownCmd'},\n        ];\n        if (!firefly.originalAppProps) {\n            props.menu= fallbackMenu;\n        }\n        if (fireflyURL.endsWith('irsaviewer')) {\n            // make icon file path absolute, otherwise it won't be found\n            const originalAppIconProp = firefly?.originalAppProps?.appIcon;\n            if (originalAppIconProp) props.appIcon = fireflyURL + '/' + originalAppIconProp;\n            // resize it to fit in its parent container\n            props.bannerLeftStyle = {display: 'flex', marginTop: 'unset'};\n        }\n        action.dispatchApiToolsView(true,false);\n        this.controlApp= util.startAsAppFromApi(id, props);\n    }\n\n    dispose() {\n        widgetId= undefined;\n    }\n    close() {\n        super.close();\n        widgetId= undefined;\n        delete openWidgets[this.id];\n        if (this.controlApp) this.controlApp.unrender();\n        this.controlApp= undefined;\n    }\n\n    activate() {\n        super.activate();\n        if (this.controlApp) {\n            this.controlApp.unrender();\n            this.controlApp.render();\n        }\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n}\n\n\nfunction createNode(filename) {\n    const node = document.createElement('div');\n    node.id= filename;\n    const tmpElement=  document.createElement('div');\n    tmpElement.innerHTML= '<div>Firefly Loading...</div>';\n    node.appendChild(tmpElement);\n    return node;\n}\n",
+        "import { Widget } from '@lumino/widgets';\nimport { ICommandPalette, IFrame } from '@jupyterlab/apputils';\nimport { JupyterFrontEnd } from '@jupyterlab/application';\nimport { ILauncher } from '@jupyterlab/launcher';\nimport { LabIcon } from '@jupyterlab/ui-components';\n\nimport { findFirefly } from './FireflyCommonUtils.js';\nimport fireflyIconStr from '../style/fftools-logo.svg';\n\n\nlet widgetId;\nlet widgetCnt= 1;\nlet openWidgets= {};\n\n\n/**\n * Extension can be started in two ways.\n * 1. as a jupyter command\n * 2. firefly_client sending a 'StartLabWindow' action\n * @param {JupyterFrontEnd} app\n * @param {ICommandPalette} palette\n * @param {ILauncher | null} launcher\n */\nexport function activateSlateCommandExt(app, palette, launcher) {\n    findFirefly().then( (ffConfig) => {\n        const {firefly}= ffConfig;\n        firefly.util.addActionListener(['StartLabWindow'], (action,state) => {\n            openSlateMulti(app, action.payload.renderTreeId, false);\n        });\n        firefly.util.addActionListener(['StartBrowserTab'], (action,state) => {\n            firefly.setViewerConfig(firefly.ViewerType.Grid);\n            firefly.getViewer(action.payload.channel).openViewer();\n        });\n\n    });\n\n    // for starting extension as a jupyter command -----------\n    const command = 'firefly:open-slate';\n    const category = 'Firefly';\n    const icon = new LabIcon({\n        name: 'jupyter_firefly_extensions:firefly-icon',\n        svgstr: fireflyIconStr\n      }); \n\n    app.commands.addCommand(command, {\n        label: 'Open Firefly',\n        caption: 'Open Firefly',\n        icon: icon,\n        isEnabled: () => true,\n        execute: () => {\n            const id= 'slate-'+ widgetCnt;\n            widgetCnt++;\n            openSlateMulti(app, id, true);\n        }\n    });\n\n    palette.addItem({ command, category });\n    if (launcher) launcher.add({ command, category});\n}\n\nfunction openSlateMulti(app, id, activate) {\n    activate= window.document.getElementById(id) || activate;\n    if (!openWidgets[id]) {\n        let widget = new SlateRootWidget(id);\n        if (app.shell.addToMainArea) app.shell.addToMainArea(widget); // --- pre version 1\n        else if (app.shell.add) app.shell.add(widget, 'main');  // version 1\n        else throw Error('Could not add firefly to tab');\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n        openWidgets[id]= widget;\n    }\n    if (activate) app.shell.activateById(id);\n\n}\n\n\n/**\n * Open only one slate tab.  Using this funtion keeps the slate tab as a singleton.\n *\n * Currently not used.\n * @param app\n */\nfunction openSlateSingleOnly(app) {\n    if (!widgetId) {\n        let widget = new SlateRootWidget('slate-1');\n        app.shell.addToMainArea(widget);\n        widgetId= widget.id;\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n    else {\n\n    }\n    app.shell.activateById(widgetId);\n}\n\n\n\nexport class SlateRootWidget extends Widget {\n    /**\n     * Construct a new output widget.\n     */\n    constructor(id) {\n        super({node: createNode(id)});\n        this.id= id;\n        this.title.label= 'Firefly: '+ id;\n        this.title.closable= true;\n        findFirefly().then( (ffConfig) => {\n            this.startViewer(ffConfig.firefly, id, ffConfig.fireflyURL);\n        } );\n    }\n\n    startViewer(firefly, id, fireflyURL) {\n        const {util,action}= firefly;\n        const props=  {\n            div: id,\n            renderTreeId: id,\n            template: 'FireflySlate',\n            disableDefaultDropDown: true,\n        };\n        const fallbackMenu= [\n            {label:'Images', action:'ImageSelectDropDownSlateCmd'},\n            {label:'TAP Searches', action: 'TAPSearch'},\n            {label:'Catalogs', action:'IrsaCatalogDropDown'},\n            {label:'Charts', action:'ChartSelectDropDownCmd'},\n            {label:'Upload', action: 'FileUploadDropDownCmd'},\n        ];\n        if (!firefly.originalAppProps) {\n            props.menu= fallbackMenu;\n        }\n        if (fireflyURL.endsWith('irsaviewer')) {\n            // make icon file path absolute, otherwise it won't be found\n            const originalAppIconProp = firefly?.originalAppProps?.appIcon;\n            if (originalAppIconProp) props.appIcon = fireflyURL + '/' + originalAppIconProp;\n            // resize it to fit in its parent container\n            props.bannerLeftStyle = {display: 'flex', marginTop: 'unset'};\n        }\n        action.dispatchApiToolsView(true,false);\n        this.controlApp= util.startAsAppFromApi(id, props);\n    }\n\n    dispose() {\n        widgetId= undefined;\n    }\n    close() {\n        super.close();\n        widgetId= undefined;\n        delete openWidgets[this.id];\n        if (this.controlApp) this.controlApp.unrender();\n        this.controlApp= undefined;\n    }\n\n    activate() {\n        super.activate();\n        if (this.controlApp) {\n            this.controlApp.unrender();\n            this.controlApp.render();\n        }\n        findFirefly().then( (ffConfig) => {\n            const {action}= ffConfig.firefly;\n            action.dispatchChangeActivePlotView(undefined);\n        });\n    }\n}\n\n\nfunction createNode(filename) {\n    const node = document.createElement('div');\n    node.id= filename;\n    const tmpElement=  document.createElement('div');\n    tmpElement.innerHTML= '<div>Firefly Loading...</div>';\n    node.appendChild(tmpElement);\n    return node;\n}\n",
         "import { JupyterFrontEndPlugin, ILayoutRestorer } from '@jupyterlab/application';\nimport { ICommandPalette } from '@jupyterlab/apputils';\nimport { ILauncher } from '@jupyterlab/launcher';\n\n\nimport { activateSlateCommandExt } from './SlateCommandExt.js';\nimport { activateFitsViewerExt } from './FitsViewerExt.js';\n\n/**\n * Initialization data for each extension.\n */\nconst showSlateExt: JupyterFrontEndPlugin<void> = {\n  id: 'jupyter_firefly_extensions:showSlate',\n  description: 'Show firefly slate',\n  autoStart: true,\n  requires: [ICommandPalette],\n  optional: [ILauncher],\n  activate: activateSlateCommandExt\n};\n\nconst fitsViewerExt: JupyterFrontEndPlugin<void> = {\n  id: 'jupyter_firefly_extensions:fitsviewer',\n  description: 'View a FITS file',\n  autoStart: true,\n  requires: [ILayoutRestorer],\n  activate: activateFitsViewerExt\n};\n\n// More than one extension/plugin can be exported as a list\nexport default [showSlateExt, fitsViewerExt];\n"
     ],
     "version": 3
 }
```

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/node_modules_b64-to-blob_b64toBlob_js.c490fc7119beea72c47e.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/remoteEntry.cc1485ece5d30f69b3de.js` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.d65ffc2462e0ee205d4e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "c1d115cfda38af519d09",
+                "lib_index_js": "d1c31609190d65e955f6",
                 "style_index_js": "1e1ab72bb82b2e804877",
                 "node_modules_b64-to-blob_b64toBlob_js": "c490fc7119beea72c47e",
                 "vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js": "11d96cd25e15e62dfcc9"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -433,15 +433,15 @@
                 /******/
                 case "default": {
                     /******/
                     register("b64-to-blob", "1.2.19", () => (__webpack_require__.e("node_modules_b64-to-blob_b64toBlob_js").then(() => (() => (__webpack_require__( /*! ./node_modules/b64-to-blob/b64toBlob.js */ "./node_modules/b64-to-blob/b64toBlob.js"))))));
                     /******/
                     register("firefly-api-access", "0.0.4", () => (__webpack_require__.e("vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js").then(() => (() => (__webpack_require__( /*! ./node_modules/firefly-api-access/distribution/firefly-api-access.min.js */ "./node_modules/firefly-api-access/distribution/firefly-api-access.min.js"))))));
                     /******/
-                    register("jupyter_firefly_extensions", "4.0.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyter_firefly_extensions", "4.1.0", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -834,29 +834,33 @@
             /******/
         });
         /******/
         var installedModules = {};
         /******/
         var moduleToHandlerMapping = {
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 0, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/application": () => (loadSingletonVersionCheck("default", "@jupyterlab/application", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 1, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/apputils": () => (loadSingletonVersionCheck("default", "@jupyterlab/apputils", [1, 4, 2, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 0, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/launcher": () => (loadSingletonVersionCheck("default", "@jupyterlab/launcher", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 0, 1])),
+            "webpack/sharing/consume/default/@lumino/widgets": () => (loadSingletonVersionCheck("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0])),
+            /******/
+            "webpack/sharing/consume/default/@jupyterlab/ui-components": () => (loadSingletonVersionCheck("default", "@jupyterlab/ui-components", [1, 4, 1, 6])),
             /******/
             "webpack/sharing/consume/default/firefly-api-access/firefly-api-access": () => (loadStrictVersionCheckFallback("default", "firefly-api-access", [4, 0, 0, 4], () => (__webpack_require__.e("vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js").then(() => (() => (__webpack_require__( /*! firefly-api-access */ "./node_modules/firefly-api-access/distribution/firefly-api-access.min.js"))))))),
             /******/
+            "webpack/sharing/consume/default/@jupyterlab/services": () => (loadSingletonVersionCheck("default", "@jupyterlab/services", [1, 7, 1, 6])),
+            /******/
             "webpack/sharing/consume/default/b64-to-blob/b64-to-blob": () => (loadStrictVersionCheckFallback("default", "b64-to-blob", [1, 1, 2, 19], () => (__webpack_require__.e("node_modules_b64-to-blob_b64toBlob_js").then(() => (() => (__webpack_require__( /*! b64-to-blob */ "./node_modules/b64-to-blob/b64toBlob.js"))))))),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/docregistry": () => (loadVersionCheck("default", "@jupyterlab/docregistry", [1, 4, 0, 5])),
+            "webpack/sharing/consume/default/@jupyterlab/docregistry": () => (loadVersionCheck("default", "@jupyterlab/docregistry", [1, 4, 1, 6])),
             /******/
-            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 0, 5]))
+            "webpack/sharing/consume/default/@jupyterlab/coreutils": () => (loadSingletonVersionCheck("default", "@jupyterlab/coreutils", [1, 6, 1, 6]))
             /******/
         };
         /******/ // no consumes in initial chunks
         /******/
         var chunkMapping = {
             /******/
             "lib_index_js": [
@@ -865,16 +869,20 @@
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/apputils",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/launcher",
                 /******/
                 "webpack/sharing/consume/default/@lumino/widgets",
                 /******/
+                "webpack/sharing/consume/default/@jupyterlab/ui-components",
+                /******/
                 "webpack/sharing/consume/default/firefly-api-access/firefly-api-access",
                 /******/
+                "webpack/sharing/consume/default/@jupyterlab/services",
+                /******/
                 "webpack/sharing/consume/default/b64-to-blob/b64-to-blob",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/docregistry",
                 /******/
                 "webpack/sharing/consume/default/@jupyterlab/coreutils"
                 /******/
             ]
@@ -1106,8 +1114,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyter_firefly_extensions");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyter_firefly_extensions = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.cc1485ece5d30f69b3de.js.map
+//# sourceMappingURL=remoteEntry.d65ffc2462e0ee205d4e.js.map
```

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/remoteEntry.cc1485ece5d30f69b3de.js.map` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/remoteEntry.53df49ccb005af25f721.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8367346938775511%*

 * *Differences: {"'file'": "'remoteEntry.53df49ccb005af25f721.js'",*

 * * "'mappings'": "';;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "remoteEntry.cc1485ece5d30f69b3de.js",
-    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qPAAqP;WACnR;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC/CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCxLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
+    "file": "remoteEntry.53df49ccb005af25f721.js",
+    "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,qPAAqP;WACnR;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC/CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1LA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyter_firefly_extensions/webpack/container-entry",
         "webpack://jupyter_firefly_extensions/webpack/bootstrap",
         "webpack://jupyter_firefly_extensions/webpack/runtime/compat get default export",
         "webpack://jupyter_firefly_extensions/webpack/runtime/define property getters",
@@ -25,22 +25,22 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn __webpack_require__.e(\"style_index_js\").then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"c1d115cfda38af519d09\",\"style_index_js\":\"1e1ab72bb82b2e804877\",\"node_modules_b64-to-blob_b64toBlob_js\":\"c490fc7119beea72c47e\",\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\":\"11d96cd25e15e62dfcc9\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"7646a236feb88a665a4b\",\"style_index_js\":\"1e1ab72bb82b2e804877\",\"node_modules_b64-to-blob_b64toBlob_js\":\"c490fc7119beea72c47e\",\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\":\"11d96cd25e15e62dfcc9\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyter_firefly_extensions:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter_firefly_extensions\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"b64-to-blob\", \"1.2.19\", () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/b64-to-blob/b64toBlob.js */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))));\n\t\t\tregister(\"firefly-api-access\", \"0.0.4\", () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/firefly-api-access/distribution/firefly-api-access.min.js */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))));\n\t\t\tregister(\"jupyter_firefly_extensions\", \"4.0.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyter_firefly_extensions\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"b64-to-blob\", \"1.2.19\", () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/b64-to-blob/b64toBlob.js */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))));\n\t\t\tregister(\"firefly-api-access\", \"0.0.4\", () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/firefly-api-access/distribution/firefly-api-access.min.js */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))));\n\t\t\tregister(\"jupyter_firefly_extensions\", \"4.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,1,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,0,1])),\n\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\": () => (loadStrictVersionCheckFallback(\"default\", \"firefly-api-access\", [4,0,0,4], () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! firefly-api-access */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))))),\n\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\": () => (loadStrictVersionCheckFallback(\"default\", \"b64-to-blob\", [1,1,2,19], () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! b64-to-blob */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\": () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,4,0,5])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,5]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\",\n\t\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
+        "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/application\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/application\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,2,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/launcher\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/launcher\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@lumino/widgets\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/widgets\", [1,2,3,1,,\"alpha\",0])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\": () => (loadStrictVersionCheckFallback(\"default\", \"firefly-api-access\", [4,0,0,4], () => (__webpack_require__.e(\"vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js\").then(() => (() => (__webpack_require__(/*! firefly-api-access */ \"./node_modules/firefly-api-access/distribution/firefly-api-access.min.js\"))))))),\n\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\": () => (loadStrictVersionCheckFallback(\"default\", \"b64-to-blob\", [1,1,2,19], () => (__webpack_require__.e(\"node_modules_b64-to-blob_b64toBlob_js\").then(() => (() => (__webpack_require__(/*! b64-to-blob */ \"./node_modules/b64-to-blob/b64toBlob.js\"))))))),\n\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\": () => (loadVersionCheck(\"default\", \"@jupyterlab/docregistry\", [1,4,1,6])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,1,6]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/application\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/launcher\",\n\t\t\"webpack/sharing/consume/default/@lumino/widgets\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\",\n\t\t\"webpack/sharing/consume/default/firefly-api-access/firefly-api-access\",\n\t\t\"webpack/sharing/consume/default/b64-to-blob/b64-to-blob\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/docregistry\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyter_firefly_extensions\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyter_firefly_extensions\"] = self[\"webpackChunkjupyter_firefly_extensions\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyter_firefly_extensions\");\n",
         ""
     ],
     "version": 3
```

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/style_index_js.1e1ab72bb82b2e804877.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map` & `jupyter_firefly_extensions-4.1.1/jupyter_firefly_extensions/labextension/static/vendors-node_modules_firefly-api-access_distribution_firefly-api-access_min_js.11d96cd25e15e62dfcc9.js.map`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/src/FireflyCommonUtils.js` & `jupyter_firefly_extensions-4.1.1/src/FireflyCommonUtils.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,13 @@
 import {
     initFirefly
 } from 'firefly-api-access';
+import {
+    ServerConnection
+} from '@jupyterlab/services';
 
 
 let cachedLoc;
 let cachedFindFireflyResult;
 const ffLocURL = makeLabEndpoint('lab/fireflyLocation');
 const fetchOptions = {
     method: 'get',
@@ -21,38 +24,50 @@
  * Results are cache so this function can be call many times.
  * @return {Promise<{firefly: Object, channel: string, fireflyURL: string}>}
  */
 export async function findFirefly() {
     if (cachedFindFireflyResult) return cachedFindFireflyResult;
 
     try {
-        if (!cachedLoc) cachedLoc = await (await fetch(ffLocURL, fetchOptions)).json();
+        // request the config from server at /lab/fireflyLocation (see handlers.py)
+        const settings = ServerConnection.makeSettings();
+        if (!cachedLoc) cachedLoc = await (await ServerConnection.makeRequest(ffLocURL, fetchOptions, settings)).json();
 
+        // make sure that response of above request contains non-empty fireflyURL
         const {
-            fireflyURL = 'http://localhost:8080/firefly', fireflyChannel: channel
+            fireflyURL,
+            fireflyChannel: channel
         } = cachedLoc;
+        if (!fireflyURL) throw new Error(`fireflyURL couldn't be retrieved from ${ffLocURL}`);
+
+        // load firefly API from fireflyURL at /lab (window)
+        // (CORS errors might happen here if headers aren't set up correctly, maybe due to caching)
         if (!window.firefly?.initialized) window.firefly = {
             ...window.firefly,
             wsch: channel
         };
         if (!window.getFireflyAPI) window.getFireflyAPI = initFirefly(fireflyURL);
         const firefly = await window.getFireflyAPI();
+
+        // resolve Promise
         cachedFindFireflyResult = {
             fireflyURL,
             channel,
             firefly
         };
+        console.log('Firefly loaded successfully\n', cachedFindFireflyResult);
         return cachedFindFireflyResult;
     } catch (e) {
+        // log information about error(s) before rejecting Promise
         console.group('Firefly Load Failed');
         console.log('findFirefly: Could not determine firefly location or load firefly, call failed');
-        console.log(`find firefly url: ${ffLocURL}`);
-        if (cachedLoc) console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.channel}`);
+        if (cachedLoc) console.log(`firefly url: ${cachedLoc.fireflyURL} channel: ${cachedLoc.fireflyChannel}`);
         console.log(e);
         console.groupEnd('Firefly Load Failed');
+        throw e; // to let promise reject
     }
 
 }
 
 
 
 export function buildURLErrorHtml(e) {
```

### Comparing `jupyter_firefly_extensions-4.1.0/src/FitsViewerExt.js` & `jupyter_firefly_extensions-4.1.1/src/FitsViewerExt.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/src/SlateCommandExt.js` & `jupyter_firefly_extensions-4.1.1/src/SlateCommandExt.js`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/src/handler.ts` & `jupyter_firefly_extensions-4.1.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/src/index.ts` & `jupyter_firefly_extensions-4.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/style/fftools-logo.svg` & `jupyter_firefly_extensions-4.1.1/style/fftools-logo.svg`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/.gitignore` & `jupyter_firefly_extensions-4.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/README.md` & `jupyter_firefly_extensions-4.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,26 +21,34 @@
 
 * Firefly server - you can run it locally via a Firefly Docker image obtained from https://hub.docker.com/r/ipac/firefly.
 
 * astropy ^3.0.0 - (optional) used for convenience in example notebooks.
 
 * nodejs ^18.0.0 - only needed if you're doing [development install](#development-install)
 
+If you have conda installed and are setting up a fresh environment, you can use:
+```bash
+conda create -n jl-ff-ext -c conda-forge python jupyterlab firefly_client astropy
+conda activate jl-ff-ext
+```
+
 
 ### _Very Important_: first setup the Firefly URL - 3 ways
 
- * Add the following line to your `~/.jupyter/jupyter_notebook_config.py`
+You must provide **URL to a Firefly server** before running jupyter_firefly_extensions using ANY of the following ways:
+
+ * Add the following line to your `~/.jupyter/jupyter_config.py`
 
    ```python
    c.Firefly.url = 'http://localhost:8080/firefly'
    ```
 
 _Or_
 
- * Add the following line to your `~/.jupyter/jupyter_notebook_config.json` under the root object.
+ * Add the following line to your `~/.jupyter/jupyter_config.json` under the root object.
 
    ```json
    "Firefly": {
      "url": "http://localhost:8080/firefly"
    }
    ```
 
@@ -54,20 +62,22 @@
       ```
     
     in tcsh:
       ```
       setenv FIREFLY_URL http://localhost:8080/firefly
       ```
 
-**where the URL points to a Firefly server.**
-
+_Note:_ If your configuration is set in more than one way as described above, precedence order is:
+environment variable > jupyter_config.json > jupyter_config.py
 
 
 ## Installation
 
+In your environment with the prerequisites met,
+
 ```bash
 pip install jupyter_firefly_extensions
 ```
 
 Open JupyterLab (with `jupyter lab`) to start using these extensions - see [examples](#examples) to learn how.
 
 
@@ -91,16 +101,19 @@
 
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 
 # Enable the server extension
 jupyter server extension enable jupyter_firefly_extensions
 
-# Rebuild extension TS/JS source each time you make a change
+# Build extension TS/JS source
 jlpm run build
+
+# Alternatively, watch TS/JS source so that changes in it reflect automatically on lab
+jlpm watch
 ```
 
 
 ### Helpful commands
 
  - `jupyter server extension list` - show a list of server extensions
  - `jupyter lab extension list` - show a list of lab extensions
```

### Comparing `jupyter_firefly_extensions-4.1.0/pyproject.toml` & `jupyter_firefly_extensions-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_firefly_extensions-4.1.0/PKG-INFO` & `jupyter_firefly_extensions-4.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyter_firefly_extensions
-Version: 4.1.0
+Version: 4.1.1
+Dynamic: Keywords
 Summary: Jupyterlab extensions for rendering FITS and displaying tables, images, & charts with Firefly
 Project-URL: Homepage, https://github.com/Caltech-IPAC/jupyter_firefly_extensions
 Project-URL: Bug Tracker, https://github.com/Caltech-IPAC/jupyter_firefly_extensions/issues
 Project-URL: Repository, https://github.com/Caltech-IPAC/jupyter_firefly_extensions.git
 Author-email: Trey Roby <roby@ipac.caltech.edu>
 License: BSD-3-Clause License
 Classifier: Framework :: Jupyter
@@ -56,26 +57,34 @@
 
 * Firefly server - you can run it locally via a Firefly Docker image obtained from https://hub.docker.com/r/ipac/firefly.
 
 * astropy ^3.0.0 - (optional) used for convenience in example notebooks.
 
 * nodejs ^18.0.0 - only needed if you're doing [development install](#development-install)
 
+If you have conda installed and are setting up a fresh environment, you can use:
+```bash
+conda create -n jl-ff-ext -c conda-forge python jupyterlab firefly_client astropy
+conda activate jl-ff-ext
+```
+
 
 ### _Very Important_: first setup the Firefly URL - 3 ways
 
- * Add the following line to your `~/.jupyter/jupyter_notebook_config.py`
+You must provide **URL to a Firefly server** before running jupyter_firefly_extensions using ANY of the following ways:
+
+ * Add the following line to your `~/.jupyter/jupyter_config.py`
 
    ```python
    c.Firefly.url = 'http://localhost:8080/firefly'
    ```
 
 _Or_
 
- * Add the following line to your `~/.jupyter/jupyter_notebook_config.json` under the root object.
+ * Add the following line to your `~/.jupyter/jupyter_config.json` under the root object.
 
    ```json
    "Firefly": {
      "url": "http://localhost:8080/firefly"
    }
    ```
 
@@ -89,20 +98,22 @@
       ```
     
     in tcsh:
       ```
       setenv FIREFLY_URL http://localhost:8080/firefly
       ```
 
-**where the URL points to a Firefly server.**
-
+_Note:_ If your configuration is set in more than one way as described above, precedence order is:
+environment variable > jupyter_config.json > jupyter_config.py
 
 
 ## Installation
 
+In your environment with the prerequisites met,
+
 ```bash
 pip install jupyter_firefly_extensions
 ```
 
 Open JupyterLab (with `jupyter lab`) to start using these extensions - see [examples](#examples) to learn how.
 
 
@@ -126,16 +137,19 @@
 
 # Link your development version of the extension with JupyterLab
 jupyter labextension develop . --overwrite
 
 # Enable the server extension
 jupyter server extension enable jupyter_firefly_extensions
 
-# Rebuild extension TS/JS source each time you make a change
+# Build extension TS/JS source
 jlpm run build
+
+# Alternatively, watch TS/JS source so that changes in it reflect automatically on lab
+jlpm watch
 ```
 
 
 ### Helpful commands
 
  - `jupyter server extension list` - show a list of server extensions
  - `jupyter lab extension list` - show a list of lab extensions
```

