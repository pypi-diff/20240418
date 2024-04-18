# Comparing `tmp/dash_pager-0.0.1.tar.gz` & `tmp/dash_pager-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pager-0.0.1.tar", last modified: Thu Apr 18 00:57:58 2024, max compression
+gzip compressed data, was "dash_pager-0.1.0.tar", last modified: Thu Apr 18 01:12:12 2024, max compression
```

## Comparing `dash_pager-0.0.1.tar` & `dash_pager-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 00:57:58.680421 dash_pager-0.0.1/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1583 2024-04-18 00:53:59.000000 dash_pager-0.0.1/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.0.1/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3987 2024-04-18 00:57:58.680294 dash_pager-0.0.1/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3700 2024-04-18 00:53:59.000000 dash_pager-0.0.1/README.md
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 00:57:58.679477 dash_pager-0.0.1/dash_pager/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1656 2024-04-18 00:57:10.000000 dash_pager-0.0.1/dash_pager/Pager.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.0.1/dash_pager/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 00:57:10.000000 dash_pager-0.0.1/dash_pager/_imports_.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4257 2024-04-18 00:57:09.000000 dash_pager-0.0.1/dash_pager/async-Pager.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6645 2024-04-18 00:57:09.000000 dash_pager-0.0.1/dash_pager/async-Pager.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3894 2024-04-18 00:57:09.000000 dash_pager-0.0.1/dash_pager/dash_pager.min.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)    19088 2024-04-18 00:57:09.000000 dash_pager-0.0.1/dash_pager/dash_pager.min.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3060 2024-04-18 00:57:10.000000 dash_pager-0.0.1/dash_pager/metadata.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 00:57:10.000000 dash_pager-0.0.1/dash_pager/package-info.json
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 00:57:58.679967 dash_pager-0.0.1/dash_pager.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3987 2024-04-18 00:57:58.000000 dash_pager-0.0.1/dash_pager.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 00:57:58.000000 dash_pager-0.0.1/dash_pager.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 00:57:58.000000 dash_pager-0.0.1/dash_pager.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 00:57:58.000000 dash_pager-0.0.1/dash_pager.egg-info/top_level.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 00:53:59.000000 dash_pager-0.0.1/package.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 00:57:58.680458 dash_pager-0.0.1/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.0.1/setup.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 00:57:58.680102 dash_pager-0.0.1/tests/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.0.1/tests/test_usage.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.252372 dash_pager-0.1.0/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.0/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.0/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 01:12:12.252212 dash_pager-0.1.0/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.0/README.md
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.251256 dash_pager-0.1.0/dash_pager/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1656 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/Pager.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.0/dash_pager/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/_imports_.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4257 2024-04-18 00:57:09.000000 dash_pager-0.1.0/dash_pager/async-Pager.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     6645 2024-04-18 00:57:09.000000 dash_pager-0.1.0/dash_pager/async-Pager.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3894 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/dash_pager.min.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    19088 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/dash_pager.min.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3060 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/metadata.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/package-info.json
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.251766 dash_pager-0.1.0/dash_pager.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/top_level.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 01:11:56.000000 dash_pager-0.1.0/package.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 01:12:12.252423 dash_pager-0.1.0/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.0/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.251903 dash_pager-0.1.0/tests/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.0/tests/test_usage.py
```

### Comparing `dash_pager-0.0.1/PKG-INFO` & `dash_pager-0.1.0/dash_pager.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 Metadata-Version: 2.1
-Name: dash_pager
-Version: 0.0.1
+Name: dash-pager
+Version: 0.1.0
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dash-pager
 
 dash-pager is a Dash component library.
 
-Generic pagination component for dash and dash bootstrap components
+Generic pagination component for dash and dash bootstrap components. 
+
+The component is a selector for an interval of values.
+
+![Screenshot](./Screenshot.png)
+
+Example usage (add to a dash layout):
+
+    import dash_pager
+    
+    dash_pager.Pager(
+        id='input',
+        value=[1,10],
+        maxValue=10,
+    )
+
 
 Get started with:
 1. Install Dash and its dependencies: https://dash.plotly.com/installation
 2. Run `python usage.py`
 3. Visit http://localhost:8050 in your web browser
 
+
+
 ## Contributing
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md)
 
 ### Install dependencies
 
 If you have selected install_dependencies during the prompt, you can skip this part.
```

### Comparing `dash_pager-0.0.1/README.md` & `dash_pager-0.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,35 @@
 # dash-pager
 
 dash-pager is a Dash component library.
 
-Generic pagination component for dash and dash bootstrap components
+Generic pagination component for dash and dash bootstrap components. 
+
+The component is a selector for an interval of values.
+
+![Screenshot](./Screenshot.png)
+
+Example usage (add to a dash layout):
+
+    import dash_pager
+    
+    dash_pager.Pager(
+        id='input',
+        value=[1,10],
+        maxValue=10,
+    )
+
 
 Get started with:
 1. Install Dash and its dependencies: https://dash.plotly.com/installation
 2. Run `python usage.py`
 3. Visit http://localhost:8050 in your web browser
 
+
+
 ## Contributing
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md)
 
 ### Install dependencies
 
 If you have selected install_dependencies during the prompt, you can skip this part.
```

### Comparing `dash_pager-0.0.1/dash_pager/Pager.py` & `dash_pager-0.1.0/dash_pager/Pager.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.0.1/dash_pager/__init__.py` & `dash_pager-0.1.0/dash_pager/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.0.1/dash_pager/async-Pager.js` & `dash_pager-0.1.0/dash_pager/async-Pager.js`

 * *Files identical despite different names*

### Comparing `dash_pager-0.0.1/dash_pager/async-Pager.js.map` & `dash_pager-0.1.0/dash_pager/async-Pager.js.map`

 * *Files identical despite different names*

### Comparing `dash_pager-0.0.1/dash_pager/dash_pager.min.js` & `dash_pager-0.1.0/dash_pager/dash_pager.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -95,15 +95,15 @@
         var s = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var r, t = (r = i(), /\/_dash-component-suites\//.test(r.src)),
                 n = s(e);
             if (!t) return n;
             var o = n.split("/"),
                 a = o.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_1m1713401829"), o.splice(-1, 1, a.join(".")), o.join("/")
+            return a.splice(1, 0, "v0_1_0m1713402728"), o.splice(-1, 1, a.join(".")), o.join("/")
         }
     }(() => {
         var e = {
             792: 0
         };
         o.f.j = (r, t) => {
             var n = o.o(e, r) ? e[r] : void 0;
```

### Comparing `dash_pager-0.0.1/dash_pager/dash_pager.min.js.map` & `dash_pager-0.1.0/dash_pager/dash_pager.min.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915966386554622%*

 * *Differences: {"'sourcesContent'": "{insert: [(12, 'var getCurrentScript = function() {\\n    var script = "*

 * *                     'document.currentScript;\\n    if (!script) {\\n        /* Shim for IE11 and '*

 * *                     'below */\\n        /* Do not take into account async scripts and inline '*

 * *                     'scripts */\\n\\n        var doc_scripts = '*

 * *                     "document.getElementsByTagName(\\'script\\');\\n        var scripts = "*

 * *                     '[];\\n\\n        for (var i = 0; i < doc […]*

```diff
@@ -171,14 +171,14 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + \"async-Pager\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_0_1m1713401829\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_0m1713402728\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t792: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_pager\"] = self[\"webpackChunkdash_pager\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "export const Pager = React.lazy(() => import(/* webpackChunkName: \"Pager\" */ './fragments/Pager.react'));",
         "import React from 'react';\nimport PropTypes from 'prop-types';\nimport { Pager as RealComponent } from '../LazyLoader';\n\n/**\n * ExampleComponent is an example component.\n * It takes a property, `label`, and\n * displays it.\n * It renders an input with the property `value`\n * which is editable by the user.\n */\nconst Pager = (props) => {\n    return (\n        <React.Suspense fallback={null}>\n            <RealComponent {...props}/>\n        </React.Suspense>\n    );\n};\n\nPager.defaultProps = {\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * A label that will be printed when this component is rendered.\n     */\n    maxValue: PropTypes.number.isRequired,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n\nexport default Pager;\n\nexport const defaultProps = Pager.defaultProps;\nexport const propTypes = Pager.propTypes;\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.0.1/dash_pager/metadata.json` & `dash_pager-0.1.0/dash_pager/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_pager-0.0.1/dash_pager/package-info.json` & `dash_pager-0.1.0/dash_pager/package-info.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.1.0"
 }
```

### Comparing `dash_pager-0.0.1/dash_pager.egg-info/PKG-INFO` & `dash_pager-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,45 @@
 Metadata-Version: 2.1
-Name: dash-pager
-Version: 0.0.1
+Name: dash_pager
+Version: 0.1.0
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dash-pager
 
 dash-pager is a Dash component library.
 
-Generic pagination component for dash and dash bootstrap components
+Generic pagination component for dash and dash bootstrap components. 
+
+The component is a selector for an interval of values.
+
+![Screenshot](./Screenshot.png)
+
+Example usage (add to a dash layout):
+
+    import dash_pager
+    
+    dash_pager.Pager(
+        id='input',
+        value=[1,10],
+        maxValue=10,
+    )
+
 
 Get started with:
 1. Install Dash and its dependencies: https://dash.plotly.com/installation
 2. Run `python usage.py`
 3. Visit http://localhost:8050 in your web browser
 
+
+
 ## Contributing
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md)
 
 ### Install dependencies
 
 If you have selected install_dependencies during the prompt, you can skip this part.
```

### Comparing `dash_pager-0.0.1/package.json` & `dash_pager-0.1.0/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.1"
+    "version": "0.1.0"
 }
```

### Comparing `dash_pager-0.0.1/setup.py` & `dash_pager-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.0.1/tests/test_usage.py` & `dash_pager-0.1.0/tests/test_usage.py`

 * *Files identical despite different names*

