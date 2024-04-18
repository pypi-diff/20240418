# Comparing `tmp/py_research-5.1.0.tar.gz` & `tmp/py_research-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_research-5.1.0.tar", last modified: Sun Apr 14 09:27:26 2024, max compression
+gzip compressed data, was "py_research-5.1.1.tar", last modified: Thu Apr 18 09:15:35 2024, max compression
```

## Comparing `py_research-5.1.0.tar` & `py_research-5.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1070 2024-04-14 09:27:18.396074 py_research-5.1.0/LICENSE
--rw-r--r--   0        0        0     3079 2024-04-14 09:27:18.396074 py_research-5.1.0/README.md
--rw-r--r--   0        0        0     2290 2024-04-14 09:27:26.560068 py_research-5.1.0/pyproject.toml
--rw-r--r--   0        0        0       56 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/__init__.py
--rw-r--r--   0        0        0     9849 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/caching.py
--rw-r--r--   0        0        0     3805 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/colors.py
--rw-r--r--   0        0        0     4904 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/data.py
--rw-r--r--   0        0        0      249 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/db/__init__.py
--rw-r--r--   0        0        0    53926 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/db/base.py
--rw-r--r--   0        0        0      799 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/db/conflicts.py
--rw-r--r--   0        0        0    16309 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/db/importing.py
--rw-r--r--   0        0        0      432 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/enums.py
--rw-r--r--   0        0        0      613 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/files.py
--rw-r--r--   0        0        0    14046 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/geo.py
--rw-r--r--   0        0        0     2658 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/hashing.py
--rw-r--r--   0        0        0    28664 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/intl.py
--rw-r--r--   0        0        0    10319 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/plots/__init__.py
--rw-r--r--   0        0        0     1986 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/plots/responsive_plotly.js
--rw-r--r--   0        0        0     4778 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/ranking.py
--rw-r--r--   0        0        0       40 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/reflect/__init__.py
--rw-r--r--   0        0        0     5689 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/reflect/deps.py
--rw-r--r--   0        0        0     3720 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/reflect/dist.py
--rw-r--r--   0        0        0     1852 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/reflect/env.py
--rw-r--r--   0        0        0     8354 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/reflect/ref.py
--rw-r--r--   0        0        0     1735 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/reflect/runtime.py
--rw-r--r--   0        0        0    23621 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/sql.py
--rw-r--r--   0        0        0     4539 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/stats.py
--rw-r--r--   0        0        0    24346 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/tables.py
--rw-r--r--   0        0        0     7541 2024-04-14 09:27:18.400074 py_research-5.1.0/src/py_research/telemetry.py
--rw-r--r--   0        0        0     4955 2024-04-14 09:27:18.404074 py_research-5.1.0/src/py_research/time.py
--rw-r--r--   0        0        0     2421 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_caching.py
--rw-r--r--   0        0        0      588 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_colors.py
--rw-r--r--   0        0        0    18077 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_db_base.py
--rw-r--r--   0        0        0     6692 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_db_importing.py
--rw-r--r--   0        0        0      348 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_enums.py
--rw-r--r--   0        0        0      950 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_files.py
--rw-r--r--   0        0        0     6106 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_geo.py
--rw-r--r--   0        0        0      717 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_hashing.py
--rw-r--r--   0        0        0     3754 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_intl.py
--rw-r--r--   0        0        0     1376 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_plots.py
--rw-r--r--   0        0        0     3130 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_ranking.py
--rw-r--r--   0        0        0     1250 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_reflect.py
--rw-r--r--   0        0        0     2374 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_stats.py
--rw-r--r--   0        0        0     4485 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_tables.py
--rw-r--r--   0        0        0      319 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_telemetry.py
--rw-r--r--   0        0        0      625 2024-04-14 09:27:18.404074 py_research-5.1.0/tests/py_research/test_time.py
--rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 py_research-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-18 09:15:27.890488 py_research-5.1.1/LICENSE
+-rw-r--r--   0        0        0     3079 2024-04-18 09:15:27.890488 py_research-5.1.1/README.md
+-rw-r--r--   0        0        0     2290 2024-04-18 09:15:35.574496 py_research-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-18 09:15:27.890488 py_research-5.1.1/src/py_research/__init__.py
+-rw-r--r--   0        0        0     9849 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/caching.py
+-rw-r--r--   0        0        0     3805 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/colors.py
+-rw-r--r--   0        0        0     4904 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/data.py
+-rw-r--r--   0        0        0      249 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/db/__init__.py
+-rw-r--r--   0        0        0    53926 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/db/base.py
+-rw-r--r--   0        0        0      799 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/db/conflicts.py
+-rw-r--r--   0        0        0    16309 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/db/importing.py
+-rw-r--r--   0        0        0      432 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/enums.py
+-rw-r--r--   0        0        0      613 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/files.py
+-rw-r--r--   0        0        0    14046 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/geo.py
+-rw-r--r--   0        0        0     2658 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/hashing.py
+-rw-r--r--   0        0        0    28664 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/intl.py
+-rw-r--r--   0        0        0    10324 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/plots/__init__.py
+-rw-r--r--   0        0        0     2184 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/plots/responsive_plotly.js
+-rw-r--r--   0        0        0     4778 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/ranking.py
+-rw-r--r--   0        0        0       40 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/reflect/__init__.py
+-rw-r--r--   0        0        0     5689 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/reflect/deps.py
+-rw-r--r--   0        0        0     3720 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/reflect/dist.py
+-rw-r--r--   0        0        0     1852 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/reflect/env.py
+-rw-r--r--   0        0        0     8354 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/reflect/ref.py
+-rw-r--r--   0        0        0     1735 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/reflect/runtime.py
+-rw-r--r--   0        0        0    23621 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/sql.py
+-rw-r--r--   0        0        0     4539 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/stats.py
+-rw-r--r--   0        0        0    24346 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/tables.py
+-rw-r--r--   0        0        0     7541 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/telemetry.py
+-rw-r--r--   0        0        0     4955 2024-04-18 09:15:27.894488 py_research-5.1.1/src/py_research/time.py
+-rw-r--r--   0        0        0     2421 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_caching.py
+-rw-r--r--   0        0        0      588 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_colors.py
+-rw-r--r--   0        0        0    18077 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_db_base.py
+-rw-r--r--   0        0        0     6692 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_db_importing.py
+-rw-r--r--   0        0        0      348 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_enums.py
+-rw-r--r--   0        0        0      950 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_files.py
+-rw-r--r--   0        0        0     6106 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_geo.py
+-rw-r--r--   0        0        0      717 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_hashing.py
+-rw-r--r--   0        0        0     3754 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_intl.py
+-rw-r--r--   0        0        0     1376 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_plots.py
+-rw-r--r--   0        0        0     3130 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_ranking.py
+-rw-r--r--   0        0        0     1250 2024-04-18 09:15:27.894488 py_research-5.1.1/tests/py_research/test_reflect.py
+-rw-r--r--   0        0        0     2374 2024-04-18 09:15:27.898488 py_research-5.1.1/tests/py_research/test_stats.py
+-rw-r--r--   0        0        0     4485 2024-04-18 09:15:27.898488 py_research-5.1.1/tests/py_research/test_tables.py
+-rw-r--r--   0        0        0      319 2024-04-18 09:15:27.898488 py_research-5.1.1/tests/py_research/test_telemetry.py
+-rw-r--r--   0        0        0      625 2024-04-18 09:15:27.898488 py_research-5.1.1/tests/py_research/test_time.py
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 py_research-5.1.1/PKG-INFO
```

### Comparing `py_research-5.1.0/LICENSE` & `py_research-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/README.md` & `py_research-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/pyproject.toml` & `py_research-5.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "ipywidgets>=8.1.1",
     "ipython>=8.21.0",
     "sphinx>=7.2.6",
 ]
 name = "py-research"
 description = "Collection of utilities for R&D coding in Python 🐍"
 readme = "README.md"
-version = "5.1.0"
+version = "5.1.1"
 
 [project.urls]
 Documentation = "https://cloudlane-one.github.io/py-research/"
 
 [build-system]
 requires = [
     "pdm-backend",
```

### Comparing `py_research-5.1.0/src/py_research/caching.py` & `py_research-5.1.1/src/py_research/caching.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/colors.py` & `py_research-5.1.1/src/py_research/colors.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/data.py` & `py_research-5.1.1/src/py_research/data.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/db/base.py` & `py_research-5.1.1/src/py_research/db/base.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/db/conflicts.py` & `py_research-5.1.1/src/py_research/db/conflicts.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/db/importing.py` & `py_research-5.1.1/src/py_research/db/importing.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/files.py` & `py_research-5.1.1/src/py_research/files.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/geo.py` & `py_research-5.1.1/src/py_research/geo.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/hashing.py` & `py_research-5.1.1/src/py_research/hashing.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/intl.py` & `py_research-5.1.1/src/py_research/intl.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/plots/__init__.py` & `py_research-5.1.1/src/py_research/plots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             <div class="plotly-responsive-container" style="width: 100%;">
                 {_ind(plotly_js_script, 16)}
                 {_ind(fig_html, 16)}
                 <script
                     id="{script_id}"
                     {_ind(script_attr_str, 20)}
                 >
-                    const scriptID = "{script_id}";
+                    var resplotScriptID = "{script_id}";
                     {_ind(plotly_responsive_js, 20)}
                 </script>
             </div>
             """
         )
 
     # Wrap the figure in a full html document if requested.
```

### Comparing `py_research-5.1.0/src/py_research/ranking.py` & `py_research-5.1.1/src/py_research/ranking.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/reflect/deps.py` & `py_research-5.1.1/src/py_research/reflect/deps.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/reflect/dist.py` & `py_research-5.1.1/src/py_research/reflect/dist.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/reflect/env.py` & `py_research-5.1.1/src/py_research/reflect/env.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/reflect/ref.py` & `py_research-5.1.1/src/py_research/reflect/ref.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/reflect/runtime.py` & `py_research-5.1.1/src/py_research/reflect/runtime.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/sql.py` & `py_research-5.1.1/src/py_research/sql.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/stats.py` & `py_research-5.1.1/src/py_research/stats.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/tables.py` & `py_research-5.1.1/src/py_research/tables.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/telemetry.py` & `py_research-5.1.1/src/py_research/telemetry.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/src/py_research/time.py` & `py_research-5.1.1/src/py_research/time.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_caching.py` & `py_research-5.1.1/tests/py_research/test_caching.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_colors.py` & `py_research-5.1.1/tests/py_research/test_colors.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_db_base.py` & `py_research-5.1.1/tests/py_research/test_db_base.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_db_importing.py` & `py_research-5.1.1/tests/py_research/test_db_importing.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_files.py` & `py_research-5.1.1/tests/py_research/test_files.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_geo.py` & `py_research-5.1.1/tests/py_research/test_geo.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_hashing.py` & `py_research-5.1.1/tests/py_research/test_hashing.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_intl.py` & `py_research-5.1.1/tests/py_research/test_intl.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_plots.py` & `py_research-5.1.1/tests/py_research/test_plots.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_ranking.py` & `py_research-5.1.1/tests/py_research/test_ranking.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_reflect.py` & `py_research-5.1.1/tests/py_research/test_reflect.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_stats.py` & `py_research-5.1.1/tests/py_research/test_stats.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_tables.py` & `py_research-5.1.1/tests/py_research/test_tables.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/tests/py_research/test_time.py` & `py_research-5.1.1/tests/py_research/test_time.py`

 * *Files identical despite different names*

### Comparing `py_research-5.1.0/PKG-INFO` & `py_research-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-research
-Version: 5.1.0
+Version: 5.1.1
 Summary: Collection of utilities for R&D coding in Python 🐍
 Author-Email: Lorenzo Wormer <l.wormer@mailbox.org>
 Project-URL: Documentation, https://cloudlane-one.github.io/py-research/
 Requires-Python: <3.12,>=3.10
 Requires-Dist: pandas<3.0,>=2.2.0
 Requires-Dist: PyYAML<7.0,>=6.0
 Requires-Dist: openpyxl<4.0.0,>=3.0.9
```

