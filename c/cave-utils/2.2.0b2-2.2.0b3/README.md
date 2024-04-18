# Comparing `tmp/cave_utils-2.2.0b2.tar.gz` & `tmp/cave_utils-2.2.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-2.2.0b2.tar", last modified: Thu Mar 14 15:26:16 2024, max compression
+gzip compressed data, was "cave_utils-2.2.0b3.tar", last modified: Thu Apr 18 18:34:26 2024, max compression
```

## Comparing `cave_utils-2.2.0b2.tar` & `cave_utils-2.2.0b3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.127748 cave_utils-2.2.0b2/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b2/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b2/NOTICE.md
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-03-14 15:26:16.127748 cave_utils-2.2.0b2/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b2/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.123748 cave_utils-2.2.0b2/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      414 2024-03-04 18:45:40.000000 cave_utils-2.2.0b2/cave_utils/__init__.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.123748 cave_utils-2.2.0b2/cave_utils/api/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     8244 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/api/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     5002 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/api/appBar.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1063 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/api/extraKwargs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2210 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/api/globalOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    15834 2024-01-31 16:20:08.000000 cave_utils-2.2.0b2/cave_utils/api/groupedOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11210 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/api/mapFeatures.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    30324 2024-02-26 14:04:23.000000 cave_utils-2.2.0b2/cave_utils/api/maps.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12609 2024-01-31 16:20:08.000000 cave_utils-2.2.0b2/cave_utils/api/pages.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     7085 2024-01-31 16:20:08.000000 cave_utils-2.2.0b2/cave_utils/api/panes.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    14720 2024-01-31 16:20:08.000000 cave_utils-2.2.0b2/cave_utils/api/settings.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.123748 cave_utils-2.2.0b2/cave_utils/api_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b2/cave_utils/api_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    33939 2024-01-31 16:20:08.000000 cave_utils-2.2.0b2/cave_utils/api_utils/general.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      980 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/api_utils/validator.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12799 2024-01-19 21:36:14.000000 cave_utils-2.2.0b2/cave_utils/api_utils/validator_utils.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b2/cave_utils/arguments.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.123748 cave_utils-2.2.0b2/cave_utils/builders/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b2/cave_utils/builders/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b2/cave_utils/builders/groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-2.2.0b2/cave_utils/socket.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.127748 cave_utils-2.2.0b2/cave_utils.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-03-14 15:26:16.000000 cave_utils-2.2.0b2/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      895 2024-03-14 15:26:16.000000 cave_utils-2.2.0b2/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-03-14 15:26:16.000000 cave_utils-2.2.0b2/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-03-14 15:26:16.000000 cave_utils-2.2.0b2/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-03-14 15:26:16.000000 cave_utils-2.2.0b2/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-03-14 15:23:32.000000 cave_utils-2.2.0b2/pyproject.toml
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-03-14 15:26:16.127748 cave_utils-2.2.0b2/setup.cfg
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-03-14 15:26:16.127748 cave_utils-2.2.0b2/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b2/test/test_builders_groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b2/test/test_import.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b2/test/test_log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b2/test/test_validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b3/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b3/NOTICE.md
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b3/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      414 2024-03-04 18:45:40.000000 cave_utils-2.2.0b3/cave_utils/__init__.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/api/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     8244 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     5002 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/appBar.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1063 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/extraKwargs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2210 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/globalOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    16980 2024-04-18 16:17:39.000000 cave_utils-2.2.0b3/cave_utils/api/groupedOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11210 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/mapFeatures.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    30324 2024-02-26 14:04:23.000000 cave_utils-2.2.0b3/cave_utils/api/maps.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12779 2024-04-18 18:22:52.000000 cave_utils-2.2.0b3/cave_utils/api/pages.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     7085 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/cave_utils/api/panes.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    14720 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/cave_utils/api/settings.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/api_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b3/cave_utils/api_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    33939 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/cave_utils/api_utils/general.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      980 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api_utils/validator.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12799 2024-01-19 21:36:14.000000 cave_utils-2.2.0b3/cave_utils/api_utils/validator_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b3/cave_utils/arguments.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/builders/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b3/cave_utils/builders/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b3/cave_utils/builders/groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-2.2.0b3/cave_utils/socket.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/cave_utils.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      895 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-04-18 18:31:36.000000 cave_utils-2.2.0b3/pyproject.toml
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b3/test/test_builders_groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b3/test/test_import.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/test/test_log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/test/test_validator.py
```

### Comparing `cave_utils-2.2.0b2/LICENSE` & `cave_utils-2.2.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/NOTICE.md` & `cave_utils-2.2.0b3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/PKG-INFO` & `cave_utils-2.2.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b2
+Version: 2.2.0b3
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b2/README.md` & `cave_utils-2.2.0b3/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/__init__.py` & `cave_utils-2.2.0b3/cave_utils/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/appBar.py` & `cave_utils-2.2.0b3/cave_utils/api/appBar.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/extraKwargs.py` & `cave_utils-2.2.0b3/cave_utils/api/extraKwargs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/globalOutputs.py` & `cave_utils-2.2.0b3/cave_utils/api/globalOutputs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/groupedOutputs.py` & `cave_utils-2.2.0b3/cave_utils/api/groupedOutputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,21 +275,21 @@
             },
         }
 
     def __extend_spec__(self, **kwargs):
         levels_data = self.data.get("levels", {})
         levels_data_keys = list(levels_data.keys())
         data_data = self.data.get("data", {})
-
         CustomKeyValidator(
             data=levels_data,
             log=self.log,
             prepend_path=["levels"],
             validator=groupedOutputs_groupings_star_levels_star,
             acceptable_parents=levels_data_keys,
+            acceptable_data_levels=data_data,
             **kwargs,
         )
         groupedOutputs_groupings_star_data(
             data=data_data,
             log=self.log,
             prepend_path=["data"],
             acceptable_data_keys=levels_data_keys,
@@ -344,43 +344,58 @@
 @type_enforced.Enforcer
 class groupedOutputs_groupings_star_levels_star(ApiValidator):
     """
     The level data is located under the path **`groupedOutputs.groupings.*.levels.*`**.
     """
 
     @staticmethod
-    def spec(name: str, parent: [str, None] = None, ordering: [list, None] = None, **kwargs):
+    def spec(name: str, parent: [str, None] = None, ordering: [list, None] = None, orderWithParent: bool = True, coloring: [dict, None] = None, **kwargs):
         """
         Arguments:
 
         * **`name`**: `[str]` &rarr; The name of the level.
         * **`parent`**: `[str]` &rarr;
             * The key of the parent level. This is used to create a hierarchy of levels.
             * **Notes**:
                 * The parent level key must be defined in `groupedOutputs.groupings.*.levels.*`
                 * If `None`, this will be considered to be the root of the hierarchy.
+        * **`ordering`**: `[list]` &rarr;
+            * The ordering of individual values for this level in charts and tables.
+            * **Note**: If none, the ordering will be alphabetical.
+            * **Note**: If a partial ordering is provided, the provided values will be placed first in order.
+            * **Note**: If a partial ordering is provided, the remaining values will be placed in alphabetical order.
+            * **Note**: All items in this list must be defined in `groupedOutputs.groupings.*.levels.*.values.*`
+        * **`orderWithParent`**: `[bool]`=True &rarr;
+            * Weather or not to order this level based on the parent level.
+            * If `True`, the ordering of this level will also be based on the parent level.
+            * If `False`, the ordering will be based on the ordering of this level only.
+        * **`coloring`**: `[dict]` &rarr;
+            * A dictionary of colors to be used for the level.
+            * Each key in this dictionary is a value in the level.
+            * Each value in this dictionary is an rgba string.
+            * **See**: `cave_utils.api.groupedOutputs.groupedOutputs_groupings_star_levels_star_coloring`
         """
-        # TODO: Figure out new way for ordering
-        # - `ordering`:
-        #     - Type: list
-        #     - What: The ordering of individual values for this level in charts and tables.
-        #     - Note: If none, the ordering will be alphabetical.
-        #     - Note: If a partial ordering is provided, the provided values will be placed first in order.
-        #     - Note: If a partial ordering is provided, the remaining values will be placed in alphabetical order.
-        #     - Note: All items in this list must be defined in `groupedOutputs.groupings.*.levels.*.values.*`
-        # """
         return {"kwargs": kwargs, "accepted_values": {}}
 
     def __extend_spec__(self, **kwargs):
         parent = self.data.get("parent")
         if parent is not None:
             self.__check_subset_valid__(
                 subset=[parent],
                 valid_values=kwargs.get("acceptable_parents", []),
                 prepend_path=["parent"],
             )
-        # ordering = self.data.get("ordering")
-        # if ordering is not None:
-        #     print(ordering, kwargs.get("acceptable_data_keys", []))
-        #     self.__check_subset_valid__(
-        #         subset=ordering, valid_values=kwargs.get("acceptable_data_keys", []), prepend_path=["ordering"]
-        #     )
+        ordering = self.data.get("ordering")
+        if ordering is not None:
+            self.__check_subset_valid__(
+                subset=ordering, valid_values=kwargs.get("acceptable_data_levels", {}).get(kwargs.get('CustomKeyValidatorFieldId'),[]), prepend_path=["ordering"]
+            )
+
+        coloring = self.data.get("coloring")
+        if coloring is not None:
+            self.__check_subset_valid__(
+                subset=list(coloring.keys()),
+                valid_values=kwargs.get("acceptable_data_levels", {}).get(kwargs.get('CustomKeyValidatorFieldId'),[]),
+                prepend_path=["coloring"],
+            )
+            for key, value in coloring.items():
+                self.__check_rgba_string_valid__(rgba_string=value, prepend_path=['coloring', key])
```

### Comparing `cave_utils-2.2.0b2/cave_utils/api/mapFeatures.py` & `cave_utils-2.2.0b3/cave_utils/api/mapFeatures.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/maps.py` & `cave_utils-2.2.0b3/cave_utils/api/maps.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/pages.py` & `cave_utils-2.2.0b3/cave_utils/api/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         groupingLevel: [list, None] = None,
         lockedLayout: bool = False,
         statAggregation: str = "sum",
         groupedOutputDataId: [str, list, None] = None,
         statId: [str, list, None] = None,
         showToolbar: bool = True,
         maximized: bool = False,
+        defaultToZero: bool = False,
         **kwargs,
     ):
         """
         Arguments:
 
         * **`type`**: `[str]` = `"groupedOutput"` &rarr; The type of the page layout.
             * **Accepted Values**:
@@ -131,15 +132,16 @@
                 * `"max"`: Find the maximum values the aggregated data
         * **`groupedOutputDataId`**: `[str | list]` = `None` &rarr; The id or list of ids representing the grouped output data to use.
         * **`statId`**: `[str | list]` = `None` &rarr; The id or list of ids corresponding to the stat(s) to be used.
         * **`showToolbar`**: `[bool]` = `None` &rarr; Whether or not the chart toolbar should be shown.
             * **Note**: If left unspecified (i.e., `None`), it will default to `settings.showToolbar`.
         * **`maximized`**: `[bool]` = `False` &rarr; Whether or not the layout should be maximized.
             * **Note**: If more than one chart belonging to the same page layout is set to `True`, the first one found in the list will take precedence.
-
+        * **`defaultToZero`**: `[bool]` = `False` &rarr; Whether or not the chart should default missing values to zero.
+            
         [area chart]: https://en.wikipedia.org/wiki/Area_chart
         [bar chart]: https://en.wikipedia.org/wiki/Bar_chart
         [stacked bar chart]: https://en.wikipedia.org/wiki/Bar_chart
         [box plot chart]: https://en.wikipedia.org/wiki/Box_plot
         [cumulative line chart]: #
         [gauge chart]: https://echarts.apache.org/examples/en/index.html#chart-type-gauge
         [heatmap chart]: https://en.wikipedia.org/wiki/Heat_map
```

### Comparing `cave_utils-2.2.0b2/cave_utils/api/panes.py` & `cave_utils-2.2.0b3/cave_utils/api/panes.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api/settings.py` & `cave_utils-2.2.0b3/cave_utils/api/settings.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api_utils/general.py` & `cave_utils-2.2.0b3/cave_utils/api_utils/general.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api_utils/validator.py` & `cave_utils-2.2.0b3/cave_utils/api_utils/validator.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/api_utils/validator_utils.py` & `cave_utils-2.2.0b3/cave_utils/api_utils/validator_utils.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/arguments.py` & `cave_utils-2.2.0b3/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/builders/groups.py` & `cave_utils-2.2.0b3/cave_utils/builders/groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils/log.py` & `cave_utils-2.2.0b3/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/cave_utils.egg-info/PKG-INFO` & `cave_utils-2.2.0b3/cave_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b2
+Version: 2.2.0b3
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b2/cave_utils.egg-info/SOURCES.txt` & `cave_utils-2.2.0b3/cave_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/pyproject.toml` & `cave_utils-2.2.0b3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cave_utils"
-version = "2.2.0b2"
+version = "2.2.0b3"
 description = "Python wrapper for api use in the cave_app"
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cave_utils-2.2.0b2/test/test_builders_groups.py` & `cave_utils-2.2.0b3/test/test_builders_groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b2/test/test_validator.py` & `cave_utils-2.2.0b3/test/test_validator.py`

 * *Files identical despite different names*

