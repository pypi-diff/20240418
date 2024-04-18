# Comparing `tmp/dash_pager-0.1.1.tar.gz` & `tmp/dash_pager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pager-0.1.1.tar", last modified: Thu Apr 18 02:09:03 2024, max compression
+gzip compressed data, was "dash_pager-0.1.2.tar", last modified: Thu Apr 18 02:24:44 2024, max compression
```

## Comparing `dash_pager-0.1.1.tar` & `dash_pager-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.597528 dash_pager-0.1.1/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.1/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.1/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 02:09:03.597386 dash_pager-0.1.1/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.1/README.md
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.596378 dash_pager-0.1.1/dash_pager/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1802 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/Pager.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.1/dash_pager/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/_imports_.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4561 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/async-Pager.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)     7964 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/async-Pager.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3925 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/dash_pager.min.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)    19262 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/dash_pager.min.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3622 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/metadata.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/package-info.json
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.596896 dash_pager-0.1.1/dash_pager.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/top_level.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 02:08:25.000000 dash_pager-0.1.1/package.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 02:09:03.597569 dash_pager-0.1.1/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.1/setup.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.597037 dash_pager-0.1.1/tests/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.1/tests/test_usage.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:24:44.596360 dash_pager-0.1.2/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.2/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.2/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 02:24:44.596201 dash_pager-0.1.2/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.2/README.md
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:24:44.595024 dash_pager-0.1.2/dash_pager/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1802 2024-04-18 02:24:38.000000 dash_pager-0.1.2/dash_pager/Pager.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.2/dash_pager/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 02:24:38.000000 dash_pager-0.1.2/dash_pager/_imports_.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4581 2024-04-18 02:22:52.000000 dash_pager-0.1.2/dash_pager/async-Pager.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     8072 2024-04-18 02:22:52.000000 dash_pager-0.1.2/dash_pager/async-Pager.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3925 2024-04-18 02:24:37.000000 dash_pager-0.1.2/dash_pager/dash_pager.min.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    19262 2024-04-18 02:24:37.000000 dash_pager-0.1.2/dash_pager/dash_pager.min.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3622 2024-04-18 02:24:38.000000 dash_pager-0.1.2/dash_pager/metadata.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 02:24:38.000000 dash_pager-0.1.2/dash_pager/package-info.json
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:24:44.595736 dash_pager-0.1.2/dash_pager.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 02:24:44.000000 dash_pager-0.1.2/dash_pager.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 02:24:44.000000 dash_pager-0.1.2/dash_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 02:24:44.000000 dash_pager-0.1.2/dash_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 02:24:44.000000 dash_pager-0.1.2/dash_pager.egg-info/top_level.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 02:22:47.000000 dash_pager-0.1.2/package.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 02:24:44.596445 dash_pager-0.1.2/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.2/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:24:44.595870 dash_pager-0.1.2/tests/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.2/tests/test_usage.py
```

### Comparing `dash_pager-0.1.1/LICENSE` & `dash_pager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.1/PKG-INFO` & `dash_pager-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_pager
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_pager-0.1.1/README.md` & `dash_pager-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.1/dash_pager/Pager.py` & `dash_pager-0.1.2/dash_pager/Pager.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.1/dash_pager/__init__.py` & `dash_pager-0.1.2/dash_pager/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.1/dash_pager/async-Pager.js` & `dash_pager-0.1.2/dash_pager/async-Pager.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -143,15 +143,15 @@
                                 })
                             },
                             type: "number",
                             style: {
                                 width: "10ch",
                                 display: "inline"
                             },
-                            className: "form-control" + (c != n[0] ? " is-invalid" : "")
+                            className: "form-control" + (c != n[0] || c < i || c > s ? " is-invalid" : "")
                         }), o().createElement("span", {
                             className: "me-2"
                         }, " to "), o().createElement("input", {
                             id: t + "-ip-to",
                             value: s,
                             onChange: function(e) {
                                 return u({
@@ -159,15 +159,15 @@
                                 })
                             },
                             type: "number",
                             style: {
                                 width: "10ch",
                                 display: "inline"
                             },
-                            className: "form-control" + (s != n[1] ? " is-invalid" : "")
+                            className: "form-control" + (s != n[1] || s > r || s < c ? " is-invalid" : "")
                         }), o().createElement("span", {
                             className: "me-2"
                         }, " of ", r, " "), o().createElement("button", {
                             id: t + "-p",
                             className: "btn btn-outline-primary me-2",
                             type: "button",
                             onClick: function(e) {
```

### Comparing `dash_pager-0.1.1/dash_pager/async-Pager.js.map` & `dash_pager-0.1.2/dash_pager/async-Pager.js.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'mappings'": "'2mDAGA,IAGqBA,EAAK,SAAAC,GAAA,SAAAD,IAAA,O,4FAAAE,CAAA,KAAAF,GAAAG,EAAA,KAAAH,EAAAI,UAAA,Q,qRAAAC,CAAAL,EAAAC,G,EAAAD,G,EAAA,EAAAM,IAAA,SAAAC,MACtB,WACI,IAAAC,EAAoEC,KAAKC,MAAlEC,EAAEH,EAAFG,GAAIJ,EAAKC,EAALD,MAAOK,EAAQJ,EAARI,SAAUC,EAAQL,EAARK,SAAUC,EAAON,EAAPM,QAASC,EAAOP,EAAPO,QAASC,EAAQR,EAARQ,SAEpDC,EAAOV,EAAM,GACbW,EAAOX,EAAM,GA2BjB,OAzBIQ,IACgB,OAAZA,EACAE,EAAOJ,EACY,MAAZE,EACPE,GAAY,EACO,OAAZF,EACPG,EAAKN,EACc,MAAZG,EACPG,GAAQ,EACDH,EAAQI,WAAW,MAC1BC,MAAOH,EAAOI,SAASN,EAAQO,QAAQ,IAA […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "async-Pager.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "Pager",
         "_Component",
         "_classCallCheck",
         "_callSuper",
         "arguments",
         "_inherits",
@@ -42,11 +42,11 @@
         "isRequired"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/lib/fragments/Pager.react.js"
     ],
     "sourcesContent": [
-        "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Generic pagination component.\n */\nexport default class Pager extends Component {\n    render() {\n        const {id, value, maxValue, minValue, symbols, tempVal, setProps} = this.props;\n        \n        var from = value[0];\n        var to   = value[1];\n\n        if (tempVal) {\n            if (tempVal === 'MM'){\n                from = minValue\n            } else if (tempVal === 'M'){\n                from = from-1\n            } else if (tempVal === 'PP'){\n                to = maxValue\n            } else if (tempVal === 'P'){\n                to = to+1\n            } else if (tempVal.startsWith(\"F\") && \n                isNaN( from = parseInt(tempVal.replace(\"F\", \"\")) )\n               ) {\n                from = tempVal.replace(\"F\", \"\");\n            } else if (tempVal.startsWith(\"T\") && \n                isNaN( to = parseInt(tempVal.replace(\"T\", \"\")) ) \n               ) {\n                to = tempVal.replace(\"T\", \"\");\n            } \n        \n            if (typeof from === \"number\" && value[0] != from && from >= 1 && from <= maxValue)\n                this.props.setProps({ 'value': [from, value[1]], 'tempVal': null });\n            if (typeof to === \"number\" && value[1] != to && to >= value[0] && to <= maxValue)\n                this.props.setProps({ 'value': [value[0], to], 'tempVal': null });\n        }\n        \n        return (\n            <div id={id+\"-container\"} className=\"form-row\">\n                <button id={id+\"-mm\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'MM' })\n                    }>\n                    <i className=\"bi bi-chevron-double-left\"></i>{symbols[0]}\n                </button>\n                <button id={id+\"-m\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'M' })\n                    }>\n                    <i className=\"bi bi-chevron-left\"></i>{symbols[1]}\n                </button>\n                <span className=\"me-2\"> From </span>\n                <input\n                    id={id+\"-ip-from\"}\n                    value={from}\n                    onChange={\n                        e => setProps({ tempVal: 'F'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((from != value[0]) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> to </span>\n                <input\n                    id={id+\"-ip-to\"}\n                    value={to}\n                    onChange={\n                        e => setProps({ tempVal: 'T'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((to != value[1]) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> of {maxValue} </span>\n                <button id={id+\"-p\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'P' })\n                    }>\n                    <i className=\"bi bi-chevron-right\"></i>{symbols[2]}\n                </button>\n                <button id={id+\"-pp\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'PP' })\n                    }>\n                    <i className=\"bi bi-chevron-double-right\"></i>{symbols[3]}\n                </button>\n                <input\n                    id={id}\n                    value={value}\n                    type=\"hidden\"\n                />\n            </div>\n        );\n    }\n}\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    tempVal: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n"
+        "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Generic pagination component.\n */\nexport default class Pager extends Component {\n    render() {\n        const {id, value, maxValue, minValue, symbols, tempVal, setProps} = this.props;\n        \n        var from = value[0];\n        var to   = value[1];\n\n        if (tempVal) {\n            if (tempVal === 'MM'){\n                from = minValue\n            } else if (tempVal === 'M'){\n                from = from-1\n            } else if (tempVal === 'PP'){\n                to = maxValue\n            } else if (tempVal === 'P'){\n                to = to+1\n            } else if (tempVal.startsWith(\"F\") && \n                isNaN( from = parseInt(tempVal.replace(\"F\", \"\")) )\n               ) {\n                from = tempVal.replace(\"F\", \"\");\n            } else if (tempVal.startsWith(\"T\") && \n                isNaN( to = parseInt(tempVal.replace(\"T\", \"\")) ) \n               ) {\n                to = tempVal.replace(\"T\", \"\");\n            } \n        \n            if (typeof from === \"number\" && value[0] != from && from >= 1 && from <= maxValue)\n                this.props.setProps({ 'value': [from, value[1]], 'tempVal': null });\n            if (typeof to === \"number\" && value[1] != to && to >= value[0] && to <= maxValue)\n                this.props.setProps({ 'value': [value[0], to], 'tempVal': null });\n        }\n        \n        return (\n            <div id={id+\"-container\"} className=\"form-row\">\n                <button id={id+\"-mm\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'MM' })\n                    }>\n                    <i className=\"bi bi-chevron-double-left\"></i>{symbols[0]}\n                </button>\n                <button id={id+\"-m\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'M' })\n                    }>\n                    <i className=\"bi bi-chevron-left\"></i>{symbols[1]}\n                </button>\n                <span className=\"me-2\"> From </span>\n                <input\n                    id={id+\"-ip-from\"}\n                    value={from}\n                    onChange={\n                        e => setProps({ tempVal: 'F'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((from != value[0] || from < minValue || from > to) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> to </span>\n                <input\n                    id={id+\"-ip-to\"}\n                    value={to}\n                    onChange={\n                        e => setProps({ tempVal: 'T'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((to != value[1] || to > maxValue || to < from) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> of {maxValue} </span>\n                <button id={id+\"-p\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'P' })\n                    }>\n                    <i className=\"bi bi-chevron-right\"></i>{symbols[2]}\n                </button>\n                <button id={id+\"-pp\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'PP' })\n                    }>\n                    <i className=\"bi bi-chevron-double-right\"></i>{symbols[3]}\n                </button>\n                <input\n                    id={id}\n                    value={value}\n                    type=\"hidden\"\n                />\n            </div>\n        );\n    }\n}\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    tempVal: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.1.1/dash_pager/dash_pager.min.js` & `dash_pager-0.1.2/dash_pager/dash_pager.min.js`

 * *Files 1% similar despite different names*

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
-            return a.splice(1, 0, "v0_1_1m1713406128"), o.splice(-1, 1, a.join(".")), o.join("/")
+            return a.splice(1, 0, "v0_1_2m1713407077"), o.splice(-1, 1, a.join(".")), o.join("/")
         }
     }(() => {
         var e = {
             792: 0
         };
         o.f.j = (r, t) => {
             var n = o.o(e, r) ? e[r] : void 0;
```

### Comparing `dash_pager-0.1.1/dash_pager/dash_pager.min.js.map` & `dash_pager-0.1.2/dash_pager/dash_pager.min.js.map`

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
@@ -172,14 +172,14 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + \"async-Pager\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_1m1713406128\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_2m1713407077\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t792: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_pager\"] = self[\"webpackChunkdash_pager\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "export const Pager = React.lazy(() => import(/* webpackChunkName: \"Pager\" */ './fragments/Pager.react'));",
         "import React from 'react';\nimport PropTypes from 'prop-types';\nimport { Pager as RealComponent } from '../LazyLoader';\n\n/**\n * ExampleComponent is an example component.\n * It takes a property, `label`, and\n * displays it.\n * It renders an input with the property `value`\n * which is editable by the user.\n */\nconst Pager = (props) => {\n    return (\n        <React.Suspense fallback={null}>\n            <RealComponent {...props}/>\n        </React.Suspense>\n    );\n};\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * A label that will be printed when this component is rendered.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n\nexport default Pager;\n\nexport const defaultProps = Pager.defaultProps;\nexport const propTypes = Pager.propTypes;\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.1.1/dash_pager/metadata.json` & `dash_pager-0.1.2/dash_pager/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.1/dash_pager/package-info.json` & `dash_pager-0.1.2/dash_pager/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `dash_pager-0.1.1/dash_pager.egg-info/PKG-INFO` & `dash_pager-0.1.2/dash_pager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pager
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_pager-0.1.1/package.json` & `dash_pager-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `dash_pager-0.1.1/setup.py` & `dash_pager-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.1/tests/test_usage.py` & `dash_pager-0.1.2/tests/test_usage.py`

 * *Files identical despite different names*

