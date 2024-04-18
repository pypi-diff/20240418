# Comparing `tmp/jupyter_bokeh-4.0.1.tar.gz` & `tmp/jupyter_bokeh-4.0.2.tar.gz`

## Comparing `jupyter_bokeh-4.0.1.tar` & `jupyter_bokeh-4.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.eslintignore
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.eslintrc.js
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.yarnrc.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/DEVGUIDE.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/MANIFEST.in
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/install.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh.json
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/package.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/setup.cfg
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/setup.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/tsconfig.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/webpack.config.js
--rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/yarn.lock
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/conda.recipe/meta.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/jupyter_interactors.ipynb
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/jupyter_sliders.ipynb
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/jupyter_widgets.ipynb
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/notebook_comms.ipynb
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/server_embed.ipynb
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/examples/static_plot.ipynb
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/_version.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/widgets.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/package.json
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
--rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/7.4b7742c84d4af5271005.js
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/7.4b7742c84d4af5271005.js.LICENSE.txt
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/824.ce3da0e5e0e81f9850cf.js
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/remoteEntry.3cff93f6f99a3674a3dc.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/style.js
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/nbextension/extension.js
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/jupyter_bokeh/nbextension/index.js.LICENSE.txt
--rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/scripts/deploy.sh
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/extension.ts
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/index.ts
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/manager.ts
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/metadata.d.ts
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/plugin.ts
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/renderer.ts
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/src/widgets.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/style/index.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/LICENSE.txt
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/README.md
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/pyproject.toml
--rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/.eslintignore
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/.eslintrc.js
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/.yarnrc.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/DEVGUIDE.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/MANIFEST.in
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/install.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh.json
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/package.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/setup.cfg
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/setup.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/tsconfig.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/webpack.config.js
+-rw-r--r--   0        0        0   202074 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/yarn.lock
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/examples/jupyter_interactors.ipynb
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/examples/jupyter_sliders.ipynb
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/examples/jupyter_widgets.ipynb
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/examples/notebook_comms.ipynb
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/examples/server_embed.ipynb
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/examples/static_plot.ipynb
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/_version.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/widgets.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/package.json
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js
+-rw-r--r--   0        0        0   171237 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js.LICENSE.txt
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/824.b5bbd9637d89cdd5d973.js
+-rw-r--r--   0        0        0     7455 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/remoteEntry.b9eab9ac067c8b2f22e3.js
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/style.js
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/nbextension/extension.js
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/jupyter_bokeh/nbextension/index.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/scripts/deploy.sh
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/extension.ts
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/index.ts
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/manager.ts
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/metadata.d.ts
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/plugin.ts
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/renderer.ts
+-rw-r--r--   0        0        0     6649 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/src/widgets.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/style/index.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/README.md
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7119 2020-02-02 00:00:00.000000 jupyter_bokeh-4.0.2/PKG-INFO
```

### Comparing `jupyter_bokeh-4.0.1/.eslintrc.js` & `jupyter_bokeh-4.0.2/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/package.json` & `jupyter_bokeh-4.0.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'4.0.2'"}*

```diff
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.1"
+    "version": "4.0.2"
 }
```

### Comparing `jupyter_bokeh-4.0.1/tsconfig.json` & `jupyter_bokeh-4.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/webpack.config.js` & `jupyter_bokeh-4.0.2/webpack.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/yarn.lock` & `jupyter_bokeh-4.0.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/conda.recipe/meta.yaml` & `jupyter_bokeh-4.0.2/conda.recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/examples/jupyter_interactors.ipynb` & `jupyter_bokeh-4.0.2/examples/jupyter_interactors.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/examples/jupyter_sliders.ipynb` & `jupyter_bokeh-4.0.2/examples/jupyter_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/examples/jupyter_widgets.ipynb` & `jupyter_bokeh-4.0.2/examples/jupyter_widgets.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/examples/notebook_comms.ipynb` & `jupyter_bokeh-4.0.2/examples/notebook_comms.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/examples/server_embed.ipynb` & `jupyter_bokeh-4.0.2/examples/server_embed.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/examples/static_plot.ipynb` & `jupyter_bokeh-4.0.2/examples/static_plot.ipynb`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/__init__.py` & `jupyter_bokeh-4.0.2/jupyter_bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/widgets.py` & `jupyter_bokeh-4.0.2/jupyter_bokeh/widgets.py`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/package.json` & `jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9755291005291005%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b9eab9ac067c8b2f22e3.js'}}",*

 * * "'version'": "'4.0.2'"}*

```diff
@@ -36,15 +36,15 @@
         "{dist,lib}/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/bokeh/jupyter_bokeh",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3cff93f6f99a3674a3dc.js",
+            "load": "static/remoteEntry.b9eab9ac067c8b2f22e3.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_bokeh/labextension"
     },
     "keywords": [
         "jupyter",
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "4.0.1"
+    "version": "4.0.2"
 }
```

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js` & `jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/25.a1f00326924633b92ed3.js`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/7.4b7742c84d4af5271005.js` & `jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/7.2d4b977066efef2921dc.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 7.4b7742c84d4af5271005.js.LICENSE.txt */
+/*! For license information please see 7.2d4b977066efef2921dc.js.LICENSE.txt */
 (self.webpackChunk_bokeh_jupyter_bokeh = self.webpackChunk_bokeh_jupyter_bokeh || []).push([
     [7], {
         4007: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 BROKEN_FILE_SVG_ICON: () => v,
                 DOMWidgetModel: () => D,
@@ -217,15 +217,15 @@
                         }
                         this._domEvents.length = 0
                     }
                     return this
                 }
             }
             var E = n(6230),
-                T = n(1534);
+                T = n(5256);
             const k = "2.0.0",
                 S = "2.1.0",
                 A = "IPY_MODEL_";
 
             function C(e, t) {
                 if (Array.isArray(e)) {
                     const n = [];
```

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/824.ce3da0e5e0e81f9850cf.js` & `jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/824.b5bbd9637d89cdd5d973.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -20,15 +20,15 @@
                 get isDisposed() {
                     return null == this._context
                 }
                 dispose() {
                     this.isDisposed || (this._context = null)
                 }
             }
-            var r = s(1534);
+            var r = s(5256);
             const d = "application/vnd.bokehjs_load.v0+json",
                 c = "application/vnd.bokehjs_exec.v0+json";
             class l extends r.Widget {
                 constructor(e) {
                     super(), this._load_mimetype = d, this._script_element = document.createElement("script")
                 }
                 renderModel(e) {
@@ -167,16 +167,20 @@
                 _send(e) {
                     !this._idle && this._combine && this.model.get("combine_events") ? this._msgs = this._combine_events(e) : (this._idle = !1, this.send(e))
                 }
                 _change_event(e) {
                     if (this._blocked) return;
                     const {
                         Serializer: t
-                    } = m("core/serialization"), s = (new t).encode(e);
-                    s.event = "jsevent", this._send(s)
+                    } = m("core/serialization"), s = new Map;
+                    for (const t of e.document._all_models.values()) s.set(t, t.ref());
+                    const n = new t({
+                        references: s
+                    }).encode(e);
+                    n.event = "jsevent", this._send(n)
                 }
                 _consume_patch(e, t) {
                     if (null != this._document && "patch" == e.msg) {
                         const {
                             payload: s
                         } = e;
                         this._receiver.consume(null != s ? s : t[0].buffer);
@@ -223,12 +227,12 @@
                 },
                 autoStart: !0
             }
         },
         2288: (e, t) => {
             Object.assign(t, {
                 name: "@bokeh/jupyter_bokeh",
-                version: "4.0.1"
+                version: "4.0.2"
             })
         }
     }
 ]);
```

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/remoteEntry.3cff93f6f99a3674a3dc.js` & `jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/remoteEntry.b9eab9ac067c8b2f22e3.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, o, n, a, i, u, l, s, f, d, c, p, h, b, v, m, g, y, w = {
+    var e, r, t, o, n, a, i, u, l, d, s, f, c, p, h, b, v, m, g, y, w = {
             55: (e, r, t) => {
                 var o = {
-                        "./index": () => Promise.all([t.e(534), t.e(824)]).then((() => () => t(9824))),
-                        "./extension": () => Promise.all([t.e(534), t.e(824)]).then((() => () => t(9824))),
+                        "./index": () => Promise.all([t.e(256), t.e(824)]).then((() => () => t(9824))),
+                        "./extension": () => Promise.all([t.e(256), t.e(824)]).then((() => () => t(9824))),
                         "./style": () => t.e(25).then((() => () => t(4025)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(o, e) ? o[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -44,55 +44,55 @@
         }), r
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
-        7: "4b7742c84d4af5271005",
+        7: "2d4b977066efef2921dc",
         25: "a1f00326924633b92ed3",
-        534: "1b69f2ef59b1212f7f5f",
+        256: "3673b9e8accbe04f1c8a",
         805: "5070eeb32117fc99ba19",
-        824: "ce3da0e5e0e81f9850cf"
+        824: "b5bbd9637d89cdd5d973"
     } [e] + ".js?v=" + {
-        7: "4b7742c84d4af5271005",
+        7: "2d4b977066efef2921dc",
         25: "a1f00326924633b92ed3",
-        534: "1b69f2ef59b1212f7f5f",
+        256: "3673b9e8accbe04f1c8a",
         805: "5070eeb32117fc99ba19",
-        824: "ce3da0e5e0e81f9850cf"
+        824: "b5bbd9637d89cdd5d973"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@bokeh/jupyter_bokeh:", j.l = (t, o, n, a) => {
         if (e[t]) e[t].push(o);
         else {
             var i, u;
             if (void 0 !== n)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var s = l[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [o];
-            var d = (r, o) => {
+            var f = (r, o) => {
                     i.onerror = i.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(o))), r) return r(o)
                 },
-                c = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -114,15 +114,15 @@
                         (!u || !u.loaded && (!o != !u.eager ? o : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!o
                         })
                     },
                     l = [];
-                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.1", (() => Promise.all([j.e(534), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(534)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@bokeh/jupyter_bokeh", "4.0.2", (() => Promise.all([j.e(256), j.e(824)]).then((() => () => j(9824))))), u("@jupyter-widgets/base", "6.0.7", (() => Promise.all([j.e(7), j.e(805), j.e(256)]).then((() => () => j(4007)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -172,33 +172,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var o = e[0],
                 n = o < 0;
             n && (o = -o - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > o && !n : "" == d != n);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > o && !n : "" == f != n);
+                if ("u" == s) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == f)
+                    if (f == s)
                         if (u <= o) {
-                            if (s != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (n ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (n ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (n || u <= o) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= o || f < d != n) return !1;
+                    if (u <= o || s < f != n) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
@@ -207,41 +207,41 @@
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && o(e, r) ? r : e), 0)
-    }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", s = (e, r, t, o) => {
+    }, l = (e, r, t, o) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(o) + ")", d = (e, r, t, o) => {
         var n = u(e, t);
-        return a(o, n) || d(l(e, t, n, o)), c(e[t][n])
-    }, f = (e, r, t) => {
+        return a(o, n) || f(l(e, t, n, o)), c(e[t][n])
+    }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !a(t, r) || e && !o(e, r) ? e : r), 0)) && n[r]
-    }, d = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, o, n) {
         var a = j.I(r);
         return a && a.then ? a.then(e.bind(e, r, j.S[r], t, o, n)) : e(r, j.S[r], t, o, n)
-    })(((e, r, t, o) => (i(e, t), s(r, 0, t, o)))), b = p(((e, r, t, o, n) => {
-        var a = r && j.o(r, t) && f(r, t, o);
+    })(((e, r, t, o) => (i(e, t), d(r, 0, t, o)))), b = p(((e, r, t, o, n) => {
+        var a = r && j.o(r, t) && s(r, t, o);
         return a ? c(a) : n()
     })), v = {}, m = {
-        1534: () => h("default", "@lumino/widgets", [1, 2, 0, 1]),
+        5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         1803: () => b("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ], (() => Promise.all([j.e(7), j.e(805)]).then((() => () => j(4007))))),
         9012: () => h("default", "@lumino/disposable", [1, 2, 0, 0]),
         6230: () => h("default", "@lumino/messaging", [1, 2, 0, 0]),
         7262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0])
     }, g = {
-        534: [1534],
+        256: [5256],
         805: [6230, 7262],
         824: [1803, 9012]
     }, y = {}, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(v, e)) return r.push(v[e]);
             if (!y[e]) {
                 var t = r => {
@@ -267,15 +267,15 @@
         var e = {
             332: 0
         };
         j.f.j = (r, t) => {
             var o = j.o(e, r) ? e[r] : void 0;
             if (0 !== o)
                 if (o) t.push(o[2]);
-                else if (/^(534|805)$/.test(r)) e[r] = 0;
+                else if (/^(256|805)$/.test(r)) e[r] = 0;
             else {
                 var n = new Promise(((t, n) => o = e[r] = [t, n]));
                 t.push(o[2] = n);
                 var a = j.p + j.u(r),
                     i = new Error;
                 j.l(a, (t => {
                     if (j.o(e, r) && (0 !== (o = e[r]) && (e[r] = void 0), o)) {
```

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/labextension/static/third-party-licenses.json` & `jupyter_bokeh-4.0.2/jupyter_bokeh/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/jupyter_bokeh/nbextension/index.js.LICENSE.txt` & `jupyter_bokeh-4.0.2/jupyter_bokeh/nbextension/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/src/manager.ts` & `jupyter_bokeh-4.0.2/src/manager.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/src/plugin.ts` & `jupyter_bokeh-4.0.2/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/src/renderer.ts` & `jupyter_bokeh-4.0.2/src/renderer.ts`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/src/widgets.ts` & `jupyter_bokeh-4.0.2/src/widgets.ts`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 type DocsJson = any
 type RenderItem = any
 type Document = any
 type DocumentChangedEvent = any
 type Receiver = any
 type Fragment = any
+type HasProps = any
+type Ref = any
 
 const { keys, values } = Object
 
 const version_range = `^${version}`
 
 export type RenderBundle = {
   docs_json: DocsJson
@@ -195,15 +197,19 @@
   }
 
   protected _change_event(event: DocumentChangedEvent): void {
     if (this._blocked) {
       return
     }
     const { Serializer } = bk_require('core/serialization')
-    const serializer = new Serializer()
+    const references: Map<HasProps, Ref> = new Map()
+    for (const model of event.document._all_models.values()) {
+      references.set(model, model.ref())
+    }
+    const serializer = new Serializer({references})
     const event_rep = serializer.encode(event)
     event_rep.event = 'jsevent'
     this._send(event_rep)
   }
 
   protected _consume_patch(
     content: { msg: 'patch'; payload?: Fragment },
```

### Comparing `jupyter_bokeh-4.0.1/LICENSE.txt` & `jupyter_bokeh-4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/README.md` & `jupyter_bokeh-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/pyproject.toml` & `jupyter_bokeh-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_bokeh-4.0.1/PKG-INFO` & `jupyter_bokeh-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_bokeh
-Version: 4.0.1
+Version: 4.0.2
 Summary: A Jupyter extension for rendering Bokeh content.
 Project-URL: Homepage, https://github.com/bokeh/jupyter_bokeh
 Project-URL: Bug Tracker, https://github.com/bokeh/jupyter_bokeh/issues
 Project-URL: Repository, https://github.com/bokeh/jupyter_bokeh.git
 Author-email: Bokeh team <info@bokeh.org>
 License: Copyright (c) 2012 - 2020, Anaconda, Inc., and Bokeh Contributors
         All rights reserved.
```

