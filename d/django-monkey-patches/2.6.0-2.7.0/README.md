# Comparing `tmp/django_monkey_patches-2.6.0.tar.gz` & `tmp/django_monkey_patches-2.7.0.tar.gz`

## Comparing `django_monkey_patches-2.6.0.tar` & `django_monkey_patches-2.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/README_printable.md
--rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/build_and_checks.sh
--rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/build_readme.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/__init__.py
--rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
--rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set.py
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get_or_create.py
--rw-r--r--   0        0        0    25621 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_wrapper.py
--rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django__test_case__tear_down.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/PKG-INFO
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/requires.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/top_level.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/COPYING
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/COPYING.LESSER
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/pyproject.toml
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/README_printable.md
+-rwxr-xr-x   0        0        0     1646 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/build_and_checks.sh
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/build_readme.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/__init__.py
+-rw-r--r--   0        0        0    39138 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__base_cache__make_cache_key.py
+-rw-r--r--   0        0        0    15301 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set.py
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get_or_create.py
+-rw-r--r--   0        0        0    26767 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_wrapper.py
+-rw-r--r--   0        0        0     7538 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django__test_case__tear_down.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__field__get_request.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/requires.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/top_level.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/COPYING
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/COPYING.LESSER
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 django_monkey_patches-2.7.0/PKG-INFO
```

### Comparing `django_monkey_patches-2.6.0/README_printable.md` & `django_monkey_patches-2.7.0/README_printable.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/build_and_checks.sh` & `django_monkey_patches-2.7.0/build_and_checks.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/build_readme.sh` & `django_monkey_patches-2.7.0/build_readme.sh`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/dev_side_code__django__orm__prefetch_1.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__base_cache__make_cache_key.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__base_cache__make_cache_key.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__orm__prefetch_without_useless_order_by.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_set__get_or_create.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_set__get_or_create.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__query_wrapper.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__query_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -413,19 +413,21 @@
     You should call this function or a custom one
     before using the custom query wrapper.
     """
 
     connections.django_monkey_patches_dict = (
         get_extra_data_template_for_set_of_queries_v1()
     )
+    connections.django_monkey_patches_stash_stack = []
     for connection_key in connections:
         connection = connections[connection_key]
         connection.django_monkey_patches_dict = (
             get_extra_data_template_for_set_of_queries_v1()
         )
+        connection.django_monkey_patches_stash_stack = []
 
 
 # pylint: disable-next=too-many-arguments
 def insert_in_connections_extra_data_v1(
     execute,
     sql,
     params,
@@ -644,21 +646,55 @@
     with the given custom_query_wrapper
     on an ExitStack() instance,
     for given connections or all connections if none is given.
     """
 
     if connections_to_wrap is None:
         connections_to_wrap = connections
-    for connection_key in connections:
+    for connection_key in connections_to_wrap:
         connection = connections[connection_key]
         exit_stack.enter_context(
             connection.execute_wrapper(custom_query_wrapper)
         )
 
 
+def stash_extra_data_dicts():
+    """
+    Stash current django_monkey_patches_dicts
+    in django_monkey_patches_stash_stacks.
+    """
+
+    connections.django_monkey_patches_stash_stack.append(
+        connections.django_monkey_patches_dict
+    )
+    connections.django_monkey_patches_dict = None
+    for connection_key in connections:
+        connection = connections[connection_key]
+        connection.django_monkey_patches_stash_stack.append(
+            connection.django_monkey_patches_dict
+        )
+        connection.django_monkey_patches_dict = None
+
+
+def pop_extra_data_dicts():
+    """
+    Pop last dicts in django_monkey_patches_stash_stacks
+    to django_monkey_patches_dicts.
+    """
+
+    connections.django_monkey_patches_dict = (
+        connections.django_monkey_patches_stash_stack.pop()
+    )
+    for connection_key in connections:
+        connection = connections[connection_key]
+        connection.django_monkey_patches_dict = (
+            connection.django_monkey_patches_stash_stack.pop()
+        )
+
+
 # You should extract the data to logs or files,
 # during execution or at the end,
 # using custom insertion_callback or post_processing_callback.
 # Here is an example of intermediate complexity
 # using all of the above.
 #
 # from contextlib import ExitStack
```

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django__test_case__tear_down.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django__test_case__tear_down.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__field__get_request.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__field__get_request.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py` & `django_monkey_patches-2.7.0/src/django_monkey_patches/django_rest_framework__list_serializer__to_representation.py`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/PKG-INFO` & `django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/src/django_monkey_patches.egg-info/SOURCES.txt` & `django_monkey_patches-2.7.0/src/django_monkey_patches.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/COPYING` & `django_monkey_patches-2.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/COPYING.LESSER` & `django_monkey_patches-2.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/README.md` & `django_monkey_patches-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django_monkey_patches-2.6.0/pyproject.toml` & `django_monkey_patches-2.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-monkey-patches"
-version = "2.6.0"
+version = "2.7.0"
 description = """\
 Add monkey-patches to correct and enhance your favorite framework\
 """
 readme = "README.md"
 authors = [
     { name = "Laurent Lyaudet", email = "laurent.lyaudet@gmail.com" },
 ]
```

### Comparing `django_monkey_patches-2.6.0/PKG-INFO` & `django_monkey_patches-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-monkey-patches
-Version: 2.6.0
+Version: 2.7.0
 Summary: Add monkey-patches to correct and enhance your favorite framework
 Project-URL: Homepage, https://github.com/LLyaudet/django-monkey-patches
 Project-URL: Bug Tracker, https://github.com/LLyaudet/django-monkey-patches/issues
 Author-email: Laurent Lyaudet <laurent.lyaudet@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

