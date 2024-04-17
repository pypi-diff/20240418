# Comparing `tmp/django_monkey_patches-2.5.1.tar.gz` & `tmp/django_monkey_patches-2.6.0.tar.gz`

## Comparing `django_monkey_patches-2.5.1.tar` & `django_monkey_patches-2.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/README_printable.md
--rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/build_and_checks.sh
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/build_readme.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    24809 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/COPYING.LESSER
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/pyproject.toml
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/README_printable.md
+-rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/build_and_checks.sh
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/build_readme.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    25621 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/COPYING.LESSER
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/PKG-INFO
```

### Comparing `django_monkey_patches-2.5.1/README_printable.md` & `django_monkey_patches-2.6.0/README_printable.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/build_and_checks.sh` & `django_monkey_patches-2.6.0/build_and_checks.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/build_readme.sh` & `django_monkey_patches-2.6.0/build_readme.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import time
 import traceback
 
 # pylint: disable-next=import-error
 from django.db import connections
 
 # Remind that you can modify the constants below during execution:
-# import django__query_wrapper
+# from django_monkey_patches import django__query_wrapper
 # django__query_wrapper.COUNT_QUERIES = True
 # ... the code I'm looking at closely
 # django__query_wrapper.COUNT_QUERIES = False
 # logger.info(f"Number of queries : {...}")
 
 # Why you may want to throttle queries?
 # To see the impact of some conditions,
@@ -110,14 +110,15 @@
 
         def __call__(self, request):
             # Optional but recommended, see below.
             # At least an equivalent is needed,
             # if you activate COUNT_QUERIES.
             init_connections_extra_data_v1()
 
+            # See at end of file to wrap all connections.
             with connection.execute_wrapper(custom_query_wrapper_v1):
                 return self.get_response(request)
 
     In settings.py, add:
     # ######### MIDDLEWARE CONFIGURATION
     MIDDLEWARE = (
         ...
@@ -131,14 +132,15 @@
         ...
         def execute(self, *args, **options):
             # Copy the code of BaseCommand.execute()
             # And in it replace at least:
             #   output = self.handle(*args, **options)
             # with:
             with connection.execute_wrapper(custom_query_wrapper_v1):
+                # See at end of file to wrap all connections.
                 output = self.handle(*args, **options)
         ...
     And then, make all your commands inherit from CustomBaseCommand.
     You can go way further
     in this line of customization and monitoring.
     """
 
@@ -628,21 +630,44 @@
     main_dict[some_sub_dict_key] = (
         reorder_dict_by_total_duration_of_sub_dicts(
             main_dict[some_sub_dict_key]
         )
     )
 
 
+def wrap_connections(
+    exit_stack,
+    custom_query_wrapper,
+    connections_to_wrap=None,
+):
+    """
+    Apply the context-manager connection.execute_wrapper()
+    with the given custom_query_wrapper
+    on an ExitStack() instance,
+    for given connections or all connections if none is given.
+    """
+
+    if connections_to_wrap is None:
+        connections_to_wrap = connections
+    for connection_key in connections:
+        connection = connections[connection_key]
+        exit_stack.enter_context(
+            connection.execute_wrapper(custom_query_wrapper)
+        )
+
+
 # You should extract the data to logs or files,
 # during execution or at the end,
 # using custom insertion_callback or post_processing_callback.
 # Here is an example of intermediate complexity
 # using all of the above.
 #
-# import django_monkey_patches.django__query_wrapper
+# from contextlib import ExitStack
+#
+# from django_monkey_patches import django__query_wrapper
 # from django_monkey_patches.django__query_wrapper import (
 #     apply_reorder_dict_by_total_duration_of_sub_dicts_to,
 #     custom_query_wrapper_v1,
 #     get_extra_data_template_for_set_of_queries_v1,
 #     get_sql_signature_v1,
 #     init_connections_extra_data_v1,
 #     insert_in_connections_extra_data_v1,
@@ -706,15 +731,16 @@
 #             lambda x: (
 #               apply_reorder_dict_by_total_duration_of_sub_dicts_to(
 #                 x["allocated_subsets_extra_data"],
 #                 "per_sql_signature_v1",
 #               )
 #             )
 #         )
-#         with connection.execute_wrapper(custom_query_wrapper_v1):
+#         with ExitStack() as exit_stack:
+#             wrap_connections(exit_stack, custom_query_wrapper_v1)
 #             response = self.get_response(request)
 #             synthetize_connections_extra_data_v1()
 #             # dump to file or log:
 #             # connections.django_monkey_patches_dict
 #             # for connection_key in connections:
 #             #     some_connection = connections[connection_key]
 #             #     # dump to file or log:
```

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/COPYING` & `django_monkey_patches-2.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/COPYING.LESSER` & `django_monkey_patches-2.6.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/README.md` & `django_monkey_patches-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.5.1/pyproject.toml` & `django_monkey_patches-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "2.5.1"
+version = "2.6.0"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `django_monkey_patches-2.5.1/PKG-INFO` & `django_monkey_patches-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 2.5.1
+Version: 2.6.0
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

