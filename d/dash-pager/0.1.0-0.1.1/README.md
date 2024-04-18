# Comparing `tmp/dash_pager-0.1.0.tar.gz` & `tmp/dash_pager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pager-0.1.0.tar", last modified: Thu Apr 18 01:12:12 2024, max compression
+gzip compressed data, was "dash_pager-0.1.1.tar", last modified: Thu Apr 18 02:09:03 2024, max compression
```

## Comparing `dash_pager-0.1.0.tar` & `dash_pager-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.252372 dash_pager-0.1.0/
--rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.0/LICENSE
--rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.0/MANIFEST.in
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 01:12:12.252212 dash_pager-0.1.0/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.0/README.md
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.251256 dash_pager-0.1.0/dash_pager/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     1656 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/Pager.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.0/dash_pager/__init__.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/_imports_.py
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4257 2024-04-18 00:57:09.000000 dash_pager-0.1.0/dash_pager/async-Pager.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)     6645 2024-04-18 00:57:09.000000 dash_pager-0.1.0/dash_pager/async-Pager.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3894 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/dash_pager.min.js
--rw-r--r--   0 tarlisportela   (501) staff       (20)    19088 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/dash_pager.min.js.map
--rw-r--r--   0 tarlisportela   (501) staff       (20)     3060 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/metadata.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 01:12:08.000000 dash_pager-0.1.0/dash_pager/package-info.json
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.251766 dash_pager-0.1.0/dash_pager.egg-info/
--rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/PKG-INFO
--rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/SOURCES.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/dependency_links.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 01:12:12.000000 dash_pager-0.1.0/dash_pager.egg-info/top_level.txt
--rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 01:11:56.000000 dash_pager-0.1.0/package.json
--rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 01:12:12.252423 dash_pager-0.1.0/setup.cfg
--rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.0/setup.py
-drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 01:12:12.251903 dash_pager-0.1.0/tests/
--rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.0/tests/test_usage.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.597528 dash_pager-0.1.1/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    35129 2024-04-18 01:01:07.000000 dash_pager-0.1.1/LICENSE
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      333 2024-04-18 00:53:59.000000 dash_pager-0.1.1/MANIFEST.in
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 02:09:03.597386 dash_pager-0.1.1/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3952 2024-04-18 01:10:30.000000 dash_pager-0.1.1/README.md
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.596378 dash_pager-0.1.1/dash_pager/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     1802 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/Pager.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2257 2024-04-18 00:53:59.000000 dash_pager-0.1.1/dash_pager/__init__.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       89 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/_imports_.py
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4561 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/async-Pager.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     7964 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/async-Pager.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3925 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/dash_pager.min.js
+-rw-r--r--   0 tarlisportela   (501) staff       (20)    19262 2024-04-18 02:08:47.000000 dash_pager-0.1.1/dash_pager/dash_pager.min.js.map
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     3622 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/metadata.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 02:08:48.000000 dash_pager-0.1.1/dash_pager/package-info.json
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.596896 dash_pager-0.1.1/dash_pager.egg-info/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     4239 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/PKG-INFO
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      446 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/SOURCES.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)        1 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/dependency_links.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       11 2024-04-18 02:09:03.000000 dash_pager-0.1.1/dash_pager.egg-info/top_level.txt
+-rw-r--r--   0 tarlisportela   (501) staff       (20)     2102 2024-04-18 02:08:25.000000 dash_pager-0.1.1/package.json
+-rw-r--r--   0 tarlisportela   (501) staff       (20)       38 2024-04-18 02:09:03.597569 dash_pager-0.1.1/setup.cfg
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      695 2024-04-18 00:53:59.000000 dash_pager-0.1.1/setup.py
+drwxr-xr-x   0 tarlisportela   (501) staff       (20)        0 2024-04-18 02:09:03.597037 dash_pager-0.1.1/tests/
+-rw-r--r--   0 tarlisportela   (501) staff       (20)      920 2024-04-18 00:53:59.000000 dash_pager-0.1.1/tests/test_usage.py
```

### Comparing `dash_pager-0.1.0/LICENSE` & `dash_pager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.0/PKG-INFO` & `dash_pager-0.1.1/dash_pager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dash_pager
-Version: 0.1.0
+Name: dash-pager
+Version: 0.1.1
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_pager-0.1.0/README.md` & `dash_pager-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.0/dash_pager/Pager.py` & `dash_pager-0.1.1/dash_pager/Pager.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 
 - id (string; optional):
     The ID used to identify this component in Dash callbacks.
 
 - maxValue (number; required):
     A label that will be printed when this component is rendered.
 
+- minValue (number; default 1):
+    The minimum number of elements displayed in the input.
+
 - symbols (list of strings; default ['','','','']):
     The text symbols for the buttons.
 
 - value (list of numbers; optional):
     The value displayed in the input."""
     _children_props = []
     _base_nodes = ['children']
     _namespace = 'dash_pager'
     _type = 'Pager'
     @_explicitize_args
-    def __init__(self, id=Component.UNDEFINED, value=Component.UNDEFINED, maxValue=Component.REQUIRED, symbols=Component.UNDEFINED, **kwargs):
-        self._prop_names = ['id', 'maxValue', 'symbols', 'value']
+    def __init__(self, id=Component.UNDEFINED, value=Component.UNDEFINED, maxValue=Component.REQUIRED, minValue=Component.UNDEFINED, symbols=Component.UNDEFINED, **kwargs):
+        self._prop_names = ['id', 'maxValue', 'minValue', 'symbols', 'value']
         self._valid_wildcard_attributes =            []
-        self.available_properties = ['id', 'maxValue', 'symbols', 'value']
+        self.available_properties = ['id', 'maxValue', 'minValue', 'symbols', 'value']
         self.available_wildcard_properties =            []
         _explicit_args = kwargs.pop('_explicit_args')
         _locals = locals()
         _locals.update(kwargs)  # For wildcard attrs and excess named props
         args = {k: _locals[k] for k in _explicit_args}
 
         for k in ['maxValue']:
```

### Comparing `dash_pager-0.1.0/dash_pager/__init__.py` & `dash_pager-0.1.1/dash_pager/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.0/dash_pager/async-Pager.js` & `dash_pager-0.1.1/dash_pager/async-Pager.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,58 +1,58 @@
 "use strict";
 (self.webpackChunkdash_pager = self.webpackChunkdash_pager || []).push([
     [119], {
-        993: (e, t, r) => {
-            r.r(t), r.d(t, {
+        993: (e, t, n) => {
+            n.r(t), n.d(t, {
                 default: () => b
             });
-            var n = r(609),
-                o = r.n(n),
-                a = r(120),
-                i = r.n(a);
+            var r = n(609),
+                o = n.n(r),
+                i = n(120),
+                a = n.n(i);
 
-            function u(e) {
-                return u = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+            function l(e) {
+                return l = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                     return typeof e
                 } : function(e) {
                     return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                }, u(e)
+                }, l(e)
             }
 
-            function l(e, t) {
-                for (var r = 0; r < t.length; r++) {
-                    var n = t[r];
-                    n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, c(n.key), n)
+            function u(e, t) {
+                for (var n = 0; n < t.length; n++) {
+                    var r = t[n];
+                    r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, c(r.key), r)
                 }
             }
 
             function c(e) {
                 var t = function(e, t) {
-                    if ("object" != u(e) || !e) return e;
-                    var r = e[Symbol.toPrimitive];
-                    if (void 0 !== r) {
-                        var n = r.call(e, "string");
-                        if ("object" != u(n)) return n;
+                    if ("object" != l(e) || !e) return e;
+                    var n = e[Symbol.toPrimitive];
+                    if (void 0 !== n) {
+                        var r = n.call(e, "string");
+                        if ("object" != l(r)) return r;
                         throw new TypeError("@@toPrimitive must return a primitive value.")
                     }
                     return String(e)
                 }(e);
-                return "symbol" == u(t) ? t : t + ""
+                return "symbol" == l(t) ? t : t + ""
             }
 
-            function s(e, t, r) {
+            function s(e, t, n) {
                 return t = m(t),
                     function(e, t) {
-                        if (t && ("object" === u(t) || "function" == typeof t)) return t;
+                        if (t && ("object" === l(t) || "function" == typeof t)) return t;
                         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                         return function(e) {
                             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                             return e
                         }(e)
-                    }(e, p() ? Reflect.construct(t, r || [], m(e).constructor) : t.apply(e, r))
+                    }(e, p() ? Reflect.construct(t, n || [], m(e).constructor) : t.apply(e, n))
             }
 
             function p() {
                 try {
                     var e = !Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {})))
                 } catch (e) {}
                 return (p = function() {
@@ -84,109 +84,134 @@
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
                     }), Object.defineProperty(e, "prototype", {
                         writable: !1
                     }), t && f(e, t)
-                }(t, e), r = t, (n = [{
+                }(t, e), n = t, (r = [{
                     key: "render",
                     value: function() {
                         var e = this.props,
                             t = e.id,
-                            r = e.value,
-                            n = e.maxValue,
+                            n = e.value,
+                            r = e.maxValue,
+                            i = e.minValue,
                             a = e.symbols,
-                            i = e.tempVal,
+                            l = e.tempVal,
                             u = e.setProps,
-                            l = r[0],
-                            c = r[1];
-                        return i && (i.startsWith("F") && isNaN(l = parseInt(i.replace("F", ""))) ? l = i.replace("F", "") : i.startsWith("T") && isNaN(c = parseInt(i.replace("T", ""))) && (c = i.replace("T", ""))), "number" == typeof l && r[0] != l && l >= 1 && l <= n && this.props.setProps({
-                            value: [l, r[1]]
-                        }), "number" == typeof c && r[1] != c && c >= r[0] && c <= n && this.props.setProps({
-                            value: [r[0], c]
-                        }), o().createElement("div", {
+                            c = n[0],
+                            s = n[1];
+                        return l && ("MM" === l ? c = i : "M" === l ? c -= 1 : "PP" === l ? s = r : "P" === l ? s += 1 : l.startsWith("F") && isNaN(c = parseInt(l.replace("F", ""))) ? c = l.replace("F", "") : l.startsWith("T") && isNaN(s = parseInt(l.replace("T", ""))) && (s = l.replace("T", "")), "number" == typeof c && n[0] != c && c >= 1 && c <= r && this.props.setProps({
+                            value: [c, n[1]],
+                            tempVal: null
+                        }), "number" == typeof s && n[1] != s && s >= n[0] && s <= r && this.props.setProps({
+                            value: [n[0], s],
+                            tempVal: null
+                        })), o().createElement("div", {
                             id: t + "-container",
                             className: "form-row"
                         }, o().createElement("button", {
                             id: t + "-mm",
                             className: "btn btn-outline-primary me-2",
-                            type: "button"
+                            type: "button",
+                            onClick: function(e) {
+                                return u({
+                                    tempVal: "MM"
+                                })
+                            }
                         }, o().createElement("i", {
                             className: "bi bi-chevron-double-left"
                         }), a[0]), o().createElement("button", {
                             id: t + "-m",
                             className: "btn btn-outline-primary me-2",
-                            type: "button"
+                            type: "button",
+                            onClick: function(e) {
+                                return u({
+                                    tempVal: "M"
+                                })
+                            }
                         }, o().createElement("i", {
                             className: "bi bi-chevron-left"
                         }), a[1]), o().createElement("span", {
                             className: "me-2"
                         }, " From "), o().createElement("input", {
                             id: t + "-ip-from",
-                            value: l,
+                            value: c,
                             onChange: function(e) {
                                 return u({
                                     tempVal: "F" + e.target.value
                                 })
                             },
                             type: "number",
                             style: {
                                 width: "10ch",
                                 display: "inline"
                             },
-                            className: "form-control" + (l != r[0] ? " is-invalid" : "")
+                            className: "form-control" + (c != n[0] ? " is-invalid" : "")
                         }), o().createElement("span", {
                             className: "me-2"
                         }, " to "), o().createElement("input", {
                             id: t + "-ip-to",
-                            value: c,
+                            value: s,
                             onChange: function(e) {
                                 return u({
                                     tempVal: "T" + e.target.value
                                 })
                             },
                             type: "number",
                             style: {
                                 width: "10ch",
                                 display: "inline"
                             },
-                            className: "form-control" + (c != r[1] ? " is-invalid" : "")
+                            className: "form-control" + (s != n[1] ? " is-invalid" : "")
                         }), o().createElement("span", {
                             className: "me-2"
-                        }, " of ", n, " "), o().createElement("button", {
+                        }, " of ", r, " "), o().createElement("button", {
                             id: t + "-p",
                             className: "btn btn-outline-primary me-2",
-                            type: "button"
+                            type: "button",
+                            onClick: function(e) {
+                                return u({
+                                    tempVal: "P"
+                                })
+                            }
                         }, o().createElement("i", {
                             className: "bi bi-chevron-right"
                         }), a[2]), o().createElement("button", {
                             id: t + "-pp",
                             className: "btn btn-outline-primary me-2",
-                            type: "button"
+                            type: "button",
+                            onClick: function(e) {
+                                return u({
+                                    tempVal: "PP"
+                                })
+                            }
                         }, o().createElement("i", {
                             className: "bi bi-chevron-double-right"
                         }), a[3]), o().createElement("input", {
                             id: t,
-                            value: r,
+                            value: n,
                             type: "hidden"
                         }))
                     }
-                }]) && l(r.prototype, n), Object.defineProperty(r, "prototype", {
+                }]) && u(n.prototype, r), Object.defineProperty(n, "prototype", {
                     writable: !1
-                }), r;
-                var r, n
-            }(n.Component);
+                }), n;
+                var n, r
+            }(r.Component);
             b.defaultProps = {
+                minValue: 1,
                 symbols: ["", "", "", ""]
             }, b.propTypes = {
-                id: i().string,
-                value: i().arrayOf(i().number),
-                maxValue: i().number.isRequired,
-                symbols: i().arrayOf(i().string),
-                tempVal: i().string,
-                setProps: i().func
+                id: a().string,
+                value: a().arrayOf(a().number),
+                maxValue: a().number.isRequired,
+                minValue: a().number,
+                symbols: a().arrayOf(a().string),
+                tempVal: a().string,
+                setProps: a().func
             }
         }
     }
 ]);
 //# sourceMappingURL=async-Pager.js.map
```

### Comparing `dash_pager-0.1.0/dash_pager/async-Pager.js.map` & `dash_pager-0.1.1/dash_pager/async-Pager.js.map`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8498168498168498%*

 * *Differences: {"'mappings'": "'2mDAGA,IAGqBA,EAAK,SAAAC,GAAA,SAAAD,IAAA,O,4FAAAE,CAAA,KAAAF,GAAAG,EAAA,KAAAH,EAAAI,UAAA,Q,qRAAAC,CAAAL,EAAAC,G,EAAAD,G,EAAA,EAAAM,IAAA,SAAAC,MACtB,WACI,IAAAC,EAAoEC,KAAKC,MAAlEC,EAAEH,EAAFG,GAAIJ,EAAKC,EAALD,MAAOK,EAAQJ,EAARI,SAAUC,EAAQL,EAARK,SAAUC,EAAON,EAAPM,QAASC,EAAOP,EAAPO,QAASC,EAAQR,EAARQ,SAEpDC,EAAOV,EAAM,GACbW,EAAOX,EAAM,GA2BjB,OAzBIQ,IACgB,OAAZA,EACAE,EAAOJ,EACY,MAAZE,EACPE,GAAY,EACO,OAAZF,EACPG,EAAKN,EACc,MAAZG,EACPG,GAAQ,EACDH,EAAQI,WAAW,MAC1BC,MAAOH,EAAOI,SAASN,EAAQO,QAAQ,IAA […]*

```diff
@@ -1,38 +1,40 @@
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
         "key",
         "value",
         "_this$props",
         "this",
         "props",
         "id",
         "maxValue",
+        "minValue",
         "symbols",
         "tempVal",
         "setProps",
         "from",
         "to",
         "startsWith",
         "isNaN",
         "parseInt",
         "replace",
         "React",
         "className",
         "type",
-        "onChange",
+        "onClick",
         "e",
+        "onChange",
         "target",
         "style",
         "width",
         "display",
         "Component",
         "defaultProps",
         "propTypes",
@@ -40,11 +42,11 @@
         "isRequired"
     ],
     "sourceRoot": "",
     "sources": [
         "webpack:///./src/lib/fragments/Pager.react.js"
     ],
     "sourcesContent": [
-        "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Generic pagination component.\n */\nexport default class Pager extends Component {\n    render() {\n        const {id, value, maxValue, symbols, tempVal, setProps} = this.props;\n        \n        var from = value[0];\n        var to   = value[1];\n\n        if (tempVal) {\n            if (tempVal.startsWith(\"F\") && \n                isNaN( from = parseInt(tempVal.replace(\"F\", \"\")) )\n               ) {\n                from = tempVal.replace(\"F\", \"\");\n            } else if (tempVal.startsWith(\"T\") && \n                isNaN( to = parseInt(tempVal.replace(\"T\", \"\")) ) \n               ) {\n                to = tempVal.replace(\"T\", \"\");\n            } \n        }\n        \n        if (typeof from === \"number\" && value[0] != from && from >= 1 && from <= maxValue)\n            this.props.setProps({ 'value': [from, value[1]] });\n        if (typeof to === \"number\" && value[1] != to && to >= value[0] && to <= maxValue)\n            this.props.setProps({ 'value': [value[0], to] });\n        \n        return (\n            <div id={id+\"-container\"} className=\"form-row\">\n                <button id={id+\"-mm\"} className=\"btn btn-outline-primary me-2\" type=\"button\">\n                    <i className=\"bi bi-chevron-double-left\"></i>{symbols[0]}\n                </button>\n                <button id={id+\"-m\"} className=\"btn btn-outline-primary me-2\" type=\"button\">\n                    <i className=\"bi bi-chevron-left\"></i>{symbols[1]}\n                </button>\n                <span className=\"me-2\"> From </span>\n                <input\n                    id={id+\"-ip-from\"}\n                    value={from}\n                    onChange={\n                        e => setProps({ tempVal: 'F'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((from != value[0]) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> to </span>\n                <input\n                    id={id+\"-ip-to\"}\n                    value={to}\n                    onChange={\n                        e => setProps({ tempVal: 'T'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((to != value[1]) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> of {maxValue} </span>\n                <button id={id+\"-p\"} className=\"btn btn-outline-primary me-2\" type=\"button\">\n                    <i className=\"bi bi-chevron-right\"></i>{symbols[2]}\n                </button>\n                <button id={id+\"-pp\"} className=\"btn btn-outline-primary me-2\" type=\"button\">\n                    <i className=\"bi bi-chevron-double-right\"></i>{symbols[3]}\n                </button>\n                <input\n                    id={id}\n                    value={value}\n                    type=\"hidden\"\n                />\n            </div>\n        );\n    }\n}\n\nPager.defaultProps = {\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    maxValue: PropTypes.number.isRequired,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    tempVal: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n"
+        "import React, {Component} from 'react';\nimport PropTypes from 'prop-types';\n\n/**\n * Generic pagination component.\n */\nexport default class Pager extends Component {\n    render() {\n        const {id, value, maxValue, minValue, symbols, tempVal, setProps} = this.props;\n        \n        var from = value[0];\n        var to   = value[1];\n\n        if (tempVal) {\n            if (tempVal === 'MM'){\n                from = minValue\n            } else if (tempVal === 'M'){\n                from = from-1\n            } else if (tempVal === 'PP'){\n                to = maxValue\n            } else if (tempVal === 'P'){\n                to = to+1\n            } else if (tempVal.startsWith(\"F\") && \n                isNaN( from = parseInt(tempVal.replace(\"F\", \"\")) )\n               ) {\n                from = tempVal.replace(\"F\", \"\");\n            } else if (tempVal.startsWith(\"T\") && \n                isNaN( to = parseInt(tempVal.replace(\"T\", \"\")) ) \n               ) {\n                to = tempVal.replace(\"T\", \"\");\n            } \n        \n            if (typeof from === \"number\" && value[0] != from && from >= 1 && from <= maxValue)\n                this.props.setProps({ 'value': [from, value[1]], 'tempVal': null });\n            if (typeof to === \"number\" && value[1] != to && to >= value[0] && to <= maxValue)\n                this.props.setProps({ 'value': [value[0], to], 'tempVal': null });\n        }\n        \n        return (\n            <div id={id+\"-container\"} className=\"form-row\">\n                <button id={id+\"-mm\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'MM' })\n                    }>\n                    <i className=\"bi bi-chevron-double-left\"></i>{symbols[0]}\n                </button>\n                <button id={id+\"-m\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'M' })\n                    }>\n                    <i className=\"bi bi-chevron-left\"></i>{symbols[1]}\n                </button>\n                <span className=\"me-2\"> From </span>\n                <input\n                    id={id+\"-ip-from\"}\n                    value={from}\n                    onChange={\n                        e => setProps({ tempVal: 'F'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((from != value[0]) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> to </span>\n                <input\n                    id={id+\"-ip-to\"}\n                    value={to}\n                    onChange={\n                        e => setProps({ tempVal: 'T'+e.target.value })\n                    }\n                    type=\"number\"\n                    style={{width: \"10ch\", display: \"inline\"}}\n                    className={\"form-control\" + ((to != value[1]) ? ' is-invalid' : '')}\n                />\n                <span className=\"me-2\"> of {maxValue} </span>\n                <button id={id+\"-p\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'P' })\n                    }>\n                    <i className=\"bi bi-chevron-right\"></i>{symbols[2]}\n                </button>\n                <button id={id+\"-pp\"} className=\"btn btn-outline-primary me-2\" type=\"button\" \n                    onClick={\n                        e => setProps({ tempVal: 'PP' })\n                    }>\n                    <i className=\"bi bi-chevron-double-right\"></i>{symbols[3]}\n                </button>\n                <input\n                    id={id}\n                    value={value}\n                    type=\"hidden\"\n                />\n            </div>\n        );\n    }\n}\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * The maximum number of elements displayed in the input.\n     */\n    tempVal: PropTypes.string,\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.1.0/dash_pager/dash_pager.min.js` & `dash_pager-0.1.1/dash_pager/dash_pager.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -34,34 +34,34 @@
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), o.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "dash_pager:", o.l = (t, n, a, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var s, c;
+            var s, u;
             if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), l = 0; l < u.length; l++) {
-                    var p = u[l];
+                for (var c = document.getElementsByTagName("script"), l = 0; l < c.length; l++) {
+                    var p = c[l];
                     if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + a) {
                         s = p;
                         break
                     }
                 }
-            s || (c = !0, (s = document.createElement("script")).charset = "utf-8", s.timeout = 120, o.nc && s.setAttribute("nonce", o.nc), s.setAttribute("data-webpack", r + a), s.src = t), e[t] = [n];
+            s || (u = !0, (s = document.createElement("script")).charset = "utf-8", s.timeout = 120, o.nc && s.setAttribute("nonce", o.nc), s.setAttribute("data-webpack", r + a), s.src = t), e[t] = [n];
             var d = (r, n) => {
                     s.onerror = s.onload = null, clearTimeout(f);
                     var o = e[t];
                     if (delete e[t], s.parentNode && s.parentNode.removeChild(s), o && o.forEach((e => e(n))), r) return r(n)
                 },
                 f = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: s
                 }), 12e4);
-            s.onerror = d.bind(null, s.onerror), s.onload = d.bind(null, s.onload), c && document.head.appendChild(s)
+            s.onerror = d.bind(null, s.onerror), s.onload = d.bind(null, s.onload), u && document.head.appendChild(s)
         }
     }, o.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -95,15 +95,15 @@
         var s = jsonpScriptSrc;
         jsonpScriptSrc = function(e) {
             var r, t = (r = i(), /\/_dash-component-suites\//.test(r.src)),
                 n = s(e);
             if (!t) return n;
             var o = n.split("/"),
                 a = o.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_1_0m1713402728"), o.splice(-1, 1, a.join(".")), o.join("/")
+            return a.splice(1, 0, "v0_1_1m1713406128"), o.splice(-1, 1, a.join(".")), o.join("/")
         }
     }(() => {
         var e = {
             792: 0
         };
         o.f.j = (r, t) => {
             var n = o.o(e, r) ? e[r] : void 0;
@@ -120,28 +120,28 @@
                                 i = t && t.target && t.target.src;
                             s.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", s.name = "ChunkLoadError", s.type = a, s.request = i, n[1](s)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [i, s, c] = t,
-                    u = 0;
+                var n, a, [i, s, u] = t,
+                    c = 0;
                 if (i.some((r => 0 !== e[r]))) {
                     for (n in s) o.o(s, n) && (o.m[n] = s[n]);
-                    c && c(o)
+                    u && u(o)
                 }
-                for (r && r(t); u < i.length; u++) a = i[u], o.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); c < i.length; c++) a = i[c], o.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkdash_pager = self.webpackChunkdash_pager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var c = {};
+    var u = {};
     (() => {
-        o.r(c), o.d(c, {
+        o.r(u), o.d(u, {
             Pager: () => s
         });
         var e = o(609),
             r = o.n(e),
             t = o(120),
             n = o.n(t),
             a = React.lazy((function() {
@@ -149,19 +149,21 @@
             })),
             i = function(e) {
                 return r().createElement(r().Suspense, {
                     fallback: null
                 }, r().createElement(a, e))
             };
         i.defaultProps = {
+            minValue: 1,
             symbols: ["", "", "", ""]
         }, i.propTypes = {
             id: n().string,
             value: n().arrayOf(n().number),
             maxValue: n().number.isRequired,
+            minValue: n().number,
             symbols: n().arrayOf(n().string),
             setProps: n().func
         };
         const s = i
-    })(), window.dash_pager = c
+    })(), window.dash_pager = u
 })();
 //# sourceMappingURL=dash_pager.min.js.map
```

### Comparing `dash_pager-0.1.0/dash_pager/dash_pager.min.js.map` & `dash_pager-0.1.1/dash_pager/dash_pager.min.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9121918270854442%*

 * *Differences: {"'mappings'": "'uBAAIA,EACAC,E,WCDJC,EAAOC,QAAUC,OAAkB,S,UCAnCF,EAAOC,QAAUC,OAAc,K,GCC3BC,EAA2B,CAAC,EAGhC,SAASC,EAAoBC,GAE5B,IAAIC,EAAeH,EAAyBE,GAC5C,QAAqBE,IAAjBD,EACH,OAAOA,EAAaL,QAGrB,IAAID,EAASG,EAAyBE,GAAY,CAGjDJ,QAAS,CAAC,GAOX,OAHAO,EAAoBH,GAAUL,EAAQA,EAAOC,QAASG,GAG/CJ,EAAOC,OACf,CAGAG,EAAoBK,EAAID,ECxBxBJ,EAAoBM,EAAKV,IACxB,IAAIW,EAASX,GAAUA,EAAOY,WAC7B,IAAOZ,EAAiB,QACxB,IAAM,EAEP,OADAI,EAAoBS,EAAEF,EAAQ,CAAEG,EAAGH,IAC5BA,CAAM,ECLdP,EAAoBS,EAAI,CAACZ,EAASc,KACjC,IAAI,IAAIC,KAAOD,EACXX,EAAoBa,EAAE […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "dash_pager.min.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "inProgress",
         "dataWebpackPrefix",
         "module",
         "exports",
         "window",
         "__webpack_module_cache__",
@@ -132,14 +132,15 @@
         "Pager",
         "React",
         "lazy",
         "props",
         "fallback",
         "RealComponent",
         "defaultProps",
+        "minValue",
         "symbols",
         "propTypes",
         "PropTypes",
         "maxValue",
         "isRequired",
         "setProps"
     ],
@@ -171,14 +172,14 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + \"async-Pager\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
-        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_0m1713402728\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
+        "var getCurrentScript = function() {\n    var script = document.currentScript;\n    if (!script) {\n        /* Shim for IE11 and below */\n        /* Do not take into account async scripts and inline scripts */\n\n        var doc_scripts = document.getElementsByTagName('script');\n        var scripts = [];\n\n        for (var i = 0; i < doc_scripts.length; i++) {\n            scripts.push(doc_scripts[i]);\n        }\n\n        scripts = scripts.filter(function(s) { return !s.async && !s.text && !s.textContent; });\n        script = scripts.slice(-1)[0];\n    }\n\n    return script;\n};\n\nvar isLocalScript = function(script) {\n    return /\\/_dash-component-suites\\//.test(script.src);\n};\n\nObject.defineProperty(__webpack_require__, 'p', {\n    get: (function () {\n        var script = getCurrentScript();\n\n        var url = script.src.split('/').slice(0, -1).join('/') + '/';\n\n        return function() {\n            return url;\n        };\n    })()\n});\n\nif (typeof jsonpScriptSrc !== 'undefined') {\n    var __jsonpScriptSrc__ = jsonpScriptSrc;\n    jsonpScriptSrc = function(chunkId) {\n        var script = getCurrentScript();\n        var isLocal = isLocalScript(script);\n\n        var src = __jsonpScriptSrc__(chunkId);\n\n        if(!isLocal) {\n            return src;\n        }\n\n        var srcFragments = src.split('/');\n        var fileFragments = srcFragments.slice(-1)[0].split('.');\n\n        fileFragments.splice(1, 0, \"v0_1_1m1713406128\");\n        srcFragments.splice(-1, 1, fileFragments.join('.'))\n\n        return srcFragments.join('/');\n    };\n}\n",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t792: 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkdash_pager\"] = self[\"webpackChunkdash_pager\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "export const Pager = React.lazy(() => import(/* webpackChunkName: \"Pager\" */ './fragments/Pager.react'));",
-        "import React from 'react';\nimport PropTypes from 'prop-types';\nimport { Pager as RealComponent } from '../LazyLoader';\n\n/**\n * ExampleComponent is an example component.\n * It takes a property, `label`, and\n * displays it.\n * It renders an input with the property `value`\n * which is editable by the user.\n */\nconst Pager = (props) => {\n    return (\n        <React.Suspense fallback={null}>\n            <RealComponent {...props}/>\n        </React.Suspense>\n    );\n};\n\nPager.defaultProps = {\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * A label that will be printed when this component is rendered.\n     */\n    maxValue: PropTypes.number.isRequired,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n\nexport default Pager;\n\nexport const defaultProps = Pager.defaultProps;\nexport const propTypes = Pager.propTypes;\n"
+        "import React from 'react';\nimport PropTypes from 'prop-types';\nimport { Pager as RealComponent } from '../LazyLoader';\n\n/**\n * ExampleComponent is an example component.\n * It takes a property, `label`, and\n * displays it.\n * It renders an input with the property `value`\n * which is editable by the user.\n */\nconst Pager = (props) => {\n    return (\n        <React.Suspense fallback={null}>\n            <RealComponent {...props}/>\n        </React.Suspense>\n    );\n};\n\nPager.defaultProps = {\n    minValue: 1,\n    symbols: ['','','','']\n};\n\nPager.propTypes = {\n    /**\n     * The ID used to identify this component in Dash callbacks.\n     */\n    id: PropTypes.string,\n\n    /**\n     * The value displayed in the input.\n     */\n    value: PropTypes.arrayOf(PropTypes.number),\n\n    /**\n     * A label that will be printed when this component is rendered.\n     */\n    maxValue: PropTypes.number.isRequired,\n\n    /**\n     * The minimum number of elements displayed in the input.\n     */\n    minValue: PropTypes.number,\n    \n    /**\n     * The text symbols for the buttons.\n     */\n    symbols: PropTypes.arrayOf(PropTypes.string),\n\n    /**\n     * Dash-assigned callback that should be called to report property changes\n     * to Dash, to make them available for callbacks.\n     */\n    setProps: PropTypes.func\n};\n\nexport default Pager;\n\nexport const defaultProps = Pager.defaultProps;\nexport const propTypes = Pager.propTypes;\n"
     ],
     "version": 3
 }
```

### Comparing `dash_pager-0.1.0/dash_pager/metadata.json` & `dash_pager-0.1.1/dash_pager/metadata.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333334%*

 * *Differences: {"'src/lib/components/.ipynb_checkpoints/Pager.react-checkpoint.js'": "{'props': {'minValue': "*

 * *                                                                      "OrderedDict([('type', "*

 * *                                                                      "OrderedDict([('name', "*

 * *                                                                      "'number')])), ('required', "*

 * *                                                                      "False), ('description', "*

 * *                              […]*

```diff
@@ -14,14 +14,25 @@
             "maxValue": {
                 "description": "A label that will be printed when this component is rendered.",
                 "required": true,
                 "type": {
                     "name": "number"
                 }
             },
+            "minValue": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "1"
+                },
+                "description": "The minimum number of elements displayed in the input.",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
@@ -66,14 +77,25 @@
             "maxValue": {
                 "description": "A label that will be printed when this component is rendered.",
                 "required": true,
                 "type": {
                     "name": "number"
                 }
             },
+            "minValue": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "1"
+                },
+                "description": "The minimum number of elements displayed in the input.",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
             "setProps": {
                 "description": "Dash-assigned callback that should be called to report property changes\nto Dash, to make them available for callbacks.",
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             },
```

### Comparing `dash_pager-0.1.0/dash_pager/package-info.json` & `dash_pager-0.1.1/dash_pager/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `dash_pager-0.1.0/dash_pager.egg-info/PKG-INFO` & `dash_pager-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dash-pager
-Version: 0.1.0
+Name: dash_pager
+Version: 0.1.1
 Summary: Generic pagination component for dash and dash bootstrap components
 Author: Tarlis Portela <tarlis@tarlis.com.br>
 License: GPL-3.0
 Classifier: Framework :: Dash
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `dash_pager-0.1.0/package.json` & `dash_pager-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -50,9 +50,9 @@
         "build:backends": "dash-generate-components ./src/lib/components dash_pager -p package-info.json --r-prefix 'dccPager' --jl-prefix 'dccPager' --ignore \\.test\\.",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:backends)",
         "build:js": "webpack --mode production",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack serve --config ./webpack.serve.config.js --open",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `dash_pager-0.1.0/setup.py` & `dash_pager-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `dash_pager-0.1.0/tests/test_usage.py` & `dash_pager-0.1.1/tests/test_usage.py`

 * *Files identical despite different names*

