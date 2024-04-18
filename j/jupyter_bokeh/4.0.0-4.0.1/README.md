# Comparing `tmp/jupyter_bokeh-4.0.0.tar.gz` & `tmp/jupyter_bokeh-4.0.1.tar.gz`

## Comparing `jupyter_bokeh-4.0.0.tar` & `jupyter_bokeh-4.0.1.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/.eslintignore
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/.eslintrc.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/.yarnrc.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/DEVGUIDE.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/MANIFEST.in
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/install.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh.json
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/package.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/setup.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/tsconfig.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/webpack.config.js
--rw-r--r--   0        0        0   213222 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/yarn.lock
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/conda.recipe/meta.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/examples/jupyter_interactors.ipynb
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/examples/jupyter_sliders.ipynb
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/examples/jupyter_widgets.ipynb
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/examples/notebook_comms.ipynb
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/examples/server_embed.ipynb
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/examples/static_plot.ipynb
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/_version.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/widgets.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/package.json
--rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/199.e7fe4770dab71924b124.js
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/747.215e5b72fb89796bdb64.js
--rw-r--r--   0        0        0   171267 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/790.b027b82b72b7c2fb1ea7.js
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/790.b027b82b72b7c2fb1ea7.js.LICENSE.txt
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/remoteEntry.e32a0a8e32155667dea0.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/style.js
--rw-r--r--   0        0        0    10016 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/nbextension/extension.js
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/jupyter_bokeh/nbextension/index.js.LICENSE.txt
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/scripts/.deploy.sh.swp
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/scripts/deploy.sh
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/extension.ts
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/index.ts
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/manager.ts
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/metadata.d.ts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/plugin.ts
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/renderer.ts
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/src/widgets.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/style/index.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/LICENSE.txt
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/README.md
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.eslintignore
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.eslintrc.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/DEVGUIDE.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/install.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh.json
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/package.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/setup.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/tsconfig.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/webpack.config.js
+-rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/yarn.lock
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/jupyter_interactors.ipynb
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/jupyter_sliders.ipynb
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/jupyter_widgets.ipynb
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/notebook_comms.ipynb
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/server_embed.ipynb
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/static_plot.ipynb
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/_version.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/widgets.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/package.json
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
+-rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/7.4b7742c84d4af5271005.js
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/7.4b7742c84d4af5271005.js.LICENSE.txt
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/824.ce3da0e5e0e81f9850cf.js
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/remoteEntry.3cff93f6f99a3674a3dc.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/style.js
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/nbextension/extension.js
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/nbextension/index.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/scripts/deploy.sh
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/extension.ts
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/index.ts
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/manager.ts
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/metadata.d.ts
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/plugin.ts
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/renderer.ts
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/widgets.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/style/index.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/README.md
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/PKG-INFO
```

### Comparing `jupyter_bokeh-4.0.0/.eslintrc.js` & `jupyter_bokeh-4.0.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/package.json` & `jupyter_bokeh-4.0.1/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9623737373737374%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4', '@jupyterlab/apputils': '^4', "*

 * *                   "'@jupyterlab/docregistry': '^4', '@jupyterlab/notebook': '^4', "*

 * *                   "'@jupyterlab/services': '^7', '@jupyterlab/settingregistry': '^4', "*

 * *                   "'@jupyterlab/ui-components': '^4', '@lumino/disposable': '^2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4'}",*

 * * "'resolutions'": "{'@lumino/widgets': '^2'}",*

 * * "'version'": "'4.0.1'"}*

```diff
@@ -4,28 +4,28 @@
         "name": "Bokeh team"
     },
     "bugs": {
         "url": "https://github.com/bokeh/jupyter_bokeh/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
-        "@jupyterlab/application": "^4.0.3",
-        "@jupyterlab/apputils": "^4.1.3",
-        "@jupyterlab/docregistry": "^4.0.3",
-        "@jupyterlab/notebook": "^4.0.3",
-        "@jupyterlab/services": "^7.1.1",
-        "@jupyterlab/settingregistry": "^4.1.1",
-        "@jupyterlab/ui-components": "^4.0.3",
-        "@lumino/disposable": "^2.1.1",
+        "@jupyterlab/application": "^4",
+        "@jupyterlab/apputils": "^4",
+        "@jupyterlab/docregistry": "^4",
+        "@jupyterlab/notebook": "^4",
+        "@jupyterlab/services": "^7",
+        "@jupyterlab/settingregistry": "^4",
+        "@jupyterlab/ui-components": "^4",
+        "@lumino/disposable": "^2",
         "css-loader": "^5.1.3",
         "style-loader": "^2.0.0"
     },
     "description": "A Jupyter extension for rendering Bokeh content.",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.2",
+        "@jupyterlab/builder": "^4",
         "@typescript-eslint/eslint-plugin": "^7.0.1",
         "@typescript-eslint/parser": "^7.0.1",
         "eslint": "^8.36.0",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.4.1",
         "source-map-loader": "^5.0.0",
         "typescript": "~5.0.2",
@@ -53,15 +53,15 @@
         "@jupyter-widgets/jupyterlab-manager": "^5.0.4"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/bokeh/jupyter_bokeh.git"
     },
     "resolutions": {
-        "@lumino/widgets": "^2.1.1",
+        "@lumino/widgets": "^2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "scripts": {
         "__prepare": "jlpm run clean && jlpm run build:prod",
         "build": "jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.0"
+    "version": "4.0.1"
 }
```

### Comparing `jupyter_bokeh-4.0.0/tsconfig.json` & `jupyter_bokeh-4.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/webpack.config.js` & `jupyter_bokeh-4.0.1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/yarn.lock` & `jupyter_bokeh-4.0.1/yarn.lock`

 * *Files 4% similar despite different names*

```diff
@@ -13,23 +13,23 @@
   linkType: hard
 
 "@bokeh/jupyter_bokeh@workspace:.":
   version: 0.0.0-use.local
   resolution: "@bokeh/jupyter_bokeh@workspace:."
   dependencies:
     "@jupyter-widgets/base": ^2 || ^3 || ^4 || ^5 || ^6
-    "@jupyterlab/application": ^4.0.3
-    "@jupyterlab/apputils": ^4.1.3
-    "@jupyterlab/builder": ^4.0.2
-    "@jupyterlab/docregistry": ^4.0.3
-    "@jupyterlab/notebook": ^4.0.3
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/ui-components": ^4.0.3
-    "@lumino/disposable": ^2.1.1
+    "@jupyterlab/application": ^4
+    "@jupyterlab/apputils": ^4
+    "@jupyterlab/builder": ^4
+    "@jupyterlab/docregistry": ^4
+    "@jupyterlab/notebook": ^4
+    "@jupyterlab/services": ^7
+    "@jupyterlab/settingregistry": ^4
+    "@jupyterlab/ui-components": ^4
+    "@lumino/disposable": ^2
     "@typescript-eslint/eslint-plugin": ^7.0.1
     "@typescript-eslint/parser": ^7.0.1
     css-loader: ^5.1.3
     eslint: ^8.36.0
     npm-run-all: ^4.1.5
     rimraf: ^4.4.1
     source-map-loader: ^5.0.0
@@ -39,27 +39,27 @@
     webpack-cli: ^4.10.0
   peerDependencies:
     "@jupyter-widgets/jupyterlab-manager": ^5.0.4
   languageName: unknown
   linkType: soft
 
 "@codemirror/autocomplete@npm:^6.0.0, @codemirror/autocomplete@npm:^6.3.2, @codemirror/autocomplete@npm:^6.5.1, @codemirror/autocomplete@npm:^6.7.1":
-  version: 6.12.0
-  resolution: "@codemirror/autocomplete@npm:6.12.0"
+  version: 6.13.0
+  resolution: "@codemirror/autocomplete@npm:6.13.0"
   dependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
   peerDependencies:
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.0.0
     "@lezer/common": ^1.0.0
-  checksum: 1d4da6ccc12f5a67053a76b361f2683b5af031dd405a0bd2a261a265eb8cb7dfb115343a3291260d1ba31ce7ccb5427208ebe50f50f6747fcf27a50b62c87f7e
+  checksum: c40be5768e7494ae6541ccb9baf86701c764dabb174eae2fffd422e419caf6cd171a03a4b2efe4f8b108e29f5f6639a83ff5d20840803c85b4b65bc32978c947
   languageName: node
   linkType: hard
 
 "@codemirror/commands@npm:^6.2.3":
   version: 6.3.3
   resolution: "@codemirror/commands@npm:6.3.3"
   dependencies:
@@ -118,25 +118,25 @@
     "@codemirror/language": ^6.0.0
     "@lezer/java": ^1.0.0
   checksum: 4679104683cbffcd224ac04c7e5d144b787494697b26470b07017259035b7bb3fa62609d9a61bfbc566f1756d9f972f9f26d96a3c1362dd48881c1172f9a914d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-javascript@npm:^6.0.0, @codemirror/lang-javascript@npm:^6.1.7":
-  version: 6.2.1
-  resolution: "@codemirror/lang-javascript@npm:6.2.1"
+  version: 6.2.2
+  resolution: "@codemirror/lang-javascript@npm:6.2.2"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.6.0
     "@codemirror/lint": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@codemirror/view": ^6.17.0
     "@lezer/common": ^1.0.0
     "@lezer/javascript": ^1.0.0
-  checksum: 3df38c4cced06195283a9a2a9365aaa7c8c1b157852b331bc3a118403f774bbba57d2a392de52f5e28d2b344a323bc0146bcf7c8ef8be2473f167d815e4a37cd
+  checksum: 66379942a8347dff2bd76d10ed7cf313bca83872f8336fdd3e14accfef23e7b690cd913c9d11a3854fba2b32299da07fc3275995327642c9ee43c2a8e538c19d
   languageName: node
   linkType: hard
 
 "@codemirror/lang-json@npm:^6.0.1":
   version: 6.0.1
   resolution: "@codemirror/lang-json@npm:6.0.1"
   dependencies:
@@ -194,24 +194,24 @@
     "@codemirror/language": ^6.0.0
     "@lezer/rust": ^1.0.0
   checksum: 8a439944cb22159b0b3465ca4fa4294c69843219d5d30e278ae6df8e48f30a7a9256129723c025ec9b5e694d31a3560fb004300b125ffcd81c22d13825845170
   languageName: node
   linkType: hard
 
 "@codemirror/lang-sql@npm:^6.4.1":
-  version: 6.5.5
-  resolution: "@codemirror/lang-sql@npm:6.5.5"
+  version: 6.6.1
+  resolution: "@codemirror/lang-sql@npm:6.6.1"
   dependencies:
     "@codemirror/autocomplete": ^6.0.0
     "@codemirror/language": ^6.0.0
     "@codemirror/state": ^6.0.0
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 404003ae73b986bd7a00f6924db78b7ffb28fdc38d689fdc11416aaafe2d5c6dc37cc18972530f82e940acb61e18ac74a1cf7712beef448c145344ff93970dc3
+  checksum: 65f59b2a4477ddff27aba9435f4c3f1d236cbc03aa7c9cf3b2f70b8bbcd748c8883aae249efd9077fdbd9b23a9c0f046a29c945ffb0d8e6ef4e9ee9f61d35a88
   languageName: node
   linkType: hard
 
 "@codemirror/lang-wast@npm:^6.0.1":
   version: 6.0.2
   resolution: "@codemirror/lang-wast@npm:6.0.2"
   dependencies:
@@ -278,28 +278,28 @@
     "@codemirror/view": ^6.0.0
     crelt: ^1.0.5
   checksum: 19dc88d09fc750563347001e83c6194bbb2a25c874bd919d2d81809e1f98d6330222ddbd284aa9758a09eeb41fd153ec7c2cf810b2ee51452c25963d7f5833d5
   languageName: node
   linkType: hard
 
 "@codemirror/state@npm:^6.0.0, @codemirror/state@npm:^6.2.0, @codemirror/state@npm:^6.4.0":
-  version: 6.4.0
-  resolution: "@codemirror/state@npm:6.4.0"
-  checksum: c5236fe5786f1b85d17273a5c17fa8aeb063658c1404ab18caeb6e7591663ec96b65d453ab8162f75839c3801b04cd55ba4bc48f44cb61ebfeeee383f89553c7
+  version: 6.4.1
+  resolution: "@codemirror/state@npm:6.4.1"
+  checksum: b81b55574091349eed4d32fc0eadb0c9688f1f7c98b681318f59138ee0f527cb4c4a97831b70547c0640f02f3127647838ae6730782de4a3dd2cc58836125d01
   languageName: node
   linkType: hard
 
 "@codemirror/view@npm:^6.0.0, @codemirror/view@npm:^6.17.0, @codemirror/view@npm:^6.23.0, @codemirror/view@npm:^6.9.6":
-  version: 6.24.0
-  resolution: "@codemirror/view@npm:6.24.0"
+  version: 6.25.0
+  resolution: "@codemirror/view@npm:6.25.0"
   dependencies:
     "@codemirror/state": ^6.4.0
     style-mod: ^4.1.0
     w3c-keyname: ^2.2.4
-  checksum: c594f7628074d6f1a87636bb1281d1a1b579d0d73df4f8e04972eb7aca53de9c98f45e585d059f682920a89fa68dcad85a1418df90c28a746ae52aa06cdd0b8f
+  checksum: 5283cc5167fba2d905684c9b36e523b7c5bd12e70b497f0d55b2b63453f13a3eb858e0ce60c2eb97784c4202712da95a40b88a6495c632fd33b0fdab5360888f
   languageName: node
   linkType: hard
 
 "@discoveryjs/json-ext@npm:^0.5.0":
   version: 0.5.7
   resolution: "@discoveryjs/json-ext@npm:0.5.7"
   checksum: 2176d301cc258ea5c2324402997cf8134ebb212469c0d397591636cea8d3c02f2b3cf9fd58dcb748c7a0dade77ebdc1b10284fa63e608c033a1db52fddc69918
@@ -337,29 +337,29 @@
     js-yaml: ^4.1.0
     minimatch: ^3.1.2
     strip-json-comments: ^3.1.1
   checksum: 10957c7592b20ca0089262d8c2a8accbad14b4f6507e35416c32ee6b4dbf9cad67dfb77096bbd405405e9ada2b107f3797fe94362e1c55e0b09d6e90dd149127
   languageName: node
   linkType: hard
 
-"@eslint/js@npm:8.56.0":
-  version: 8.56.0
-  resolution: "@eslint/js@npm:8.56.0"
-  checksum: 5804130574ef810207bdf321c265437814e7a26f4e6fac9b496de3206afd52f533e09ec002a3be06cd9adcc9da63e727f1883938e663c4e4751c007d5b58e539
+"@eslint/js@npm:8.57.0":
+  version: 8.57.0
+  resolution: "@eslint/js@npm:8.57.0"
+  checksum: 315dc65b0e9893e2bff139bddace7ea601ad77ed47b4550e73da8c9c2d2766c7a575c3cddf17ef85b8fd6a36ff34f91729d0dcca56e73ca887c10df91a41b0bb
   languageName: node
   linkType: hard
 
 "@fortawesome/fontawesome-free@npm:^5.12.0":
   version: 5.15.4
   resolution: "@fortawesome/fontawesome-free@npm:5.15.4"
   checksum: 32281c3df4075290d9a96dfc22f72fadb3da7055d4117e48d34046b8c98032a55fa260ae351b0af5d6f6fb57a2f5d79a4abe52af456da35195f7cb7dda27b4a2
   languageName: node
   linkType: hard
 
-"@humanwhocodes/config-array@npm:^0.11.13":
+"@humanwhocodes/config-array@npm:^0.11.14":
   version: 0.11.14
   resolution: "@humanwhocodes/config-array@npm:0.11.14"
   dependencies:
     "@humanwhocodes/object-schema": ^2.0.2
     debug: ^4.3.1
     minimatch: ^3.0.5
   checksum: 861ccce9eaea5de19546653bccf75bf09fe878bc39c3aab00aeee2d2a0e654516adad38dd1098aab5e3af0145bbcbf3f309bdf4d964f8dab9dcd5834ae4c02f2
@@ -377,82 +377,62 @@
   version: 2.0.2
   resolution: "@humanwhocodes/object-schema@npm:2.0.2"
   checksum: 2fc11503361b5fb4f14714c700c02a3f4c7c93e9acd6b87a29f62c522d90470f364d6161b03d1cc618b979f2ae02aed1106fd29d302695d8927e2fc8165ba8ee
   languageName: node
   linkType: hard
 
 "@jridgewell/gen-mapping@npm:^0.3.0":
-  version: 0.3.2
-  resolution: "@jridgewell/gen-mapping@npm:0.3.2"
+  version: 0.3.5
+  resolution: "@jridgewell/gen-mapping@npm:0.3.5"
   dependencies:
-    "@jridgewell/set-array": ^1.0.1
+    "@jridgewell/set-array": ^1.2.1
     "@jridgewell/sourcemap-codec": ^1.4.10
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 1832707a1c476afebe4d0fbbd4b9434fdb51a4c3e009ab1e9938648e21b7a97049fa6009393bdf05cab7504108413441df26d8a3c12193996e65493a4efb6882
+    "@jridgewell/trace-mapping": ^0.3.24
+  checksum: ff7a1764ebd76a5e129c8890aa3e2f46045109dabde62b0b6c6a250152227647178ff2069ea234753a690d8f3c4ac8b5e7b267bbee272bffb7f3b0a370ab6e52
   languageName: node
   linkType: hard
 
-"@jridgewell/resolve-uri@npm:3.1.0":
-  version: 3.1.0
-  resolution: "@jridgewell/resolve-uri@npm:3.1.0"
-  checksum: b5ceaaf9a110fcb2780d1d8f8d4a0bfd216702f31c988d8042e5f8fbe353c55d9b0f55a1733afdc64806f8e79c485d2464680ac48a0d9fcadb9548ee6b81d267
-  languageName: node
-  linkType: hard
-
-"@jridgewell/set-array@npm:^1.0.1":
-  version: 1.1.2
-  resolution: "@jridgewell/set-array@npm:1.1.2"
-  checksum: 69a84d5980385f396ff60a175f7177af0b8da4ddb81824cb7016a9ef914eee9806c72b6b65942003c63f7983d4f39a5c6c27185bbca88eb4690b62075602e28e
+"@jridgewell/resolve-uri@npm:^3.1.0":
+  version: 3.1.2
+  resolution: "@jridgewell/resolve-uri@npm:3.1.2"
+  checksum: 83b85f72c59d1c080b4cbec0fef84528963a1b5db34e4370fa4bd1e3ff64a0d80e0cee7369d11d73c704e0286fb2865b530acac7a871088fbe92b5edf1000870
   languageName: node
   linkType: hard
 
-"@jridgewell/source-map@npm:^0.3.2":
-  version: 0.3.2
-  resolution: "@jridgewell/source-map@npm:0.3.2"
-  dependencies:
-    "@jridgewell/gen-mapping": ^0.3.0
-    "@jridgewell/trace-mapping": ^0.3.9
-  checksum: 1b83f0eb944e77b70559a394d5d3b3f98a81fcc186946aceb3ef42d036762b52ef71493c6c0a3b7c1d2f08785f53ba2df1277fe629a06e6109588ff4cdcf7482
+"@jridgewell/set-array@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "@jridgewell/set-array@npm:1.2.1"
+  checksum: 832e513a85a588f8ed4f27d1279420d8547743cc37fcad5a5a76fc74bb895b013dfe614d0eed9cb860048e6546b798f8f2652020b4b2ba0561b05caa8c654b10
   languageName: node
   linkType: hard
 
 "@jridgewell/source-map@npm:^0.3.3":
   version: 0.3.5
   resolution: "@jridgewell/source-map@npm:0.3.5"
   dependencies:
     "@jridgewell/gen-mapping": ^0.3.0
     "@jridgewell/trace-mapping": ^0.3.9
   checksum: 1ad4dec0bdafbade57920a50acec6634f88a0eb735851e0dda906fa9894e7f0549c492678aad1a10f8e144bfe87f238307bf2a914a1bc85b7781d345417e9f6f
   languageName: node
   linkType: hard
 
-"@jridgewell/sourcemap-codec@npm:1.4.14, @jridgewell/sourcemap-codec@npm:^1.4.10":
-  version: 1.4.14
-  resolution: "@jridgewell/sourcemap-codec@npm:1.4.14"
-  checksum: 61100637b6d173d3ba786a5dff019e1a74b1f394f323c1fee337ff390239f053b87266c7a948777f4b1ee68c01a8ad0ab61e5ff4abb5a012a0b091bec391ab97
-  languageName: node
-  linkType: hard
-
-"@jridgewell/trace-mapping@npm:^0.3.14, @jridgewell/trace-mapping@npm:^0.3.9":
-  version: 0.3.17
-  resolution: "@jridgewell/trace-mapping@npm:0.3.17"
-  dependencies:
-    "@jridgewell/resolve-uri": 3.1.0
-    "@jridgewell/sourcemap-codec": 1.4.14
-  checksum: 9d703b859cff5cd83b7308fd457a431387db5db96bd781a63bf48e183418dd9d3d44e76b9e4ae13237f6abeeb25d739ec9215c1d5bfdd08f66f750a50074a339
+"@jridgewell/sourcemap-codec@npm:^1.4.10, @jridgewell/sourcemap-codec@npm:^1.4.14":
+  version: 1.4.15
+  resolution: "@jridgewell/sourcemap-codec@npm:1.4.15"
+  checksum: b881c7e503db3fc7f3c1f35a1dd2655a188cc51a3612d76efc8a6eb74728bef5606e6758ee77423e564092b4a518aba569bbb21c9bac5ab7a35b0c6ae7e344c8
   languageName: node
   linkType: hard
 
-"@jridgewell/trace-mapping@npm:^0.3.17":
-  version: 0.3.18
-  resolution: "@jridgewell/trace-mapping@npm:0.3.18"
+"@jridgewell/trace-mapping@npm:^0.3.20, @jridgewell/trace-mapping@npm:^0.3.24, @jridgewell/trace-mapping@npm:^0.3.9":
+  version: 0.3.25
+  resolution: "@jridgewell/trace-mapping@npm:0.3.25"
   dependencies:
-    "@jridgewell/resolve-uri": 3.1.0
-    "@jridgewell/sourcemap-codec": 1.4.14
-  checksum: 0572669f855260808c16fe8f78f5f1b4356463b11d3f2c7c0b5580c8ba1cbf4ae53efe9f627595830856e57dbac2325ac17eb0c3dd0ec42102e6f227cc289c02
+    "@jridgewell/resolve-uri": ^3.1.0
+    "@jridgewell/sourcemap-codec": ^1.4.14
+  checksum: 9d3c40d225e139987b50c48988f8717a54a8c994d8a948ee42e1412e08988761d0754d7d10b803061cc3aebf35f92a5dbbab493bd0e1a9ef9e89a2130e83ba34
   languageName: node
   linkType: hard
 
 "@jupyter-widgets/base@npm:^2 || ^3 || ^4 || ^5 || ^6":
   version: 6.0.7
   resolution: "@jupyter-widgets/base@npm:6.0.7"
   dependencies:
@@ -466,33 +446,33 @@
     jquery: ^3.1.1
     lodash: ^4.17.4
   checksum: d4f385a8412b16d696db618eec771011000326f8a5645f6c3ca61ed6fa181aed6e16780189f792cb342fa80473092501299b418460a8be3a2eba5237c5a33f1d
   languageName: node
   linkType: hard
 
 "@jupyter/react-components@npm:^0.15.2":
-  version: 0.15.2
-  resolution: "@jupyter/react-components@npm:0.15.2"
+  version: 0.15.3
+  resolution: "@jupyter/react-components@npm:0.15.3"
   dependencies:
-    "@jupyter/web-components": ^0.15.2
+    "@jupyter/web-components": ^0.15.3
     "@microsoft/fast-react-wrapper": ^0.3.22
     react: ">=17.0.0 <19.0.0"
-  checksum: d6d339ff9c2fed1fd5afda612be500d73c4a83eee5470d50e94020dadd1e389a3bf745c7240b0a48edbc6d3fdacec93367b7b5e40588f2df588419caada705be
+  checksum: 1a6b256314259c6465c4b6d958575710536b82234a7bf0fba3e889a07e1f19ff8ab321450be354359876f92c45dbcc9d21a840237ff4a619806d9de696f55496
   languageName: node
   linkType: hard
 
-"@jupyter/web-components@npm:^0.15.2":
-  version: 0.15.2
-  resolution: "@jupyter/web-components@npm:0.15.2"
+"@jupyter/web-components@npm:^0.15.2, @jupyter/web-components@npm:^0.15.3":
+  version: 0.15.3
+  resolution: "@jupyter/web-components@npm:0.15.3"
   dependencies:
     "@microsoft/fast-colors": ^5.3.1
     "@microsoft/fast-element": ^1.12.0
     "@microsoft/fast-foundation": ^2.49.4
     "@microsoft/fast-web-utilities": ^5.4.1
-  checksum: f272ef91de08e28f9414a26dbd2388e1a8985c90f4ab00231978cee49bd5212f812411397a9038d298c8c0c4b41eb28cc86f1127bc7ace309bda8df60c4a87c8
+  checksum: a0980af934157bfdbdb6cc169c0816c1b2e57602d524c56bdcef746a4c25dfeb8f505150d83207c8695ed89b5486cf53d35a3382584d25ef64db666e4e16e45b
   languageName: node
   linkType: hard
 
 "@jupyter/ydoc@npm:^1.1.1":
   version: 1.1.1
   resolution: "@jupyter/ydoc@npm:1.1.1"
   dependencies:
@@ -502,101 +482,101 @@
     "@lumino/signaling": ^1.10.0 || ^2.0.0
     y-protocols: ^1.0.5
     yjs: ^13.5.40
   checksum: a239b1dd57cfc9ba36c06ac5032a1b6388849ae01a1d0db0d45094f71fdadf4d473b4bf8becbef0cfcdc85cae505361fbec0822b02da5aa48e06b66f742dd7a0
   languageName: node
   linkType: hard
 
-"@jupyterlab/application@npm:^4.0.3":
-  version: 4.1.1
-  resolution: "@jupyterlab/application@npm:4.1.1"
+"@jupyterlab/application@npm:^4":
+  version: 4.1.3
+  resolution: "@jupyterlab/application@npm:4.1.3"
   dependencies:
     "@fortawesome/fontawesome-free": ^5.12.0
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/docregistry": ^4.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/statedb": ^4.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/application": ^2.3.0
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
-  checksum: d8b1254c6eb5db30133703926d82e75d8655001af863007bf69e73e4e3e98cc0159ffd55a32f03121b602215b354e7e467fed0cabd7b109b9928c81f45166375
+  checksum: f9970bdcfec0e9b0139bea11683309154052f5de340bd57021b29d06dfb08b8f598b17c299a7d6706cf5e3c583436be5a5e9832655b501e207f2bfc17f9547c6
   languageName: node
   linkType: hard
 
-"@jupyterlab/apputils@npm:^4.1.3, @jupyterlab/apputils@npm:^4.2.1":
-  version: 4.2.1
-  resolution: "@jupyterlab/apputils@npm:4.2.1"
-  dependencies:
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+"@jupyterlab/apputils@npm:^4, @jupyterlab/apputils@npm:^4.2.3":
+  version: 4.2.3
+  resolution: "@jupyterlab/apputils@npm:4.2.3"
+  dependencies:
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/settingregistry": ^4.1.3
+    "@jupyterlab/statedb": ^4.1.3
+    "@jupyterlab/statusbar": ^4.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     "@types/react": ^18.0.26
     react: ^18.2.0
     sanitize-html: ~2.7.3
-  checksum: e64f4d342c97a32ec74ef7045fd4793d998fea0f9bb296835a597b4a0e0739904dd8dd3ff5531fbcd8fc53bae40f6c796143a0b06dd7851c78afd1d4ffaa7ccd
+  checksum: 783ff7a1c1d05efffd1e4c40c54595306e913474a5297521a3df0914436981e3535c8bea3995161be6af90c0b5e31ac0dcb103ec56416b8bbfbd52ccdaaf2c64
   languageName: node
   linkType: hard
 
-"@jupyterlab/attachments@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/attachments@npm:4.1.1"
+"@jupyterlab/attachments@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/attachments@npm:4.1.3"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
-  checksum: a0dfbcf9b74743574ecbb917f8193ad443e360471c911c946b5f810f06259e80b54c530133badd6fef7042ab13c1f3f57fb3a8d3bbc9462df3541bd5d0ea0017
+  checksum: 1922213e066ba339adbe641937e29e5fe3f3d2d543df7925cf948e7d5cc85e88ef369e21e54a3c3a9b6228360df49460a1f9de87eeb29e40112539a8c988de1b
   languageName: node
   linkType: hard
 
-"@jupyterlab/builder@npm:^4.0.2":
-  version: 4.0.3
-  resolution: "@jupyterlab/builder@npm:4.0.3"
+"@jupyterlab/builder@npm:^4":
+  version: 4.1.3
+  resolution: "@jupyterlab/builder@npm:4.1.3"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/application": ^2.1.1
-    "@lumino/commands": ^2.1.1
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.1
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-    "@lumino/widgets": ^2.1.1
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/application": ^2.3.0
+    "@lumino/commands": ^2.2.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+    "@lumino/widgets": ^2.3.1
     ajv: ^8.12.0
     commander: ^9.4.1
     css-loader: ^6.7.1
     duplicate-package-checker-webpack-plugin: ^3.0.0
     fs-extra: ^10.1.0
     glob: ~7.1.6
     license-webpack-plugin: ^2.3.14
@@ -610,81 +590,81 @@
     terser-webpack-plugin: ^5.3.7
     webpack: ^5.76.1
     webpack-cli: ^5.0.1
     webpack-merge: ^5.8.0
     worker-loader: ^3.0.2
   bin:
     build-labextension: lib/build-labextension.js
-  checksum: 7d6402f859bc43cf7baa90893e57bd8d421716256c51fe72b1f80f4b471446e918d77912babe9bfac87a4edcc2ae3d6434334688f13414d293ff340266607b46
+  checksum: 1db53221d05cf91780a79d506f2e8dfb844a8f226634ba7e8cd74ad6288425e06a72c002c14fad59dc74d087ba0359d523b1792c9e795910f6c44909d1f3308c
   languageName: node
   linkType: hard
 
-"@jupyterlab/cells@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/cells@npm:4.1.1"
+"@jupyterlab/cells@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/cells@npm:4.1.3"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/attachments": ^4.1.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/codemirror": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/documentsearch": ^4.1.1
-    "@jupyterlab/filebrowser": ^4.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/outputarea": ^4.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/toc": ^6.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/attachments": ^4.1.3
+    "@jupyterlab/codeeditor": ^4.1.3
+    "@jupyterlab/codemirror": ^4.1.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/documentsearch": ^4.1.3
+    "@jupyterlab/filebrowser": ^4.1.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/outputarea": ^4.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/toc": ^6.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 5590da50acdd1f25255ce28e4f50d6c5425d872c241723074ed8ab050dc650362cac1f74b355eb01066654eb9fa532b993f002bcce01ab3768fac7552498492b
+  checksum: 6cab8994b74e03f32a9a5eac2a7ed580fd6ef46ab764d871d4bd6de76345ae04036af733d3182cbd00143ad7e667682010d777efdc6b9a3c44cff6833fd4b7ec
   languageName: node
   linkType: hard
 
-"@jupyterlab/codeeditor@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/codeeditor@npm:4.1.1"
+"@jupyterlab/codeeditor@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/codeeditor@npm:4.1.3"
   dependencies:
     "@codemirror/state": ^6.2.0
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/statusbar": ^4.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: d29817772368d30352da4631592f3bacf73dba12031f06247c16e2e3122a65ab7d5feca254f69fb61e3f4dad83cc1f148310b3474a00be60b8fc25cc15846dda
+  checksum: 2f32da79147d1f9c0f20b1ca0559c173f8cd1b3daf1359ae0e3dbfa32820bec427bf520f8c3bb7b1dd452691d9bdf06d9379d524c349631070ef5e0783d2ffce
   languageName: node
   linkType: hard
 
-"@jupyterlab/codemirror@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/codemirror@npm:4.1.1"
+"@jupyterlab/codemirror@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/codemirror@npm:4.1.3"
   dependencies:
     "@codemirror/autocomplete": ^6.5.1
     "@codemirror/commands": ^6.2.3
     "@codemirror/lang-cpp": ^6.0.2
     "@codemirror/lang-css": ^6.1.1
     "@codemirror/lang-html": ^6.4.3
     "@codemirror/lang-java": ^6.0.1
@@ -699,387 +679,387 @@
     "@codemirror/lang-xml": ^6.0.2
     "@codemirror/language": ^6.6.0
     "@codemirror/legacy-modes": ^6.3.2
     "@codemirror/search": ^6.3.0
     "@codemirror/state": ^6.2.0
     "@codemirror/view": ^6.9.6
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/documentsearch": ^4.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/codeeditor": ^4.1.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/documentsearch": ^4.1.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/translation": ^4.1.3
     "@lezer/common": ^1.0.2
     "@lezer/generator": ^1.2.2
     "@lezer/highlight": ^1.1.4
     "@lezer/markdown": ^1.0.2
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     yjs: ^13.5.40
-  checksum: 453a09bab7a443c014fb84843f052f1186be5ed153415b56ecd4d1cae7c41122e7e37eeaa62348ab0c4a29711e169b3e1fbb953514b0e0fe0624eb8f3609bb0b
+  checksum: cea7a1e993f573560a494ced1a9b627d57a4973b8fa06bb418af0018af1dcc4bad3c0f31abf17cd28fd393e169042917c732c515828570b80892d2ca371718c3
   languageName: node
   linkType: hard
 
-"@jupyterlab/coreutils@npm:^6.1.1":
-  version: 6.1.1
-  resolution: "@jupyterlab/coreutils@npm:6.1.1"
+"@jupyterlab/coreutils@npm:^6.1.3":
+  version: 6.1.3
+  resolution: "@jupyterlab/coreutils@npm:6.1.3"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     minimist: ~1.2.0
     path-browserify: ^1.0.0
     url-parse: ~1.5.4
-  checksum: bdcd5135a1f13a7c8df1e22ad081d3da81bb7d9f802d1339baa3aaa6238099d8066ce10a3452f879069c737e471a2a55409a855398c5c211bc044c17056c9e7c
+  checksum: 99e1580a8b7231aef7d54d14234a299ee1fb5988b2d63e3312a1bcaf91a1a2e69c36f5ff52dc0a2ac1049217eb14a61b82a79e98b2447ab73d4d55bacd590c11
   languageName: node
   linkType: hard
 
-"@jupyterlab/docmanager@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/docmanager@npm:4.1.1"
+"@jupyterlab/docmanager@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/docmanager@npm:4.1.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/docregistry": ^4.1.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/statusbar": ^4.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 835e8ce43145fb9700ea4df8e433eb7f2c24e81003d34e8085b9118d0b769bad612ccd2d2d7fb209f4baf2bccda9d2dd36063776742a810c9d81220f3a50a356
+  checksum: ea47f404199e80b747996bd4dced7ca7fc06b80ab1adbc15d8896ede914765d544545e4b53930a3ec85cf4ac2ad75600eacaa67057e48c6aedb4f531a63847fe
   languageName: node
   linkType: hard
 
-"@jupyterlab/docregistry@npm:^4.0.3, @jupyterlab/docregistry@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/docregistry@npm:4.1.1"
+"@jupyterlab/docregistry@npm:^4, @jupyterlab/docregistry@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/docregistry@npm:4.1.3"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/codeeditor": ^4.1.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 8ad2e4deb280b6e95dc5f3e917d362462b018f65f4d438ad46994bef5ee9ba4350e7264455e68fb329286ac3e83aebbc63e80ca4ded0feab05974e83b73ba410
+  checksum: 250fdccc313e700f4d7aff1a9a17c661414af5e202360a34138a5a1be82a6be23cdda3bca0e64d77db4d217ec2434090672debcc2223c8f22bdd168463b57c7f
   languageName: node
   linkType: hard
 
-"@jupyterlab/documentsearch@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/documentsearch@npm:4.1.1"
+"@jupyterlab/documentsearch@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/documentsearch@npm:4.1.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: d54976b192154dd32bc7d1794c76013d74e54ee63ffbeba51e3334d8153435d5412649a313cb5d16dced3cca749ea7bf04354f243f2c4c5f0f453e036a848f8f
+  checksum: b83056060b8c13460f7e50eacefc423604235ef1578002e04f5ba7529f2b33d384ab3216b5c2ff2dd3deaa62b5805f8610f93c3a48de1595beb397f51494aef1
   languageName: node
   linkType: hard
 
-"@jupyterlab/filebrowser@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/filebrowser@npm:4.1.1"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docmanager": ^4.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statedb": ^4.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+"@jupyterlab/filebrowser@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/filebrowser@npm:4.1.3"
+  dependencies:
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/docmanager": ^4.1.3
+    "@jupyterlab/docregistry": ^4.1.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/statedb": ^4.1.3
+    "@jupyterlab/statusbar": ^4.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 38a1b2650334047958eba3d51735069dc5791259e62ed34bb6cae598f6e8a300a918aa638776380e9d066b1455dd9fdeabcbeebe4d9ddd8661d10a6f824805ce
+  checksum: cd7df40ee048ed0a9b76049da2ef488758e99241cf353db4c84b8047f5add1fa0be1b23125fbc795cd630823b0c421742f1233e92c1bcf96635d954707ec7b02
   languageName: node
   linkType: hard
 
-"@jupyterlab/lsp@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/lsp@npm:4.1.1"
+"@jupyterlab/lsp@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/lsp@npm:4.1.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/codemirror": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/codeeditor": ^4.1.3
+    "@jupyterlab/codemirror": ^4.1.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/docregistry": ^4.1.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/translation": ^4.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     lodash.mergewith: ^4.6.1
     vscode-jsonrpc: ^6.0.0
     vscode-languageserver-protocol: ^3.17.0
     vscode-ws-jsonrpc: ~1.0.2
-  checksum: 55a96a0cf03b49a156bd14e9df776289be7bbd26ced685f23613c71f4a5d8d34a510c1a52956ab893e393dfb209c4c9f35df71dc0aca2b19d148e568bccb3700
+  checksum: 1f748126ab862d6c2341becf57debc625bc7a5917e87923789d48cfcb748ef6e023a8dbadab7d27588c2dc2300f079da9f91f222147d3b0e8e0450de669579f8
   languageName: node
   linkType: hard
 
-"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/nbformat@npm:4.1.1"
+"@jupyterlab/nbformat@npm:^3.0.0 || ^4.0.0-alpha.21 || ^4.0.0, @jupyterlab/nbformat@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/nbformat@npm:4.1.3"
   dependencies:
     "@lumino/coreutils": ^2.1.2
-  checksum: 8c952760e077d4b5b7c54a12e7b5a50880bdc6d4a13c4a9a5901763eaa04077b00c9a81a4c91c4a7eaafef72fb4d7a3ac1230e3fc9b91914bef27b7a8933e756
+  checksum: db323f225fea8204407a069745aff80687cafbb2c2ec663bf2e820fb41ebf7cb1f9d03ba9c0480a4d54a6e64bb0cd1833541e36b5314e9f8e16bd4a321316d40
   languageName: node
   linkType: hard
 
-"@jupyterlab/notebook@npm:^4.0.3":
-  version: 4.1.1
-  resolution: "@jupyterlab/notebook@npm:4.1.1"
+"@jupyterlab/notebook@npm:^4":
+  version: 4.1.3
+  resolution: "@jupyterlab/notebook@npm:4.1.3"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/cells": ^4.1.1
-    "@jupyterlab/codeeditor": ^4.1.1
-    "@jupyterlab/codemirror": ^4.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/documentsearch": ^4.1.1
-    "@jupyterlab/lsp": ^4.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/statusbar": ^4.1.1
-    "@jupyterlab/toc": ^6.1.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/cells": ^4.1.3
+    "@jupyterlab/codeeditor": ^4.1.3
+    "@jupyterlab/codemirror": ^4.1.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/docregistry": ^4.1.3
+    "@jupyterlab/documentsearch": ^4.1.3
+    "@jupyterlab/lsp": ^4.1.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/settingregistry": ^4.1.3
+    "@jupyterlab/statusbar": ^4.1.3
+    "@jupyterlab/toc": ^6.1.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/domutils": ^2.0.1
     "@lumino/dragdrop": ^2.1.4
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/virtualdom": ^2.0.1
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: ffc0a95a794266129a341ae779d380b30abe70819ce60002e2b3bbef8a47dba8f4e55d32754f6350a715d4fa7790cece4da31b4e45714d35af84d9b3fa75244b
+  checksum: a2983911327a7bcee8dcbf7f1d68e4713e33a7db4f8730cb986144c0689e6d251cc7b45a75af952fa2fd60315a24a9551388d20a1064afdb5758da33d2fd5275
   languageName: node
   linkType: hard
 
-"@jupyterlab/observables@npm:^5.1.1":
-  version: 5.1.1
-  resolution: "@jupyterlab/observables@npm:5.1.1"
+"@jupyterlab/observables@npm:^5.1.3":
+  version: 5.1.3
+  resolution: "@jupyterlab/observables@npm:5.1.3"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 611b70e274043ef86b268e406725c9f31141f6c6ce62df76e5be2ca76eee883e0b045859a8ee5541547d5e4f79941f606c9e11b4d2be5caf1156ac16a4853c32
+  checksum: 30f606706b7c3d3a40eea20f299e31b2635531a2042f4f6137c3e2a8764786559a627f1974b5147aa8255a26a6ffa0c0fbefb780e2c5abb994e4aae0548fe881
   languageName: node
   linkType: hard
 
-"@jupyterlab/outputarea@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/outputarea@npm:4.1.1"
+"@jupyterlab/outputarea@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/outputarea@npm:4.1.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/translation": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
-  checksum: 0bcc11058a9b33e5c8f3edf1eb383f1a641410388df389aa39d11a396d390cd7ff5bcb998982a96aa149cdf32c64666268d471c73ec48c439336c66b11938e2c
+  checksum: 313587b54e25b393ad319bfb8055e737695fdf5dab7f01376c23e4ad1e933f0a57fc1bdeba03791428f5340a207bcd8e4afbc51370de86965b5365c2c72260d0
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime-interfaces@npm:^3.9.1":
-  version: 3.9.1
-  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.1"
+"@jupyterlab/rendermime-interfaces@npm:^3.9.3":
+  version: 3.9.3
+  resolution: "@jupyterlab/rendermime-interfaces@npm:3.9.3"
   dependencies:
     "@lumino/coreutils": ^1.11.0 || ^2.1.2
     "@lumino/widgets": ^1.37.2 || ^2.3.1
-  checksum: 5a746134a1f9f073213002bd8336327907d871599d879806994816b5fe4875c5ace3af919f1d9125e6a12f3d93f0df15b52c2fbe778b977463b621b1eb93c502
+  checksum: 8992792c2473a8bd3f32a1c50cd83f4a9e32e6d0b8d830371d9f2ef31edf6c42a98afdae7e1418cb457870ab776025c2282d5f7c3258989f98680a2ccb81bed6
   languageName: node
   linkType: hard
 
-"@jupyterlab/rendermime@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/rendermime@npm:4.1.1"
+"@jupyterlab/rendermime@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/rendermime@npm:4.1.3"
   dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/translation": ^4.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     lodash.escape: ^4.0.1
-  checksum: 9c23fa5714ba38956e9e94164777b3494591cd8a25e46fad4c6acef52fad30b36ab77b06bf078cc8b229fb577108561c3871a07c7ceebc35cb8ec87c12048f0f
+  checksum: 6cd4cdbe693f767201003030fd16440c12464df6b8143a5c9ef1d20b445af555245c86a775a207819c737f53811a7195fef5019521cbf9377867294d8764fea6
   languageName: node
   linkType: hard
 
-"@jupyterlab/services@npm:^6.0.0 || ^7.0.0, @jupyterlab/services@npm:^7.1.1":
-  version: 7.1.1
-  resolution: "@jupyterlab/services@npm:7.1.1"
+"@jupyterlab/services@npm:^6.0.0 || ^7.0.0, @jupyterlab/services@npm:^7, @jupyterlab/services@npm:^7.1.3":
+  version: 7.1.3
+  resolution: "@jupyterlab/services@npm:7.1.3"
   dependencies:
     "@jupyter/ydoc": ^1.1.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/settingregistry": ^4.1.1
-    "@jupyterlab/statedb": ^4.1.1
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/settingregistry": ^4.1.3
+    "@jupyterlab/statedb": ^4.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
     ws: ^8.11.0
-  checksum: d2dbd3af7944f551653f2771e2c8ff87b84f42ce9bd3bf0b71bb0e6dbb422410719b8e4edeb668710211a939340f6e20cd49a137128cc4efa07ecc3fa32a66b9
+  checksum: 9c602ccb7c3b70671331608aec08ee3277edc6983b9ef5427496cde5ba295e91ed6d51f4a3c005ded7f206e510d1ce08eeca4d1a3036fc3e3fbeb7a4e429b601
   languageName: node
   linkType: hard
 
-"@jupyterlab/settingregistry@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/settingregistry@npm:4.1.1"
+"@jupyterlab/settingregistry@npm:^4, @jupyterlab/settingregistry@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/settingregistry@npm:4.1.3"
   dependencies:
-    "@jupyterlab/nbformat": ^4.1.1
-    "@jupyterlab/statedb": ^4.1.1
+    "@jupyterlab/nbformat": ^4.1.3
+    "@jupyterlab/statedb": ^4.1.3
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
     "@rjsf/utils": ^5.13.4
     ajv: ^8.12.0
     json5: ^2.2.3
   peerDependencies:
     react: ">=16"
-  checksum: 1beddc68e8a5f01062ea856286d2e4ae2bb1993a89f71adb3a0725a191cbf2fdf927f95235b69cdfd73f848452ba40d9e7dd35ed985dd9e382c70cfbaf54cf67
+  checksum: 6678cf1ec9fbb8be09070d84ffb2f22d6ecc230549ad7510c64d9a171a840ae26d800d4b39333fdc37c7704b3e7c80c1b7c1f077dda128d95f92b5f6aec8ea39
   languageName: node
   linkType: hard
 
-"@jupyterlab/statedb@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/statedb@npm:4.1.1"
+"@jupyterlab/statedb@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/statedb@npm:4.1.3"
   dependencies:
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/properties": ^2.0.1
     "@lumino/signaling": ^2.1.2
-  checksum: 3291a9f10557c545b41730e657890557dbfa2b7893679ee8d406562bc62b7da3906f3691f099c9aae1bfc490cd3642552f0cbfbaed58cf58e6877e7f8ca8fd9a
+  checksum: 87571e57a0ede95fd67d7619deda26eb62ade0c3ac4ef03f46f55dff7928146ffffa793fc8db63b67604ebb8fda80e4cb3848070edb55093da722d522d65c780
   languageName: node
   linkType: hard
 
-"@jupyterlab/statusbar@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/statusbar@npm:4.1.1"
+"@jupyterlab/statusbar@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/statusbar@npm:4.1.3"
   dependencies:
-    "@jupyterlab/ui-components": ^4.1.1
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: c060b1ce5c87f8277407e1fcdc0cf03bfdba496a6288c8821e19a785b5d656b454ae72fb5103cf7361a167f4eef07432c2b143883de67a54baab66444b371258
+  checksum: e0690f312f6cb8cc8ac8f2c8ea7563f6d83b09ef2daca15461be156b4ce0717ff81c9f4675cc391af3b2a72785cb7ff74d982f7dda5745b693b9656fb91f4eef
   languageName: node
   linkType: hard
 
-"@jupyterlab/toc@npm:^6.1.1":
-  version: 6.1.1
-  resolution: "@jupyterlab/toc@npm:6.1.1"
-  dependencies:
-    "@jupyterlab/apputils": ^4.2.1
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/docregistry": ^4.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime": ^4.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/translation": ^4.1.1
-    "@jupyterlab/ui-components": ^4.1.1
+"@jupyterlab/toc@npm:^6.1.3":
+  version: 6.1.3
+  resolution: "@jupyterlab/toc@npm:6.1.3"
+  dependencies:
+    "@jupyterlab/apputils": ^4.2.3
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/docregistry": ^4.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime": ^4.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/translation": ^4.1.3
+    "@jupyterlab/ui-components": ^4.1.3
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/signaling": ^2.1.2
     "@lumino/widgets": ^2.3.1
     react: ^18.2.0
-  checksum: 4affcdc2015f363e3f57da3e8613b4cff2f6e8477f308e97ce055f8ceafcab117dbb72780d2eba8dbcbba90b77affac7b8c7dd3dbc8f65db4dbc4b22629fdd4e
+  checksum: cf9e15a59a6a1aa424eb89acd1828f2f645a7cd0257e44092fea2cbeb2fcc5499556d83662654acac3844af0ab7e38f7c356e9f7e8954913e247ca842ad69d3c
   languageName: node
   linkType: hard
 
-"@jupyterlab/translation@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/translation@npm:4.1.1"
+"@jupyterlab/translation@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/translation@npm:4.1.3"
   dependencies:
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/services": ^7.1.1
-    "@jupyterlab/statedb": ^4.1.1
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/services": ^7.1.3
+    "@jupyterlab/statedb": ^4.1.3
     "@lumino/coreutils": ^2.1.2
-  checksum: adb9840f8e98af6d06d986120d542469ee349c4337e3a7f84f449535f88cc84839fe169a562447abf7bf31254bf28d1d4627684b5c521b6cb2bd21fab73e0234
+  checksum: cd5b4e75cc5411ea8e0d0b00180db6010acaf703af8e4d3ad4731a45c375ccc0c7bbe8c21d86aa4ad693718f03f37696da21c7262e77dddee56026becd38199d
   languageName: node
   linkType: hard
 
-"@jupyterlab/ui-components@npm:^4.0.3, @jupyterlab/ui-components@npm:^4.1.1":
-  version: 4.1.1
-  resolution: "@jupyterlab/ui-components@npm:4.1.1"
+"@jupyterlab/ui-components@npm:^4, @jupyterlab/ui-components@npm:^4.1.3":
+  version: 4.1.3
+  resolution: "@jupyterlab/ui-components@npm:4.1.3"
   dependencies:
     "@jupyter/react-components": ^0.15.2
     "@jupyter/web-components": ^0.15.2
-    "@jupyterlab/coreutils": ^6.1.1
-    "@jupyterlab/observables": ^5.1.1
-    "@jupyterlab/rendermime-interfaces": ^3.9.1
-    "@jupyterlab/translation": ^4.1.1
+    "@jupyterlab/coreutils": ^6.1.3
+    "@jupyterlab/observables": ^5.1.3
+    "@jupyterlab/rendermime-interfaces": ^3.9.3
+    "@jupyterlab/translation": ^4.1.3
     "@lumino/algorithm": ^2.0.1
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/messaging": ^2.0.1
     "@lumino/polling": ^2.1.2
     "@lumino/properties": ^2.0.1
@@ -1089,15 +1069,15 @@
     "@rjsf/core": ^5.13.4
     "@rjsf/utils": ^5.13.4
     react: ^18.2.0
     react-dom: ^18.2.0
     typestyle: ^2.0.4
   peerDependencies:
     react: ^18.2.0
-  checksum: ac0762493671fdb146b9655b260d09de95163030a7adcbaedb41a74c67b21b72916b3a6b51e3fb54a9f1785364f5e413edd2667a9615a5d98922bdaaeb5142e4
+  checksum: 37a666f71440e4e9e8c4eca683d605763c3a3c90a00c3f5696c4f6e4ba59bc6e46aff303419c07689c7356d9a04a7ebf60ed1d3d4cc65153a453eea0636258dd
   languageName: node
   linkType: hard
 
 "@lezer/common@npm:^1.0.0, @lezer/common@npm:^1.0.2, @lezer/common@npm:^1.1.0, @lezer/common@npm:^1.2.0, @lezer/common@npm:^1.2.1":
   version: 1.2.1
   resolution: "@lezer/common@npm:1.2.1"
   checksum: 0bd092e293a509ce334f4aaf9a4d4a25528f743cd9d7e7948c697e34ac703b805b288b62ad01563488fb206fc34ff05084f7fc5d864be775924b3d0d53ea5dd2
@@ -1112,21 +1092,21 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: a319cd46fd32affc07c9432e9b2b9954becf7766be0361176c525d03474bb794cc051aad9932f48c9df33833eee1d6bfdccab12e571f2b137b4ca765c60c75de
   languageName: node
   linkType: hard
 
 "@lezer/css@npm:^1.0.0, @lezer/css@npm:^1.1.0":
-  version: 1.1.7
-  resolution: "@lezer/css@npm:1.1.7"
+  version: 1.1.8
+  resolution: "@lezer/css@npm:1.1.8"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 7760d294fd0b1ac6db319c4990517c1ed9027d6757de537553624238056df6e1ef1b6a571a023a4bce3d7a2b891036d9f85f76f2109f503bea94837f90c64bc2
+  checksum: 1f5968360dbac7ba27f0c2a194143769f7b01824715274dd8507dacf13cc790bb8c48ce95de355e9c58be93bb3e271bf98b9fc51213f79e4ce918e7c7ebbef04
   languageName: node
   linkType: hard
 
 "@lezer/generator@npm:^1.2.2":
   version: 1.6.0
   resolution: "@lezer/generator@npm:1.6.0"
   dependencies:
@@ -1144,21 +1124,21 @@
   dependencies:
     "@lezer/common": ^1.0.0
   checksum: 5b9dfe741f95db13f6124cb9556a43011cb8041ecf490be98d44a86b04d926a66e912bcd3a766f6a3d79e064410f1a2f60ab240b50b645a12c56987bf4870086
   languageName: node
   linkType: hard
 
 "@lezer/html@npm:^1.3.0":
-  version: 1.3.8
-  resolution: "@lezer/html@npm:1.3.8"
+  version: 1.3.9
+  resolution: "@lezer/html@npm:1.3.9"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 06bce804487435ea6ccb39595176bb65d68691f082b0b68fb7d22d90d4de9798a8202f16e9aefe22865db15257a37f6fca93275d660715eea98f7578579e7135
+  checksum: 40d89b0af4379768ce7d3e7162988e9ec73b42984e333e877c7451f7e2c10131e39e4b50150bc334093cbd84a3b34f9fc1a6ac62cbba51f503a495ad243e880b
   languageName: node
   linkType: hard
 
 "@lezer/java@npm:^1.0.0":
   version: 1.1.1
   resolution: "@lezer/java@npm:1.1.1"
   dependencies:
@@ -1240,56 +1220,38 @@
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
   checksum: fc5e97852b42beeb44a0ebe316dc64e3cc49ff481c22e3e67d6003fc4a5c257fcd94959cfcc76cd154fa172db9b3b4b28de5c09f10550d6e5f14869ddc274e5b
   languageName: node
   linkType: hard
 
 "@lezer/xml@npm:^1.0.0":
-  version: 1.0.4
-  resolution: "@lezer/xml@npm:1.0.4"
+  version: 1.0.5
+  resolution: "@lezer/xml@npm:1.0.5"
   dependencies:
     "@lezer/common": ^1.2.0
     "@lezer/highlight": ^1.0.0
     "@lezer/lr": ^1.0.0
-  checksum: 68a82085bff6c1525f4ef03cd9f9dac0132b3e03fe574e0289700dd4475056e40e8744cde15cf5ad6d3760d0d584ff85ce707e26a7c938d0c5fe2e325c1c336e
+  checksum: a0a077b9e455b03593b93a7fdff2a4eab2cb7b230c8e1b878a8bebe80184632b9cc75ca018f1f9e2acb3a26e1386f4777385ab6e87aea70ccf479cde5ca268ee
   languageName: node
   linkType: hard
 
 "@lumino/algorithm@npm:^1.9.2":
   version: 1.9.2
   resolution: "@lumino/algorithm@npm:1.9.2"
   checksum: a89e7c63504236119634858e271db1cc649684d30ced5a6ebe2788af7c0837f1e05a6fd3047d8525eb756c42ce137f76b3688f75fd3ef915b71cd4f213dfbb96
   languageName: node
   linkType: hard
 
-"@lumino/algorithm@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/algorithm@npm:2.0.0"
-  checksum: 663edf536e94397b449c6a2643a735e602fbb396dec86b56ad1193a768dce27c6e7da5ad0384aa90086ea44cbb64dde3f9d565e9fd81858f1eb0c6b4253f3b94
-  languageName: node
-  linkType: hard
-
 "@lumino/algorithm@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/algorithm@npm:2.0.1"
   checksum: cbf7fcf6ee6b785ea502cdfddc53d61f9d353dcb9659343511d5cd4b4030be2ff2ca4c08daec42f84417ab0318a3d9972a17319fa5231693e109ab112dcf8000
   languageName: node
   linkType: hard
 
-"@lumino/application@npm:^2.1.1":
-  version: 2.2.0
-  resolution: "@lumino/application@npm:2.2.0"
-  dependencies:
-    "@lumino/commands": ^2.1.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/widgets": ^2.2.0
-  checksum: b62da44b21d110c5d3478a49549326974b59325b8c60a58905d8e5ef08210273cd013cb60387d1f082fb79377a230278e2cf63e345491b0a54c75fdcc6164a68
-  languageName: node
-  linkType: hard
-
 "@lumino/application@npm:^2.3.0":
   version: 2.3.0
   resolution: "@lumino/application@npm:2.3.0"
   dependencies:
     "@lumino/commands": ^2.2.0
     "@lumino/coreutils": ^2.1.2
     "@lumino/widgets": ^2.3.1
@@ -1302,47 +1264,23 @@
   resolution: "@lumino/collections@npm:1.9.3"
   dependencies:
     "@lumino/algorithm": ^1.9.2
   checksum: 1c87a12743eddd6f6b593e47945a5645e2f99ad61c5192499b0745e48ee9aff263c7145541e77dfeea4c9f50bdd017fddfa47bfc60e718de4f28533ce45bf8c3
   languageName: node
   linkType: hard
 
-"@lumino/collections@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/collections@npm:2.0.0"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0
-  checksum: 4a7fc3571e92a1368a1ef01300ad7b6e0d4ff13cb78b89533d5962eea66d4a7550e15d8b80fa3ab1816b1a89382f35015f9dddf72ab04654c17e5b516b845d8f
-  languageName: node
-  linkType: hard
-
 "@lumino/collections@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/collections@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: 8a29b7973a388a33c5beda0819dcd2dc2aad51a8406dcfd4581b055a9f77a39dc5800f7a8b4ae3c0bb97ae7b56a7a869e2560ffb7a920a28e93b477ba05907d6
   languageName: node
   linkType: hard
 
-"@lumino/commands@npm:^2.1.1, @lumino/commands@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/commands@npm:2.1.2"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/keyboard": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-  checksum: c0b5ce8c5e1a86a98a90f54bb07b74742748110cf3362b86ff8328c1b5475c4dc05f1c4c9f50bf79e51c4e2ddc5cd69d6194f3d39dd5b58f357b0f30758bf35b
-  languageName: node
-  linkType: hard
-
 "@lumino/commands@npm:^2.2.0":
   version: 2.2.0
   resolution: "@lumino/commands@npm:2.2.0"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
@@ -1357,80 +1295,40 @@
 "@lumino/coreutils@npm:^1.11.0 || ^2.0.0, @lumino/coreutils@npm:^1.11.0 || ^2.1.2, @lumino/coreutils@npm:^1.11.1 || ^2.1, @lumino/coreutils@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/coreutils@npm:2.1.2"
   checksum: 7865317ac0676b448d108eb57ab5d8b2a17c101995c0f7a7106662d9fe6c859570104525f83ee3cda12ae2e326803372206d6f4c1f415a5b59e4158a7b81066f
   languageName: node
   linkType: hard
 
-"@lumino/coreutils@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/coreutils@npm:2.1.1"
-  checksum: dfdeb2b0282caae17b6c3edfebadf4ce7c75fc879fa60cacfef9b154412f4b35e4ffd95b1833b99d8dacb99aaaa04513570129ae2024c3f33e2677a01f0576ce
-  languageName: node
-  linkType: hard
-
-"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2.1.2":
+"@lumino/disposable@npm:^1.10.0 || ^2.0.0, @lumino/disposable@npm:^2, @lumino/disposable@npm:^2.1.2":
   version: 2.1.2
   resolution: "@lumino/disposable@npm:2.1.2"
   dependencies:
     "@lumino/signaling": ^2.1.2
   checksum: ac2fb2bf18d0b2939fda454f3db248a0ff6e8a77b401e586d1caa9293b3318f808b93a117c9c3ac27cd17aab545aea83b49108d099b9b2f5503ae2a012fbc6e2
   languageName: node
   linkType: hard
 
-"@lumino/disposable@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/disposable@npm:2.1.1"
-  dependencies:
-    "@lumino/signaling": ^2.1.1
-  checksum: ed6cdfe13f3346178a087690d4e7baeccaed7e73ca23cb239765202409f5c01b4729a4058b4717f963462ee9ef2e5cb14ad1974e3163741267290edc3715c85c
-  languageName: node
-  linkType: hard
-
-"@lumino/domutils@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/domutils@npm:2.0.0"
-  checksum: 4a146bfc1006d5fd00ccecc61d9803965d269c15c48c892fd87216336ce967f0db91f31203c5616c83d260224cddf25af4abb6704a6770757d19e44068f690bf
-  languageName: node
-  linkType: hard
-
 "@lumino/domutils@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/domutils@npm:2.0.1"
   checksum: 61fa0ab226869dfbb763fc426790cf5a43b7d6f4cea1364c6dd56d61c44bff05eea188d33ff847449608ef58ed343161bee15c19b96f35410e4ee35815dc611a
   languageName: node
   linkType: hard
 
-"@lumino/dragdrop@npm:^2.1.1, @lumino/dragdrop@npm:^2.1.2":
-  version: 2.1.2
-  resolution: "@lumino/dragdrop@npm:2.1.2"
-  dependencies:
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-  checksum: 7ac64ec11423ec89fea937aa6c9ca818933ee98e775e500018a0a948f32171932033a1e302a48395cbe9bfeaa635acde2393fd935db14d7b1d569ca6a1daaa77
-  languageName: node
-  linkType: hard
-
 "@lumino/dragdrop@npm:^2.1.4":
   version: 2.1.4
   resolution: "@lumino/dragdrop@npm:2.1.4"
   dependencies:
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
   checksum: 43d82484b13b38b612e7dfb424a840ed6a38d0db778af10655c4ba235c67b5b12db1683929b35a36ab2845f77466066dfd1ee25c1c273e8e175677eba9dc560d
   languageName: node
   linkType: hard
 
-"@lumino/keyboard@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/keyboard@npm:2.0.0"
-  checksum: 3852ba51f437b1c1d7e552a0f844592a05e04dd5012070dc6e4384c58965d1ebf536c6875c1b7bae03cde3c715ddc36cd290992fcefc1a8c39094194f4689fdd
-  languageName: node
-  linkType: hard
-
 "@lumino/keyboard@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/keyboard@npm:2.0.1"
   checksum: cf33f13427a418efd7cc91061233321e860d5404f3d86397781028309bef86c8ad2d88276ffe335c1db0fe619bd9d1e60641c81f881696957a58703ee4652c3e
   languageName: node
   linkType: hard
 
@@ -1440,24 +1338,14 @@
   dependencies:
     "@lumino/algorithm": ^1.9.2
     "@lumino/collections": ^1.9.3
   checksum: 1131e80379fa9b8a9b5d3418c90e25d4be48e2c92ec711518190772f9e8845a695bef45daddd06a129168cf6f158c8ad80ae86cb245f566e9195bbd9a0843b7a
   languageName: node
   linkType: hard
 
-"@lumino/messaging@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/messaging@npm:2.0.0"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/collections": ^2.0.0
-  checksum: 1e82dcf9b110834d4342dc63dfeac0ee780880fb99051bd82d00a1f83afd91b276c1cea5af85a414d92c527adc365d54f20ec780123b562f89c5a2cd3e96bf81
-  languageName: node
-  linkType: hard
-
 "@lumino/messaging@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/messaging@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/collections": ^2.0.1
   checksum: 964c4651c374b17452b4252b7d71500b32d2ecd87c192fc5bcf5d3bd1070661d78d07edcac8eca7d1d6fd50aa25992505485e1296d6dd995691b8e349b652045
@@ -1471,21 +1359,14 @@
     "@lumino/coreutils": ^2.1.2
     "@lumino/disposable": ^2.1.2
     "@lumino/signaling": ^2.1.2
   checksum: fa9b401e6dbeb8f31d7e3ba485e8ef1e0c92b3f2da086239c0ed49931026f5d3528709193c93e031e35ac624fb4bbbfcdcbaa0e25eb797f36e2952e5cd91e9e3
   languageName: node
   linkType: hard
 
-"@lumino/properties@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/properties@npm:2.0.0"
-  checksum: 81187a11a779eed4e20ff0035e77dee99bd271b0cf649096c4e8809dd6bdd06955b1a974bc1a115e536f8d2840b30183bb78a362b2c6991824477df6d17e6c59
-  languageName: node
-  linkType: hard
-
 "@lumino/properties@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/properties@npm:2.0.1"
   checksum: c50173a935148cc4148fdaea119df1d323ee004ae16ab666800388d27e9730345629662d85f25591683329b39f0cdae60ee8c94e8943b4d0ef7d7370a38128d6
   languageName: node
   linkType: hard
 
@@ -1495,58 +1376,39 @@
   dependencies:
     "@lumino/algorithm": ^2.0.1
     "@lumino/coreutils": ^2.1.2
   checksum: ad7d7153db57980da899c43e412e6130316ef30b231a70250e7af49058db16cadb018c1417a2ea8083d83c48623cfe6b705fa82bf10216b1a8949aed9f4aca4e
   languageName: node
   linkType: hard
 
-"@lumino/signaling@npm:^2.1.1":
-  version: 2.1.1
-  resolution: "@lumino/signaling@npm:2.1.1"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/coreutils": ^2.1.1
-  checksum: 283ad4239b8577f68aca3d0b2606f73cc1c775f84cab25cf49aa6cd195f0d87949ef43fdff03b38b5a49ebbf2468581c6786d5f8b6159a04b2051260be5eab86
-  languageName: node
-  linkType: hard
-
-"@lumino/virtualdom@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "@lumino/virtualdom@npm:2.0.0"
-  dependencies:
-    "@lumino/algorithm": ^2.0.0
-  checksum: 6fc1d88e7d4a656be7664ccfc5745eb1d4e3d2034db0b11ad6abefcc642f22d265003eef0e1d02bca2e42b6da127123118c631369006f78e88a08885a6f36c25
-  languageName: node
-  linkType: hard
-
 "@lumino/virtualdom@npm:^2.0.1":
   version: 2.0.1
   resolution: "@lumino/virtualdom@npm:2.0.1"
   dependencies:
     "@lumino/algorithm": ^2.0.1
   checksum: cf59b6f15b430e13e9e657b7a0619b9056cd9ea7b2a87f407391d071c501b77403c302b6a66dca510382045e75b2e3fe551630bb391f1c6b33678057d4bec164
   languageName: node
   linkType: hard
 
-"@lumino/widgets@npm:^2.1.1":
-  version: 2.2.0
-  resolution: "@lumino/widgets@npm:2.2.0"
+"@lumino/widgets@npm:^2":
+  version: 2.3.1
+  resolution: "@lumino/widgets@npm:2.3.1"
   dependencies:
-    "@lumino/algorithm": ^2.0.0
-    "@lumino/commands": ^2.1.2
-    "@lumino/coreutils": ^2.1.1
-    "@lumino/disposable": ^2.1.1
-    "@lumino/domutils": ^2.0.0
-    "@lumino/dragdrop": ^2.1.2
-    "@lumino/keyboard": ^2.0.0
-    "@lumino/messaging": ^2.0.0
-    "@lumino/properties": ^2.0.0
-    "@lumino/signaling": ^2.1.1
-    "@lumino/virtualdom": ^2.0.0
-  checksum: 963c0e54102b786a9cbf3467041c9f6f5c275af751afc311ebeba30d56516767c463c425e321bb389eaa66726dfc4420119a9a58573dcbf3110aba9515c80606
+    "@lumino/algorithm": ^2.0.1
+    "@lumino/commands": ^2.2.0
+    "@lumino/coreutils": ^2.1.2
+    "@lumino/disposable": ^2.1.2
+    "@lumino/domutils": ^2.0.1
+    "@lumino/dragdrop": ^2.1.4
+    "@lumino/keyboard": ^2.0.1
+    "@lumino/messaging": ^2.0.1
+    "@lumino/properties": ^2.0.1
+    "@lumino/signaling": ^2.1.2
+    "@lumino/virtualdom": ^2.0.1
+  checksum: ba7b8f8839c1cd2a41dbda13281094eb6981a270cccf4f25a0cf83686dcc526a2d8044a20204317630bb7dd4a04d65361408c7623a921549c781afca84b91c67
   languageName: node
   linkType: hard
 
 "@microsoft/fast-colors@npm:^5.3.1":
   version: 5.3.1
   resolution: "@microsoft/fast-colors@npm:5.3.1"
   checksum: ff87f402faadb4b5aeee3d27762566c11807f927cd4012b8bbc7f073ca68de0e2197f95330ff5dfd7038f4b4f0e2f51b11feb64c5d570f5c598d37850a5daf60
@@ -1617,514 +1479,393 @@
     "@nodelib/fs.scandir": 2.1.5
     fastq: ^1.6.0
   checksum: 190c643f156d8f8f277bf2a6078af1ffde1fd43f498f187c2db24d35b4b4b5785c02c7dc52e356497b9a1b65b13edc996de08de0b961c32844364da02986dc53
   languageName: node
   linkType: hard
 
 "@rjsf/core@npm:^5.13.4":
-  version: 5.17.0
-  resolution: "@rjsf/core@npm:5.17.0"
+  version: 5.17.1
+  resolution: "@rjsf/core@npm:5.17.1"
   dependencies:
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     markdown-to-jsx: ^7.4.1
     nanoid: ^3.3.7
     prop-types: ^15.8.1
   peerDependencies:
     "@rjsf/utils": ^5.16.x
     react: ^16.14.0 || >=17
-  checksum: adfcbd1d44cef5f9e5de2873096085abd03b146dcef2c9c226060341ce2c935b5399e4ad5f00ad5091394224f5859bd6ac9bac533537dc5c8e2edb16b52b67cf
+  checksum: 2dead2886a4db152d259d3e85281c1fa5975eeac5f05c2840201ccc583ef1cf9d48c922cd404d515133e140eae7a8fca4aa63ccde0bcfe63d0b3fbe3cd621aed
   languageName: node
   linkType: hard
 
 "@rjsf/utils@npm:^5.13.4":
-  version: 5.17.0
-  resolution: "@rjsf/utils@npm:5.17.0"
+  version: 5.17.1
+  resolution: "@rjsf/utils@npm:5.17.1"
   dependencies:
     json-schema-merge-allof: ^0.8.1
     jsonpointer: ^5.0.1
     lodash: ^4.17.21
     lodash-es: ^4.17.21
     react-is: ^18.2.0
   peerDependencies:
     react: ^16.14.0 || >=17
-  checksum: 01d0001f83083764a8552e009aa7df084621df9d1fc6ccdfad9d534513084421b1ad7494cab77b9b8205d680fd915f612d87800e20ab242e7066f33184c73d4f
+  checksum: 83010de66b06f1046b023a0b7d0bf30b5f47b152893c3b12f1f42faa89e7c7d18b2f04fe2e9035e5f63454317f09e6d5753fc014d43b933c8023b71fc50c3acf
   languageName: node
   linkType: hard
 
 "@types/backbone@npm:1.4.14":
   version: 1.4.14
   resolution: "@types/backbone@npm:1.4.14"
   dependencies:
     "@types/jquery": "*"
     "@types/underscore": "*"
   checksum: 4f44bfb71d75332b5de610be7687f4ae523ad4ef02da844a828403b534b6a94a6288b32cab64371d0ad526e35cfed511652ac53af22d0b9caaac3f4cfb4375dd
   languageName: node
   linkType: hard
 
 "@types/eslint-scope@npm:^3.7.3":
-  version: 3.7.4
-  resolution: "@types/eslint-scope@npm:3.7.4"
+  version: 3.7.7
+  resolution: "@types/eslint-scope@npm:3.7.7"
   dependencies:
     "@types/eslint": "*"
     "@types/estree": "*"
-  checksum: ea6a9363e92f301cd3888194469f9ec9d0021fe0a397a97a6dd689e7545c75de0bd2153dfb13d3ab532853a278b6572c6f678ce846980669e41029d205653460
+  checksum: e2889a124aaab0b89af1bab5959847c5bec09809209255de0e63b9f54c629a94781daa04adb66bffcdd742f5e25a17614fb933965093c0eea64aacda4309380e
   languageName: node
   linkType: hard
 
 "@types/eslint@npm:*":
-  version: 8.21.1
-  resolution: "@types/eslint@npm:8.21.1"
+  version: 8.56.5
+  resolution: "@types/eslint@npm:8.56.5"
   dependencies:
     "@types/estree": "*"
     "@types/json-schema": "*"
-  checksum: 584068441e4000c7b41c8928274fdcc737bc62f564928c30eb64ec41bbdbac31612f9fedaf490bceab31ec8305e99615166428188ea345d58878394683086fae
-  languageName: node
-  linkType: hard
-
-"@types/estree@npm:*, @types/estree@npm:^0.0.51":
-  version: 0.0.51
-  resolution: "@types/estree@npm:0.0.51"
-  checksum: e56a3bcf759fd9185e992e7fdb3c6a5f81e8ff120e871641607581fb3728d16c811702a7d40fa5f869b7f7b4437ab6a87eb8d98ffafeee51e85bbe955932a189
+  checksum: 95a7a23ca38c78e5c27a2ed36ef60f094d5e6589e3473c320b6ff69eb3ca6333d5b7f0d5053416369f5ab2fb86874df19562d4d67a98237c17def6e30abff540
   languageName: node
   linkType: hard
 
-"@types/estree@npm:^1.0.0":
-  version: 1.0.1
-  resolution: "@types/estree@npm:1.0.1"
-  checksum: e9aa175eacb797216fafce4d41e8202c7a75555bc55232dee0f9903d7171f8f19f0ae7d5191bb1a88cb90e65468be508c0df850a9fb81b4433b293a5a749899d
+"@types/estree@npm:*, @types/estree@npm:^1.0.5":
+  version: 1.0.5
+  resolution: "@types/estree@npm:1.0.5"
+  checksum: dd8b5bed28e6213b7acd0fb665a84e693554d850b0df423ac8076cc3ad5823a6bc26b0251d080bdc545af83179ede51dd3f6fa78cad2c46ed1f29624ddf3e41a
   languageName: node
   linkType: hard
 
 "@types/jquery@npm:*":
   version: 3.5.29
   resolution: "@types/jquery@npm:3.5.29"
   dependencies:
     "@types/sizzle": "*"
   checksum: 5e959762d6f7050b07b4387b6507a308113384566a77cfc4f8d0f54c2fb0a79f6bc8c057706c6aa4840cde56f32ad0e5814fb53c5f078c5db9e01670a1ecd535
   languageName: node
   linkType: hard
 
-"@types/json-schema@npm:*, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8":
-  version: 7.0.11
-  resolution: "@types/json-schema@npm:7.0.11"
-  checksum: 527bddfe62db9012fccd7627794bd4c71beb77601861055d87e3ee464f2217c85fca7a4b56ae677478367bbd248dbde13553312b7d4dbc702a2f2bbf60c4018d
-  languageName: node
-  linkType: hard
-
-"@types/json-schema@npm:^7.0.12":
+"@types/json-schema@npm:*, @types/json-schema@npm:^7.0.12, @types/json-schema@npm:^7.0.5, @types/json-schema@npm:^7.0.8, @types/json-schema@npm:^7.0.9":
   version: 7.0.15
   resolution: "@types/json-schema@npm:7.0.15"
   checksum: 97ed0cb44d4070aecea772b7b2e2ed971e10c81ec87dd4ecc160322ffa55ff330dace1793489540e3e318d90942064bb697cc0f8989391797792d919737b3b98
   languageName: node
   linkType: hard
 
-"@types/json-schema@npm:^7.0.9":
-  version: 7.0.12
-  resolution: "@types/json-schema@npm:7.0.12"
-  checksum: 00239e97234eeb5ceefb0c1875d98ade6e922bfec39dd365ec6bd360b5c2f825e612ac4f6e5f1d13601b8b30f378f15e6faa805a3a732f4a1bbe61915163d293
-  languageName: node
-  linkType: hard
-
 "@types/lodash@npm:^4.14.134":
   version: 4.14.202
   resolution: "@types/lodash@npm:4.14.202"
   checksum: a91acf3564a568c6f199912f3eb2c76c99c5a0d7e219394294213b3f2d54f672619f0fde4da22b29dc5d4c31457cd799acc2e5cb6bd90f9af04a1578483b6ff7
   languageName: node
   linkType: hard
 
 "@types/node@npm:*":
-  version: 18.14.6
-  resolution: "@types/node@npm:18.14.6"
-  checksum: 2f88f482cabadc6dbddd627a1674239e68c3c9beab56eb4ae2309fb96fd17fc3a509d99b0309bafe13b58529574f49ecf3a583f2ebe2896dd32fe4be436dc96e
+  version: 20.11.24
+  resolution: "@types/node@npm:20.11.24"
+  dependencies:
+    undici-types: ~5.26.4
+  checksum: b11a650e09e254f4725c94f226752b69949a9ac4a5e004e98f109437ac50b02df3ab4d12b2086722fedf2cb62e68b9e723abd3f358a7d7d90d741a0d3bee90c2
   languageName: node
   linkType: hard
 
 "@types/prop-types@npm:*":
-  version: 15.7.5
-  resolution: "@types/prop-types@npm:15.7.5"
-  checksum: 5b43b8b15415e1f298243165f1d44390403bb2bd42e662bca3b5b5633fdd39c938e91b7fce3a9483699db0f7a715d08cef220c121f723a634972fdf596aec980
+  version: 15.7.11
+  resolution: "@types/prop-types@npm:15.7.11"
+  checksum: 7519ff11d06fbf6b275029fe03fff9ec377b4cb6e864cac34d87d7146c7f5a7560fd164bdc1d2dbe00b60c43713631251af1fd3d34d46c69cd354602bc0c7c54
   languageName: node
   linkType: hard
 
 "@types/react@npm:^18.0.26":
-  version: 18.2.55
-  resolution: "@types/react@npm:18.2.55"
+  version: 18.2.63
+  resolution: "@types/react@npm:18.2.63"
   dependencies:
     "@types/prop-types": "*"
     "@types/scheduler": "*"
     csstype: ^3.0.2
-  checksum: a8eb4fa77f73831b9112d4f11a7006217dc0740361649b9b0da3fd441d151a9cd415d5d68b91c0af4e430e063424d301c77489e5edaddc9f711c4e46cf9818a5
+  checksum: f3d496b9e3c40fe984aa2f22e0f3776a4f0be223f436ad3a2b79fed4b496ba1549999083408c2c975e5c8b029bfc9e8a2924788325e00de205cf70a10ef772d0
   languageName: node
   linkType: hard
 
 "@types/scheduler@npm:*":
-  version: 0.16.2
-  resolution: "@types/scheduler@npm:0.16.2"
-  checksum: b6b4dcfeae6deba2e06a70941860fb1435730576d3689225a421280b7742318d1548b3d22c1f66ab68e414f346a9542f29240bc955b6332c5b11e561077583bc
+  version: 0.16.8
+  resolution: "@types/scheduler@npm:0.16.8"
+  checksum: 6c091b096daa490093bf30dd7947cd28e5b2cd612ec93448432b33f724b162587fed9309a0acc104d97b69b1d49a0f3fc755a62282054d62975d53d7fd13472d
   languageName: node
   linkType: hard
 
 "@types/semver@npm:^7.5.0":
-  version: 7.5.7
-  resolution: "@types/semver@npm:7.5.7"
-  checksum: 5af9b13e3d74d86d4b618f6506ccbded801fb35dbc28608cd5a7bfb8bcac0021dd35ef305a72a0c2a8def0cff60acd706bfee16a9ed1c39a893d2a175e778ea7
+  version: 7.5.8
+  resolution: "@types/semver@npm:7.5.8"
+  checksum: ea6f5276f5b84c55921785a3a27a3cd37afee0111dfe2bcb3e03c31819c197c782598f17f0b150a69d453c9584cd14c4c4d7b9a55d2c5e6cacd4d66fdb3b3663
   languageName: node
   linkType: hard
 
 "@types/sizzle@npm:*":
   version: 2.3.8
   resolution: "@types/sizzle@npm:2.3.8"
   checksum: 2ac62443dc917f5f903cbd9afc51c7d6cc1c6569b4e1a15faf04aea5b13b486e7f208650014c3dc4fed34653eded3e00fe5abffe0e6300cbf0e8a01beebf11a6
   languageName: node
   linkType: hard
 
 "@types/source-list-map@npm:*":
-  version: 0.1.2
-  resolution: "@types/source-list-map@npm:0.1.2"
-  checksum: fda8f37537aca9d3ed860d559289ab1dddb6897e642e6f53e909bbd18a7ac3129a8faa2a7d093847c91346cf09c86ef36e350c715406fba1f2271759b449adf6
+  version: 0.1.6
+  resolution: "@types/source-list-map@npm:0.1.6"
+  checksum: 9cd294c121f1562062de5d241fe4d10780b1131b01c57434845fe50968e9dcf67ede444591c2b1ad6d3f9b6bc646ac02cc8f51a3577c795f9c64cf4573dcc6b1
   languageName: node
   linkType: hard
 
 "@types/underscore@npm:*":
   version: 1.11.15
   resolution: "@types/underscore@npm:1.11.15"
   checksum: 25fdf6da96e0d11ca39a4740aab6fa3bd717e57301be4cb9e7893dc0ad6ce330992d0c8e0b02cac5c5ea86df6f8949c5a8f1fb95f3666b85418d399d3b1112e9
   languageName: node
   linkType: hard
 
 "@types/webpack-sources@npm:^0.1.5":
-  version: 0.1.9
-  resolution: "@types/webpack-sources@npm:0.1.9"
+  version: 0.1.12
+  resolution: "@types/webpack-sources@npm:0.1.12"
   dependencies:
     "@types/node": "*"
     "@types/source-list-map": "*"
     source-map: ^0.6.1
-  checksum: bc09c584c7047e8aed29801a3981787dee3898e9e7a99891a362df114fcac3879eea5a00932314866a01b25220391839be09fe1487b16d4970ff4a7afd5b9725
+  checksum: 75342659a9889478969f7bb7360b998aa084ba11ab523c172ded6a807dac43ab2a9e1212078ef8bbf0f33e4fadd2c8a91b75d38184d8030d96a32fe819c9bb57
   languageName: node
   linkType: hard
 
 "@typescript-eslint/eslint-plugin@npm:^7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/eslint-plugin@npm:7.0.1"
+  version: 7.1.1
+  resolution: "@typescript-eslint/eslint-plugin@npm:7.1.1"
   dependencies:
     "@eslint-community/regexpp": ^4.5.1
-    "@typescript-eslint/scope-manager": 7.0.1
-    "@typescript-eslint/type-utils": 7.0.1
-    "@typescript-eslint/utils": 7.0.1
-    "@typescript-eslint/visitor-keys": 7.0.1
+    "@typescript-eslint/scope-manager": 7.1.1
+    "@typescript-eslint/type-utils": 7.1.1
+    "@typescript-eslint/utils": 7.1.1
+    "@typescript-eslint/visitor-keys": 7.1.1
     debug: ^4.3.4
     graphemer: ^1.4.0
     ignore: ^5.2.4
     natural-compare: ^1.4.0
     semver: ^7.5.4
     ts-api-utils: ^1.0.1
   peerDependencies:
     "@typescript-eslint/parser": ^7.0.0
     eslint: ^8.56.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: d2a6e84bb0aa22cb6d2f47bbb2e229e700a8ebc2e3fa02ead70450542345d5678411fa41e5d063debc3f014697f792cb1eb71deb8f45da80501cad912b313757
+  checksum: e439a09996dd1b2bc8a643d7a1c7aad09b744ee38f6d3a8d391a7a846a23eafd3b1513c73da363df62e756f8b3a27c569b12fcbedad0fc1f87c0af20fd53db8e
   languageName: node
   linkType: hard
 
 "@typescript-eslint/parser@npm:^7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/parser@npm:7.0.1"
+  version: 7.1.1
+  resolution: "@typescript-eslint/parser@npm:7.1.1"
   dependencies:
-    "@typescript-eslint/scope-manager": 7.0.1
-    "@typescript-eslint/types": 7.0.1
-    "@typescript-eslint/typescript-estree": 7.0.1
-    "@typescript-eslint/visitor-keys": 7.0.1
+    "@typescript-eslint/scope-manager": 7.1.1
+    "@typescript-eslint/types": 7.1.1
+    "@typescript-eslint/typescript-estree": 7.1.1
+    "@typescript-eslint/visitor-keys": 7.1.1
     debug: ^4.3.4
   peerDependencies:
     eslint: ^8.56.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: de86c90e3697c949a1572d3f258eedf1cb2358adde9b0069138082d06ffade463605bec8b516df656b8a7250e34579afbecfe7cebc9a991ab79a60528b62358f
+  checksum: 9a8494a3ca517759e33c8a153779efe1331d86bcd4af5110d14c79e2507596265dd7cf113c9312fdf97832b60e76646dbabe9b87eb55b6616ba2a0c038b9fad1
   languageName: node
   linkType: hard
 
-"@typescript-eslint/scope-manager@npm:7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/scope-manager@npm:7.0.1"
+"@typescript-eslint/scope-manager@npm:7.1.1":
+  version: 7.1.1
+  resolution: "@typescript-eslint/scope-manager@npm:7.1.1"
   dependencies:
-    "@typescript-eslint/types": 7.0.1
-    "@typescript-eslint/visitor-keys": 7.0.1
-  checksum: b949cb829e4ad4409539be1a434a18ee5b59e56a4b4c0a4687ffde5c70ddda0edf1638426e9832ca9840fb0a831632c926f43dcce86b41ddd16256fd21165505
+    "@typescript-eslint/types": 7.1.1
+    "@typescript-eslint/visitor-keys": 7.1.1
+  checksum: 4f91bed41b14051335ec7f73bb2c8970018ba2c056dda3166a722d85a620a610643e7f703304c03106759d0a195ea1d9ff44edcc86feb2c62817ae3d06276c49
   languageName: node
   linkType: hard
 
-"@typescript-eslint/type-utils@npm:7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/type-utils@npm:7.0.1"
+"@typescript-eslint/type-utils@npm:7.1.1":
+  version: 7.1.1
+  resolution: "@typescript-eslint/type-utils@npm:7.1.1"
   dependencies:
-    "@typescript-eslint/typescript-estree": 7.0.1
-    "@typescript-eslint/utils": 7.0.1
+    "@typescript-eslint/typescript-estree": 7.1.1
+    "@typescript-eslint/utils": 7.1.1
     debug: ^4.3.4
     ts-api-utils: ^1.0.1
   peerDependencies:
     eslint: ^8.56.0
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: eab9bea237c308d0c80ab68805ef6a3fa54d881cde59033a9740d8317f316821508b29eaeaff007a618dbda635b318ddfafe7e343e641d1a5364854792a7bc5f
+  checksum: d1afa5c5e4602495a545d0d32aca0bbf6963fb0cbf77e47b2a95883e96d35bd9d51e8eb8d51c7d5b7e4e6ed7a275970eb80ed566e25833c8b4517791df8e648a
   languageName: node
   linkType: hard
 
-"@typescript-eslint/types@npm:7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/types@npm:7.0.1"
-  checksum: 3bd1b16171f578064b47d0fa8c5c6e85e857de764e0898ac08fc79a551ec7447242b74d1e2f8eaac1da70d3fa045c9a4d0001c52bbc81b83e7d02ee8230c3d71
+"@typescript-eslint/types@npm:7.1.1":
+  version: 7.1.1
+  resolution: "@typescript-eslint/types@npm:7.1.1"
+  checksum: 42be2d881728d99ab50cb4133656d2f54770304a5dca83777a032b9ec20f6e11ca38db79d2b77b29b9cb41a052aa872f4ac2e37b61d40b438efe91e355ec798f
   languageName: node
   linkType: hard
 
-"@typescript-eslint/typescript-estree@npm:7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/typescript-estree@npm:7.0.1"
+"@typescript-eslint/typescript-estree@npm:7.1.1":
+  version: 7.1.1
+  resolution: "@typescript-eslint/typescript-estree@npm:7.1.1"
   dependencies:
-    "@typescript-eslint/types": 7.0.1
-    "@typescript-eslint/visitor-keys": 7.0.1
+    "@typescript-eslint/types": 7.1.1
+    "@typescript-eslint/visitor-keys": 7.1.1
     debug: ^4.3.4
     globby: ^11.1.0
     is-glob: ^4.0.3
     minimatch: 9.0.3
     semver: ^7.5.4
     ts-api-utils: ^1.0.1
   peerDependenciesMeta:
     typescript:
       optional: true
-  checksum: d7124ed84622725785cdd885d15eb3ba446e332d1727a3ccb1ab44f785b023b98912da2573dacba506c89c5146037cb9982a499ec64c100d607357334ecdf6a8
+  checksum: 19c62c792ff05ccea7e8c6054f55be7d2423695cb7ef84b955ee2b74d950e769b353100032467be71a436f3439ecba3b8709513581755e98e910ecb9d8198223
   languageName: node
   linkType: hard
 
-"@typescript-eslint/utils@npm:7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/utils@npm:7.0.1"
+"@typescript-eslint/utils@npm:7.1.1":
+  version: 7.1.1
+  resolution: "@typescript-eslint/utils@npm:7.1.1"
   dependencies:
     "@eslint-community/eslint-utils": ^4.4.0
     "@types/json-schema": ^7.0.12
     "@types/semver": ^7.5.0
-    "@typescript-eslint/scope-manager": 7.0.1
-    "@typescript-eslint/types": 7.0.1
-    "@typescript-eslint/typescript-estree": 7.0.1
+    "@typescript-eslint/scope-manager": 7.1.1
+    "@typescript-eslint/types": 7.1.1
+    "@typescript-eslint/typescript-estree": 7.1.1
     semver: ^7.5.4
   peerDependencies:
     eslint: ^8.56.0
-  checksum: b36669163136646aa8f9ef831f7e3026acc853e9083461a53fb89e53b7b0e5ade315a8387820632d370bfe8445db6489524570a253bcd8817e460e0e2b409c47
+  checksum: 76a499c28dec37effb3512a49e51e1d788e49647ab750fc8a0d16c3aae4b9fea83f1cd20b5bd0be6113eb6112a96e93ee3327ccfd5c80028526c3ce5a73b5027
   languageName: node
   linkType: hard
 
-"@typescript-eslint/visitor-keys@npm:7.0.1":
-  version: 7.0.1
-  resolution: "@typescript-eslint/visitor-keys@npm:7.0.1"
+"@typescript-eslint/visitor-keys@npm:7.1.1":
+  version: 7.1.1
+  resolution: "@typescript-eslint/visitor-keys@npm:7.1.1"
   dependencies:
-    "@typescript-eslint/types": 7.0.1
+    "@typescript-eslint/types": 7.1.1
     eslint-visitor-keys: ^3.4.1
-  checksum: ca07f5c6369f00d73e8bd22b1032288d11a5b4d25baca0f198c86f490c423b244b6a39e31c55fb45203a41879017d7eeab895fade7942c1795ec745bee6b411b
+  checksum: fc98a8782ad9c5dbb0d6ed89baa89c37d3cb28ecc08fb013180bed4e5336e1d289ad3cdb1cd71b9c0abb7b624858258c0d68fe4db8911416b61f13ec7c553a47
   languageName: node
   linkType: hard
 
 "@ungap/structured-clone@npm:^1.2.0":
   version: 1.2.0
   resolution: "@ungap/structured-clone@npm:1.2.0"
   checksum: 4f656b7b4672f2ce6e272f2427d8b0824ed11546a601d8d5412b9d7704e83db38a8d9f402ecdf2b9063fc164af842ad0ec4a55819f621ed7e7ea4d1efcc74524
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ast@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/ast@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/helper-numbers": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-  checksum: 1eee1534adebeece635362f8e834ae03e389281972611408d64be7895fc49f48f98fddbbb5339bf8a72cb101bcb066e8bca3ca1bf1ef47dadf89def0395a8d87
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/ast@npm:1.11.6, @webassemblyjs/ast@npm:^1.11.5":
   version: 1.11.6
   resolution: "@webassemblyjs/ast@npm:1.11.6"
   dependencies:
     "@webassemblyjs/helper-numbers": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
   checksum: 38ef1b526ca47c210f30975b06df2faf1a8170b1636ce239fc5738fc231ce28389dd61ecedd1bacfc03cbe95b16d1af848c805652080cb60982836eb4ed2c6cf
   languageName: node
   linkType: hard
 
-"@webassemblyjs/floating-point-hex-parser@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.1"
-  checksum: b8efc6fa08e4787b7f8e682182d84dfdf8da9d9c77cae5d293818bc4a55c1f419a87fa265ab85252b3e6c1fd323d799efea68d825d341a7c365c64bc14750e97
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/floating-point-hex-parser@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/floating-point-hex-parser@npm:1.11.6"
   checksum: 29b08758841fd8b299c7152eda36b9eb4921e9c584eb4594437b5cd90ed6b920523606eae7316175f89c20628da14326801090167cc7fbffc77af448ac84b7e2
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-api-error@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-api-error@npm:1.11.1"
-  checksum: 0792813f0ed4a0e5ee0750e8b5d0c631f08e927f4bdfdd9fe9105dc410c786850b8c61bff7f9f515fdfb149903bec3c976a1310573a4c6866a94d49bc7271959
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/helper-api-error@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-api-error@npm:1.11.6"
   checksum: e8563df85161096343008f9161adb138a6e8f3c2cc338d6a36011aa55eabb32f2fd138ffe63bc278d009ada001cc41d263dadd1c0be01be6c2ed99076103689f
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-buffer@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-buffer@npm:1.11.1"
-  checksum: a337ee44b45590c3a30db5a8b7b68a717526cf967ada9f10253995294dbd70a58b2da2165222e0b9830cd4fc6e4c833bf441a721128d1fe2e9a7ab26b36003ce
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/helper-buffer@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-buffer@npm:1.11.6"
   checksum: b14d0573bf680d22b2522e8a341ec451fddd645d1f9c6bd9012ccb7e587a2973b86ab7b89fe91e1c79939ba96095f503af04369a3b356c8023c13a5893221644
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-numbers@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-numbers@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/floating-point-hex-parser": 1.11.1
-    "@webassemblyjs/helper-api-error": 1.11.1
-    "@xtuc/long": 4.2.2
-  checksum: 44d2905dac2f14d1e9b5765cf1063a0fa3d57295c6d8930f6c59a36462afecc6e763e8a110b97b342a0f13376166c5d41aa928e6ced92e2f06b071fd0db59d3a
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/helper-numbers@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-numbers@npm:1.11.6"
   dependencies:
     "@webassemblyjs/floating-point-hex-parser": 1.11.6
     "@webassemblyjs/helper-api-error": 1.11.6
     "@xtuc/long": 4.2.2
   checksum: f4b562fa219f84368528339e0f8d273ad44e047a07641ffcaaec6f93e5b76fd86490a009aa91a294584e1436d74b0a01fa9fde45e333a4c657b58168b04da424
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-bytecode@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.1"
-  checksum: eac400113127832c88f5826bcc3ad1c0db9b3dbd4c51a723cfdb16af6bfcbceb608170fdaac0ab7731a7e18b291be7af68a47fcdb41cfe0260c10857e7413d97
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-wasm-bytecode@npm:1.11.6"
   checksum: 3535ef4f1fba38de3475e383b3980f4bbf3de72bbb631c2b6584c7df45be4eccd62c6ff48b5edd3f1bcff275cfd605a37679ec199fc91fd0a7705d7f1e3972dc
   languageName: node
   linkType: hard
 
-"@webassemblyjs/helper-wasm-section@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-buffer": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/wasm-gen": 1.11.1
-  checksum: 617696cfe8ecaf0532763162aaf748eb69096fb27950219bb87686c6b2e66e11cd0614d95d319d0ab1904bc14ebe4e29068b12c3e7c5e020281379741fe4bedf
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/helper-wasm-section@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/helper-wasm-section@npm:1.11.6"
   dependencies:
     "@webassemblyjs/ast": 1.11.6
     "@webassemblyjs/helper-buffer": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/wasm-gen": 1.11.6
   checksum: b2cf751bf4552b5b9999d27bbb7692d0aca75260140195cb58ea6374d7b9c2dc69b61e10b211a0e773f66209c3ddd612137ed66097e3684d7816f854997682e9
   languageName: node
   linkType: hard
 
-"@webassemblyjs/ieee754@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/ieee754@npm:1.11.1"
-  dependencies:
-    "@xtuc/ieee754": ^1.2.0
-  checksum: 23a0ac02a50f244471631802798a816524df17e56b1ef929f0c73e3cde70eaf105a24130105c60aff9d64a24ce3b640dad443d6f86e5967f922943a7115022ec
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/ieee754@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/ieee754@npm:1.11.6"
   dependencies:
     "@xtuc/ieee754": ^1.2.0
   checksum: 13574b8e41f6ca39b700e292d7edf102577db5650fe8add7066a320aa4b7a7c09a5056feccac7a74eb68c10dea9546d4461412af351f13f6b24b5f32379b49de
   languageName: node
   linkType: hard
 
-"@webassemblyjs/leb128@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/leb128@npm:1.11.1"
-  dependencies:
-    "@xtuc/long": 4.2.2
-  checksum: 33ccc4ade2f24de07bf31690844d0b1ad224304ee2062b0e464a610b0209c79e0b3009ac190efe0e6bd568b0d1578d7c3047fc1f9d0197c92fc061f56224ff4a
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/leb128@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/leb128@npm:1.11.6"
   dependencies:
     "@xtuc/long": 4.2.2
   checksum: 7ea942dc9777d4b18a5ebfa3a937b30ae9e1d2ce1fee637583ed7f376334dd1d4274f813d2e250056cca803e0952def4b954913f1a3c9068bcd4ab4ee5143bf0
   languageName: node
   linkType: hard
 
-"@webassemblyjs/utf8@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/utf8@npm:1.11.1"
-  checksum: 972c5cfc769d7af79313a6bfb96517253a270a4bf0c33ba486aa43cac43917184fb35e51dfc9e6b5601548cd5931479a42e42c89a13bb591ffabebf30c8a6a0b
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/utf8@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/utf8@npm:1.11.6"
   checksum: 807fe5b5ce10c390cfdd93e0fb92abda8aebabb5199980681e7c3743ee3306a75729bcd1e56a3903980e96c885ee53ef901fcbaac8efdfa480f9c0dae1d08713
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-edit@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-edit@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-buffer": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/helper-wasm-section": 1.11.1
-    "@webassemblyjs/wasm-gen": 1.11.1
-    "@webassemblyjs/wasm-opt": 1.11.1
-    "@webassemblyjs/wasm-parser": 1.11.1
-    "@webassemblyjs/wast-printer": 1.11.1
-  checksum: 6d7d9efaec1227e7ef7585a5d7ff0be5f329f7c1c6b6c0e906b18ed2e9a28792a5635e450aca2d136770d0207225f204eff70a4b8fd879d3ac79e1dcc26dbeb9
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/wasm-edit@npm:^1.11.5":
   version: 1.11.6
   resolution: "@webassemblyjs/wasm-edit@npm:1.11.6"
   dependencies:
     "@webassemblyjs/ast": 1.11.6
     "@webassemblyjs/helper-buffer": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
@@ -2133,102 +1874,53 @@
     "@webassemblyjs/wasm-opt": 1.11.6
     "@webassemblyjs/wasm-parser": 1.11.6
     "@webassemblyjs/wast-printer": 1.11.6
   checksum: 29ce75870496d6fad864d815ebb072395a8a3a04dc9c3f4e1ffdc63fc5fa58b1f34304a1117296d8240054cfdbc38aca88e71fb51483cf29ffab0a61ef27b481
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-gen@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-gen@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/ieee754": 1.11.1
-    "@webassemblyjs/leb128": 1.11.1
-    "@webassemblyjs/utf8": 1.11.1
-  checksum: 1f6921e640293bf99fb16b21e09acb59b340a79f986c8f979853a0ae9f0b58557534b81e02ea2b4ef11e929d946708533fd0693c7f3712924128fdafd6465f5b
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/wasm-gen@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/wasm-gen@npm:1.11.6"
   dependencies:
     "@webassemblyjs/ast": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
   checksum: a645a2eecbea24833c3260a249704a7f554ef4a94c6000984728e94bb2bc9140a68dfd6fd21d5e0bbb09f6dfc98e083a45760a83ae0417b41a0196ff6d45a23a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-opt@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-opt@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-buffer": 1.11.1
-    "@webassemblyjs/wasm-gen": 1.11.1
-    "@webassemblyjs/wasm-parser": 1.11.1
-  checksum: 21586883a20009e2b20feb67bdc451bbc6942252e038aae4c3a08e6f67b6bae0f5f88f20bfc7bd0452db5000bacaf5ab42b98cf9aa034a6c70e9fc616142e1db
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/wasm-opt@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/wasm-opt@npm:1.11.6"
   dependencies:
     "@webassemblyjs/ast": 1.11.6
     "@webassemblyjs/helper-buffer": 1.11.6
     "@webassemblyjs/wasm-gen": 1.11.6
     "@webassemblyjs/wasm-parser": 1.11.6
   checksum: b4557f195487f8e97336ddf79f7bef40d788239169aac707f6eaa2fa5fe243557c2d74e550a8e57f2788e70c7ae4e7d32f7be16101afe183d597b747a3bdd528
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wasm-parser@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wasm-parser@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/helper-api-error": 1.11.1
-    "@webassemblyjs/helper-wasm-bytecode": 1.11.1
-    "@webassemblyjs/ieee754": 1.11.1
-    "@webassemblyjs/leb128": 1.11.1
-    "@webassemblyjs/utf8": 1.11.1
-  checksum: 1521644065c360e7b27fad9f4bb2df1802d134dd62937fa1f601a1975cde56bc31a57b6e26408b9ee0228626ff3ba1131ae6f74ffb7d718415b6528c5a6dbfc2
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/wasm-parser@npm:1.11.6, @webassemblyjs/wasm-parser@npm:^1.11.5":
   version: 1.11.6
   resolution: "@webassemblyjs/wasm-parser@npm:1.11.6"
   dependencies:
     "@webassemblyjs/ast": 1.11.6
     "@webassemblyjs/helper-api-error": 1.11.6
     "@webassemblyjs/helper-wasm-bytecode": 1.11.6
     "@webassemblyjs/ieee754": 1.11.6
     "@webassemblyjs/leb128": 1.11.6
     "@webassemblyjs/utf8": 1.11.6
   checksum: 8200a8d77c15621724a23fdabe58d5571415cda98a7058f542e670ea965dd75499f5e34a48675184947c66f3df23adf55df060312e6d72d57908e3f049620d8a
   languageName: node
   linkType: hard
 
-"@webassemblyjs/wast-printer@npm:1.11.1":
-  version: 1.11.1
-  resolution: "@webassemblyjs/wast-printer@npm:1.11.1"
-  dependencies:
-    "@webassemblyjs/ast": 1.11.1
-    "@xtuc/long": 4.2.2
-  checksum: f15ae4c2441b979a3b4fce78f3d83472fb22350c6dc3fd34bfe7c3da108e0b2360718734d961bba20e7716cb8578e964b870da55b035e209e50ec9db0378a3f7
-  languageName: node
-  linkType: hard
-
 "@webassemblyjs/wast-printer@npm:1.11.6":
   version: 1.11.6
   resolution: "@webassemblyjs/wast-printer@npm:1.11.6"
   dependencies:
     "@webassemblyjs/ast": 1.11.6
     "@xtuc/long": 4.2.2
   checksum: d2fa6a4c427325ec81463e9c809aa6572af6d47f619f3091bf4c4a6fc34f1da3df7caddaac50b8e7a457f8784c62cd58c6311b6cb69b0162ccd8d4c072f79cf8
@@ -2318,23 +2010,14 @@
 "abab@npm:^2.0.3":
   version: 2.0.6
   resolution: "abab@npm:2.0.6"
   checksum: 6ffc1af4ff315066c62600123990d87551ceb0aafa01e6539da77b0f5987ac7019466780bf480f1787576d4385e3690c81ccc37cfda12819bf510b8ab47e5a3e
   languageName: node
   linkType: hard
 
-"acorn-import-assertions@npm:^1.7.6":
-  version: 1.8.0
-  resolution: "acorn-import-assertions@npm:1.8.0"
-  peerDependencies:
-    acorn: ^8
-  checksum: 5c4cf7c850102ba7ae0eeae0deb40fb3158c8ca5ff15c0bca43b5c47e307a1de3d8ef761788f881343680ea374631ae9e9615ba8876fee5268dbe068c98bcba6
-  languageName: node
-  linkType: hard
-
 "acorn-import-assertions@npm:^1.9.0":
   version: 1.9.0
   resolution: "acorn-import-assertions@npm:1.9.0"
   peerDependencies:
     acorn: ^8
   checksum: 944fb2659d0845c467066bdcda2e20c05abe3aaf11972116df457ce2627628a81764d800dd55031ba19de513ee0d43bb771bc679cc0eda66dc8b4fade143bc0c
   languageName: node
@@ -2345,33 +2028,15 @@
   resolution: "acorn-jsx@npm:5.3.2"
   peerDependencies:
     acorn: ^6.0.0 || ^7.0.0 || ^8.0.0
   checksum: c3d3b2a89c9a056b205b69530a37b972b404ee46ec8e5b341666f9513d3163e2a4f214a71f4dfc7370f5a9c07472d2fd1c11c91c3f03d093e37637d95da98950
   languageName: node
   linkType: hard
 
-"acorn@npm:^8.5.0, acorn@npm:^8.7.1":
-  version: 8.8.2
-  resolution: "acorn@npm:8.8.2"
-  bin:
-    acorn: bin/acorn
-  checksum: f790b99a1bf63ef160c967e23c46feea7787e531292bb827126334612c234ed489a0dc2c7ba33156416f0ffa8d25bf2b0fdb7f35c2ba60eb3e960572bece4001
-  languageName: node
-  linkType: hard
-
-"acorn@npm:^8.8.2":
-  version: 8.10.0
-  resolution: "acorn@npm:8.10.0"
-  bin:
-    acorn: bin/acorn
-  checksum: 538ba38af0cc9e5ef983aee196c4b8b4d87c0c94532334fa7e065b2c8a1f85863467bb774231aae91613fcda5e68740c15d97b1967ae3394d20faddddd8af61d
-  languageName: node
-  linkType: hard
-
-"acorn@npm:^8.9.0":
+"acorn@npm:^8.7.1, acorn@npm:^8.8.2, acorn@npm:^8.9.0":
   version: 8.11.3
   resolution: "acorn@npm:8.11.3"
   bin:
     acorn: bin/acorn
   checksum: 76d8e7d559512566b43ab4aadc374f11f563f0a9e21626dd59cb2888444e9445923ae9f3699972767f18af61df89cd89f5eaaf772d1327b055b45cb829b4a88c
   languageName: node
   linkType: hard
@@ -2462,25 +2127,53 @@
 "argparse@npm:^2.0.1":
   version: 2.0.1
   resolution: "argparse@npm:2.0.1"
   checksum: 83644b56493e89a254bae05702abf3a1101b4fa4d0ca31df1c9985275a5a5bd47b3c27b7fa0b71098d41114d8ca000e6ed90cad764b306f8a503665e4d517ced
   languageName: node
   linkType: hard
 
+"array-buffer-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "array-buffer-byte-length@npm:1.0.1"
+  dependencies:
+    call-bind: ^1.0.5
+    is-array-buffer: ^3.0.4
+  checksum: 53524e08f40867f6a9f35318fafe467c32e45e9c682ba67b11943e167344d2febc0f6977a17e699b05699e805c3e8f073d876f8bbf1b559ed494ad2cd0fae09e
+  languageName: node
+  linkType: hard
+
 "array-union@npm:^2.1.0":
   version: 2.1.0
   resolution: "array-union@npm:2.1.0"
   checksum: 5bee12395cba82da674931df6d0fea23c4aa4660cb3b338ced9f828782a65caa232573e6bf3968f23e0c5eb301764a382cef2f128b170a9dc59de0e36c39f98d
   languageName: node
   linkType: hard
 
-"available-typed-arrays@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "available-typed-arrays@npm:1.0.5"
-  checksum: 20eb47b3cefd7db027b9bbb993c658abd36d4edd3fe1060e83699a03ee275b0c9b216cc076ff3f2db29073225fb70e7613987af14269ac1fe2a19803ccc97f1a
+"arraybuffer.prototype.slice@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "arraybuffer.prototype.slice@npm:1.0.3"
+  dependencies:
+    array-buffer-byte-length: ^1.0.1
+    call-bind: ^1.0.5
+    define-properties: ^1.2.1
+    es-abstract: ^1.22.3
+    es-errors: ^1.2.1
+    get-intrinsic: ^1.2.3
+    is-array-buffer: ^3.0.4
+    is-shared-array-buffer: ^1.0.2
+  checksum: 352259cba534dcdd969c92ab002efd2ba5025b2e3b9bead3973150edbdf0696c629d7f4b3f061c5931511e8207bdc2306da614703c820b45dabce39e3daf7e3e
+  languageName: node
+  linkType: hard
+
+"available-typed-arrays@npm:^1.0.6, available-typed-arrays@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "available-typed-arrays@npm:1.0.7"
+  dependencies:
+    possible-typed-array-names: ^1.0.0
+  checksum: 1aa3ffbfe6578276996de660848b6e95669d9a95ad149e3dd0c0cda77db6ee1dbd9d1dd723b65b6d277b882dd0c4b91a654ae9d3cf9e1254b7e93e4908d78fd3
   languageName: node
   linkType: hard
 
 "backbone@npm:1.4.0":
   version: 1.4.0
   resolution: "backbone@npm:1.4.0"
   dependencies:
@@ -2527,56 +2220,59 @@
   resolution: "braces@npm:3.0.2"
   dependencies:
     fill-range: ^7.0.1
   checksum: e2a8e769a863f3d4ee887b5fe21f63193a891c68b612ddb4b68d82d1b5f3ff9073af066c343e9867a393fe4c2555dcb33e89b937195feb9c1613d259edfcd459
   languageName: node
   linkType: hard
 
-"browserslist@npm:^4.14.5":
-  version: 4.21.5
-  resolution: "browserslist@npm:4.21.5"
-  dependencies:
-    caniuse-lite: ^1.0.30001449
-    electron-to-chromium: ^1.4.284
-    node-releases: ^2.0.8
-    update-browserslist-db: ^1.0.10
+"browserslist@npm:^4.21.10":
+  version: 4.23.0
+  resolution: "browserslist@npm:4.23.0"
+  dependencies:
+    caniuse-lite: ^1.0.30001587
+    electron-to-chromium: ^1.4.668
+    node-releases: ^2.0.14
+    update-browserslist-db: ^1.0.13
   bin:
     browserslist: cli.js
-  checksum: 9755986b22e73a6a1497fd8797aedd88e04270be33ce66ed5d85a1c8a798292a65e222b0f251bafa1c2522261e237d73b08b58689d4920a607e5a53d56dc4706
+  checksum: 436f49e796782ca751ebab7edc010cfc9c29f68536f387666cd70ea22f7105563f04dd62c6ff89cb24cc3254d17cba385f979eeeb3484d43e012412ff7e75def
   languageName: node
   linkType: hard
 
 "buffer-from@npm:^1.0.0":
   version: 1.1.2
   resolution: "buffer-from@npm:1.1.2"
   checksum: 0448524a562b37d4d7ed9efd91685a5b77a50672c556ea254ac9a6d30e3403a517d8981f10e565db24e8339413b43c97ca2951f10e399c6125a0d8911f5679bb
   languageName: node
   linkType: hard
 
-"call-bind@npm:^1.0.0, call-bind@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "call-bind@npm:1.0.2"
+"call-bind@npm:^1.0.2, call-bind@npm:^1.0.5, call-bind@npm:^1.0.6, call-bind@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "call-bind@npm:1.0.7"
   dependencies:
-    function-bind: ^1.1.1
-    get-intrinsic: ^1.0.2
-  checksum: f8e31de9d19988a4b80f3e704788c4a2d6b6f3d17cfec4f57dc29ced450c53a49270dc66bf0fbd693329ee948dd33e6c90a329519aef17474a4d961e8d6426b0
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
+    function-bind: ^1.1.2
+    get-intrinsic: ^1.2.4
+    set-function-length: ^1.2.1
+  checksum: 295c0c62b90dd6522e6db3b0ab1ce26bdf9e7404215bda13cfee25b626b5ff1a7761324d58d38b1ef1607fc65aca2d06e44d2e18d0dfc6c14b465b00d8660029
   languageName: node
   linkType: hard
 
 "callsites@npm:^3.0.0":
   version: 3.1.0
   resolution: "callsites@npm:3.1.0"
   checksum: 072d17b6abb459c2ba96598918b55868af677154bec7e73d222ef95a8fdb9bbf7dae96a8421085cdad8cd190d86653b5b6dc55a4484f2e5b2e27d5e0c3fc15b3
   languageName: node
   linkType: hard
 
-"caniuse-lite@npm:^1.0.30001449":
-  version: 1.0.30001460
-  resolution: "caniuse-lite@npm:1.0.30001460"
-  checksum: dad91eb82aa65aecf33ad6a04ad620b9df6f0152020dc6c1874224e8c6f4aa50695f585201b3dfcd2760b3c43326a86c9505cc03af856698fbef67b267ef786f
+"caniuse-lite@npm:^1.0.30001587":
+  version: 1.0.30001594
+  resolution: "caniuse-lite@npm:1.0.30001594"
+  checksum: 59e52b2213f34fa9317813037fbab4f9b163f9bfeaeeb53035a57046ee2366b69eafc257997eab22982dc061d0576d1f4ef97c29425e1989f6589a7b1d8ed2d5
   languageName: node
   linkType: hard
 
 "chalk@npm:^2.3.0, chalk@npm:^2.4.1":
   version: 2.4.2
   resolution: "chalk@npm:2.4.2"
   dependencies:
@@ -2644,17 +2340,17 @@
   version: 1.1.4
   resolution: "color-name@npm:1.1.4"
   checksum: b0445859521eb4021cd0fb0cc1a75cecf67fceecae89b63f62b201cca8d345baf8b952c966862a9d9a2632987d4f6581f0ec8d957dfacece86f0a7919316f610
   languageName: node
   linkType: hard
 
 "colorette@npm:^2.0.14":
-  version: 2.0.19
-  resolution: "colorette@npm:2.0.19"
-  checksum: 888cf5493f781e5fcf54ce4d49e9d7d698f96ea2b2ef67906834bb319a392c667f9ec69f4a10e268d2946d13a9503d2d19b3abaaaf174e3451bfe91fb9d82427
+  version: 2.0.20
+  resolution: "colorette@npm:2.0.20"
+  checksum: 0c016fea2b91b733eb9f4bcdb580018f52c0bc0979443dad930e5037a968237ac53d9beb98e218d2e9235834f8eebce7f8e080422d6194e957454255bde71d3d
   languageName: node
   linkType: hard
 
 "commander@npm:^10.0.1":
   version: 10.0.1
   resolution: "commander@npm:10.0.1"
   checksum: 436901d64a818295803c1996cd856621a74f30b9f9e28a588e726b2b1670665bccd7c1a77007ebf328729f0139838a88a19265858a0fa7a8728c4656796db948
@@ -2760,28 +2456,34 @@
   peerDependencies:
     webpack: ^4.27.0 || ^5.0.0
   checksum: fb0742b30ac0919f94b99a323bdefe6d48ae46d66c7d966aae59031350532f368f8bba5951fcd268f2e053c5e6e4655551076268e9073ccb58e453f98ae58f8e
   languageName: node
   linkType: hard
 
 "css-loader@npm:^6.7.1":
-  version: 6.8.1
-  resolution: "css-loader@npm:6.8.1"
+  version: 6.10.0
+  resolution: "css-loader@npm:6.10.0"
   dependencies:
     icss-utils: ^5.1.0
-    postcss: ^8.4.21
+    postcss: ^8.4.33
     postcss-modules-extract-imports: ^3.0.0
-    postcss-modules-local-by-default: ^4.0.3
-    postcss-modules-scope: ^3.0.0
+    postcss-modules-local-by-default: ^4.0.4
+    postcss-modules-scope: ^3.1.1
     postcss-modules-values: ^4.0.0
     postcss-value-parser: ^4.2.0
-    semver: ^7.3.8
+    semver: ^7.5.4
   peerDependencies:
+    "@rspack/core": 0.x || 1.x
     webpack: ^5.0.0
-  checksum: 7c1784247bdbe76dc5c55fb1ac84f1d4177a74c47259942c9cfdb7a8e6baef11967a0bc85ac285f26bd26d5059decb848af8154a03fdb4f4894f41212f45eef3
+  peerDependenciesMeta:
+    "@rspack/core":
+      optional: true
+    webpack:
+      optional: true
+  checksum: ee3d62b5f7e4eb24281a22506431e920d07a45bd6ea627731ce583f3c6a846ab8b8b703bace599b9b35256b9e762f9f326d969abb72b69c7e6055eacf39074fd
   languageName: node
   linkType: hard
 
 "cssesc@npm:^3.0.0":
   version: 3.0.0
   resolution: "cssesc@npm:3.0.0"
   bin:
@@ -2794,17 +2496,17 @@
   version: 3.0.10
   resolution: "csstype@npm:3.0.10"
   checksum: 20a8fa324f2b33ddf94aa7507d1b6ab3daa6f3cc308888dc50126585d7952f2471de69b2dbe0635d1fdc31223fef8e070842691877e725caf456e2378685a631
   languageName: node
   linkType: hard
 
 "csstype@npm:^3.0.2":
-  version: 3.0.11
-  resolution: "csstype@npm:3.0.11"
-  checksum: 95e56abfe9ca219ae065acb4e43f61771a03170eed919127f558dfa168240867aba7629c8d98a201a0dd06d9a5ce82686f0570031c928516c61816adbc7c877f
+  version: 3.1.3
+  resolution: "csstype@npm:3.1.3"
+  checksum: 8db785cc92d259102725b3c694ec0c823f5619a84741b5c7991b8ad135dfaa66093038a1cc63e03361a6cd28d122be48f2106ae72334e067dd619a51f49eddf7
   languageName: node
   linkType: hard
 
 "data-urls@npm:^2.0.0":
   version: 2.0.0
   resolution: "data-urls@npm:2.0.0"
   dependencies:
@@ -2831,27 +2533,39 @@
   version: 0.1.4
   resolution: "deep-is@npm:0.1.4"
   checksum: edb65dd0d7d1b9c40b2f50219aef30e116cedd6fc79290e740972c132c09106d2e80aa0bc8826673dd5a00222d4179c84b36a790eef63a4c4bca75a37ef90804
   languageName: node
   linkType: hard
 
 "deepmerge@npm:^4.2.2":
-  version: 4.3.0
-  resolution: "deepmerge@npm:4.3.0"
-  checksum: c7980eb5c5be040b371f1df0d566473875cfabed9f672ccc177b81ba8eee5686ce2478de2f1d0076391621cbe729e5eacda397179a59ef0f68901849647db126
+  version: 4.3.1
+  resolution: "deepmerge@npm:4.3.1"
+  checksum: 2024c6a980a1b7128084170c4cf56b0fd58a63f2da1660dcfe977415f27b17dbe5888668b59d0b063753f3220719d5e400b7f113609489c90160bb9a5518d052
   languageName: node
   linkType: hard
 
-"define-properties@npm:^1.1.3, define-properties@npm:^1.1.4":
-  version: 1.2.0
-  resolution: "define-properties@npm:1.2.0"
+"define-data-property@npm:^1.0.1, define-data-property@npm:^1.1.2, define-data-property@npm:^1.1.4":
+  version: 1.1.4
+  resolution: "define-data-property@npm:1.1.4"
+  dependencies:
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
+    gopd: ^1.0.1
+  checksum: 8068ee6cab694d409ac25936eb861eea704b7763f7f342adbdfe337fc27c78d7ae0eff2364b2917b58c508d723c7a074326d068eef2e45c4edcd85cf94d0313b
+  languageName: node
+  linkType: hard
+
+"define-properties@npm:^1.1.3, define-properties@npm:^1.2.0, define-properties@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "define-properties@npm:1.2.1"
   dependencies:
+    define-data-property: ^1.0.1
     has-property-descriptors: ^1.0.0
     object-keys: ^1.1.1
-  checksum: e60aee6a19b102df4e2b1f301816804e81ab48bb91f00d0d935f269bf4b3f79c88b39e4f89eaa132890d23267335fd1140dfcd8d5ccd61031a0a2c41a54e33a6
+  checksum: b4ccd00597dd46cb2d4a379398f5b19fca84a16f3374e2249201992f36b30f6835949a9429669ee6b41b6e837205a163eadd745e472069e70dfc10f03e5fcc12
   languageName: node
   linkType: hard
 
 "dir-glob@npm:^3.0.1":
   version: 3.0.1
   resolution: "dir-glob@npm:3.0.1"
   dependencies:
@@ -2915,136 +2629,143 @@
     find-root: ^1.0.0
     lodash: ^4.17.4
     semver: ^5.4.1
   checksum: d77be45cb72d79a429c64d8f8f7603fea681d182fb795459a3d4afa608faad9a923378a7e80c6855f465263e1983140b6fc3682bd0213228b8cd7906ab4b934d
   languageName: node
   linkType: hard
 
-"electron-to-chromium@npm:^1.4.284":
-  version: 1.4.320
-  resolution: "electron-to-chromium@npm:1.4.320"
-  checksum: ea2c02bc286c0471ed7ad9b61225f6561921cf5f24a060cd1c46c2ea9932283ab924f66c370fbe5a229225dc1f747b395c943a0f5a9d058b72f561b1d8225787
+"electron-to-chromium@npm:^1.4.668":
+  version: 1.4.693
+  resolution: "electron-to-chromium@npm:1.4.693"
+  checksum: 3a173467da27d6c82e0e645ee2de3b6aa9cdbd0a8f6b314ddeeadc5b18ebe3555644ed9a720d9b72b7b9ed0574e2617277b7d34e6ee9c5aa962fd55cf1b1a41c
   languageName: node
   linkType: hard
 
 "emojis-list@npm:^3.0.0":
   version: 3.0.0
   resolution: "emojis-list@npm:3.0.0"
   checksum: ddaaa02542e1e9436c03970eeed445f4ed29a5337dfba0fe0c38dfdd2af5da2429c2a0821304e8a8d1cadf27fdd5b22ff793571fa803ae16852a6975c65e8e70
   languageName: node
   linkType: hard
 
-"enhanced-resolve@npm:^5.10.0":
-  version: 5.12.0
-  resolution: "enhanced-resolve@npm:5.12.0"
-  dependencies:
-    graceful-fs: ^4.2.4
-    tapable: ^2.2.0
-  checksum: bf3f787facaf4ce3439bef59d148646344e372bef5557f0d37ea8aa02c51f50a925cd1f07b8d338f18992c29f544ec235a8c64bcdb56030196c48832a5494174
-  languageName: node
-  linkType: hard
-
 "enhanced-resolve@npm:^5.15.0":
-  version: 5.15.0
-  resolution: "enhanced-resolve@npm:5.15.0"
+  version: 5.15.1
+  resolution: "enhanced-resolve@npm:5.15.1"
   dependencies:
     graceful-fs: ^4.2.4
     tapable: ^2.2.0
-  checksum: fbd8cdc9263be71cc737aa8a7d6c57b43d6aa38f6cc75dde6fcd3598a130cc465f979d2f4d01bb3bf475acb43817749c79f8eef9be048683602ca91ab52e4f11
+  checksum: 360f646c794323f2984b1ac751a878dd02ef30b565e106640b3d881a13ad16ce9c66e7c593cc34133f251ba3708cf6ae461e071b0f53ee65ff6650a779ed25a1
   languageName: node
   linkType: hard
 
 "entities@npm:^2.0.0":
   version: 2.2.0
   resolution: "entities@npm:2.2.0"
   checksum: 19010dacaf0912c895ea262b4f6128574f9ccf8d4b3b65c7e8334ad0079b3706376360e28d8843ff50a78aabcb8f08f0a32dbfacdc77e47ed77ca08b713669b3
   languageName: node
   linkType: hard
 
 "envinfo@npm:^7.7.3":
-  version: 7.8.1
-  resolution: "envinfo@npm:7.8.1"
+  version: 7.11.1
+  resolution: "envinfo@npm:7.11.1"
   bin:
     envinfo: dist/cli.js
-  checksum: de736c98d6311c78523628ff127af138451b162e57af5293c1b984ca821d0aeb9c849537d2fde0434011bed33f6bca5310ca2aab8a51a3f28fc719e89045d648
+  checksum: f3d38ab6bc62388466e86e2f5665f90f238ca349c81bb36b311d908cb5ca96650569b43b308c9dcb6725a222693f6c43a704794e74a68fb445ec5575a90ca05e
   languageName: node
   linkType: hard
 
 "error-ex@npm:^1.3.1":
   version: 1.3.2
   resolution: "error-ex@npm:1.3.2"
   dependencies:
     is-arrayish: ^0.2.1
   checksum: c1c2b8b65f9c91b0f9d75f0debaa7ec5b35c266c2cac5de412c1a6de86d4cbae04ae44e510378cb14d032d0645a36925d0186f8bb7367bcc629db256b743a001
   languageName: node
   linkType: hard
 
-"es-abstract@npm:^1.19.0, es-abstract@npm:^1.20.4":
-  version: 1.21.1
-  resolution: "es-abstract@npm:1.21.1"
-  dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
-    es-set-tostringtag: ^2.0.1
+"es-abstract@npm:^1.22.1, es-abstract@npm:^1.22.3":
+  version: 1.22.5
+  resolution: "es-abstract@npm:1.22.5"
+  dependencies:
+    array-buffer-byte-length: ^1.0.1
+    arraybuffer.prototype.slice: ^1.0.3
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
+    es-define-property: ^1.0.0
+    es-errors: ^1.3.0
+    es-set-tostringtag: ^2.0.3
     es-to-primitive: ^1.2.1
-    function-bind: ^1.1.1
-    function.prototype.name: ^1.1.5
-    get-intrinsic: ^1.1.3
-    get-symbol-description: ^1.0.0
+    function.prototype.name: ^1.1.6
+    get-intrinsic: ^1.2.4
+    get-symbol-description: ^1.0.2
     globalthis: ^1.0.3
     gopd: ^1.0.1
-    has: ^1.0.3
-    has-property-descriptors: ^1.0.0
-    has-proto: ^1.0.1
+    has-property-descriptors: ^1.0.2
+    has-proto: ^1.0.3
     has-symbols: ^1.0.3
-    internal-slot: ^1.0.4
-    is-array-buffer: ^3.0.1
+    hasown: ^2.0.1
+    internal-slot: ^1.0.7
+    is-array-buffer: ^3.0.4
     is-callable: ^1.2.7
-    is-negative-zero: ^2.0.2
+    is-negative-zero: ^2.0.3
     is-regex: ^1.1.4
-    is-shared-array-buffer: ^1.0.2
+    is-shared-array-buffer: ^1.0.3
     is-string: ^1.0.7
-    is-typed-array: ^1.1.10
+    is-typed-array: ^1.1.13
     is-weakref: ^1.0.2
-    object-inspect: ^1.12.2
+    object-inspect: ^1.13.1
     object-keys: ^1.1.1
-    object.assign: ^4.1.4
-    regexp.prototype.flags: ^1.4.3
-    safe-regex-test: ^1.0.0
-    string.prototype.trimend: ^1.0.6
-    string.prototype.trimstart: ^1.0.6
-    typed-array-length: ^1.0.4
+    object.assign: ^4.1.5
+    regexp.prototype.flags: ^1.5.2
+    safe-array-concat: ^1.1.0
+    safe-regex-test: ^1.0.3
+    string.prototype.trim: ^1.2.8
+    string.prototype.trimend: ^1.0.7
+    string.prototype.trimstart: ^1.0.7
+    typed-array-buffer: ^1.0.2
+    typed-array-byte-length: ^1.0.1
+    typed-array-byte-offset: ^1.0.2
+    typed-array-length: ^1.0.5
     unbox-primitive: ^1.0.2
-    which-typed-array: ^1.1.9
-  checksum: 23ff60d42d17a55d150e7bcedbdb065d4077a8b98c436e0e2e1ef4dd532a6d78a56028673de0bd8ed464a43c46ba781c50d9af429b6a17e44dbd14c7d7fb7926
+    which-typed-array: ^1.1.14
+  checksum: 984ab92f8226812365d1c4ecf12f3a408a4cc7a5bfe448f231fd39fa1ca9fb8cd65f27c76fc1a0bc3d1492c54b6637e57ad8e4954402e39bb916e9db4bcdbc61
   languageName: node
   linkType: hard
 
-"es-module-lexer@npm:^0.9.0":
-  version: 0.9.3
-  resolution: "es-module-lexer@npm:0.9.3"
-  checksum: 84bbab23c396281db2c906c766af58b1ae2a1a2599844a504df10b9e8dc77ec800b3211fdaa133ff700f5703d791198807bba25d9667392d27a5e9feda344da8
+"es-define-property@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "es-define-property@npm:1.0.0"
+  dependencies:
+    get-intrinsic: ^1.2.4
+  checksum: f66ece0a887b6dca71848fa71f70461357c0e4e7249696f81bad0a1f347eed7b31262af4a29f5d726dc026426f085483b6b90301855e647aa8e21936f07293c6
   languageName: node
   linkType: hard
 
-"es-module-lexer@npm:^1.2.1":
+"es-errors@npm:^1.2.1, es-errors@npm:^1.3.0":
   version: 1.3.0
-  resolution: "es-module-lexer@npm:1.3.0"
-  checksum: 48fd9f504a9d2a894126f75c8b7ccc6273a289983e9b67255f165bfd9ae765d50100218251e94e702ca567826905ea2f7b3b4a0c4d74d3ce99cce3a2a606a238
+  resolution: "es-errors@npm:1.3.0"
+  checksum: ec1414527a0ccacd7f15f4a3bc66e215f04f595ba23ca75cdae0927af099b5ec865f9f4d33e9d7e86f512f252876ac77d4281a7871531a50678132429b1271b5
   languageName: node
   linkType: hard
 
-"es-set-tostringtag@npm:^2.0.1":
-  version: 2.0.1
-  resolution: "es-set-tostringtag@npm:2.0.1"
+"es-module-lexer@npm:^1.2.1":
+  version: 1.4.1
+  resolution: "es-module-lexer@npm:1.4.1"
+  checksum: a11b5a256d4e8e9c7d94c2fd87415ccd1591617b6edd847e064503f8eaece2d25e2e9078a02c5ce3ed5e83bb748f5b4820efbe78072c8beb07ac619c2edec35d
+  languageName: node
+  linkType: hard
+
+"es-set-tostringtag@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "es-set-tostringtag@npm:2.0.3"
   dependencies:
-    get-intrinsic: ^1.1.3
-    has: ^1.0.3
-    has-tostringtag: ^1.0.0
-  checksum: ec416a12948cefb4b2a5932e62093a7cf36ddc3efd58d6c58ca7ae7064475ace556434b869b0bbeb0c365f1032a8ccd577211101234b69837ad83ad204fff884
+    get-intrinsic: ^1.2.4
+    has-tostringtag: ^1.0.2
+    hasown: ^2.0.1
+  checksum: 7227fa48a41c0ce83e0377b11130d324ac797390688135b8da5c28994c0165be8b252e15cd1de41e1325e5a5412511586960213e88f9ab4a5e7d028895db5129
   languageName: node
   linkType: hard
 
 "es-to-primitive@npm:^1.2.1":
   version: 1.2.1
   resolution: "es-to-primitive@npm:1.2.1"
   dependencies:
@@ -3052,17 +2773,17 @@
     is-date-object: ^1.0.1
     is-symbol: ^1.0.2
   checksum: 4ead6671a2c1402619bdd77f3503991232ca15e17e46222b0a41a5d81aebc8740a77822f5b3c965008e631153e9ef0580540007744521e72de8e33599fca2eed
   languageName: node
   linkType: hard
 
 "escalade@npm:^3.1.1":
-  version: 3.1.1
-  resolution: "escalade@npm:3.1.1"
-  checksum: a3e2a99f07acb74b3ad4989c48ca0c3140f69f923e56d0cba0526240ee470b91010f9d39001f2a4a313841d237ede70a729e92125191ba5d21e74b106800b133
+  version: 3.1.2
+  resolution: "escalade@npm:3.1.2"
+  checksum: 1ec0977aa2772075493002bdbd549d595ff6e9393b1cb0d7d6fcaf78c750da0c158f180938365486f75cb69fba20294351caddfce1b46552a7b6c3cde52eaa02
   languageName: node
   linkType: hard
 
 "escape-string-regexp@npm:^1.0.5":
   version: 1.0.5
   resolution: "escape-string-regexp@npm:1.0.5"
   checksum: 6092fda75c63b110c706b6a9bfde8a612ad595b628f0bd2147eea1d3406723020810e591effc7db1da91d80a71a737a313567c5abb3813e8d9c71f4aa595b410
@@ -3100,22 +2821,22 @@
   version: 3.4.3
   resolution: "eslint-visitor-keys@npm:3.4.3"
   checksum: 36e9ef87fca698b6fd7ca5ca35d7b2b6eeaaf106572e2f7fd31c12d3bfdaccdb587bba6d3621067e5aece31c8c3a348b93922ab8f7b2cbc6aaab5e1d89040c60
   languageName: node
   linkType: hard
 
 "eslint@npm:^8.36.0":
-  version: 8.56.0
-  resolution: "eslint@npm:8.56.0"
+  version: 8.57.0
+  resolution: "eslint@npm:8.57.0"
   dependencies:
     "@eslint-community/eslint-utils": ^4.2.0
     "@eslint-community/regexpp": ^4.6.1
     "@eslint/eslintrc": ^2.1.4
-    "@eslint/js": 8.56.0
-    "@humanwhocodes/config-array": ^0.11.13
+    "@eslint/js": 8.57.0
+    "@humanwhocodes/config-array": ^0.11.14
     "@humanwhocodes/module-importer": ^1.0.1
     "@nodelib/fs.walk": ^1.2.8
     "@ungap/structured-clone": ^1.2.0
     ajv: ^6.12.4
     chalk: ^4.0.0
     cross-spawn: ^7.0.2
     debug: ^4.3.2
@@ -3143,15 +2864,15 @@
     minimatch: ^3.1.2
     natural-compare: ^1.4.0
     optionator: ^0.9.3
     strip-ansi: ^6.0.1
     text-table: ^0.2.0
   bin:
     eslint: bin/eslint.js
-  checksum: 883436d1e809b4a25d9eb03d42f584b84c408dbac28b0019f6ea07b5177940bf3cca86208f749a6a1e0039b63e085ee47aca1236c30721e91f0deef5cc5a5136
+  checksum: 3a48d7ff85ab420a8447e9810d8087aea5b1df9ef68c9151732b478de698389ee656fd895635b5f2871c89ee5a2652b3f343d11e9db6f8486880374ebc74a2d9
   languageName: node
   linkType: hard
 
 "espree@npm:^9.6.0, espree@npm:^9.6.1":
   version: 9.6.1
   resolution: "espree@npm:9.6.1"
   dependencies:
@@ -3219,23 +2940,23 @@
   version: 3.1.3
   resolution: "fast-deep-equal@npm:3.1.3"
   checksum: e21a9d8d84f53493b6aa15efc9cfd53dd5b714a1f23f67fb5dc8f574af80df889b3bce25dc081887c6d25457cce704e636395333abad896ccdec03abaf1f3f9d
   languageName: node
   linkType: hard
 
 "fast-glob@npm:^3.2.9":
-  version: 3.2.12
-  resolution: "fast-glob@npm:3.2.12"
+  version: 3.3.2
+  resolution: "fast-glob@npm:3.3.2"
   dependencies:
     "@nodelib/fs.stat": ^2.0.2
     "@nodelib/fs.walk": ^1.2.3
     glob-parent: ^5.1.2
     merge2: ^1.3.0
     micromatch: ^4.0.4
-  checksum: 0b1990f6ce831c7e28c4d505edcdaad8e27e88ab9fa65eedadb730438cfc7cde4910d6c975d6b7b8dc8a73da4773702ebcfcd6e3518e73938bb1383badfe01c2
+  checksum: 900e4979f4dbc3313840078419245621259f349950411ca2fa445a2f9a1a6d98c3b5e7e0660c5ccd563aa61abe133a21765c6c0dec8e57da1ba71d8000b05ec1
   languageName: node
   linkType: hard
 
 "fast-json-stable-stringify@npm:^2.0.0":
   version: 2.1.0
   resolution: "fast-json-stable-stringify@npm:2.1.0"
   checksum: b191531e36c607977e5b1c47811158733c34ccb3bfde92c44798929e9b4154884378536d26ad90dfecd32e1ffc09c545d23535ad91b3161a27ddbb8ebe0cbecb
@@ -3253,19 +2974,19 @@
   version: 1.0.16
   resolution: "fastest-levenshtein@npm:1.0.16"
   checksum: a78d44285c9e2ae2c25f3ef0f8a73f332c1247b7ea7fb4a191e6bb51aa6ee1ef0dfb3ed113616dcdc7023e18e35a8db41f61c8d88988e877cf510df8edafbc71
   languageName: node
   linkType: hard
 
 "fastq@npm:^1.6.0":
-  version: 1.15.0
-  resolution: "fastq@npm:1.15.0"
+  version: 1.17.1
+  resolution: "fastq@npm:1.17.1"
   dependencies:
     reusify: ^1.0.4
-  checksum: 0170e6bfcd5d57a70412440b8ef600da6de3b2a6c5966aeaf0a852d542daff506a0ee92d6de7679d1de82e644bce69d7a574a6c93f0b03964b5337eed75ada1a
+  checksum: a8c5b26788d5a1763f88bae56a8ddeee579f935a831c5fe7a8268cea5b0a91fbfe705f612209e02d639b881d7b48e461a50da4a10cfaa40da5ca7cc9da098d88
   languageName: node
   linkType: hard
 
 "file-entry-cache@npm:^6.0.1":
   version: 6.0.1
   resolution: "file-entry-cache@npm:6.0.1"
   dependencies:
@@ -3307,27 +3028,37 @@
     locate-path: ^6.0.0
     path-exists: ^4.0.0
   checksum: 07955e357348f34660bde7920783204ff5a26ac2cafcaa28bace494027158a97b9f56faaf2d89a6106211a8174db650dd9f503f9c0d526b1202d5554a00b9095
   languageName: node
   linkType: hard
 
 "flat-cache@npm:^3.0.4":
-  version: 3.0.4
-  resolution: "flat-cache@npm:3.0.4"
+  version: 3.2.0
+  resolution: "flat-cache@npm:3.2.0"
   dependencies:
-    flatted: ^3.1.0
+    flatted: ^3.2.9
+    keyv: ^4.5.3
     rimraf: ^3.0.2
-  checksum: 4fdd10ecbcbf7d520f9040dd1340eb5dfe951e6f0ecf2252edeec03ee68d989ec8b9a20f4434270e71bcfd57800dc09b3344fca3966b2eb8f613072c7d9a2365
+  checksum: e7e0f59801e288b54bee5cb9681e9ee21ee28ef309f886b312c9d08415b79fc0f24ac842f84356ce80f47d6a53de62197ce0e6e148dc42d5db005992e2a756ec
+  languageName: node
+  linkType: hard
+
+"flat@npm:^5.0.2":
+  version: 5.0.2
+  resolution: "flat@npm:5.0.2"
+  bin:
+    flat: cli.js
+  checksum: 12a1536ac746db74881316a181499a78ef953632ddd28050b7a3a43c62ef5462e3357c8c29d76072bb635f147f7a9a1f0c02efef6b4be28f8db62ceb3d5c7f5d
   languageName: node
   linkType: hard
 
-"flatted@npm:^3.1.0":
-  version: 3.2.7
-  resolution: "flatted@npm:3.2.7"
-  checksum: 427633049d55bdb80201c68f7eb1cbd533e03eac541f97d3aecab8c5526f12a20ccecaeede08b57503e772c769e7f8680b37e8d482d1e5f8d7e2194687f9ea35
+"flatted@npm:^3.2.9":
+  version: 3.3.1
+  resolution: "flatted@npm:3.3.1"
+  checksum: 85ae7181650bb728c221e7644cbc9f4bf28bc556f2fc89bb21266962bdf0ce1029cc7acc44bb646cd469d9baac7c317f64e841c4c4c00516afa97320cdac7f94
   languageName: node
   linkType: hard
 
 "for-each@npm:^0.3.3":
   version: 0.3.3
   resolution: "for-each@npm:0.3.3"
   dependencies:
@@ -3357,58 +3088,61 @@
 "fs.realpath@npm:^1.0.0":
   version: 1.0.0
   resolution: "fs.realpath@npm:1.0.0"
   checksum: 99ddea01a7e75aa276c250a04eedeffe5662bce66c65c07164ad6264f9de18fb21be9433ead460e54cff20e31721c811f4fb5d70591799df5f85dce6d6746fd0
   languageName: node
   linkType: hard
 
-"function-bind@npm:^1.1.1":
-  version: 1.1.1
-  resolution: "function-bind@npm:1.1.1"
-  checksum: b32fbaebb3f8ec4969f033073b43f5c8befbb58f1a79e12f1d7490358150359ebd92f49e72ff0144f65f2c48ea2a605bff2d07965f548f6474fd8efd95bf361a
+"function-bind@npm:^1.1.2":
+  version: 1.1.2
+  resolution: "function-bind@npm:1.1.2"
+  checksum: 2b0ff4ce708d99715ad14a6d1f894e2a83242e4a52ccfcefaee5e40050562e5f6dafc1adbb4ce2d4ab47279a45dc736ab91ea5042d843c3c092820dfe032efb1
   languageName: node
   linkType: hard
 
-"function.prototype.name@npm:^1.1.5":
-  version: 1.1.5
-  resolution: "function.prototype.name@npm:1.1.5"
+"function.prototype.name@npm:^1.1.6":
+  version: 1.1.6
+  resolution: "function.prototype.name@npm:1.1.6"
   dependencies:
     call-bind: ^1.0.2
-    define-properties: ^1.1.3
-    es-abstract: ^1.19.0
-    functions-have-names: ^1.2.2
-  checksum: acd21d733a9b649c2c442f067567743214af5fa248dbeee69d8278ce7df3329ea5abac572be9f7470b4ec1cd4d8f1040e3c5caccf98ebf2bf861a0deab735c27
+    define-properties: ^1.2.0
+    es-abstract: ^1.22.1
+    functions-have-names: ^1.2.3
+  checksum: 7a3f9bd98adab09a07f6e1f03da03d3f7c26abbdeaeee15223f6c04a9fb5674792bdf5e689dac19b97ac71de6aad2027ba3048a9b883aa1b3173eed6ab07f479
   languageName: node
   linkType: hard
 
-"functions-have-names@npm:^1.2.2":
+"functions-have-names@npm:^1.2.3":
   version: 1.2.3
   resolution: "functions-have-names@npm:1.2.3"
   checksum: c3f1f5ba20f4e962efb71344ce0a40722163e85bee2101ce25f88214e78182d2d2476aa85ef37950c579eb6cf6ee811c17b3101bb84004bb75655f3e33f3fdb5
   languageName: node
   linkType: hard
 
-"get-intrinsic@npm:^1.0.2, get-intrinsic@npm:^1.1.1, get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.0":
-  version: 1.2.0
-  resolution: "get-intrinsic@npm:1.2.0"
+"get-intrinsic@npm:^1.1.3, get-intrinsic@npm:^1.2.1, get-intrinsic@npm:^1.2.2, get-intrinsic@npm:^1.2.3, get-intrinsic@npm:^1.2.4":
+  version: 1.2.4
+  resolution: "get-intrinsic@npm:1.2.4"
   dependencies:
-    function-bind: ^1.1.1
-    has: ^1.0.3
+    es-errors: ^1.3.0
+    function-bind: ^1.1.2
+    has-proto: ^1.0.1
     has-symbols: ^1.0.3
-  checksum: 78fc0487b783f5c58cf2dccafc3ae656ee8d2d8062a8831ce4a95e7057af4587a1d4882246c033aca0a7b4965276f4802b45cc300338d1b77a73d3e3e3f4877d
+    hasown: ^2.0.0
+  checksum: 414e3cdf2c203d1b9d7d33111df746a4512a1aa622770b361dadddf8ed0b5aeb26c560f49ca077e24bfafb0acb55ca908d1f709216ccba33ffc548ec8a79a951
   languageName: node
   linkType: hard
 
-"get-symbol-description@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "get-symbol-description@npm:1.0.0"
+"get-symbol-description@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "get-symbol-description@npm:1.0.2"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.1.1
-  checksum: 9ceff8fe968f9270a37a1f73bf3f1f7bda69ca80f4f80850670e0e7b9444ff99323f7ac52f96567f8b5f5fbe7ac717a0d81d3407c7313e82810c6199446a5247
+    call-bind: ^1.0.5
+    es-errors: ^1.3.0
+    get-intrinsic: ^1.2.4
+  checksum: e1cb53bc211f9dbe9691a4f97a46837a553c4e7caadd0488dc24ac694db8a390b93edd412b48dcdd0b4bbb4c595de1709effc75fc87c0839deedc6968f5bd973
   languageName: node
   linkType: hard
 
 "glob-parent@npm:^5.1.2":
   version: 5.1.2
   resolution: "glob-parent@npm:5.1.2"
   dependencies:
@@ -3429,25 +3163,25 @@
 "glob-to-regexp@npm:^0.4.1":
   version: 0.4.1
   resolution: "glob-to-regexp@npm:0.4.1"
   checksum: e795f4e8f06d2a15e86f76e4d92751cf8bbfcf0157cea5c2f0f35678a8195a750b34096b1256e436f0cebc1883b5ff0888c47348443e69546a5a87f9e1eb1167
   languageName: node
   linkType: hard
 
-"glob@npm:^7.1.3, glob@npm:~7.1.6":
-  version: 7.1.7
-  resolution: "glob@npm:7.1.7"
+"glob@npm:^7.1.3":
+  version: 7.2.3
+  resolution: "glob@npm:7.2.3"
   dependencies:
     fs.realpath: ^1.0.0
     inflight: ^1.0.4
     inherits: 2
-    minimatch: ^3.0.4
+    minimatch: ^3.1.1
     once: ^1.3.0
     path-is-absolute: ^1.0.0
-  checksum: b61f48973bbdcf5159997b0874a2165db572b368b931135832599875919c237fc05c12984e38fe828e69aa8a921eb0e8a4997266211c517c9cfaae8a93988bb8
+  checksum: 29452e97b38fa704dabb1d1045350fb2467cf0277e155aa9ff7077e90ad81d1ea9d53d3ee63bd37c05b09a065e90f16aec4a65f5b8de401d1dac40bc5605d133
   languageName: node
   linkType: hard
 
 "glob@npm:^9.2.0":
   version: 9.3.5
   resolution: "glob@npm:9.3.5"
   dependencies:
@@ -3455,14 +3189,28 @@
     minimatch: ^8.0.2
     minipass: ^4.2.4
     path-scurry: ^1.6.1
   checksum: 94b093adbc591bc36b582f77927d1fb0dbf3ccc231828512b017601408be98d1fe798fc8c0b19c6f2d1a7660339c3502ce698de475e9d938ccbb69b47b647c84
   languageName: node
   linkType: hard
 
+"glob@npm:~7.1.6":
+  version: 7.1.7
+  resolution: "glob@npm:7.1.7"
+  dependencies:
+    fs.realpath: ^1.0.0
+    inflight: ^1.0.4
+    inherits: 2
+    minimatch: ^3.0.4
+    once: ^1.3.0
+    path-is-absolute: ^1.0.0
+  checksum: b61f48973bbdcf5159997b0874a2165db572b368b931135832599875919c237fc05c12984e38fe828e69aa8a921eb0e8a4997266211c517c9cfaae8a93988bb8
+  languageName: node
+  linkType: hard
+
 "globals@npm:^13.19.0":
   version: 13.24.0
   resolution: "globals@npm:13.24.0"
   dependencies:
     type-fest: ^0.20.2
   checksum: 56066ef058f6867c04ff203b8a44c15b038346a62efbc3060052a1016be9f56f4cf0b2cd45b74b22b81e521a889fc7786c73691b0549c2f3a6e825b3d394f43c
   languageName: node
@@ -3497,17 +3245,17 @@
   dependencies:
     get-intrinsic: ^1.1.3
   checksum: a5ccfb8806e0917a94e0b3de2af2ea4979c1da920bc381667c260e00e7cafdbe844e2cb9c5bcfef4e5412e8bf73bab837285bc35c7ba73aaaf0134d4583393a6
   languageName: node
   linkType: hard
 
 "graceful-fs@npm:^4.1.2, graceful-fs@npm:^4.1.6, graceful-fs@npm:^4.2.0, graceful-fs@npm:^4.2.4, graceful-fs@npm:^4.2.9":
-  version: 4.2.10
-  resolution: "graceful-fs@npm:4.2.10"
-  checksum: 3f109d70ae123951905d85032ebeae3c2a5a7a997430df00ea30df0e3a6c60cf6689b109654d6fdacd28810a053348c4d14642da1d075049e6be1ba5216218da
+  version: 4.2.11
+  resolution: "graceful-fs@npm:4.2.11"
+  checksum: ac85f94da92d8eb6b7f5a8b20ce65e43d66761c55ce85ac96df6865308390da45a8d3f0296dd3a663de65d30ba497bd46c696cc1e248c72b13d6d567138a4fc7
   languageName: node
   linkType: hard
 
 "graphemer@npm:^1.4.0":
   version: 1.4.0
   resolution: "graphemer@npm:1.4.0"
   checksum: bab8f0be9b568857c7bec9fda95a89f87b783546d02951c40c33f84d05bb7da3fd10f863a9beb901463669b6583173a8c8cc6d6b306ea2b9b9d5d3d943c3a673
@@ -3531,52 +3279,52 @@
 "has-flag@npm:^4.0.0":
   version: 4.0.0
   resolution: "has-flag@npm:4.0.0"
   checksum: 261a1357037ead75e338156b1f9452c016a37dcd3283a972a30d9e4a87441ba372c8b81f818cd0fbcd9c0354b4ae7e18b9e1afa1971164aef6d18c2b6095a8ad
   languageName: node
   linkType: hard
 
-"has-property-descriptors@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "has-property-descriptors@npm:1.0.0"
+"has-property-descriptors@npm:^1.0.0, has-property-descriptors@npm:^1.0.1, has-property-descriptors@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "has-property-descriptors@npm:1.0.2"
   dependencies:
-    get-intrinsic: ^1.1.1
-  checksum: a6d3f0a266d0294d972e354782e872e2fe1b6495b321e6ef678c9b7a06a40408a6891817350c62e752adced73a94ac903c54734fee05bf65b1905ee1368194bb
+    es-define-property: ^1.0.0
+  checksum: fcbb246ea2838058be39887935231c6d5788babed499d0e9d0cc5737494c48aba4fe17ba1449e0d0fbbb1e36175442faa37f9c427ae357d6ccb1d895fbcd3de3
   languageName: node
   linkType: hard
 
-"has-proto@npm:^1.0.1":
-  version: 1.0.1
-  resolution: "has-proto@npm:1.0.1"
-  checksum: febc5b5b531de8022806ad7407935e2135f1cc9e64636c3916c6842bd7995994ca3b29871ecd7954bd35f9e2986c17b3b227880484d22259e2f8e6ce63fd383e
+"has-proto@npm:^1.0.1, has-proto@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "has-proto@npm:1.0.3"
+  checksum: fe7c3d50b33f50f3933a04413ed1f69441d21d2d2944f81036276d30635cad9279f6b43bc8f32036c31ebdfcf6e731150f46c1907ad90c669ffe9b066c3ba5c4
   languageName: node
   linkType: hard
 
 "has-symbols@npm:^1.0.2, has-symbols@npm:^1.0.3":
   version: 1.0.3
   resolution: "has-symbols@npm:1.0.3"
   checksum: a054c40c631c0d5741a8285010a0777ea0c068f99ed43e5d6eb12972da223f8af553a455132fdb0801bdcfa0e0f443c0c03a68d8555aa529b3144b446c3f2410
   languageName: node
   linkType: hard
 
-"has-tostringtag@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "has-tostringtag@npm:1.0.0"
+"has-tostringtag@npm:^1.0.0, has-tostringtag@npm:^1.0.1, has-tostringtag@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "has-tostringtag@npm:1.0.2"
   dependencies:
-    has-symbols: ^1.0.2
-  checksum: cc12eb28cb6ae22369ebaad3a8ab0799ed61270991be88f208d508076a1e99abe4198c965935ce85ea90b60c94ddda73693b0920b58e7ead048b4a391b502c1c
+    has-symbols: ^1.0.3
+  checksum: 999d60bb753ad714356b2c6c87b7fb74f32463b8426e159397da4bde5bca7e598ab1073f4d8d4deafac297f2eb311484cd177af242776bf05f0d11565680468d
   languageName: node
   linkType: hard
 
-"has@npm:^1.0.3":
-  version: 1.0.3
-  resolution: "has@npm:1.0.3"
+"hasown@npm:^2.0.0, hasown@npm:^2.0.1":
+  version: 2.0.1
+  resolution: "hasown@npm:2.0.1"
   dependencies:
-    function-bind: ^1.1.1
-  checksum: b9ad53d53be4af90ce5d1c38331e712522417d017d5ef1ebd0507e07c2fbad8686fffb8e12ddecd4c39ca9b9b47431afbb975b8abf7f3c3b82c98e9aad052792
+    function-bind: ^1.1.2
+  checksum: 9081c382a4fe8a62639a8da5c7d3322b203c319147e48783763dd741863d9f2dcaa743574fe2a1283871c445d8ba99ea45d5fff384e5ad27ca9dd7a367d79de0
   languageName: node
   linkType: hard
 
 "hosted-git-info@npm:^2.1.4":
   version: 2.8.9
   resolution: "hosted-git-info@npm:2.8.9"
   checksum: c955394bdab888a1e9bb10eb33029e0f7ce5a2ac7b3f158099dc8c486c99e73809dca609f5694b223920ca2174db33d32b12f9a2a47141dc59607c29da5a62dd
@@ -3609,22 +3357,15 @@
   resolution: "icss-utils@npm:5.1.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 5c324d283552b1269cfc13a503aaaa172a280f914e5b81544f3803bc6f06a3b585fb79f66f7c771a2c052db7982c18bf92d001e3b47282e3abbbb4c4cc488d68
   languageName: node
   linkType: hard
 
-"ignore@npm:^5.2.0":
-  version: 5.2.4
-  resolution: "ignore@npm:5.2.4"
-  checksum: 3d4c309c6006e2621659311783eaea7ebcd41fe4ca1d78c91c473157ad6666a57a2df790fe0d07a12300d9aac2888204d7be8d59f9aaf665b1c7fcdb432517ef
-  languageName: node
-  linkType: hard
-
-"ignore@npm:^5.2.4":
+"ignore@npm:^5.2.0, ignore@npm:^5.2.4":
   version: 5.3.1
   resolution: "ignore@npm:5.3.1"
   checksum: 71d7bb4c1dbe020f915fd881108cbe85a0db3d636a0ea3ba911393c53946711d13a9b1143c7e70db06d571a5822c0a324a6bcde5c9904e7ca5047f01f1bf8cd3
   languageName: node
   linkType: hard
 
 "import-fresh@npm:^3.2.1":
@@ -3669,22 +3410,22 @@
 "inherits@npm:2":
   version: 2.0.4
   resolution: "inherits@npm:2.0.4"
   checksum: 4a48a733847879d6cf6691860a6b1e3f0f4754176e4d71494c41f3475553768b10f84b5ce1d40fbd0e34e6bfbb864ee35858ad4dd2cf31e02fc4a154b724d7f1
   languageName: node
   linkType: hard
 
-"internal-slot@npm:^1.0.4":
-  version: 1.0.5
-  resolution: "internal-slot@npm:1.0.5"
+"internal-slot@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "internal-slot@npm:1.0.7"
   dependencies:
-    get-intrinsic: ^1.2.0
-    has: ^1.0.3
+    es-errors: ^1.3.0
+    hasown: ^2.0.0
     side-channel: ^1.0.4
-  checksum: 97e84046bf9e7574d0956bd98d7162313ce7057883b6db6c5c7b5e5f05688864b0978ba07610c726d15d66544ffe4b1050107d93f8a39ebc59b15d8b429b497a
+  checksum: cadc5eea5d7d9bc2342e93aae9f31f04c196afebb11bde97448327049f492cd7081e18623ae71388aac9cd237b692ca3a105be9c68ac39c1dec679d7409e33eb
   languageName: node
   linkType: hard
 
 "interpret@npm:^2.2.0":
   version: 2.2.0
   resolution: "interpret@npm:2.2.0"
   checksum: f51efef7cb8d02da16408ffa3504cd6053014c5aeb7bb8c223727e053e4235bf565e45d67028b0c8740d917c603807aa3c27d7bd2f21bf20b6417e2bb3e5fd6e
@@ -3694,22 +3435,21 @@
 "interpret@npm:^3.1.1":
   version: 3.1.1
   resolution: "interpret@npm:3.1.1"
   checksum: 35cebcf48c7351130437596d9ab8c8fe131ce4038da4561e6d665f25640e0034702a031cf7e3a5cea60ac7ac548bf17465e0571ede126f3d3a6933152171ac82
   languageName: node
   linkType: hard
 
-"is-array-buffer@npm:^3.0.1":
-  version: 3.0.2
-  resolution: "is-array-buffer@npm:3.0.2"
+"is-array-buffer@npm:^3.0.4":
+  version: 3.0.4
+  resolution: "is-array-buffer@npm:3.0.4"
   dependencies:
     call-bind: ^1.0.2
-    get-intrinsic: ^1.2.0
-    is-typed-array: ^1.1.10
-  checksum: dcac9dda66ff17df9cabdc58214172bf41082f956eab30bb0d86bc0fab1e44b690fc8e1f855cf2481245caf4e8a5a006a982a71ddccec84032ed41f9d8da8c14
+    get-intrinsic: ^1.2.1
+  checksum: e4e3e6ef0ff2239e75371d221f74bc3c26a03564a22efb39f6bb02609b598917ddeecef4e8c877df2a25888f247a98198959842a5e73236bc7f22cabdf6351a7
   languageName: node
   linkType: hard
 
 "is-arrayish@npm:^0.2.1":
   version: 0.2.1
   resolution: "is-arrayish@npm:0.2.1"
   checksum: eef4417e3c10e60e2c810b6084942b3ead455af16c4509959a27e490e7aee87cfb3f38e01bbde92220b528a0ee1a18d52b787e1458ee86174d8c7f0e58cd488f
@@ -3738,29 +3478,20 @@
 "is-callable@npm:^1.1.3, is-callable@npm:^1.1.4, is-callable@npm:^1.2.7":
   version: 1.2.7
   resolution: "is-callable@npm:1.2.7"
   checksum: 61fd57d03b0d984e2ed3720fb1c7a897827ea174bd44402878e059542ea8c4aeedee0ea0985998aa5cc2736b2fa6e271c08587addb5b3959ac52cf665173d1ac
   languageName: node
   linkType: hard
 
-"is-core-module@npm:^2.12.0":
-  version: 2.12.1
-  resolution: "is-core-module@npm:2.12.1"
+"is-core-module@npm:^2.13.0":
+  version: 2.13.1
+  resolution: "is-core-module@npm:2.13.1"
   dependencies:
-    has: ^1.0.3
-  checksum: f04ea30533b5e62764e7b2e049d3157dc0abd95ef44275b32489ea2081176ac9746ffb1cdb107445cf1ff0e0dfcad522726ca27c27ece64dadf3795428b8e468
-  languageName: node
-  linkType: hard
-
-"is-core-module@npm:^2.9.0":
-  version: 2.11.0
-  resolution: "is-core-module@npm:2.11.0"
-  dependencies:
-    has: ^1.0.3
-  checksum: f96fd490c6b48eb4f6d10ba815c6ef13f410b0ba6f7eb8577af51697de523e5f2cd9de1c441b51d27251bf0e4aebc936545e33a5d26d5d51f28d25698d4a8bab
+    hasown: ^2.0.0
+  checksum: 256559ee8a9488af90e4bad16f5583c6d59e92f0742e9e8bb4331e758521ee86b810b93bae44f390766ffbc518a0488b18d9dab7da9a5ff997d499efc9403f7c
   languageName: node
   linkType: hard
 
 "is-date-object@npm:^1.0.1":
   version: 1.0.5
   resolution: "is-date-object@npm:1.0.5"
   dependencies:
@@ -3781,18 +3512,18 @@
   resolution: "is-glob@npm:4.0.3"
   dependencies:
     is-extglob: ^2.1.1
   checksum: d381c1319fcb69d341cc6e6c7cd588e17cd94722d9a32dbd60660b993c4fb7d0f19438674e68dfec686d09b7c73139c9166b47597f846af387450224a8101ab4
   languageName: node
   linkType: hard
 
-"is-negative-zero@npm:^2.0.2":
-  version: 2.0.2
-  resolution: "is-negative-zero@npm:2.0.2"
-  checksum: f3232194c47a549da60c3d509c9a09be442507616b69454716692e37ae9f37c4dea264fb208ad0c9f3efd15a796a46b79df07c7e53c6227c32170608b809149a
+"is-negative-zero@npm:^2.0.3":
+  version: 2.0.3
+  resolution: "is-negative-zero@npm:2.0.3"
+  checksum: c1e6b23d2070c0539d7b36022d5a94407132411d01aba39ec549af824231f3804b1aea90b5e4e58e807a65d23ceb538ed6e355ce76b267bdd86edb757ffcbdcd
   languageName: node
   linkType: hard
 
 "is-number-object@npm:^1.0.4":
   version: 1.0.7
   resolution: "is-number-object@npm:1.0.7"
   dependencies:
@@ -3837,20 +3568,20 @@
   dependencies:
     call-bind: ^1.0.2
     has-tostringtag: ^1.0.0
   checksum: 362399b33535bc8f386d96c45c9feb04cf7f8b41c182f54174c1a45c9abbbe5e31290bbad09a458583ff6bf3b2048672cdb1881b13289569a7c548370856a652
   languageName: node
   linkType: hard
 
-"is-shared-array-buffer@npm:^1.0.2":
-  version: 1.0.2
-  resolution: "is-shared-array-buffer@npm:1.0.2"
+"is-shared-array-buffer@npm:^1.0.2, is-shared-array-buffer@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "is-shared-array-buffer@npm:1.0.3"
   dependencies:
-    call-bind: ^1.0.2
-  checksum: 9508929cf14fdc1afc9d61d723c6e8d34f5e117f0bffda4d97e7a5d88c3a8681f633a74f8e3ad1fe92d5113f9b921dc5ca44356492079612f9a247efbce7032a
+    call-bind: ^1.0.7
+  checksum: a4fff602c309e64ccaa83b859255a43bb011145a42d3f56f67d9268b55bc7e6d98a5981a1d834186ad3105d6739d21547083fe7259c76c0468483fc538e716d8
   languageName: node
   linkType: hard
 
 "is-string@npm:^1.0.5, is-string@npm:^1.0.7":
   version: 1.0.7
   resolution: "is-string@npm:1.0.7"
   dependencies:
@@ -3864,36 +3595,39 @@
   resolution: "is-symbol@npm:1.0.4"
   dependencies:
     has-symbols: ^1.0.2
   checksum: 92805812ef590738d9de49d677cd17dfd486794773fb6fa0032d16452af46e9b91bb43ffe82c983570f015b37136f4b53b28b8523bfb10b0ece7a66c31a54510
   languageName: node
   linkType: hard
 
-"is-typed-array@npm:^1.1.10, is-typed-array@npm:^1.1.9":
-  version: 1.1.10
-  resolution: "is-typed-array@npm:1.1.10"
+"is-typed-array@npm:^1.1.13":
+  version: 1.1.13
+  resolution: "is-typed-array@npm:1.1.13"
   dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
-    for-each: ^0.3.3
-    gopd: ^1.0.1
-    has-tostringtag: ^1.0.0
-  checksum: aac6ecb59d4c56a1cdeb69b1f129154ef462bbffe434cb8a8235ca89b42f258b7ae94073c41b3cb7bce37f6a1733ad4499f07882d5d5093a7ba84dfc4ebb8017
+    which-typed-array: ^1.1.14
+  checksum: 150f9ada183a61554c91e1c4290086d2c100b0dff45f60b028519be72a8db964da403c48760723bf5253979b8dffe7b544246e0e5351dcd05c5fdb1dcc1dc0f0
   languageName: node
   linkType: hard
 
 "is-weakref@npm:^1.0.2":
   version: 1.0.2
   resolution: "is-weakref@npm:1.0.2"
   dependencies:
     call-bind: ^1.0.2
   checksum: 95bd9a57cdcb58c63b1c401c60a474b0f45b94719c30f548c891860f051bc2231575c290a6b420c6bc6e7ed99459d424c652bd5bf9a1d5259505dc35b4bf83de
   languageName: node
   linkType: hard
 
+"isarray@npm:^2.0.5":
+  version: 2.0.5
+  resolution: "isarray@npm:2.0.5"
+  checksum: bd5bbe4104438c4196ba58a54650116007fa0262eccef13a4c55b2e09a5b36b59f1e75b9fcc49883dd9d4953892e6fc007eef9e9155648ceea036e184b0f930a
+  languageName: node
+  linkType: hard
+
 "isexe@npm:^2.0.0":
   version: 2.0.0
   resolution: "isexe@npm:2.0.0"
   checksum: 26bf6c5480dda5161c820c5b5c751ae1e766c587b1f951ea3fcfc973bafb7831ae5b54a31a69bd670220e42e99ec154475025a468eae58ea262f813fdc8d1c62
   languageName: node
   linkType: hard
 
@@ -3943,14 +3677,21 @@
     argparse: ^2.0.1
   bin:
     js-yaml: bin/js-yaml.js
   checksum: c7830dfd456c3ef2c6e355cc5a92e6700ceafa1d14bba54497b34a99f0376cecbb3e9ac14d3e5849b426d5a5140709a66237a8c991c675431271c4ce5504151a
   languageName: node
   linkType: hard
 
+"json-buffer@npm:3.0.1":
+  version: 3.0.1
+  resolution: "json-buffer@npm:3.0.1"
+  checksum: 9026b03edc2847eefa2e37646c579300a1f3a4586cfb62bf857832b60c852042d0d6ae55d1afb8926163fa54c2b01d83ae24705f34990348bdac6273a29d4581
+  languageName: node
+  linkType: hard
+
 "json-parse-better-errors@npm:^1.0.1":
   version: 1.0.2
   resolution: "json-parse-better-errors@npm:1.0.2"
   checksum: ff2b5ba2a70e88fd97a3cb28c1840144c5ce8fae9cbeeddba15afa333a5c407cf0e42300cd0a2885dbb055227fe68d405070faad941beeffbfde9cf3b2c78c5d
   languageName: node
   linkType: hard
 
@@ -4027,14 +3768,23 @@
 "jsonpointer@npm:^5.0.1":
   version: 5.0.1
   resolution: "jsonpointer@npm:5.0.1"
   checksum: 0b40f712900ad0c846681ea2db23b6684b9d5eedf55807b4708c656f5894b63507d0e28ae10aa1bddbea551241035afe62b6df0800fc94c2e2806a7f3adecd7c
   languageName: node
   linkType: hard
 
+"keyv@npm:^4.5.3":
+  version: 4.5.4
+  resolution: "keyv@npm:4.5.4"
+  dependencies:
+    json-buffer: 3.0.1
+  checksum: 74a24395b1c34bd44ad5cb2b49140d087553e170625240b86755a6604cd65aa16efdbdeae5cdb17ba1284a0fbb25ad06263755dbc71b8d8b06f74232ce3cdd72
+  languageName: node
+  linkType: hard
+
 "kind-of@npm:^6.0.2":
   version: 6.0.3
   resolution: "kind-of@npm:6.0.3"
   checksum: 3ab01e7b1d440b22fe4c31f23d8d38b4d9b91d9f291df683476576493d5dfd2e03848a8b05813dd0c3f0e835bc63f433007ddeceb71f05cb25c45ae1b19c6d3b
   languageName: node
   linkType: hard
 
@@ -4044,20 +3794,24 @@
   dependencies:
     prelude-ls: ^1.2.1
     type-check: ~0.4.0
   checksum: 12c5021c859bd0f5248561bf139121f0358285ec545ebf48bb3d346820d5c61a4309535c7f387ed7d84361cf821e124ce346c6b7cef8ee09a67c1473b46d0fc4
   languageName: node
   linkType: hard
 
-"lib0@npm:^0.2.42, lib0@npm:^0.2.49":
-  version: 0.2.63
-  resolution: "lib0@npm:0.2.63"
+"lib0@npm:^0.2.85, lib0@npm:^0.2.86":
+  version: 0.2.91
+  resolution: "lib0@npm:0.2.91"
   dependencies:
     isomorphic.js: ^0.2.4
-  checksum: 5f39ec7f3988e72e4ba11c021ca1ee57dfbb2ef1564a353c5377491105ea8f76791cd5f270876b8f36ba5142f1ac2666ecabbddadd35db0f925e9c33bb8fab9f
+  bin:
+    0ecdsa-generate-keypair: bin/0ecdsa-generate-keypair.js
+    0gentesthtml: bin/gentesthtml.js
+    0serve: bin/0serve.js
+  checksum: 92e7893e78e732cc1acd18cb892d6123a6f4480f7d5cbd394845a397298fa28971b5436bc26c3ab0c43cb0f6c667f42a50c9ed757ef848730bbdd78c37cec0ac
   languageName: node
   linkType: hard
 
 "license-webpack-plugin@npm:^2.3.14":
   version: 2.3.21
   resolution: "license-webpack-plugin@npm:2.3.21"
   dependencies:
@@ -4233,21 +3987,22 @@
   dependencies:
     mime-db: 1.52.0
   checksum: 89a5b7f1def9f3af5dad6496c5ed50191ae4331cc5389d7c521c8ad28d5fdad2d06fd81baf38fed813dc4e46bb55c8145bb0ff406330818c9cf712fb2e9b3836
   languageName: node
   linkType: hard
 
 "mini-css-extract-plugin@npm:^2.7.0":
-  version: 2.7.6
-  resolution: "mini-css-extract-plugin@npm:2.7.6"
+  version: 2.8.1
+  resolution: "mini-css-extract-plugin@npm:2.8.1"
   dependencies:
     schema-utils: ^4.0.0
+    tapable: ^2.2.1
   peerDependencies:
     webpack: ^5.0.0
-  checksum: be6f7cefc6275168eb0a6b8fe977083a18c743c9612c9f00e6c1a62c3393ca7960e93fba1a7ebb09b75f36a0204ad087d772c1ef574bc29c90c0e8175a3c0b83
+  checksum: 209f15a18cc304b0f12911927ea7e6ca4f0c3168dcc95d741811c933c4610fdb02a8486fc1a7782a6cde75c8e1880e175b7acf04e5ddfba2b8ed045d306ef04f
   languageName: node
   linkType: hard
 
 "mini-svg-data-uri@npm:^1.4.4":
   version: 1.4.4
   resolution: "mini-svg-data-uri@npm:1.4.4"
   bin:
@@ -4261,15 +4016,15 @@
   resolution: "minimatch@npm:9.0.3"
   dependencies:
     brace-expansion: ^2.0.1
   checksum: 253487976bf485b612f16bf57463520a14f512662e592e95c571afdab1442a6a6864b6c88f248ce6fc4ff0b6de04ac7aa6c8bb51e868e99d1d65eb0658a708b5
   languageName: node
   linkType: hard
 
-"minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.2":
+"minimatch@npm:^3.0.4, minimatch@npm:^3.0.5, minimatch@npm:^3.1.1, minimatch@npm:^3.1.2":
   version: 3.1.2
   resolution: "minimatch@npm:3.1.2"
   dependencies:
     brace-expansion: ^1.1.7
   checksum: c154e566406683e7bcb746e000b84d74465b3a832c45d59912b9b55cd50dee66e5c4b1e5566dba26154040e51672f9aa450a9aef0c97cfc7336b78b7afb9540a
   languageName: node
   linkType: hard
@@ -4307,32 +4062,14 @@
 "ms@npm:2.1.2":
   version: 2.1.2
   resolution: "ms@npm:2.1.2"
   checksum: 673cdb2c3133eb050c745908d8ce632ed2c02d85640e2edb3ace856a2266a813b30c613569bf3354fdf4ea7d1a1494add3bfa95e2713baa27d0c2c71fc44f58f
   languageName: node
   linkType: hard
 
-"nanoid@npm:^3.3.4":
-  version: 3.3.4
-  resolution: "nanoid@npm:3.3.4"
-  bin:
-    nanoid: bin/nanoid.cjs
-  checksum: 2fddd6dee994b7676f008d3ffa4ab16035a754f4bb586c61df5a22cf8c8c94017aadd360368f47d653829e0569a92b129979152ff97af23a558331e47e37cd9c
-  languageName: node
-  linkType: hard
-
-"nanoid@npm:^3.3.6":
-  version: 3.3.6
-  resolution: "nanoid@npm:3.3.6"
-  bin:
-    nanoid: bin/nanoid.cjs
-  checksum: 7d0eda657002738aa5206107bd0580aead6c95c460ef1bdd0b1a87a9c7ae6277ac2e9b945306aaa5b32c6dcb7feaf462d0f552e7f8b5718abfc6ead5c94a71b3
-  languageName: node
-  linkType: hard
-
 "nanoid@npm:^3.3.7":
   version: 3.3.7
   resolution: "nanoid@npm:3.3.7"
   bin:
     nanoid: bin/nanoid.cjs
   checksum: d36c427e530713e4ac6567d488b489a36582ef89da1d6d4e3b87eded11eb10d7042a877958c6f104929809b2ab0bafa17652b076cdf84324aa75b30b722204f2
   languageName: node
@@ -4355,18 +4092,18 @@
 "nice-try@npm:^1.0.4":
   version: 1.0.5
   resolution: "nice-try@npm:1.0.5"
   checksum: 0b4af3b5bb5d86c289f7a026303d192a7eb4417231fe47245c460baeabae7277bcd8fd9c728fb6bd62c30b3e15cd6620373e2cf33353b095d8b403d3e8a15aff
   languageName: node
   linkType: hard
 
-"node-releases@npm:^2.0.8":
-  version: 2.0.10
-  resolution: "node-releases@npm:2.0.10"
-  checksum: d784ecde25696a15d449c4433077f5cce620ed30a1656c4abf31282bfc691a70d9618bae6868d247a67914d1be5cc4fde22f65a05f4398cdfb92e0fc83cadfbc
+"node-releases@npm:^2.0.14":
+  version: 2.0.14
+  resolution: "node-releases@npm:2.0.14"
+  checksum: 59443a2f77acac854c42d321bf1b43dea0aef55cd544c6a686e9816a697300458d4e82239e2d794ea05f7bbbc8a94500332e2d3ac3f11f52e4b16cbe638b3c41
   languageName: node
   linkType: hard
 
 "normalize-package-data@npm:^2.3.2":
   version: 2.5.0
   resolution: "normalize-package-data@npm:2.5.0"
   dependencies:
@@ -4402,37 +4139,37 @@
 "object-assign@npm:^4.1.1":
   version: 4.1.1
   resolution: "object-assign@npm:4.1.1"
   checksum: fcc6e4ea8c7fe48abfbb552578b1c53e0d194086e2e6bbbf59e0a536381a292f39943c6e9628af05b5528aa5e3318bb30d6b2e53cadaf5b8fe9e12c4b69af23f
   languageName: node
   linkType: hard
 
-"object-inspect@npm:^1.12.2, object-inspect@npm:^1.9.0":
-  version: 1.12.3
-  resolution: "object-inspect@npm:1.12.3"
-  checksum: dabfd824d97a5f407e6d5d24810d888859f6be394d8b733a77442b277e0808860555176719c5905e765e3743a7cada6b8b0a3b85e5331c530fd418cc8ae991db
+"object-inspect@npm:^1.13.1":
+  version: 1.13.1
+  resolution: "object-inspect@npm:1.13.1"
+  checksum: 7d9fa9221de3311dcb5c7c307ee5dc011cdd31dc43624b7c184b3840514e118e05ef0002be5388304c416c0eb592feb46e983db12577fc47e47d5752fbbfb61f
   languageName: node
   linkType: hard
 
 "object-keys@npm:^1.1.1":
   version: 1.1.1
   resolution: "object-keys@npm:1.1.1"
   checksum: b363c5e7644b1e1b04aa507e88dcb8e3a2f52b6ffd0ea801e4c7a62d5aa559affe21c55a07fd4b1fd55fc03a33c610d73426664b20032405d7b92a1414c34d6a
   languageName: node
   linkType: hard
 
-"object.assign@npm:^4.1.4":
-  version: 4.1.4
-  resolution: "object.assign@npm:4.1.4"
+"object.assign@npm:^4.1.5":
+  version: 4.1.5
+  resolution: "object.assign@npm:4.1.5"
   dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.1.4
+    call-bind: ^1.0.5
+    define-properties: ^1.2.1
     has-symbols: ^1.0.3
     object-keys: ^1.1.1
-  checksum: 76cab513a5999acbfe0ff355f15a6a125e71805fcf53de4e9d4e082e1989bdb81d1e329291e1e4e0ae7719f0e4ef80e88fb2d367ae60500d79d25a6224ac8864
+  checksum: f9aeac0541661370a1fc86e6a8065eb1668d3e771f7dbb33ee54578201336c057b21ee61207a186dd42db0c62201d91aac703d20d12a79fc79c353eed44d4e25
   languageName: node
   linkType: hard
 
 "once@npm:^1.3.0":
   version: 1.4.0
   resolution: "once@npm:1.4.0"
   dependencies:
@@ -4627,57 +4364,51 @@
   resolution: "pkg-dir@npm:4.2.0"
   dependencies:
     find-up: ^4.0.0
   checksum: 9863e3f35132bf99ae1636d31ff1e1e3501251d480336edb1c211133c8d58906bed80f154a1d723652df1fda91e01c7442c2eeaf9dc83157c7ae89087e43c8d6
   languageName: node
   linkType: hard
 
+"possible-typed-array-names@npm:^1.0.0":
+  version: 1.0.0
+  resolution: "possible-typed-array-names@npm:1.0.0"
+  checksum: b32d403ece71e042385cc7856385cecf1cd8e144fa74d2f1de40d1e16035dba097bc189715925e79b67bdd1472796ff168d3a90d296356c9c94d272d5b95f3ae
+  languageName: node
+  linkType: hard
+
 "postcss-modules-extract-imports@npm:^3.0.0":
   version: 3.0.0
   resolution: "postcss-modules-extract-imports@npm:3.0.0"
   peerDependencies:
     postcss: ^8.1.0
   checksum: 4b65f2f1382d89c4bc3c0a1bdc5942f52f3cb19c110c57bd591ffab3a5fee03fcf831604168205b0c1b631a3dce2255c70b61aaae3ef39d69cd7eb450c2552d2
   languageName: node
   linkType: hard
 
-"postcss-modules-local-by-default@npm:^4.0.0":
-  version: 4.0.0
-  resolution: "postcss-modules-local-by-default@npm:4.0.0"
-  dependencies:
-    icss-utils: ^5.0.0
-    postcss-selector-parser: ^6.0.2
-    postcss-value-parser: ^4.1.0
-  peerDependencies:
-    postcss: ^8.1.0
-  checksum: 6cf570badc7bc26c265e073f3ff9596b69bb954bc6ac9c5c1b8cba2995b80834226b60e0a3cbb87d5f399dbb52e6466bba8aa1d244f6218f99d834aec431a69d
-  languageName: node
-  linkType: hard
-
-"postcss-modules-local-by-default@npm:^4.0.3":
-  version: 4.0.3
-  resolution: "postcss-modules-local-by-default@npm:4.0.3"
+"postcss-modules-local-by-default@npm:^4.0.0, postcss-modules-local-by-default@npm:^4.0.4":
+  version: 4.0.4
+  resolution: "postcss-modules-local-by-default@npm:4.0.4"
   dependencies:
     icss-utils: ^5.0.0
     postcss-selector-parser: ^6.0.2
     postcss-value-parser: ^4.1.0
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 2f8083687f3d6067885f8863dd32dbbb4f779cfcc7e52c17abede9311d84faf6d3ed8760e7c54c6380281732ae1f78e5e56a28baf3c271b33f450a11c9e30485
+  checksum: 578b955b0773147890caa88c30b10dfc849c5b1412a47ad51751890dba16fca9528c3ab00a19b186a8c2c150c2d08e2ce64d3d907800afee1f37c6d38252e365
   languageName: node
   linkType: hard
 
-"postcss-modules-scope@npm:^3.0.0":
-  version: 3.0.0
-  resolution: "postcss-modules-scope@npm:3.0.0"
+"postcss-modules-scope@npm:^3.0.0, postcss-modules-scope@npm:^3.1.1":
+  version: 3.1.1
+  resolution: "postcss-modules-scope@npm:3.1.1"
   dependencies:
     postcss-selector-parser: ^6.0.4
   peerDependencies:
     postcss: ^8.1.0
-  checksum: 330b9398dbd44c992c92b0dc612c0626135e2cc840fee41841eb61247a6cfed95af2bd6f67ead9dd9d0bb41f5b0367129d93c6e434fa3e9c58ade391d9a5a138
+  checksum: 9e9d23abb0babc7fa243be65704d72a5a9ceb2bded4dbaef96a88210d468b03c8c3158c197f4e22300c851f08c6fdddd6ebe65f44e4c34448b45b8a2e063a16d
   languageName: node
   linkType: hard
 
 "postcss-modules-values@npm:^4.0.0":
   version: 4.0.0
   resolution: "postcss-modules-values@npm:4.0.0"
   dependencies:
@@ -4685,49 +4416,38 @@
   peerDependencies:
     postcss: ^8.1.0
   checksum: f7f2cdf14a575b60e919ad5ea52fed48da46fe80db2733318d71d523fc87db66c835814940d7d05b5746b0426e44661c707f09bdb83592c16aea06e859409db6
   languageName: node
   linkType: hard
 
 "postcss-selector-parser@npm:^6.0.2, postcss-selector-parser@npm:^6.0.4":
-  version: 6.0.11
-  resolution: "postcss-selector-parser@npm:6.0.11"
+  version: 6.0.15
+  resolution: "postcss-selector-parser@npm:6.0.15"
   dependencies:
     cssesc: ^3.0.0
     util-deprecate: ^1.0.2
-  checksum: 0b01aa9c2d2c8dbeb51e9b204796b678284be9823abc8d6d40a8b16d4149514e922c264a8ed4deb4d6dbced564b9be390f5942c058582d8656351516d6c49cde
+  checksum: 57decb94152111004f15e27b9c61131eb50ee10a3288e7fcf424cebbb4aba82c2817517ae718f8b5d704ee9e02a638d4a2acff8f47685c295a33ecee4fd31055
   languageName: node
   linkType: hard
 
 "postcss-value-parser@npm:^4.1.0, postcss-value-parser@npm:^4.2.0":
   version: 4.2.0
   resolution: "postcss-value-parser@npm:4.2.0"
   checksum: 819ffab0c9d51cf0acbabf8996dffbfafbafa57afc0e4c98db88b67f2094cb44488758f06e5da95d7036f19556a4a732525e84289a425f4f6fd8e412a9d7442f
   languageName: node
   linkType: hard
 
-"postcss@npm:^8.2.15, postcss@npm:^8.3.11":
-  version: 8.4.21
-  resolution: "postcss@npm:8.4.21"
-  dependencies:
-    nanoid: ^3.3.4
-    picocolors: ^1.0.0
-    source-map-js: ^1.0.2
-  checksum: e39ac60ccd1542d4f9d93d894048aac0d686b3bb38e927d8386005718e6793dbbb46930f0a523fe382f1bbd843c6d980aaea791252bf5e176180e5a4336d9679
-  languageName: node
-  linkType: hard
-
-"postcss@npm:^8.4.21":
-  version: 8.4.26
-  resolution: "postcss@npm:8.4.26"
+"postcss@npm:^8.2.15, postcss@npm:^8.3.11, postcss@npm:^8.4.33":
+  version: 8.4.35
+  resolution: "postcss@npm:8.4.35"
   dependencies:
-    nanoid: ^3.3.6
+    nanoid: ^3.3.7
     picocolors: ^1.0.0
     source-map-js: ^1.0.2
-  checksum: 1cf08ee10d58cbe98f94bf12ac49a5e5ed1588507d333d2642aacc24369ca987274e1f60ff4cbf0081f70d2ab18a5cd3a4a273f188d835b8e7f3ba381b184e57
+  checksum: cf3c3124d3912a507603f6d9a49b3783f741075e9aa73eb592a6dd9194f9edab9d20a8875d16d137d4f779fe7b6fbd1f5727e39bfd1c3003724980ee4995e1da
   languageName: node
   linkType: hard
 
 "prelude-ls@npm:^1.2.1":
   version: 1.2.1
   resolution: "prelude-ls@npm:1.2.1"
   checksum: cd192ec0d0a8e4c6da3bb80e4f62afe336df3f76271ac6deb0e6a36187133b6073a19e9727a1ff108cd8b9982e4768850d413baa71214dd80c7979617dca827a
@@ -4749,17 +4469,17 @@
     object-assign: ^4.1.1
     react-is: ^16.13.1
   checksum: c056d3f1c057cb7ff8344c645450e14f088a915d078dcda795041765047fa080d38e5d626560ccaac94a4e16e3aa15f3557c1a9a8d1174530955e992c675e459
   languageName: node
   linkType: hard
 
 "punycode@npm:^2.1.0, punycode@npm:^2.1.1":
-  version: 2.3.0
-  resolution: "punycode@npm:2.3.0"
-  checksum: 39f760e09a2a3bbfe8f5287cf733ecdad69d6af2fe6f97ca95f24b8921858b91e9ea3c9eeec6e08cede96181b3bb33f95c6ffd8c77e63986508aa2e8159fa200
+  version: 2.3.1
+  resolution: "punycode@npm:2.3.1"
+  checksum: bb0a0ceedca4c3c57a9b981b90601579058903c62be23c5e8e843d2c2d4148a3ecf029d5133486fb0e1822b098ba8bba09e89d6b21742d02fa26bda6441a6fb2
   languageName: node
   linkType: hard
 
 "querystringify@npm:^2.1.1":
   version: 2.2.0
   resolution: "querystringify@npm:2.2.0"
   checksum: 5641ea231bad7ef6d64d9998faca95611ed4b11c2591a8cae741e178a974f6a8e0ebde008475259abe1621cb15e692404e6b6626e927f7b849d5c09392604b15
@@ -4842,22 +4562,23 @@
   resolution: "rechoir@npm:0.8.0"
   dependencies:
     resolve: ^1.20.0
   checksum: ad3caed8afdefbc33fbc30e6d22b86c35b3d51c2005546f4e79bcc03c074df804b3640ad18945e6bef9ed12caedc035655ec1082f64a5e94c849ff939dc0a788
   languageName: node
   linkType: hard
 
-"regexp.prototype.flags@npm:^1.4.3":
-  version: 1.4.3
-  resolution: "regexp.prototype.flags@npm:1.4.3"
-  dependencies:
-    call-bind: ^1.0.2
-    define-properties: ^1.1.3
-    functions-have-names: ^1.2.2
-  checksum: 51228bae732592adb3ededd5e15426be25f289e9c4ef15212f4da73f4ec3919b6140806374b8894036a86020d054a8d2657d3fee6bb9b4d35d8939c20030b7a6
+"regexp.prototype.flags@npm:^1.5.2":
+  version: 1.5.2
+  resolution: "regexp.prototype.flags@npm:1.5.2"
+  dependencies:
+    call-bind: ^1.0.6
+    define-properties: ^1.2.1
+    es-errors: ^1.3.0
+    set-function-name: ^2.0.1
+  checksum: d7f333667d5c564e2d7a97c56c3075d64c722c9bb51b2b4df6822b2e8096d623a5e63088fb4c83df919b6951ef8113841de8b47de7224872fa6838bc5d8a7d64
   languageName: node
   linkType: hard
 
 "require-from-string@npm:^2.0.2":
   version: 2.0.2
   resolution: "require-from-string@npm:2.0.2"
   checksum: a03ef6895445f33a4015300c426699bc66b2b044ba7b670aa238610381b56d3f07c686251740d575e22f4c87531ba662d06937508f0f3c0f1ddc04db3130560b
@@ -4890,63 +4611,37 @@
 "resolve-from@npm:^5.0.0":
   version: 5.0.0
   resolution: "resolve-from@npm:5.0.0"
   checksum: 4ceeb9113e1b1372d0cd969f3468fa042daa1dd9527b1b6bb88acb6ab55d8b9cd65dbf18819f9f9ddf0db804990901dcdaade80a215e7b2c23daae38e64f5bdf
   languageName: node
   linkType: hard
 
-"resolve@npm:^1.10.0, resolve@npm:^1.9.0":
-  version: 1.22.1
-  resolution: "resolve@npm:1.22.1"
+"resolve@npm:^1.10.0, resolve@npm:^1.20.0, resolve@npm:^1.9.0":
+  version: 1.22.8
+  resolution: "resolve@npm:1.22.8"
   dependencies:
-    is-core-module: ^2.9.0
+    is-core-module: ^2.13.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: 07af5fc1e81aa1d866cbc9e9460fbb67318a10fa3c4deadc35c3ad8a898ee9a71a86a65e4755ac3195e0ea0cfbe201eb323ebe655ce90526fd61917313a34e4e
+  checksum: f8a26958aa572c9b064562750b52131a37c29d072478ea32e129063e2da7f83e31f7f11e7087a18225a8561cfe8d2f0df9dbea7c9d331a897571c0a2527dbb4c
   languageName: node
   linkType: hard
 
-"resolve@npm:^1.20.0":
-  version: 1.22.3
-  resolution: "resolve@npm:1.22.3"
+"resolve@patch:resolve@^1.10.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.20.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.9.0#~builtin<compat/resolve>":
+  version: 1.22.8
+  resolution: "resolve@patch:resolve@npm%3A1.22.8#~builtin<compat/resolve>::version=1.22.8&hash=c3c19d"
   dependencies:
-    is-core-module: ^2.12.0
+    is-core-module: ^2.13.0
     path-parse: ^1.0.7
     supports-preserve-symlinks-flag: ^1.0.0
   bin:
     resolve: bin/resolve
-  checksum: fb834b81348428cb545ff1b828a72ea28feb5a97c026a1cf40aa1008352c72811ff4d4e71f2035273dc536dcfcae20c13604ba6283c612d70fa0b6e44519c374
-  languageName: node
-  linkType: hard
-
-"resolve@patch:resolve@^1.10.0#~builtin<compat/resolve>, resolve@patch:resolve@^1.9.0#~builtin<compat/resolve>":
-  version: 1.22.1
-  resolution: "resolve@patch:resolve@npm%3A1.22.1#~builtin<compat/resolve>::version=1.22.1&hash=c3c19d"
-  dependencies:
-    is-core-module: ^2.9.0
-    path-parse: ^1.0.7
-    supports-preserve-symlinks-flag: ^1.0.0
-  bin:
-    resolve: bin/resolve
-  checksum: 5656f4d0bedcf8eb52685c1abdf8fbe73a1603bb1160a24d716e27a57f6cecbe2432ff9c89c2bd57542c3a7b9d14b1882b73bfe2e9d7849c9a4c0b8b39f02b8b
-  languageName: node
-  linkType: hard
-
-"resolve@patch:resolve@^1.20.0#~builtin<compat/resolve>":
-  version: 1.22.3
-  resolution: "resolve@patch:resolve@npm%3A1.22.3#~builtin<compat/resolve>::version=1.22.3&hash=c3c19d"
-  dependencies:
-    is-core-module: ^2.12.0
-    path-parse: ^1.0.7
-    supports-preserve-symlinks-flag: ^1.0.0
-  bin:
-    resolve: bin/resolve
-  checksum: ad59734723b596d0891321c951592ed9015a77ce84907f89c9d9307dd0c06e11a67906a3e628c4cae143d3e44898603478af0ddeb2bba3f229a9373efe342665
+  checksum: 5479b7d431cacd5185f8db64bfcb7286ae5e31eb299f4c4f404ad8aa6098b77599563ac4257cb2c37a42f59dfc06a1bec2bcf283bb448f319e37f0feb9a09847
   languageName: node
   linkType: hard
 
 "reusify@npm:^1.0.4":
   version: 1.0.4
   resolution: "reusify@npm:1.0.4"
   checksum: c3076ebcc22a6bc252cb0b9c77561795256c22b757f40c0d8110b1300723f15ec0fc8685e8d4ea6d7666f36c79ccc793b1939c748bf36f18f542744a4e379fcc
@@ -4980,29 +4675,41 @@
   resolution: "run-parallel@npm:1.2.0"
   dependencies:
     queue-microtask: ^1.2.2
   checksum: cb4f97ad25a75ebc11a8ef4e33bb962f8af8516bb2001082ceabd8902e15b98f4b84b4f8a9b222e5d57fc3bd1379c483886ed4619367a7680dad65316993021d
   languageName: node
   linkType: hard
 
+"safe-array-concat@npm:^1.1.0":
+  version: 1.1.0
+  resolution: "safe-array-concat@npm:1.1.0"
+  dependencies:
+    call-bind: ^1.0.5
+    get-intrinsic: ^1.2.2
+    has-symbols: ^1.0.3
+    isarray: ^2.0.5
+  checksum: 5c71eaa999168ee7474929f1cd3aae80f486353a651a094d9968936692cf90aa065224929a6486dcda66334a27dce4250a83612f9e0fef6dced1a925d3ac7296
+  languageName: node
+  linkType: hard
+
 "safe-buffer@npm:^5.1.0":
   version: 5.2.1
   resolution: "safe-buffer@npm:5.2.1"
   checksum: b99c4b41fdd67a6aaf280fcd05e9ffb0813654894223afb78a31f14a19ad220bba8aba1cb14eddce1fcfb037155fe6de4e861784eb434f7d11ed58d1e70dd491
   languageName: node
   linkType: hard
 
-"safe-regex-test@npm:^1.0.0":
-  version: 1.0.0
-  resolution: "safe-regex-test@npm:1.0.0"
+"safe-regex-test@npm:^1.0.3":
+  version: 1.0.3
+  resolution: "safe-regex-test@npm:1.0.3"
   dependencies:
-    call-bind: ^1.0.2
-    get-intrinsic: ^1.1.3
+    call-bind: ^1.0.6
+    es-errors: ^1.3.0
     is-regex: ^1.1.4
-  checksum: bc566d8beb8b43c01b94e67de3f070fd2781685e835959bbbaaec91cc53381145ca91f69bd837ce6ec244817afa0a5e974fc4e40a2957f0aca68ac3add1ddd34
+  checksum: 6c7d392ff1ae7a3ae85273450ed02d1d131f1d2c76e177d6b03eb88e6df8fa062639070e7d311802c1615f351f18dc58f9454501c58e28d5ffd9b8f502ba6489
   languageName: node
   linkType: hard
 
 "safer-buffer@npm:>= 2.1.2 < 3.0.0":
   version: 2.1.2
   resolution: "safer-buffer@npm:2.1.2"
   checksum: cab8f25ae6f1434abee8d80023d7e72b598cf1327164ddab31003c51215526801e40b66c5e65d658a0af1e9d6478cadcb4c745f4bd6751f97d8644786c0978b0
@@ -5039,26 +4746,15 @@
     "@types/json-schema": ^7.0.5
     ajv: ^6.12.4
     ajv-keywords: ^3.5.2
   checksum: 32c62fc9e28edd101e1bd83453a4216eb9bd875cc4d3775e4452b541908fa8f61a7bbac8ffde57484f01d7096279d3ba0337078e85a918ecbeb72872fb09fb2b
   languageName: node
   linkType: hard
 
-"schema-utils@npm:^3.0.0, schema-utils@npm:^3.1.0, schema-utils@npm:^3.1.1":
-  version: 3.1.1
-  resolution: "schema-utils@npm:3.1.1"
-  dependencies:
-    "@types/json-schema": ^7.0.8
-    ajv: ^6.12.5
-    ajv-keywords: ^3.5.2
-  checksum: fb73f3d759d43ba033c877628fe9751620a26879f6301d3dbeeb48cf2a65baec5cdf99da65d1bf3b4ff5444b2e59cbe4f81c2456b5e0d2ba7d7fd4aed5da29ce
-  languageName: node
-  linkType: hard
-
-"schema-utils@npm:^3.2.0":
+"schema-utils@npm:^3.0.0, schema-utils@npm:^3.1.1, schema-utils@npm:^3.2.0":
   version: 3.3.0
   resolution: "schema-utils@npm:3.3.0"
   dependencies:
     "@types/json-schema": ^7.0.8
     ajv: ^6.12.5
     ajv-keywords: ^3.5.2
   checksum: ea56971926fac2487f0757da939a871388891bc87c6a82220d125d587b388f1704788f3706e7f63a7b70e49fc2db974c41343528caea60444afd5ce0fe4b85c0
@@ -5074,61 +4770,65 @@
     ajv-formats: ^2.1.1
     ajv-keywords: ^5.1.0
   checksum: 26a0463d47683258106e6652e9aeb0823bf0b85843039e068b57da1892f7ae6b6b1094d48e9ed5ba5cbe9f7166469d880858b9d91abe8bd249421eb813850cde
   languageName: node
   linkType: hard
 
 "semver@npm:2 || 3 || 4 || 5, semver@npm:^5.4.1, semver@npm:^5.5.0":
-  version: 5.7.1
-  resolution: "semver@npm:5.7.1"
+  version: 5.7.2
+  resolution: "semver@npm:5.7.2"
   bin:
-    semver: ./bin/semver
-  checksum: 57fd0acfd0bac382ee87cd52cd0aaa5af086a7dc8d60379dfe65fea491fb2489b6016400813930ecd61fd0952dae75c115287a1b16c234b1550887117744dfaf
+    semver: bin/semver
+  checksum: fb4ab5e0dd1c22ce0c937ea390b4a822147a9c53dbd2a9a0132f12fe382902beef4fbf12cf51bb955248d8d15874ce8cd89532569756384f994309825f10b686
   languageName: node
   linkType: hard
 
-"semver@npm:^7.3.5":
-  version: 7.3.8
-  resolution: "semver@npm:7.3.8"
+"semver@npm:^7.3.5, semver@npm:^7.5.4":
+  version: 7.6.0
+  resolution: "semver@npm:7.6.0"
   dependencies:
     lru-cache: ^6.0.0
   bin:
     semver: bin/semver.js
-  checksum: ba9c7cbbf2b7884696523450a61fee1a09930d888b7a8d7579025ad93d459b2d1949ee5bbfeb188b2be5f4ac163544c5e98491ad6152df34154feebc2cc337c1
+  checksum: 7427f05b70786c696640edc29fdd4bc33b2acf3bbe1740b955029044f80575fc664e1a512e4113c3af21e767154a94b4aa214bf6cd6e42a1f6dba5914e0b208c
   languageName: node
   linkType: hard
 
-"semver@npm:^7.3.8":
-  version: 7.5.4
-  resolution: "semver@npm:7.5.4"
+"serialize-javascript@npm:^6.0.1":
+  version: 6.0.2
+  resolution: "serialize-javascript@npm:6.0.2"
   dependencies:
-    lru-cache: ^6.0.0
-  bin:
-    semver: bin/semver.js
-  checksum: 12d8ad952fa353b0995bf180cdac205a4068b759a140e5d3c608317098b3575ac2f1e09182206bf2eb26120e1c0ed8fb92c48c592f6099680de56bb071423ca3
+    randombytes: ^2.1.0
+  checksum: c4839c6206c1d143c0f80763997a361310305751171dd95e4b57efee69b8f6edd8960a0b7fbfc45042aadff98b206d55428aee0dc276efe54f100899c7fa8ab7
   languageName: node
   linkType: hard
 
-"semver@npm:^7.5.4":
-  version: 7.6.0
-  resolution: "semver@npm:7.6.0"
+"set-function-length@npm:^1.2.1":
+  version: 1.2.1
+  resolution: "set-function-length@npm:1.2.1"
   dependencies:
-    lru-cache: ^6.0.0
-  bin:
-    semver: bin/semver.js
-  checksum: 7427f05b70786c696640edc29fdd4bc33b2acf3bbe1740b955029044f80575fc664e1a512e4113c3af21e767154a94b4aa214bf6cd6e42a1f6dba5914e0b208c
+    define-data-property: ^1.1.2
+    es-errors: ^1.3.0
+    function-bind: ^1.1.2
+    get-intrinsic: ^1.2.3
+    gopd: ^1.0.1
+    has-property-descriptors: ^1.0.1
+  checksum: 23742476d695f2eae86348c069bd164d4f25fa7c26546a46a2b5f370f1f84b98ec64366d2cd17785d5b41bbf16b95855da4b7eb188e7056fe3b0248d61f6afda
   languageName: node
   linkType: hard
 
-"serialize-javascript@npm:^6.0.0, serialize-javascript@npm:^6.0.1":
-  version: 6.0.1
-  resolution: "serialize-javascript@npm:6.0.1"
+"set-function-name@npm:^2.0.1":
+  version: 2.0.2
+  resolution: "set-function-name@npm:2.0.2"
   dependencies:
-    randombytes: ^2.1.0
-  checksum: 3c4f4cb61d0893b988415bdb67243637333f3f574e9e9cc9a006a2ced0b390b0b3b44aef8d51c951272a9002ec50885eefdc0298891bc27eb2fe7510ea87dc4f
+    define-data-property: ^1.1.4
+    es-errors: ^1.3.0
+    functions-have-names: ^1.2.3
+    has-property-descriptors: ^1.0.2
+  checksum: d6229a71527fd0404399fc6227e0ff0652800362510822a291925c9d7b48a1ca1a468b11b281471c34cd5a2da0db4f5d7ff315a61d26655e77f6e971e6d0c80f
   languageName: node
   linkType: hard
 
 "shallow-clone@npm:^3.0.0":
   version: 3.0.1
   resolution: "shallow-clone@npm:3.0.1"
   dependencies:
@@ -5166,28 +4866,29 @@
   version: 3.0.0
   resolution: "shebang-regex@npm:3.0.0"
   checksum: 1a2bcae50de99034fcd92ad4212d8e01eedf52c7ec7830eedcf886622804fe36884278f2be8be0ea5fde3fd1c23911643a4e0f726c8685b61871c8908af01222
   languageName: node
   linkType: hard
 
 "shell-quote@npm:^1.6.1":
-  version: 1.8.0
-  resolution: "shell-quote@npm:1.8.0"
-  checksum: 6ef7c5e308b9c77eedded882653a132214fa98b4a1512bb507588cf6cd2fc78bfee73e945d0c3211af028a1eabe09c6a19b96edd8977dc149810797e93809749
+  version: 1.8.1
+  resolution: "shell-quote@npm:1.8.1"
+  checksum: 5f01201f4ef504d4c6a9d0d283fa17075f6770bfbe4c5850b074974c68062f37929ca61700d95ad2ac8822e14e8c4b990ca0e6e9272e64befd74ce5e19f0736b
   languageName: node
   linkType: hard
 
 "side-channel@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "side-channel@npm:1.0.4"
+  version: 1.0.6
+  resolution: "side-channel@npm:1.0.6"
   dependencies:
-    call-bind: ^1.0.0
-    get-intrinsic: ^1.0.2
-    object-inspect: ^1.9.0
-  checksum: 351e41b947079c10bd0858364f32bb3a7379514c399edb64ab3dce683933483fc63fb5e4efe0a15a2e8a7e3c436b6a91736ddb8d8c6591b0460a24bb4a1ee245
+    call-bind: ^1.0.7
+    es-errors: ^1.3.0
+    get-intrinsic: ^1.2.4
+    object-inspect: ^1.13.1
+  checksum: bfc1afc1827d712271453e91b7cd3878ac0efd767495fd4e594c4c2afaa7963b7b510e249572bfd54b0527e66e4a12b61b80c061389e129755f34c493aad9b97
   languageName: node
   linkType: hard
 
 "slash@npm:^3.0.0":
   version: 3.0.0
   resolution: "slash@npm:3.0.0"
   checksum: 94a93fff615f25a999ad4b83c9d5e257a7280c90a32a7cb8b4a87996e4babf322e469c42b7f649fd5796edd8687652f3fb452a86dc97a816f01113183393f11c
@@ -5249,77 +4950,88 @@
   version: 0.6.1
   resolution: "source-map@npm:0.6.1"
   checksum: 59ce8640cf3f3124f64ac289012c2b8bd377c238e316fb323ea22fbfe83da07d81e000071d7242cad7a23cd91c7de98e4df8830ec3f133cb6133a5f6e9f67bc2
   languageName: node
   linkType: hard
 
 "spdx-correct@npm:^3.0.0":
-  version: 3.1.1
-  resolution: "spdx-correct@npm:3.1.1"
+  version: 3.2.0
+  resolution: "spdx-correct@npm:3.2.0"
   dependencies:
     spdx-expression-parse: ^3.0.0
     spdx-license-ids: ^3.0.0
-  checksum: 77ce438344a34f9930feffa61be0eddcda5b55fc592906ef75621d4b52c07400a97084d8701557b13f7d2aae0cb64f808431f469e566ef3fe0a3a131dcb775a6
+  checksum: e9ae98d22f69c88e7aff5b8778dc01c361ef635580e82d29e5c60a6533cc8f4d820803e67d7432581af0cc4fb49973125076ee3b90df191d153e223c004193b2
   languageName: node
   linkType: hard
 
 "spdx-exceptions@npm:^2.1.0":
-  version: 2.3.0
-  resolution: "spdx-exceptions@npm:2.3.0"
-  checksum: cb69a26fa3b46305637123cd37c85f75610e8c477b6476fa7354eb67c08128d159f1d36715f19be6f9daf4b680337deb8c65acdcae7f2608ba51931540687ac0
+  version: 2.5.0
+  resolution: "spdx-exceptions@npm:2.5.0"
+  checksum: bb127d6e2532de65b912f7c99fc66097cdea7d64c10d3ec9b5e96524dbbd7d20e01cba818a6ddb2ae75e62bb0c63d5e277a7e555a85cbc8ab40044984fa4ae15
   languageName: node
   linkType: hard
 
 "spdx-expression-parse@npm:^3.0.0":
   version: 3.0.1
   resolution: "spdx-expression-parse@npm:3.0.1"
   dependencies:
     spdx-exceptions: ^2.1.0
     spdx-license-ids: ^3.0.0
   checksum: a1c6e104a2cbada7a593eaa9f430bd5e148ef5290d4c0409899855ce8b1c39652bcc88a725259491a82601159d6dc790bedefc9016c7472f7de8de7361f8ccde
   languageName: node
   linkType: hard
 
 "spdx-license-ids@npm:^3.0.0":
-  version: 3.0.12
-  resolution: "spdx-license-ids@npm:3.0.12"
-  checksum: 92a4dddce62ce1db6fe54a7a839cf85e06abc308fc83b776a55b44e4f1906f02e7ebd506120847039e976bbbad359ea8bdfafb7925eae5cd7e73255f02e0b7d6
+  version: 3.0.17
+  resolution: "spdx-license-ids@npm:3.0.17"
+  checksum: 0aba5d16292ff604dd20982200e23b4d425f6ba364765039bdbde2f6c956b9909fce1ad040a897916a5f87388e85e001f90cb64bf706b6e319f3908cfc445a59
   languageName: node
   linkType: hard
 
 "string.prototype.padend@npm:^3.0.0":
-  version: 3.1.4
-  resolution: "string.prototype.padend@npm:3.1.4"
+  version: 3.1.5
+  resolution: "string.prototype.padend@npm:3.1.5"
   dependencies:
     call-bind: ^1.0.2
-    define-properties: ^1.1.4
-    es-abstract: ^1.20.4
-  checksum: 76e07238fe31dc12177428f0436b7ed6985f6a7ba97470fd53e4f0a6d9860bfee127d81957f3073cc879b434233df143825d140581e1340278053ad993c92f6c
+    define-properties: ^1.2.0
+    es-abstract: ^1.22.1
+  checksum: fc915e0b6ae1dce07a9f5088429d84fda2c1c0ac9a05bc14a602f173cc2fdef32e4893dfba5656f8f955450c9c16deebdb8d303d27613a367bc6d8508a94cd5e
   languageName: node
   linkType: hard
 
-"string.prototype.trimend@npm:^1.0.6":
-  version: 1.0.6
-  resolution: "string.prototype.trimend@npm:1.0.6"
+"string.prototype.trim@npm:^1.2.8":
+  version: 1.2.8
+  resolution: "string.prototype.trim@npm:1.2.8"
   dependencies:
     call-bind: ^1.0.2
-    define-properties: ^1.1.4
-    es-abstract: ^1.20.4
-  checksum: 0fdc34645a639bd35179b5a08227a353b88dc089adf438f46be8a7c197fc3f22f8514c1c9be4629b3cd29c281582730a8cbbad6466c60f76b5f99cf2addb132e
+    define-properties: ^1.2.0
+    es-abstract: ^1.22.1
+  checksum: 49eb1a862a53aba73c3fb6c2a53f5463173cb1f4512374b623bcd6b43ad49dd559a06fb5789bdec771a40fc4d2a564411c0a75d35fb27e76bbe738c211ecff07
   languageName: node
   linkType: hard
 
-"string.prototype.trimstart@npm:^1.0.6":
-  version: 1.0.6
-  resolution: "string.prototype.trimstart@npm:1.0.6"
+"string.prototype.trimend@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "string.prototype.trimend@npm:1.0.7"
+  dependencies:
+    call-bind: ^1.0.2
+    define-properties: ^1.2.0
+    es-abstract: ^1.22.1
+  checksum: 2375516272fd1ba75992f4c4aa88a7b5f3c7a9ca308d963bcd5645adf689eba6f8a04ebab80c33e30ec0aefc6554181a3a8416015c38da0aa118e60ec896310c
+  languageName: node
+  linkType: hard
+
+"string.prototype.trimstart@npm:^1.0.7":
+  version: 1.0.7
+  resolution: "string.prototype.trimstart@npm:1.0.7"
   dependencies:
     call-bind: ^1.0.2
-    define-properties: ^1.1.4
-    es-abstract: ^1.20.4
-  checksum: 89080feef416621e6ef1279588994305477a7a91648d9436490d56010a1f7adc39167cddac7ce0b9884b8cdbef086987c4dcb2960209f2af8bac0d23ceff4f41
+    define-properties: ^1.2.0
+    es-abstract: ^1.22.1
+  checksum: 13d0c2cb0d5ff9e926fa0bec559158b062eed2b68cd5be777ffba782c96b2b492944e47057274e064549b94dd27cf81f48b27a31fee8af5b574cff253e7eb613
   languageName: node
   linkType: hard
 
 "strip-ansi@npm:^6.0.1":
   version: 6.0.1
   resolution: "strip-ansi@npm:6.0.1"
   dependencies:
@@ -5351,26 +5063,26 @@
   peerDependencies:
     webpack: ^4.0.0 || ^5.0.0
   checksum: 21425246a5a8f14d1625a657a3a56f8a323193fa341a71af818a2ed2a429efa2385a328b4381cf2f12c2d0e6380801eb9e0427ed9c3a10ff95c86e383184d632
   languageName: node
   linkType: hard
 
 "style-loader@npm:~3.3.1":
-  version: 3.3.3
-  resolution: "style-loader@npm:3.3.3"
+  version: 3.3.4
+  resolution: "style-loader@npm:3.3.4"
   peerDependencies:
     webpack: ^5.0.0
-  checksum: f59c953f56f6a935bd6a1dfa409f1128fed2b66b48ce4a7a75b85862a7156e5e90ab163878962762f528ec4d510903d828da645e143fbffd26f055dc1c094078
+  checksum: caac3f2fe2c3c89e49b7a2a9329e1cfa515ecf5f36b9c4885f9b218019fda207a9029939b2c35821dec177a264a007e7c391ccdd3ff7401881ce6287b9c8f38b
   languageName: node
   linkType: hard
 
 "style-mod@npm:^4.0.0, style-mod@npm:^4.1.0":
-  version: 4.1.0
-  resolution: "style-mod@npm:4.1.0"
-  checksum: 8402b14ca11113a3640d46b3cf7ba49f05452df7846bc5185a3535d9b6a64a3019e7fb636b59ccbb7816aeb0725b24723e77a85b05612a9360e419958e13b4e6
+  version: 4.1.2
+  resolution: "style-mod@npm:4.1.2"
+  checksum: 7c5c3e82747f9bcf5f288d8d07f50848e4630fe5ff7bfe4d94cc87d6b6a2588227cbf21b4c792ac6406e5852293300a75e710714479a5c59a06af677f0825ef8
   languageName: node
   linkType: hard
 
 "supports-color@npm:^5.3.0":
   version: 5.5.0
   resolution: "supports-color@npm:5.5.0"
   dependencies:
@@ -5407,90 +5119,54 @@
 "tabbable@npm:^5.2.0":
   version: 5.3.3
   resolution: "tabbable@npm:5.3.3"
   checksum: 1aa56e1bb617cc10616c407f4e756f0607f3e2d30f9803664d70b85db037ca27e75918ed1c71443f3dc902e21dc9f991ce4b52d63a538c9b69b3218d3babcd70
   languageName: node
   linkType: hard
 
-"tapable@npm:^2.1.1, tapable@npm:^2.2.0":
+"tapable@npm:^2.1.1, tapable@npm:^2.2.0, tapable@npm:^2.2.1":
   version: 2.2.1
   resolution: "tapable@npm:2.2.1"
   checksum: 3b7a1b4d86fa940aad46d9e73d1e8739335efd4c48322cb37d073eb6f80f5281889bf0320c6d8ffcfa1a0dd5bfdbd0f9d037e252ef972aca595330538aac4d51
   languageName: node
   linkType: hard
 
-"terser-webpack-plugin@npm:^5.1.3":
-  version: 5.3.6
-  resolution: "terser-webpack-plugin@npm:5.3.6"
+"terser-webpack-plugin@npm:^5.3.10, terser-webpack-plugin@npm:^5.3.7":
+  version: 5.3.10
+  resolution: "terser-webpack-plugin@npm:5.3.10"
   dependencies:
-    "@jridgewell/trace-mapping": ^0.3.14
-    jest-worker: ^27.4.5
-    schema-utils: ^3.1.1
-    serialize-javascript: ^6.0.0
-    terser: ^5.14.1
-  peerDependencies:
-    webpack: ^5.1.0
-  peerDependenciesMeta:
-    "@swc/core":
-      optional: true
-    esbuild:
-      optional: true
-    uglify-js:
-      optional: true
-  checksum: 8f3448d7fdb0434ce6a0c09d95c462bfd2f4a5a430233d854163337f734a7f5c07c74513d16081e06d4ca33d366d5b1a36f5444219bc41a7403afd6162107bad
-  languageName: node
-  linkType: hard
-
-"terser-webpack-plugin@npm:^5.3.7":
-  version: 5.3.9
-  resolution: "terser-webpack-plugin@npm:5.3.9"
-  dependencies:
-    "@jridgewell/trace-mapping": ^0.3.17
+    "@jridgewell/trace-mapping": ^0.3.20
     jest-worker: ^27.4.5
     schema-utils: ^3.1.1
     serialize-javascript: ^6.0.1
-    terser: ^5.16.8
+    terser: ^5.26.0
   peerDependencies:
     webpack: ^5.1.0
   peerDependenciesMeta:
     "@swc/core":
       optional: true
     esbuild:
       optional: true
     uglify-js:
       optional: true
-  checksum: 41705713d6f9cb83287936b21e27c658891c78c4392159f5148b5623f0e8c48559869779619b058382a4c9758e7820ea034695e57dc7c474b4962b79f553bc5f
-  languageName: node
-  linkType: hard
-
-"terser@npm:^5.14.1":
-  version: 5.16.5
-  resolution: "terser@npm:5.16.5"
-  dependencies:
-    "@jridgewell/source-map": ^0.3.2
-    acorn: ^8.5.0
-    commander: ^2.20.0
-    source-map-support: ~0.5.20
-  bin:
-    terser: bin/terser
-  checksum: f2c1a087fac7f4ff04b1b4e79bffc52e2fc0b068b98912bfcc0b341184c284c30c19ed73f76ac92b225b71668f7f8fc586d99a7e50a29cdc1c916cb1265522ec
+  checksum: bd6e7596cf815f3353e2a53e79cbdec959a1b0276f5e5d4e63e9d7c3c5bb5306df567729da287d1c7b39d79093e56863c569c42c6c24cc34c76aa313bd2cbcea
   languageName: node
   linkType: hard
 
-"terser@npm:^5.16.8":
-  version: 5.19.1
-  resolution: "terser@npm:5.19.1"
+"terser@npm:^5.26.0":
+  version: 5.28.1
+  resolution: "terser@npm:5.28.1"
   dependencies:
     "@jridgewell/source-map": ^0.3.3
     acorn: ^8.8.2
     commander: ^2.20.0
     source-map-support: ~0.5.20
   bin:
     terser: bin/terser
-  checksum: 18657b2a282238a1ca9c825efa966f4dd043a33196b2f8a7a2cba406a2006e14f55295b9d9cf6380a18599b697e9579e4092c99b9f40c7871ceec01cc98e3606
+  checksum: 2668823cbdf8ae4c62d17a899614c849ddbfa932fce2309e600bd9ed6e6adb87b2c0aca30acb6cdf0d8e83a77ae3858af14cd357a2cb25b9f289fae98c7f7537
   languageName: node
   linkType: hard
 
 "text-table@npm:^0.2.0":
   version: 0.2.0
   resolution: "text-table@npm:0.2.0"
   checksum: b6937a38c80c7f84d9c11dd75e49d5c44f71d95e810a3250bd1f1797fc7117c57698204adf676b71497acc205d769d65c16ae8fa10afad832ae1322630aef10a
@@ -5543,22 +5219,63 @@
 "type-fest@npm:^0.20.2":
   version: 0.20.2
   resolution: "type-fest@npm:0.20.2"
   checksum: 4fb3272df21ad1c552486f8a2f8e115c09a521ad7a8db3d56d53718d0c907b62c6e9141ba5f584af3f6830d0872c521357e512381f24f7c44acae583ad517d73
   languageName: node
   linkType: hard
 
-"typed-array-length@npm:^1.0.4":
-  version: 1.0.4
-  resolution: "typed-array-length@npm:1.0.4"
+"typed-array-buffer@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "typed-array-buffer@npm:1.0.2"
   dependencies:
-    call-bind: ^1.0.2
+    call-bind: ^1.0.7
+    es-errors: ^1.3.0
+    is-typed-array: ^1.1.13
+  checksum: 02ffc185d29c6df07968272b15d5319a1610817916ec8d4cd670ded5d1efe72901541ff2202fcc622730d8a549c76e198a2f74e312eabbfb712ed907d45cbb0b
+  languageName: node
+  linkType: hard
+
+"typed-array-byte-length@npm:^1.0.1":
+  version: 1.0.1
+  resolution: "typed-array-byte-length@npm:1.0.1"
+  dependencies:
+    call-bind: ^1.0.7
     for-each: ^0.3.3
-    is-typed-array: ^1.1.9
-  checksum: 2228febc93c7feff142b8c96a58d4a0d7623ecde6c7a24b2b98eb3170e99f7c7eff8c114f9b283085cd59dcd2bd43aadf20e25bba4b034a53c5bb292f71f8956
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+  checksum: f65e5ecd1cf76b1a2d0d6f631f3ea3cdb5e08da106c6703ffe687d583e49954d570cc80434816d3746e18be889ffe53c58bf3e538081ea4077c26a41055b216d
+  languageName: node
+  linkType: hard
+
+"typed-array-byte-offset@npm:^1.0.2":
+  version: 1.0.2
+  resolution: "typed-array-byte-offset@npm:1.0.2"
+  dependencies:
+    available-typed-arrays: ^1.0.7
+    call-bind: ^1.0.7
+    for-each: ^0.3.3
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+  checksum: c8645c8794a621a0adcc142e0e2c57b1823bbfa4d590ad2c76b266aa3823895cf7afb9a893bf6685e18454ab1b0241e1a8d885a2d1340948efa4b56add4b5f67
+  languageName: node
+  linkType: hard
+
+"typed-array-length@npm:^1.0.5":
+  version: 1.0.5
+  resolution: "typed-array-length@npm:1.0.5"
+  dependencies:
+    call-bind: ^1.0.7
+    for-each: ^0.3.3
+    gopd: ^1.0.1
+    has-proto: ^1.0.3
+    is-typed-array: ^1.1.13
+    possible-typed-array-names: ^1.0.0
+  checksum: 82f5b666155cff1b345a1f3ab018d3f7667990f525435e4c8448cc094ab0f8ea283bb7cbde4d7bc82ea0b9b1072523bf31e86620d72615951d7fa9ccb4f42dfa
   languageName: node
   linkType: hard
 
 "typescript@npm:~5.0.2":
   version: 5.0.4
   resolution: "typescript@npm:5.0.4"
   bin:
@@ -5603,32 +5320,39 @@
 "underscore@npm:>=1.8.3":
   version: 1.13.6
   resolution: "underscore@npm:1.13.6"
   checksum: d5cedd14a9d0d91dd38c1ce6169e4455bb931f0aaf354108e47bd46d3f2da7464d49b2171a5cf786d61963204a42d01ea1332a903b7342ad428deaafaf70ec36
   languageName: node
   linkType: hard
 
+"undici-types@npm:~5.26.4":
+  version: 5.26.5
+  resolution: "undici-types@npm:5.26.5"
+  checksum: 3192ef6f3fd5df652f2dc1cd782b49d6ff14dc98e5dced492aa8a8c65425227da5da6aafe22523c67f035a272c599bb89cfe803c1db6311e44bed3042fc25487
+  languageName: node
+  linkType: hard
+
 "universalify@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "universalify@npm:2.0.0"
-  checksum: 2406a4edf4a8830aa6813278bab1f953a8e40f2f63a37873ffa9a3bc8f9745d06cc8e88f3572cb899b7e509013f7f6fcc3e37e8a6d914167a5381d8440518c44
+  version: 2.0.1
+  resolution: "universalify@npm:2.0.1"
+  checksum: ecd8469fe0db28e7de9e5289d32bd1b6ba8f7183db34f3bfc4ca53c49891c2d6aa05f3fb3936a81285a905cc509fb641a0c3fc131ec786167eff41236ae32e60
   languageName: node
   linkType: hard
 
-"update-browserslist-db@npm:^1.0.10":
-  version: 1.0.10
-  resolution: "update-browserslist-db@npm:1.0.10"
+"update-browserslist-db@npm:^1.0.13":
+  version: 1.0.13
+  resolution: "update-browserslist-db@npm:1.0.13"
   dependencies:
     escalade: ^3.1.1
     picocolors: ^1.0.0
   peerDependencies:
     browserslist: ">= 4.21.0"
   bin:
-    browserslist-lint: cli.js
-  checksum: 12db73b4f63029ac407b153732e7cd69a1ea8206c9100b482b7d12859cd3cd0bc59c602d7ae31e652706189f1acb90d42c53ab24a5ba563ed13aebdddc5561a0
+    update-browserslist-db: cli.js
+  checksum: 1e47d80182ab6e4ad35396ad8b61008ae2a1330221175d0abd37689658bdb61af9b705bfc41057fd16682474d79944fb2d86767c5ed5ae34b6276b9bed353322
   languageName: node
   linkType: hard
 
 "uri-js@npm:^4.2.2":
   version: 4.4.1
   resolution: "uri-js@npm:4.4.1"
   dependencies:
@@ -5829,31 +5553,22 @@
       optional: true
   bin:
     webpack-cli: bin/cli.js
   checksum: 3a4ad0d0342a6815c850ee4633cc2a8a5dae04f918e7847f180bf24ab400803cf8a8943707ffbed03eb20fe6ce647f996f60a2aade87b0b4a9954da3da172ce0
   languageName: node
   linkType: hard
 
-"webpack-merge@npm:^5.7.3":
-  version: 5.8.0
-  resolution: "webpack-merge@npm:5.8.0"
-  dependencies:
-    clone-deep: ^4.0.1
-    wildcard: ^2.0.0
-  checksum: 88786ab91013f1bd2a683834ff381be81c245a4b0f63304a5103e90f6653f44dab496a0768287f8531761f8ad957d1f9f3ccb2cb55df0de1bd9ee343e079da26
-  languageName: node
-  linkType: hard
-
-"webpack-merge@npm:^5.8.0":
-  version: 5.9.0
-  resolution: "webpack-merge@npm:5.9.0"
+"webpack-merge@npm:^5.7.3, webpack-merge@npm:^5.8.0":
+  version: 5.10.0
+  resolution: "webpack-merge@npm:5.10.0"
   dependencies:
     clone-deep: ^4.0.1
+    flat: ^5.0.2
     wildcard: ^2.0.0
-  checksum: 64fe2c23aacc5f19684452a0e84ec02c46b990423aee6fcc5c18d7d471155bd14e9a6adb02bd3656eb3e0ac2532c8e97d69412ad14c97eeafe32fa6d10050872
+  checksum: 1fe8bf5309add7298e1ac72fb3f2090e1dfa80c48c7e79fa48aa60b5961332c7d0d61efa8851acb805e6b91a4584537a347bc106e05e9aec87fa4f7088c62f2f
   languageName: node
   linkType: hard
 
 "webpack-sources@npm:^1.2.0":
   version: 1.4.3
   resolution: "webpack-sources@npm:1.4.3"
   dependencies:
@@ -5866,85 +5581,48 @@
 "webpack-sources@npm:^3.2.3":
   version: 3.2.3
   resolution: "webpack-sources@npm:3.2.3"
   checksum: 989e401b9fe3536529e2a99dac8c1bdc50e3a0a2c8669cbafad31271eadd994bc9405f88a3039cd2e29db5e6d9d0926ceb7a1a4e7409ece021fe79c37d9c4607
   languageName: node
   linkType: hard
 
-"webpack@npm:^5.75.0":
-  version: 5.75.0
-  resolution: "webpack@npm:5.75.0"
+"webpack@npm:^5.75.0, webpack@npm:^5.76.1":
+  version: 5.90.3
+  resolution: "webpack@npm:5.90.3"
   dependencies:
     "@types/eslint-scope": ^3.7.3
-    "@types/estree": ^0.0.51
-    "@webassemblyjs/ast": 1.11.1
-    "@webassemblyjs/wasm-edit": 1.11.1
-    "@webassemblyjs/wasm-parser": 1.11.1
-    acorn: ^8.7.1
-    acorn-import-assertions: ^1.7.6
-    browserslist: ^4.14.5
-    chrome-trace-event: ^1.0.2
-    enhanced-resolve: ^5.10.0
-    es-module-lexer: ^0.9.0
-    eslint-scope: 5.1.1
-    events: ^3.2.0
-    glob-to-regexp: ^0.4.1
-    graceful-fs: ^4.2.9
-    json-parse-even-better-errors: ^2.3.1
-    loader-runner: ^4.2.0
-    mime-types: ^2.1.27
-    neo-async: ^2.6.2
-    schema-utils: ^3.1.0
-    tapable: ^2.1.1
-    terser-webpack-plugin: ^5.1.3
-    watchpack: ^2.4.0
-    webpack-sources: ^3.2.3
-  peerDependenciesMeta:
-    webpack-cli:
-      optional: true
-  bin:
-    webpack: bin/webpack.js
-  checksum: 2bcc5f3c195f375944e8af2f00bf2feea39cb9fda5f763b0d1b00077f1c51783db25c94d3fae96a07dead9fa085e6ae7474417e5ab31719c9776ea5969ceb83a
-  languageName: node
-  linkType: hard
-
-"webpack@npm:^5.76.1":
-  version: 5.88.2
-  resolution: "webpack@npm:5.88.2"
-  dependencies:
-    "@types/eslint-scope": ^3.7.3
-    "@types/estree": ^1.0.0
+    "@types/estree": ^1.0.5
     "@webassemblyjs/ast": ^1.11.5
     "@webassemblyjs/wasm-edit": ^1.11.5
     "@webassemblyjs/wasm-parser": ^1.11.5
     acorn: ^8.7.1
     acorn-import-assertions: ^1.9.0
-    browserslist: ^4.14.5
+    browserslist: ^4.21.10
     chrome-trace-event: ^1.0.2
     enhanced-resolve: ^5.15.0
     es-module-lexer: ^1.2.1
     eslint-scope: 5.1.1
     events: ^3.2.0
     glob-to-regexp: ^0.4.1
     graceful-fs: ^4.2.9
     json-parse-even-better-errors: ^2.3.1
     loader-runner: ^4.2.0
     mime-types: ^2.1.27
     neo-async: ^2.6.2
     schema-utils: ^3.2.0
     tapable: ^2.1.1
-    terser-webpack-plugin: ^5.3.7
+    terser-webpack-plugin: ^5.3.10
     watchpack: ^2.4.0
     webpack-sources: ^3.2.3
   peerDependenciesMeta:
     webpack-cli:
       optional: true
   bin:
     webpack: bin/webpack.js
-  checksum: 79476a782da31a21f6dd38fbbd06b68da93baf6a62f0d08ca99222367f3b8668f5a1f2086b7bb78e23172e31fa6df6fa7ab09b25e827866c4fc4dc2b30443ce2
+  checksum: de0c824ac220f41cc1153ac33e081d46260b104c4f2fda26f011cdf7a73f74cc091f288cb1fc16f88a36e35bac44e0aa85fc9922fdf3109dfb361f46b20f3fcc
   languageName: node
   linkType: hard
 
 "whatwg-mimetype@npm:^2.3.0":
   version: 2.3.0
   resolution: "whatwg-mimetype@npm:2.3.0"
   checksum: 23eb885940bcbcca4ff841c40a78e9cbb893ec42743993a42bf7aed16085b048b44b06f3402018931687153550f9a32d259dfa524e4f03577ab898b6965e5383
@@ -5971,25 +5649,24 @@
     is-number-object: ^1.0.4
     is-string: ^1.0.5
     is-symbol: ^1.0.3
   checksum: 53ce774c7379071729533922adcca47220228405e1895f26673bbd71bdf7fb09bee38c1d6399395927c6289476b5ae0629863427fd151491b71c4b6cb04f3a5e
   languageName: node
   linkType: hard
 
-"which-typed-array@npm:^1.1.9":
-  version: 1.1.9
-  resolution: "which-typed-array@npm:1.1.9"
+"which-typed-array@npm:^1.1.14":
+  version: 1.1.14
+  resolution: "which-typed-array@npm:1.1.14"
   dependencies:
-    available-typed-arrays: ^1.0.5
-    call-bind: ^1.0.2
+    available-typed-arrays: ^1.0.6
+    call-bind: ^1.0.5
     for-each: ^0.3.3
     gopd: ^1.0.1
-    has-tostringtag: ^1.0.0
-    is-typed-array: ^1.1.10
-  checksum: fe0178ca44c57699ca2c0e657b64eaa8d2db2372a4e2851184f568f98c478ae3dc3fdb5f7e46c384487046b0cf9e23241423242b277e03e8ba3dabc7c84c98ef
+    has-tostringtag: ^1.0.1
+  checksum: efe30c143c58630dde8ab96f9330e20165bacd77ca843c602b510120a415415573bcdef3ccbc30a0e5aaf20f257360cfe24712aea0008f149ce5bb99834c0c0b
   languageName: node
   linkType: hard
 
 "which@npm:^1.2.9":
   version: 1.3.1
   resolution: "which@npm:1.3.1"
   dependencies:
@@ -6008,17 +5685,17 @@
   bin:
     node-which: ./bin/node-which
   checksum: 1a5c563d3c1b52d5f893c8b61afe11abc3bab4afac492e8da5bde69d550de701cf9806235f20a47b5c8fa8a1d6a9135841de2596535e998027a54589000e66d1
   languageName: node
   linkType: hard
 
 "wildcard@npm:^2.0.0":
-  version: 2.0.0
-  resolution: "wildcard@npm:2.0.0"
-  checksum: 1f4fe4c03dfc492777c60f795bbba597ac78794f1b650d68f398fbee9adb765367c516ebd4220889b6a81e9626e7228bbe0d66237abb311573c2ee1f4902a5ad
+  version: 2.0.1
+  resolution: "wildcard@npm:2.0.1"
+  checksum: e0c60a12a219e4b12065d1199802d81c27b841ed6ad6d9d28240980c73ceec6f856771d575af367cbec2982d9ae7838759168b551776577f155044f5a5ba843c
   languageName: node
   linkType: hard
 
 "worker-loader@npm:^3.0.2":
   version: 3.0.8
   resolution: "worker-loader@npm:3.0.8"
   dependencies:
@@ -6049,35 +5726,37 @@
     utf-8-validate:
       optional: true
   checksum: feb3eecd2bae82fa8a8beef800290ce437d8b8063bdc69712725f21aef77c49cb2ff45c6e5e7fce622248f9c7abaee506bae0a9064067ffd6935460c7357321b
   languageName: node
   linkType: hard
 
 "y-protocols@npm:^1.0.5":
-  version: 1.0.5
-  resolution: "y-protocols@npm:1.0.5"
+  version: 1.0.6
+  resolution: "y-protocols@npm:1.0.6"
   dependencies:
-    lib0: ^0.2.42
-  checksum: d19404a4ebafcf3761c28b881abe8c32ab6e457db0e5ffc7dbb749cbc2c3bb98e003a43f3e8eba7f245b2698c76f2c4cdd1c2db869f8ec0c6ef94736d9a88652
+    lib0: ^0.2.85
+  peerDependencies:
+    yjs: ^13.0.0
+  checksum: 4b57c8811befcf2e45c3d47830005f8a33e626c734f78a42fe8a4fa3caad2233ba85a7c8bceefbd52ffc40130d3f3faee664fd0d1c324ff1fa8817a056ccdc1c
   languageName: node
   linkType: hard
 
 "yallist@npm:^4.0.0":
   version: 4.0.0
   resolution: "yallist@npm:4.0.0"
   checksum: 343617202af32df2a15a3be36a5a8c0c8545208f3d3dfbc6bb7c3e3b7e8c6f8e7485432e4f3b88da3031a6e20afa7c711eded32ddfb122896ac5d914e75848d5
   languageName: node
   linkType: hard
 
 "yjs@npm:^13.5.40":
-  version: 13.5.48
-  resolution: "yjs@npm:13.5.48"
+  version: 13.6.14
+  resolution: "yjs@npm:13.6.14"
   dependencies:
-    lib0: ^0.2.49
-  checksum: f9acd3469a8a2005b1b50fb5eed733c7c19dbb18ac75e226969bfe7a7b6dabe2a8a0de1eca28875d4b37e76d3c006be49f2cfa6db906163b73c4c99d4cd9012b
+    lib0: ^0.2.86
+  checksum: df399049049820d32d5759a7bd9d70cf30602408ca2a9771324f1b459f703bb6073fb35b5bcde7493fab3721d64e3c1b60eb88415b184e95a73fbce2947741cb
   languageName: node
   linkType: hard
 
 "yocto-queue@npm:^0.1.0":
   version: 0.1.0
   resolution: "yocto-queue@npm:0.1.0"
   checksum: f77b3d8d00310def622123df93d4ee654fc6a0096182af8bd60679ddcdfb3474c56c6c7190817c84a2785648cdee9d721c0154eb45698c62176c322fb46fc700
```

### Comparing `jupyter_bokeh-4.0.0/conda.recipe/meta.yaml` & `jupyter_bokeh-4.0.1/conda.recipe/meta.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -6,39 +6,50 @@
 {% set version = VERSION %}
 
 package:
   name: {{ name }}
   version: {{ version }}
 
 source:
-  url: ../dist/{{ name }}-{{ version }}-py3-none-any.whl
+  path: ..
 
 build:
   noarch: python
-  script: {{ PYTHON }} -m pip install -vv {{ name }}-{{ version }}-py3-none-any.whl
+  script: {{ PYTHON }} -m pip install --no-deps --ignore-installed .
+  script_env:
+    - JUPYTERLAB_TEST_VERSION
 
 requirements:
   build:
     - jupyter-packaging
-    - jupyterlab
+    - jupyterlab 4.0.*
     - notebook
     - python
-    - setuptools
+    - pip
+    - setuptools >=40.8.0
+    - wheel
     - nodejs >=18.0
-    - hatch
+    - hatchling >=1.5.0
+    - hatch-jupyter-builder>=0.8.2
+    - hatch-nodejs-version
   run:
     - python
     - bokeh 3.*
     - ipywidgets 8.*
   run_constrained:
     - jupyterlab 4.*
 
 test:
+  requires:
+    - jupyterlab
   imports:
     - jupyter_bokeh
+  commands:
+    - jupyter labextension list 2>&1
+    - jupyter labextension list 2>&1 | grep -q 'jupyter.bokeh.*enabled.*OK'
 
 about:
   home: {{ pkgjson['homepage'] }}
   license: {{ project['license']['file'] }}
   summary: {{ pkgjson['description'] }}
 
 extra:
```

### Comparing `jupyter_bokeh-4.0.0/examples/jupyter_interactors.ipynb` & `jupyter_bokeh-4.0.1/examples/jupyter_interactors.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/examples/jupyter_sliders.ipynb` & `jupyter_bokeh-4.0.1/examples/jupyter_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/examples/jupyter_widgets.ipynb` & `jupyter_bokeh-4.0.1/examples/jupyter_widgets.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/examples/notebook_comms.ipynb` & `jupyter_bokeh-4.0.1/examples/notebook_comms.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/examples/server_embed.ipynb` & `jupyter_bokeh-4.0.1/examples/server_embed.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/examples/static_plot.ipynb` & `jupyter_bokeh-4.0.1/examples/static_plot.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/__init__.py` & `jupyter_bokeh-4.0.1/jupyter_bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/widgets.py` & `jupyter_bokeh-4.0.1/jupyter_bokeh/widgets.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/package.json` & `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617123617123617%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^4', '@jupyterlab/apputils': '^4', "*

 * *                   "'@jupyterlab/docregistry': '^4', '@jupyterlab/notebook': '^4', "*

 * *                   "'@jupyterlab/services': '^7', '@jupyterlab/settingregistry': '^4', "*

 * *                   "'@jupyterlab/ui-components': '^4', '@lumino/disposable': '^2'}",*

 * * "'devDependencies'": "{'@jupyterlab/builder': '^4'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3cff93f6f99a3674a3dc.js'}}",*

 * * "'resolutions'": "{'@lum […]*

```diff
@@ -4,28 +4,28 @@
         "name": "Bokeh team"
     },
     "bugs": {
         "url": "https://github.com/bokeh/jupyter_bokeh/issues"
     },
     "dependencies": {
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6",
-        "@jupyterlab/application": "^4.0.3",
-        "@jupyterlab/apputils": "^4.1.3",
-        "@jupyterlab/docregistry": "^4.0.3",
-        "@jupyterlab/notebook": "^4.0.3",
-        "@jupyterlab/services": "^7.1.1",
-        "@jupyterlab/settingregistry": "^4.1.1",
-        "@jupyterlab/ui-components": "^4.0.3",
-        "@lumino/disposable": "^2.1.1",
+        "@jupyterlab/application": "^4",
+        "@jupyterlab/apputils": "^4",
+        "@jupyterlab/docregistry": "^4",
+        "@jupyterlab/notebook": "^4",
+        "@jupyterlab/services": "^7",
+        "@jupyterlab/settingregistry": "^4",
+        "@jupyterlab/ui-components": "^4",
+        "@lumino/disposable": "^2",
         "css-loader": "^5.1.3",
         "style-loader": "^2.0.0"
     },
     "description": "A Jupyter extension for rendering Bokeh content.",
     "devDependencies": {
-        "@jupyterlab/builder": "^4.0.2",
+        "@jupyterlab/builder": "^4",
         "@typescript-eslint/eslint-plugin": "^7.0.1",
         "@typescript-eslint/parser": "^7.0.1",
         "eslint": "^8.36.0",
         "npm-run-all": "^4.1.5",
         "rimraf": "^4.4.1",
         "source-map-loader": "^5.0.0",
         "typescript": "~5.0.2",
@@ -36,15 +36,15 @@
         "{dist,lib}/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/bokeh/jupyter_bokeh",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.e32a0a8e32155667dea0.js",
+            "load": "static/remoteEntry.3cff93f6f99a3674a3dc.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_bokeh/labextension"
     },
     "keywords": [
         "jupyter",
@@ -58,15 +58,15 @@
         "@jupyter-widgets/jupyterlab-manager": "^5.0.4"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/bokeh/jupyter_bokeh.git"
     },
     "resolutions": {
-        "@lumino/widgets": "^2.1.1",
+        "@lumino/widgets": "^2",
         "react": "^18.2.0",
         "react-dom": "^18.2.0"
     },
     "scripts": {
         "__prepare": "jlpm run clean && jlpm run build:prod",
         "build": "jlpm run build:lib && jlpm run build:nbextension && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.0"
+    "version": "4.0.1"
 }
```

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/199.e7fe4770dab71924b124.js` & `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/824.ce3da0e5e0e81f9850cf.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 (self.webpackChunk_bokeh_jupyter_bokeh = self.webpackChunk_bokeh_jupyter_bokeh || []).push([
-    [199], {
-        5199: (e, t, s) => {
+    [824], {
+        9824: (e, t, s) => {
             "use strict";
             s.r(t), s.d(t, {
                 BokehModel: () => v,
                 BokehView: () => g,
                 default: () => k
             });
-            var n = s(3826),
-                i = s(7717);
+            var n = s(1803),
+                i = s(9012);
             class o {
                 constructor(e) {
                     this._context = e
                 }
                 get context() {
                     if (null != this._context) return this._context;
                     throw new Error("context was already disposed")
@@ -20,15 +20,15 @@
                 get isDisposed() {
                     return null == this._context
                 }
                 dispose() {
                     this.isDisposed || (this._context = null)
                 }
             }
-            var r = s(8778);
+            var r = s(1534);
             const d = "application/vnd.bokehjs_load.v0+json",
                 c = "application/vnd.bokehjs_exec.v0+json";
             class l extends r.Widget {
                 constructor(e) {
                     super(), this._load_mimetype = d, this._script_element = document.createElement("script")
                 }
                 renderModel(e) {
@@ -88,15 +88,15 @@
                                 s = null === (e = this._manager.context.sessionContext.session) || void 0 === e ? void 0 : e.kernel;
                             null != s && s.requestExecute(t, !0), this._server_id = null
                         } else this._document_id && (void 0 !== Bokeh.embed.kernels && delete Bokeh.embed.kernels[this._document_id], this._document_id = null);
                         this._manager = null
                     }
                 }
             }
-            var _ = s(48);
+            var _ = s(2288);
 
             function m(e) {
                 return window.Bokeh.require(e)
             }
             const {
                 keys: h,
                 values: u
@@ -220,15 +220,15 @@
                             BokehView: g
                         }
                     })
                 },
                 autoStart: !0
             }
         },
-        48: (e, t) => {
+        2288: (e, t) => {
             Object.assign(t, {
                 name: "@bokeh/jupyter_bokeh",
-                version: "4.0.0"
+                version: "4.0.1"
             })
         }
     }
 ]);
```

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/790.b027b82b72b7c2fb1ea7.js` & `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/7.4b7742c84d4af5271005.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
-/*! For license information please see 790.b027b82b72b7c2fb1ea7.js.LICENSE.txt */
+/*! For license information please see 7.4b7742c84d4af5271005.js.LICENSE.txt */
 (self.webpackChunk_bokeh_jupyter_bokeh = self.webpackChunk_bokeh_jupyter_bokeh || []).push([
-    [790], {
-        3790: (e, t, n) => {
+    [7], {
+        4007: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 BROKEN_FILE_SVG_ICON: () => v,
                 DOMWidgetModel: () => D,
                 DOMWidgetView: () => H,
                 ErrorWidgetView: () => J,
                 IJupyterWidgetRegistry: () => U,
@@ -33,16 +33,16 @@
                 reject: () => f,
                 remove_buffers: () => g,
                 resolvePromisesDict: () => c,
                 shims: () => B,
                 unpack_models: () => C,
                 uuid: () => l
             });
-            var r = n(7930),
-                i = n(8446),
+            var r = n(7262),
+                i = n(2404),
                 o = n.n(i);
 
             function s(e, t) {
                 return e.filter((e => -1 === t.indexOf(e)))
             }
 
             function a(e, t) {
@@ -158,16 +158,16 @@
                     if (!s)
                         for (; this._pending;) n = this._pending, this._pending = !1, this.trigger("change", this, n)
                 } finally {
                     this._pending = !1, this._changing = !1
                 }
                 return this
             }
-            var y = n(2316),
-                b = n(9755),
+            var y = n(1391),
+                b = n(4692),
                 _ = n.n(b);
             const x = "undefined" != typeof Element ? Element.prototype : void 0;
             const w = x && (x.matches || x.webkitMatchesSelector || x.mozMatchesSelector || x.msMatchesSelector || x.oMatchesSelector) || function(e) {
                 const t = (this.document || this.ownerDocument).querySelectorAll(e);
                 let n = t.length;
                 for (; --n >= 0 && t.item(n) !== this;);
                 return n > -1
@@ -216,16 +216,16 @@
                             this.el.removeEventListener(e.eventName, e.handler, !1)
                         }
                         this._domEvents.length = 0
                     }
                     return this
                 }
             }
-            var E = n(5633),
-                T = n(8778);
+            var E = n(6230),
+                T = n(1534);
             const k = "2.0.0",
                 S = "2.1.0",
                 A = "IPY_MODEL_";
 
             function C(e, t) {
                 if (Array.isArray(e)) {
                     const n = [];
@@ -907,17 +907,17 @@
                             msg: t,
                             stack: String(e instanceof Error ? e.stack : e)
                         }
                     }
                 }
             }
         },
-        2316: (e, t, n) => {
+        1391: (e, t, n) => {
             var r, i, o;
-            o = "object" == typeof self && self.self === self && self || "object" == typeof n.g && n.g.global === n.g && n.g, r = [n(7794), n(9755), t], i = function(e, t, n) {
+            o = "object" == typeof self && self.self === self && self || "object" == typeof n.g && n.g.global === n.g && n.g, r = [n(884), n(4692), t], i = function(e, t, n) {
                 o.Backbone = function(e, t, n, r) {
                     var i = e.Backbone,
                         o = Array.prototype.slice;
                     t.VERSION = "1.4.0", t.$ = r, t.noConflict = function() {
                         return e.Backbone = i, this
                     }, t.emulateHTTP = !1, t.emulateJSON = !1;
                     var s, a = t.Events = {},
@@ -1882,15 +1882,15 @@
                                 n && n.call(t.context, e, r, t), e.trigger("error", e, r, t)
                             }
                         };
                     return t
                 }(o, n, e, t)
             }.apply(t, r), void 0 === i || (e.exports = i)
         },
-        9755: function(e, t) {
+        4692: function(e, t) {
             var n;
             ! function(t, n) {
                 "use strict";
                 "object" == typeof e.exports ? e.exports = t.document ? n(t, !0) : function(e) {
                     if (!e.document) throw new Error("jQuery requires a window with a document");
                     return n(e)
                 } : n(t)
@@ -5039,209 +5039,209 @@
                 var on = r.jQuery,
                     sn = r.$;
                 return T.noConflict = function(e) {
                     return r.$ === T && (r.$ = sn), e && r.jQuery === T && (r.jQuery = on), T
                 }, void 0 === i && (r.jQuery = r.$ = T), T
             }))
         },
-        8552: (e, t, n) => {
-            var r = n(852)(n(5639), "DataView");
+        5580: (e, t, n) => {
+            var r = n(6110)(n(9325), "DataView");
             e.exports = r
         },
-        1989: (e, t, n) => {
-            var r = n(1789),
-                i = n(401),
-                o = n(7667),
-                s = n(1327),
-                a = n(1866);
+        1549: (e, t, n) => {
+            var r = n(2032),
+                i = n(3862),
+                o = n(6721),
+                s = n(2749),
+                a = n(5749);
 
             function u(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.clear(); ++t < n;) {
                     var r = e[t];
                     this.set(r[0], r[1])
                 }
             }
             u.prototype.clear = r, u.prototype.delete = i, u.prototype.get = o, u.prototype.has = s, u.prototype.set = a, e.exports = u
         },
-        8407: (e, t, n) => {
-            var r = n(7040),
-                i = n(4125),
-                o = n(2117),
-                s = n(7518),
-                a = n(4705);
+        79: (e, t, n) => {
+            var r = n(3702),
+                i = n(80),
+                o = n(4739),
+                s = n(8655),
+                a = n(1175);
 
             function u(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.clear(); ++t < n;) {
                     var r = e[t];
                     this.set(r[0], r[1])
                 }
             }
             u.prototype.clear = r, u.prototype.delete = i, u.prototype.get = o, u.prototype.has = s, u.prototype.set = a, e.exports = u
         },
-        7071: (e, t, n) => {
-            var r = n(852)(n(5639), "Map");
+        8223: (e, t, n) => {
+            var r = n(6110)(n(9325), "Map");
             e.exports = r
         },
-        3369: (e, t, n) => {
-            var r = n(4785),
-                i = n(1285),
-                o = n(6e3),
-                s = n(9916),
-                a = n(5265);
+        3661: (e, t, n) => {
+            var r = n(3040),
+                i = n(7670),
+                o = n(289),
+                s = n(4509),
+                a = n(2949);
 
             function u(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.clear(); ++t < n;) {
                     var r = e[t];
                     this.set(r[0], r[1])
                 }
             }
             u.prototype.clear = r, u.prototype.delete = i, u.prototype.get = o, u.prototype.has = s, u.prototype.set = a, e.exports = u
         },
-        3818: (e, t, n) => {
-            var r = n(852)(n(5639), "Promise");
+        2804: (e, t, n) => {
+            var r = n(6110)(n(9325), "Promise");
             e.exports = r
         },
-        8525: (e, t, n) => {
-            var r = n(852)(n(5639), "Set");
+        6545: (e, t, n) => {
+            var r = n(6110)(n(9325), "Set");
             e.exports = r
         },
-        8668: (e, t, n) => {
-            var r = n(3369),
-                i = n(619),
-                o = n(2385);
+        8859: (e, t, n) => {
+            var r = n(3661),
+                i = n(1380),
+                o = n(1459);
 
             function s(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.__data__ = new r; ++t < n;) this.add(e[t])
             }
             s.prototype.add = s.prototype.push = i, s.prototype.has = o, e.exports = s
         },
-        6384: (e, t, n) => {
-            var r = n(8407),
-                i = n(7465),
-                o = n(3779),
-                s = n(7599),
-                a = n(4758),
-                u = n(4309);
+        7217: (e, t, n) => {
+            var r = n(79),
+                i = n(1420),
+                o = n(938),
+                s = n(3605),
+                a = n(9817),
+                u = n(945);
 
             function l(e) {
                 var t = this.__data__ = new r(e);
                 this.size = t.size
             }
             l.prototype.clear = i, l.prototype.delete = o, l.prototype.get = s, l.prototype.has = a, l.prototype.set = u, e.exports = l
         },
-        2705: (e, t, n) => {
-            var r = n(5639).Symbol;
+        1873: (e, t, n) => {
+            var r = n(9325).Symbol;
             e.exports = r
         },
-        1149: (e, t, n) => {
-            var r = n(5639).Uint8Array;
+        7828: (e, t, n) => {
+            var r = n(9325).Uint8Array;
             e.exports = r
         },
-        577: (e, t, n) => {
-            var r = n(852)(n(5639), "WeakMap");
+        8303: (e, t, n) => {
+            var r = n(6110)(n(9325), "WeakMap");
             e.exports = r
         },
-        4963: e => {
+        9770: e => {
             e.exports = function(e, t) {
                 for (var n = -1, r = null == e ? 0 : e.length, i = 0, o = []; ++n < r;) {
                     var s = e[n];
                     t(s, n, e) && (o[i++] = s)
                 }
                 return o
             }
         },
-        4636: (e, t, n) => {
-            var r = n(2545),
-                i = n(5694),
-                o = n(1469),
-                s = n(4144),
-                a = n(5776),
-                u = n(6719),
+        695: (e, t, n) => {
+            var r = n(8096),
+                i = n(2428),
+                o = n(6449),
+                s = n(3656),
+                a = n(361),
+                u = n(7167),
                 l = Object.prototype.hasOwnProperty;
             e.exports = function(e, t) {
                 var n = o(e),
                     c = !n && i(e),
                     f = !n && !c && s(e),
                     h = !n && !c && !f && u(e),
                     d = n || c || f || h,
                     p = d ? r(e.length, String) : [],
                     g = p.length;
                 for (var v in e) !t && !l.call(e, v) || d && ("length" == v || f && ("offset" == v || "parent" == v) || h && ("buffer" == v || "byteLength" == v || "byteOffset" == v) || a(v, g)) || p.push(v);
                 return p
             }
         },
-        2488: e => {
+        4528: e => {
             e.exports = function(e, t) {
                 for (var n = -1, r = t.length, i = e.length; ++n < r;) e[i + n] = t[n];
                 return e
             }
         },
-        2908: e => {
+        4248: e => {
             e.exports = function(e, t) {
                 for (var n = -1, r = null == e ? 0 : e.length; ++n < r;)
                     if (t(e[n], n, e)) return !0;
                 return !1
             }
         },
-        8470: (e, t, n) => {
-            var r = n(7813);
+        6025: (e, t, n) => {
+            var r = n(5288);
             e.exports = function(e, t) {
                 for (var n = e.length; n--;)
                     if (r(e[n][0], t)) return n;
                 return -1
             }
         },
-        8866: (e, t, n) => {
-            var r = n(2488),
-                i = n(1469);
+        2199: (e, t, n) => {
+            var r = n(4528),
+                i = n(6449);
             e.exports = function(e, t, n) {
                 var o = t(e);
                 return i(e) ? o : r(o, n(e))
             }
         },
-        4239: (e, t, n) => {
-            var r = n(2705),
-                i = n(9607),
-                o = n(2333),
+        2552: (e, t, n) => {
+            var r = n(1873),
+                i = n(659),
+                o = n(9350),
                 s = r ? r.toStringTag : void 0;
             e.exports = function(e) {
                 return null == e ? void 0 === e ? "[object Undefined]" : "[object Null]" : s && s in Object(e) ? i(e) : o(e)
             }
         },
-        9454: (e, t, n) => {
-            var r = n(4239),
-                i = n(7005);
+        7534: (e, t, n) => {
+            var r = n(2552),
+                i = n(346);
             e.exports = function(e) {
                 return i(e) && "[object Arguments]" == r(e)
             }
         },
-        939: (e, t, n) => {
-            var r = n(2492),
-                i = n(7005);
+        270: (e, t, n) => {
+            var r = n(7068),
+                i = n(346);
             e.exports = function e(t, n, o, s, a) {
                 return t === n || (null == t || null == n || !i(t) && !i(n) ? t != t && n != n : r(t, n, o, s, e, a))
             }
         },
-        2492: (e, t, n) => {
-            var r = n(6384),
-                i = n(7114),
-                o = n(8351),
-                s = n(6096),
-                a = n(4160),
-                u = n(1469),
-                l = n(4144),
-                c = n(6719),
+        7068: (e, t, n) => {
+            var r = n(7217),
+                i = n(5911),
+                o = n(1986),
+                s = n(689),
+                a = n(5861),
+                u = n(6449),
+                l = n(3656),
+                c = n(7167),
                 f = "[object Arguments]",
                 h = "[object Array]",
                 d = "[object Object]",
                 p = Object.prototype.hasOwnProperty;
             e.exports = function(e, t, n, g, v, m) {
                 var y = u(e),
                     b = u(t),
@@ -5263,75 +5263,75 @@
                             A = k ? t.value() : t;
                         return m || (m = new r), v(S, A, n, g, m)
                     }
                 }
                 return !!E && (m || (m = new r), s(e, t, n, g, v, m))
             }
         },
-        8458: (e, t, n) => {
-            var r = n(3560),
-                i = n(5346),
-                o = n(3218),
-                s = n(346),
+        5083: (e, t, n) => {
+            var r = n(1882),
+                i = n(7296),
+                o = n(3805),
+                s = n(7473),
                 a = /^\[object .+?Constructor\]$/,
                 u = Function.prototype,
                 l = Object.prototype,
                 c = u.toString,
                 f = l.hasOwnProperty,
                 h = RegExp("^" + c.call(f).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$");
             e.exports = function(e) {
                 return !(!o(e) || i(e)) && (r(e) ? h : a).test(s(e))
             }
         },
-        8749: (e, t, n) => {
-            var r = n(4239),
-                i = n(1780),
-                o = n(7005),
+        4901: (e, t, n) => {
+            var r = n(2552),
+                i = n(294),
+                o = n(346),
                 s = {};
             s["[object Float32Array]"] = s["[object Float64Array]"] = s["[object Int8Array]"] = s["[object Int16Array]"] = s["[object Int32Array]"] = s["[object Uint8Array]"] = s["[object Uint8ClampedArray]"] = s["[object Uint16Array]"] = s["[object Uint32Array]"] = !0, s["[object Arguments]"] = s["[object Array]"] = s["[object ArrayBuffer]"] = s["[object Boolean]"] = s["[object DataView]"] = s["[object Date]"] = s["[object Error]"] = s["[object Function]"] = s["[object Map]"] = s["[object Number]"] = s["[object Object]"] = s["[object RegExp]"] = s["[object Set]"] = s["[object String]"] = s["[object WeakMap]"] = !1, e.exports = function(e) {
                 return o(e) && i(e.length) && !!s[r(e)]
             }
         },
-        280: (e, t, n) => {
-            var r = n(5726),
-                i = n(6916),
+        8984: (e, t, n) => {
+            var r = n(5527),
+                i = n(3650),
                 o = Object.prototype.hasOwnProperty;
             e.exports = function(e) {
                 if (!r(e)) return i(e);
                 var t = [];
                 for (var n in Object(e)) o.call(e, n) && "constructor" != n && t.push(n);
                 return t
             }
         },
-        2545: e => {
+        8096: e => {
             e.exports = function(e, t) {
                 for (var n = -1, r = Array(e); ++n < e;) r[n] = t(n);
                 return r
             }
         },
-        1717: e => {
+        7301: e => {
             e.exports = function(e) {
                 return function(t) {
                     return e(t)
                 }
             }
         },
-        4757: e => {
+        9219: e => {
             e.exports = function(e, t) {
                 return e.has(t)
             }
         },
-        4429: (e, t, n) => {
-            var r = n(5639)["__core-js_shared__"];
+        5481: (e, t, n) => {
+            var r = n(9325)["__core-js_shared__"];
             e.exports = r
         },
-        7114: (e, t, n) => {
-            var r = n(8668),
-                i = n(2908),
-                o = n(4757);
+        5911: (e, t, n) => {
+            var r = n(8859),
+                i = n(4248),
+                o = n(9219);
             e.exports = function(e, t, n, s, a, u) {
                 var l = 1 & n,
                     c = e.length,
                     f = t.length;
                 if (c != f && !(l && f > c)) return !1;
                 var h = u.get(e),
                     d = u.get(t);
@@ -5359,21 +5359,21 @@
                         g = !1;
                         break
                     }
                 }
                 return u.delete(e), u.delete(t), g
             }
         },
-        8351: (e, t, n) => {
-            var r = n(2705),
-                i = n(1149),
-                o = n(7813),
-                s = n(7114),
-                a = n(8776),
-                u = n(1814),
+        1986: (e, t, n) => {
+            var r = n(1873),
+                i = n(7828),
+                o = n(5288),
+                s = n(5911),
+                a = n(317),
+                u = n(4247),
                 l = r ? r.prototype : void 0,
                 c = l ? l.valueOf : void 0;
             e.exports = function(e, t, n, r, l, f, h) {
                 switch (n) {
                     case "[object DataView]":
                         if (e.byteLength != t.byteLength || e.byteOffset != t.byteOffset) return !1;
                         e = e.buffer, t = t.buffer;
@@ -5400,16 +5400,16 @@
                         return h.delete(e), v;
                     case "[object Symbol]":
                         if (c) return c.call(e) == c.call(t)
                 }
                 return !1
             }
         },
-        6096: (e, t, n) => {
-            var r = n(8234),
+        689: (e, t, n) => {
+            var r = n(2),
                 i = Object.prototype.hasOwnProperty;
             e.exports = function(e, t, n, o, s, a) {
                 var u = 1 & n,
                     l = r(e),
                     c = l.length;
                 if (c != r(t).length && !u) return !1;
                 for (var f = c; f--;) {
@@ -5435,43 +5435,43 @@
                     var _ = e.constructor,
                         x = t.constructor;
                     _ == x || !("constructor" in e) || !("constructor" in t) || "function" == typeof _ && _ instanceof _ && "function" == typeof x && x instanceof x || (g = !1)
                 }
                 return a.delete(e), a.delete(t), g
             }
         },
-        1957: (e, t, n) => {
+        4840: (e, t, n) => {
             var r = "object" == typeof n.g && n.g && n.g.Object === Object && n.g;
             e.exports = r
         },
-        8234: (e, t, n) => {
-            var r = n(8866),
-                i = n(9551),
-                o = n(3674);
+        2: (e, t, n) => {
+            var r = n(2199),
+                i = n(4664),
+                o = n(5950);
             e.exports = function(e) {
                 return r(e, o, i)
             }
         },
-        5050: (e, t, n) => {
-            var r = n(7019);
+        2651: (e, t, n) => {
+            var r = n(4218);
             e.exports = function(e, t) {
                 var n = e.__data__;
                 return r(t) ? n["string" == typeof t ? "string" : "hash"] : n.map
             }
         },
-        852: (e, t, n) => {
-            var r = n(8458),
-                i = n(7801);
+        6110: (e, t, n) => {
+            var r = n(5083),
+                i = n(392);
             e.exports = function(e, t) {
                 var n = i(e, t);
                 return r(n) ? n : void 0
             }
         },
-        9607: (e, t, n) => {
-            var r = n(2705),
+        659: (e, t, n) => {
+            var r = n(1873),
                 i = Object.prototype,
                 o = i.hasOwnProperty,
                 s = i.toString,
                 a = r ? r.toStringTag : void 0;
             e.exports = function(e) {
                 var t = o.call(e, a),
                     n = e[a];
@@ -5479,34 +5479,34 @@
                     e[a] = void 0;
                     var r = !0
                 } catch (e) {}
                 var i = s.call(e);
                 return r && (t ? e[a] = n : delete e[a]), i
             }
         },
-        9551: (e, t, n) => {
-            var r = n(4963),
-                i = n(479),
+        4664: (e, t, n) => {
+            var r = n(9770),
+                i = n(3345),
                 o = Object.prototype.propertyIsEnumerable,
                 s = Object.getOwnPropertySymbols,
                 a = s ? function(e) {
                     return null == e ? [] : (e = Object(e), r(s(e), (function(t) {
                         return o.call(e, t)
                     })))
                 } : i;
             e.exports = a
         },
-        4160: (e, t, n) => {
-            var r = n(8552),
-                i = n(7071),
-                o = n(3818),
-                s = n(8525),
-                a = n(577),
-                u = n(4239),
-                l = n(346),
+        5861: (e, t, n) => {
+            var r = n(5580),
+                i = n(8223),
+                o = n(2804),
+                s = n(6545),
+                a = n(8303),
+                u = n(2552),
+                l = n(7473),
                 c = "[object Map]",
                 f = "[object Promise]",
                 h = "[object Set]",
                 d = "[object WeakMap]",
                 p = "[object DataView]",
                 g = l(r),
                 v = l(i),
@@ -5529,376 +5529,376 @@
                         return h;
                     case b:
                         return d
                 }
                 return t
             }), e.exports = _
         },
-        7801: e => {
+        392: e => {
             e.exports = function(e, t) {
                 return null == e ? void 0 : e[t]
             }
         },
-        1789: (e, t, n) => {
-            var r = n(4536);
+        2032: (e, t, n) => {
+            var r = n(1042);
             e.exports = function() {
                 this.__data__ = r ? r(null) : {}, this.size = 0
             }
         },
-        401: e => {
+        3862: e => {
             e.exports = function(e) {
                 var t = this.has(e) && delete this.__data__[e];
                 return this.size -= t ? 1 : 0, t
             }
         },
-        7667: (e, t, n) => {
-            var r = n(4536),
+        6721: (e, t, n) => {
+            var r = n(1042),
                 i = Object.prototype.hasOwnProperty;
             e.exports = function(e) {
                 var t = this.__data__;
                 if (r) {
                     var n = t[e];
                     return "__lodash_hash_undefined__" === n ? void 0 : n
                 }
                 return i.call(t, e) ? t[e] : void 0
             }
         },
-        1327: (e, t, n) => {
-            var r = n(4536),
+        2749: (e, t, n) => {
+            var r = n(1042),
                 i = Object.prototype.hasOwnProperty;
             e.exports = function(e) {
                 var t = this.__data__;
                 return r ? void 0 !== t[e] : i.call(t, e)
             }
         },
-        1866: (e, t, n) => {
-            var r = n(4536);
+        5749: (e, t, n) => {
+            var r = n(1042);
             e.exports = function(e, t) {
                 var n = this.__data__;
                 return this.size += this.has(e) ? 0 : 1, n[e] = r && void 0 === t ? "__lodash_hash_undefined__" : t, this
             }
         },
-        5776: e => {
+        361: e => {
             var t = /^(?:0|[1-9]\d*)$/;
             e.exports = function(e, n) {
                 var r = typeof e;
                 return !!(n = null == n ? 9007199254740991 : n) && ("number" == r || "symbol" != r && t.test(e)) && e > -1 && e % 1 == 0 && e < n
             }
         },
-        7019: e => {
+        4218: e => {
             e.exports = function(e) {
                 var t = typeof e;
                 return "string" == t || "number" == t || "symbol" == t || "boolean" == t ? "__proto__" !== e : null === e
             }
         },
-        5346: (e, t, n) => {
-            var r, i = n(4429),
+        7296: (e, t, n) => {
+            var r, i = n(5481),
                 o = (r = /[^.]+$/.exec(i && i.keys && i.keys.IE_PROTO || "")) ? "Symbol(src)_1." + r : "";
             e.exports = function(e) {
                 return !!o && o in e
             }
         },
-        5726: e => {
+        5527: e => {
             var t = Object.prototype;
             e.exports = function(e) {
                 var n = e && e.constructor;
                 return e === ("function" == typeof n && n.prototype || t)
             }
         },
-        7040: e => {
+        3702: e => {
             e.exports = function() {
                 this.__data__ = [], this.size = 0
             }
         },
-        4125: (e, t, n) => {
-            var r = n(8470),
+        80: (e, t, n) => {
+            var r = n(6025),
                 i = Array.prototype.splice;
             e.exports = function(e) {
                 var t = this.__data__,
                     n = r(t, e);
                 return !(n < 0 || (n == t.length - 1 ? t.pop() : i.call(t, n, 1), --this.size, 0))
             }
         },
-        2117: (e, t, n) => {
-            var r = n(8470);
+        4739: (e, t, n) => {
+            var r = n(6025);
             e.exports = function(e) {
                 var t = this.__data__,
                     n = r(t, e);
                 return n < 0 ? void 0 : t[n][1]
             }
         },
-        7518: (e, t, n) => {
-            var r = n(8470);
+        8655: (e, t, n) => {
+            var r = n(6025);
             e.exports = function(e) {
                 return r(this.__data__, e) > -1
             }
         },
-        4705: (e, t, n) => {
-            var r = n(8470);
+        1175: (e, t, n) => {
+            var r = n(6025);
             e.exports = function(e, t) {
                 var n = this.__data__,
                     i = r(n, e);
                 return i < 0 ? (++this.size, n.push([e, t])) : n[i][1] = t, this
             }
         },
-        4785: (e, t, n) => {
-            var r = n(1989),
-                i = n(8407),
-                o = n(7071);
+        3040: (e, t, n) => {
+            var r = n(1549),
+                i = n(79),
+                o = n(8223);
             e.exports = function() {
                 this.size = 0, this.__data__ = {
                     hash: new r,
                     map: new(o || i),
                     string: new r
                 }
             }
         },
-        1285: (e, t, n) => {
-            var r = n(5050);
+        7670: (e, t, n) => {
+            var r = n(2651);
             e.exports = function(e) {
                 var t = r(this, e).delete(e);
                 return this.size -= t ? 1 : 0, t
             }
         },
-        6e3: (e, t, n) => {
-            var r = n(5050);
+        289: (e, t, n) => {
+            var r = n(2651);
             e.exports = function(e) {
                 return r(this, e).get(e)
             }
         },
-        9916: (e, t, n) => {
-            var r = n(5050);
+        4509: (e, t, n) => {
+            var r = n(2651);
             e.exports = function(e) {
                 return r(this, e).has(e)
             }
         },
-        5265: (e, t, n) => {
-            var r = n(5050);
+        2949: (e, t, n) => {
+            var r = n(2651);
             e.exports = function(e, t) {
                 var n = r(this, e),
                     i = n.size;
                 return n.set(e, t), this.size += n.size == i ? 0 : 1, this
             }
         },
-        8776: e => {
+        317: e => {
             e.exports = function(e) {
                 var t = -1,
                     n = Array(e.size);
                 return e.forEach((function(e, r) {
                     n[++t] = [r, e]
                 })), n
             }
         },
-        4536: (e, t, n) => {
-            var r = n(852)(Object, "create");
+        1042: (e, t, n) => {
+            var r = n(6110)(Object, "create");
             e.exports = r
         },
-        6916: (e, t, n) => {
-            var r = n(5569)(Object.keys, Object);
+        3650: (e, t, n) => {
+            var r = n(4335)(Object.keys, Object);
             e.exports = r
         },
-        1167: (e, t, n) => {
+        6009: (e, t, n) => {
             e = n.nmd(e);
-            var r = n(1957),
+            var r = n(4840),
                 i = t && !t.nodeType && t,
                 o = i && e && !e.nodeType && e,
                 s = o && o.exports === i && r.process,
                 a = function() {
                     try {
                         return o && o.require && o.require("util").types || s && s.binding && s.binding("util")
                     } catch (e) {}
                 }();
             e.exports = a
         },
-        2333: e => {
+        9350: e => {
             var t = Object.prototype.toString;
             e.exports = function(e) {
                 return t.call(e)
             }
         },
-        5569: e => {
+        4335: e => {
             e.exports = function(e, t) {
                 return function(n) {
                     return e(t(n))
                 }
             }
         },
-        5639: (e, t, n) => {
-            var r = n(1957),
+        9325: (e, t, n) => {
+            var r = n(4840),
                 i = "object" == typeof self && self && self.Object === Object && self,
                 o = r || i || Function("return this")();
             e.exports = o
         },
-        619: e => {
+        1380: e => {
             e.exports = function(e) {
                 return this.__data__.set(e, "__lodash_hash_undefined__"), this
             }
         },
-        2385: e => {
+        1459: e => {
             e.exports = function(e) {
                 return this.__data__.has(e)
             }
         },
-        1814: e => {
+        4247: e => {
             e.exports = function(e) {
                 var t = -1,
                     n = Array(e.size);
                 return e.forEach((function(e) {
                     n[++t] = e
                 })), n
             }
         },
-        7465: (e, t, n) => {
-            var r = n(8407);
+        1420: (e, t, n) => {
+            var r = n(79);
             e.exports = function() {
                 this.__data__ = new r, this.size = 0
             }
         },
-        3779: e => {
+        938: e => {
             e.exports = function(e) {
                 var t = this.__data__,
                     n = t.delete(e);
                 return this.size = t.size, n
             }
         },
-        7599: e => {
+        3605: e => {
             e.exports = function(e) {
                 return this.__data__.get(e)
             }
         },
-        4758: e => {
+        9817: e => {
             e.exports = function(e) {
                 return this.__data__.has(e)
             }
         },
-        4309: (e, t, n) => {
-            var r = n(8407),
-                i = n(7071),
-                o = n(3369);
+        945: (e, t, n) => {
+            var r = n(79),
+                i = n(8223),
+                o = n(3661);
             e.exports = function(e, t) {
                 var n = this.__data__;
                 if (n instanceof r) {
                     var s = n.__data__;
                     if (!i || s.length < 199) return s.push([e, t]), this.size = ++n.size, this;
                     n = this.__data__ = new o(s)
                 }
                 return n.set(e, t), this.size = n.size, this
             }
         },
-        346: e => {
+        7473: e => {
             var t = Function.prototype.toString;
             e.exports = function(e) {
                 if (null != e) {
                     try {
                         return t.call(e)
                     } catch (e) {}
                     try {
                         return e + ""
                     } catch (e) {}
                 }
                 return ""
             }
         },
-        7813: e => {
+        5288: e => {
             e.exports = function(e, t) {
                 return e === t || e != e && t != t
             }
         },
-        5694: (e, t, n) => {
-            var r = n(9454),
-                i = n(7005),
+        2428: (e, t, n) => {
+            var r = n(7534),
+                i = n(346),
                 o = Object.prototype,
                 s = o.hasOwnProperty,
                 a = o.propertyIsEnumerable,
                 u = r(function() {
                     return arguments
                 }()) ? r : function(e) {
                     return i(e) && s.call(e, "callee") && !a.call(e, "callee")
                 };
             e.exports = u
         },
-        1469: e => {
+        6449: e => {
             var t = Array.isArray;
             e.exports = t
         },
-        8612: (e, t, n) => {
-            var r = n(3560),
-                i = n(1780);
+        4894: (e, t, n) => {
+            var r = n(1882),
+                i = n(294);
             e.exports = function(e) {
                 return null != e && i(e.length) && !r(e)
             }
         },
-        4144: (e, t, n) => {
+        3656: (e, t, n) => {
             e = n.nmd(e);
-            var r = n(5639),
-                i = n(5062),
+            var r = n(9325),
+                i = n(9935),
                 o = t && !t.nodeType && t,
                 s = o && e && !e.nodeType && e,
                 a = s && s.exports === o ? r.Buffer : void 0,
                 u = (a ? a.isBuffer : void 0) || i;
             e.exports = u
         },
-        8446: (e, t, n) => {
-            var r = n(939);
+        2404: (e, t, n) => {
+            var r = n(270);
             e.exports = function(e, t) {
                 return r(e, t)
             }
         },
-        3560: (e, t, n) => {
-            var r = n(4239),
-                i = n(3218);
+        1882: (e, t, n) => {
+            var r = n(2552),
+                i = n(3805);
             e.exports = function(e) {
                 if (!i(e)) return !1;
                 var t = r(e);
                 return "[object Function]" == t || "[object GeneratorFunction]" == t || "[object AsyncFunction]" == t || "[object Proxy]" == t
             }
         },
-        1780: e => {
+        294: e => {
             e.exports = function(e) {
                 return "number" == typeof e && e > -1 && e % 1 == 0 && e <= 9007199254740991
             }
         },
-        3218: e => {
+        3805: e => {
             e.exports = function(e) {
                 var t = typeof e;
                 return null != e && ("object" == t || "function" == t)
             }
         },
-        7005: e => {
+        346: e => {
             e.exports = function(e) {
                 return null != e && "object" == typeof e
             }
         },
-        6719: (e, t, n) => {
-            var r = n(8749),
-                i = n(1717),
-                o = n(1167),
+        7167: (e, t, n) => {
+            var r = n(4901),
+                i = n(7301),
+                o = n(6009),
                 s = o && o.isTypedArray,
                 a = s ? i(s) : r;
             e.exports = a
         },
-        3674: (e, t, n) => {
-            var r = n(4636),
-                i = n(280),
-                o = n(8612);
+        5950: (e, t, n) => {
+            var r = n(695),
+                i = n(8984),
+                o = n(4894);
             e.exports = function(e) {
                 return o(e) ? r(e) : i(e)
             }
         },
-        479: e => {
+        3345: e => {
             e.exports = function() {
                 return []
             }
         },
-        5062: e => {
+        9935: e => {
             e.exports = function() {
                 return !1
             }
         },
-        7794: (e, t, n) => {
+        884: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 VERSION: () => i,
                 after: () => Mt,
                 all: () => en,
                 allKeys: () => ve,
                 any: () => tn,
```

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/remoteEntry.e32a0a8e32155667dea0.js` & `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/remoteEntry.3cff93f6f99a3674a3dc.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, u, l, d, s, f, p, h, c, b, v, m, g, y = {
-            9815: (e, r, t) => {
+    var e, r, t, o, n, a, i, u, l, s, f, d, c, p, h, b, v, m, g, y, w = {
+            55: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(778), t.e(199)]).then((() => () => t(5199))),
-                        "./extension": () => Promise.all([t.e(778), t.e(199)]).then((() => () => t(5199))),
-                        "./style": () => t.e(747).then((() => () => t(9747)))
+                        "./index": () => Promise.all([t.e(534), t.e(824)]).then((() => () => t(9824))),
+                        "./extension": () => Promise.all([t.e(534), t.e(824)]).then((() => () => t(9824))),
+                        "./style": () => t.e(25).then((() => () => t(4025)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
                             var o = "default",
@@ -21,121 +21,121 @@
                     };
                 t.d(r, {
                     get: () => n,
                     init: () => a
                 })
             }
         },
-        w = {};
+        k = {};
 
-    function k(e) {
-        var r = w[e];
+    function j(e) {
+        var r = k[e];
         if (void 0 !== r) return r.exports;
-        var t = w[e] = {
+        var t = k[e] = {
             id: e,
             loaded: !1,
             exports: {}
         };
-        return y[e].call(t.exports, t, t.exports, k), t.loaded = !0, t.exports
+        return w[e].call(t.exports, t, t.exports, j), t.loaded = !0, t.exports
     }
-    k.m = y, k.c = w, k.n = e => {
+    j.m = w, j.c = k, j.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
-        return k.d(r, {
+        return j.d(r, {
             a: r
         }), r
-    }, k.d = (e, r) => {
-        for (var t in r) k.o(r, t) && !k.o(e, t) && Object.defineProperty(e, t, {
+    }, j.d = (e, r) => {
+        for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, k.f = {}, k.e = e => Promise.all(Object.keys(k.f).reduce(((r, t) => (k.f[t](e, r), r)), [])), k.u = e => e + "." + {
-        199: "e7fe4770dab71924b124",
-        474: "7bf61d2d7d2914369008",
-        747: "215e5b72fb89796bdb64",
-        778: "49cf2ea6508231610377",
-        790: "b027b82b72b7c2fb1ea7"
+    }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
+        7: "4b7742c84d4af5271005",
+        25: "a1f00326924633b92ed3",
+        534: "1b69f2ef59b1212f7f5f",
+        805: "5070eeb32117fc99ba19",
+        824: "ce3da0e5e0e81f9850cf"
     } [e] + ".js?v=" + {
-        199: "e7fe4770dab71924b124",
-        474: "7bf61d2d7d2914369008",
-        747: "215e5b72fb89796bdb64",
-        778: "49cf2ea6508231610377",
-        790: "b027b82b72b7c2fb1ea7"
-    } [e], k.g = function() {
+        7: "4b7742c84d4af5271005",
+        25: "a1f00326924633b92ed3",
+        534: "1b69f2ef59b1212f7f5f",
+        805: "5070eeb32117fc99ba19",
+        824: "ce3da0e5e0e81f9850cf"
+    } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), k.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@bokeh/jupyter_bokeh:", k.l = (t, o, n, a) => {
+    }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@bokeh/jupyter_bokeh:", j.l = (t, o, n, a) => {
         if (e[t]) e[t].push(o);
         else {
             var i, u;
             if (void 0 !== n)
-                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
-                    var s = l[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
-                        i = s;
+                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
+                    var f = l[s];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
-            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, k.nc && i.setAttribute("nonce", k.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var f = (r, o) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
+            var d = (r, o) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
-    }, k.r = e => {
+    }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
-    }, k.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
-        k.S = {};
+    }, j.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
+        j.S = {};
         var e = {},
             r = {};
-        k.I = (t, o) => {
+        j.I = (t, o) => {
             o || (o = []);
             var n = r[t];
             if (n || (n = r[t] = {}), !(o.indexOf(n) >= 0)) {
                 if (o.push(n), e[t]) return e[t];
-                k.o(k.S, t) || (k.S[t] = {});
-                var a = k.S[t],
+                j.o(j.S, t) || (j.S[t] = {});
+                var a = j.S[t],
                     i = "@bokeh/jupyter_bokeh",
                     u = (e, r, t, o) => {
                         var n = a[e] = a[e] || {},
                             u = n[r];
                         (!u || !u.loaded && (!o != !u.eager ? o : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     l = [];
-                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.0", (() => Promise.all([k.e(778), k.e(199)]).then((() => () => k(5199))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([k.e(790), k.e(474), k.e(778)]).then((() => () => k(3790)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.1", (() => Promise.all([j.e(534), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(534)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        k.g.importScripts && (e = k.g.location + "");
-        var r = k.g.document;
+        j.g.importScripts && (e = j.g.location + "");
+        var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var o = t.length - 1; o > -1 && !e;) e = t[o--].src
+                for (var o = t.length - 1; o > -1 && (!e || !/^http(s?):/.test(e));) e = t[o--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), k.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), j.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             o = t[1] ? r(t[1]) : [];
         return t[2] && (o.length++, o.push.apply(o, r(t[2]))), t[3] && (o.push([]), o.push.apply(o, r(t[3]))), o
     }, o = (e, r) => {
         e = t(e), r = t(r);
@@ -172,129 +172,132 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 n = o < 0;
             n && (o = -o - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > o && !n : "" == f != n);
-                if ("u" == s) {
-                    if (!l || "u" != f) return !1
+                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > o && !n : "" == d != n);
+                if ("u" == f) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (f == s)
+                    if (d == f)
                         if (u <= o) {
-                            if (d != e[u]) return !1
+                            if (s != e[u]) return !1
                         } else {
-                            if (n ? d > e[u] : d < e[u]) return !1;
-                            d != e[u] && (l = !1)
+                            if (n ? s > e[u] : s < e[u]) return !1;
+                            s != e[u] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != d && "n" != d) {
                     if (n || u <= o) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= o || s < f != n) return !1;
+                    if (u <= o || f < d != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
-        var p = [],
-            h = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
-            var c = e[i];
-            p.push(1 == c ? h() | h() : 2 == c ? h() & h() : c ? a(c, r) : !h())
+            var h = e[i];
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!h()
+        return !!p()
     }, i = (e, r) => {
-        var t = k.S[e];
-        if (!t || !k.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = j.S[e];
+        if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", d = (e, r, t, o) => {
+    }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", s = (e, r, t, o) => {
         var n = u(e, t);
-        return a(o, n) || f(l(e, t, n, o)), p(e[t][n])
-    }, s = (e, r, t) => {
+        return a(o, n) || d(l(e, t, n, o)), c(e[t][n])
+    }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, f = e => {
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), c = (h = e => function(r, t, o, n) {
-        var a = k.I(r);
-        return a && a.then ? a.then(e.bind(e, r, k.S[r], t, o, n)) : e(r, k.S[r], t, o, n)
-    })(((e, r, t, o) => (i(e, t), d(r, 0, t, o)))), b = h(((e, r, t, o, n) => {
-        var a = r && k.o(r, t) && s(r, t, o);
-        return a ? p(a) : n()
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, o, n) {
+        var a = j.I(r);
+        return a && a.then ? a.then(e.bind(e, r, j.S[r], t, o, n)) : e(r, j.S[r], t, o, n)
+    })(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), b = p(((e, r, t, o, n) => {
+        var a = r && j.o(r, t) && f(r, t, o);
+        return a ? c(a) : n()
     })), v = {}, m = {
-        8778: () => c("default", "@lumino/widgets", [1, 2, 0, 1]),
-        3826: () => b("default", "@jupyter-widgets/base", [, [1, 6],
+        1534: () => h("default", "@lumino/widgets", [1, 2, 0, 1]),
+        1803: () => b("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
-        ], (() => Promise.all([k.e(790), k.e(474)]).then((() => () => k(3790))))),
-        7717: () => c("default", "@lumino/disposable", [1, 2, 0, 0]),
-        5633: () => c("default", "@lumino/messaging", [1, 2, 0, 0]),
-        7930: () => c("default", "@lumino/coreutils", [1, 2, 0, 0])
+        ], (() => Promise.all([j.e(7), j.e(805)]).then((() => () => j(4007))))),
+        9012: () => h("default", "@lumino/disposable", [1, 2, 0, 0]),
+        6230: () => h("default", "@lumino/messaging", [1, 2, 0, 0]),
+        7262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0])
     }, g = {
-        199: [3826, 7717],
-        474: [5633, 7930],
-        778: [8778]
-    }, k.f.consumes = (e, r) => {
-        k.o(g, e) && g[e].forEach((e => {
-            if (k.o(v, e)) return r.push(v[e]);
-            var t = r => {
-                    v[e] = 0, k.m[e] = t => {
-                        delete k.c[e], t.exports = r()
+        534: [1534],
+        805: [6230, 7262],
+        824: [1803, 9012]
+    }, y = {}, j.f.consumes = (e, r) => {
+        j.o(g, e) && g[e].forEach((e => {
+            if (j.o(v, e)) return r.push(v[e]);
+            if (!y[e]) {
+                var t = r => {
+                    v[e] = 0, j.m[e] = t => {
+                        delete j.c[e], t.exports = r()
                     }
-                },
-                o = r => {
-                    delete v[e], k.m[e] = t => {
-                        throw delete k.c[e], r
+                };
+                y[e] = !0;
+                var o = r => {
+                    delete v[e], j.m[e] = t => {
+                        throw delete j.c[e], r
                     }
                 };
-            try {
-                var n = m[e]();
-                n.then ? r.push(v[e] = n.then(t).catch(o)) : t(n)
-            } catch (e) {
-                o(e)
+                try {
+                    var n = m[e]();
+                    n.then ? r.push(v[e] = n.then(t).catch(o)) : t(n)
+                } catch (e) {
+                    o(e)
+                }
             }
         }))
     }, (() => {
         var e = {
-            893: 0
+            332: 0
         };
-        k.f.j = (r, t) => {
-            var o = k.o(e, r) ? e[r] : void 0;
+        j.f.j = (r, t) => {
+            var o = j.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (/^(474|778)$/.test(r)) e[r] = 0;
+                else if (/^(534|805)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => o = e[r] = [t, n]));
                 t.push(o[2] = n);
-                var a = k.p + k.u(r),
+                var a = j.p + j.u(r),
                     i = new Error;
-                k.l(a, (t => {
-                    if (k.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
+                j.l(a, (t => {
+                    if (j.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
                             a = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + a + ")", i.name = "ChunkLoadError", i.type = n, i.request = a, o[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var o, n, [a, i, u] = t,
                     l = 0;
                 if (a.some((r => 0 !== e[r]))) {
-                    for (o in i) k.o(i, o) && (k.m[o] = i[o]);
-                    u && u(k)
+                    for (o in i) j.o(i, o) && (j.m[o] = i[o]);
+                    u && u(j)
                 }
-                for (r && r(t); l < a.length; l++) n = a[l], k.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); l < a.length; l++) n = a[l], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_bokeh_jupyter_bokeh = self.webpackChunk_bokeh_jupyter_bokeh || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), k.nc = void 0;
-    var j = k(9815);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@bokeh/jupyter_bokeh"] = j
+    })(), j.nc = void 0;
+    var S = j(55);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@bokeh/jupyter_bokeh"] = S
 })();
```

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/labextension/static/third-party-licenses.json` & `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428572%*

 * *Differences: {"'packages'": "{2: {'versionInfo': '6.10.0'}, 5: {'versionInfo': '3.3.4'}}"}*

```diff
@@ -12,15 +12,15 @@
             "name": "backbone",
             "versionInfo": "1.4.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "5.2.7"
+            "versionInfo": "6.10.0"
         },
         {
             "extractedText": "Copyright OpenJS Foundation and other contributors, https://openjsf.org/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "jquery",
             "versionInfo": "3.7.1"
         },
@@ -30,15 +30,15 @@
             "name": "lodash",
             "versionInfo": "4.17.21"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
-            "versionInfo": "2.0.0"
+            "versionInfo": "3.3.4"
         },
         {
             "extractedText": "Copyright (c) 2009-2022 Jeremy Ashkenas, Julian Gonggrijp, and DocumentCloud and Investigative Reporters & Editors\n\nPermission is hereby granted, free of charge, to any person\nobtaining a copy of this software and associated documentation\nfiles (the \"Software\"), to deal in the Software without\nrestriction, including without limitation the rights to use,\ncopy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the\nSoftware is furnished to do so, subject to the following\nconditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES\nOF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT\nHOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,\nWHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING\nFROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR\nOTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "underscore",
             "versionInfo": "1.13.6"
         }
```

### Comparing `jupyter_bokeh-4.0.0/jupyter_bokeh/nbextension/index.js.LICENSE.txt` & `jupyter_bokeh-4.0.1/jupyter_bokeh/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/src/manager.ts` & `jupyter_bokeh-4.0.1/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/src/plugin.ts` & `jupyter_bokeh-4.0.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/src/renderer.ts` & `jupyter_bokeh-4.0.1/src/renderer.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/src/widgets.ts` & `jupyter_bokeh-4.0.1/src/widgets.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/LICENSE.txt` & `jupyter_bokeh-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/README.md` & `jupyter_bokeh-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/pyproject.toml` & `jupyter_bokeh-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.0/PKG-INFO` & `jupyter_bokeh-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_bokeh
-Version: 4.0.0
+Version: 4.0.1
 Summary: A Jupyter extension for rendering Bokeh content.
 Project-URL: Homepage, https://github.com/bokeh/jupyter_bokeh
 Project-URL: Bug Tracker, https://github.com/bokeh/jupyter_bokeh/issues
 Project-URL: Repository, https://github.com/bokeh/jupyter_bokeh.git
 Author-email: Bokeh team <info@bokeh.org>
 License: Copyright (c) 2012 - 2020, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
```

