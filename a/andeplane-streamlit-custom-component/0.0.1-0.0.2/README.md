# Comparing `tmp/andeplane_streamlit_custom_component-0.0.1.tar.gz` & `tmp/andeplane_streamlit_custom_component-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_streamlit_custom_component-0.0.1.tar", last modified: Thu Apr 18 12:00:50 2024, max compression
+gzip compressed data, was "andeplane_streamlit_custom_component-0.0.2.tar", last modified: Thu Apr 18 12:14:15 2024, max compression
```

## Comparing `andeplane_streamlit_custom_component-0.0.1.tar` & `andeplane_streamlit_custom_component-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 12:00:50.479299 andeplane_streamlit_custom_component-0.0.1/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1063 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.1/LICENSE
--rw-r--r--   0 kvakkefly   (501) staff       (20)       48 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.1/MANIFEST.in
--rw-r--r--   0 kvakkefly   (501) staff       (20)      942 2024-04-18 12:00:50.479025 andeplane_streamlit_custom_component-0.0.1/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      294 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.1/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 12:00:50.478293 andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)      942 2024-04-18 12:00:50.000000 andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      386 2024-04-18 12:00:50.000000 andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 12:00:50.000000 andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 12:00:50.000000 andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)       13 2024-04-18 12:00:50.000000 andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/top_level.txt
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 12:00:50.477863 andeplane_streamlit_custom_component-0.0.1/my_component/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3437 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.1/my_component/__init__.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1179 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.1/my_component/example.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 12:00:50.479349 andeplane_streamlit_custom_component-0.0.1/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1056 2024-04-18 12:00:04.000000 andeplane_streamlit_custom_component-0.0.1/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 12:14:15.229286 andeplane_streamlit_custom_component-0.0.2/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1063 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.2/LICENSE
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       48 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.2/MANIFEST.in
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      942 2024-04-18 12:14:15.229005 andeplane_streamlit_custom_component-0.0.2/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      294 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.2/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 12:14:15.228259 andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      942 2024-04-18 12:14:15.000000 andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      386 2024-04-18 12:14:15.000000 andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 12:14:15.000000 andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 12:14:15.000000 andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       13 2024-04-18 12:14:15.000000 andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 12:14:15.227854 andeplane_streamlit_custom_component-0.0.2/my_component/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3436 2024-04-18 12:13:46.000000 andeplane_streamlit_custom_component-0.0.2/my_component/__init__.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1179 2024-04-18 11:57:50.000000 andeplane_streamlit_custom_component-0.0.2/my_component/example.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 12:14:15.229331 andeplane_streamlit_custom_component-0.0.2/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1056 2024-04-18 12:13:55.000000 andeplane_streamlit_custom_component-0.0.2/setup.py
```

### Comparing `andeplane_streamlit_custom_component-0.0.1/LICENSE` & `andeplane_streamlit_custom_component-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `andeplane_streamlit_custom_component-0.0.1/PKG-INFO` & `andeplane_streamlit_custom_component-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane-streamlit-custom-component
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to do X
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `andeplane_streamlit_custom_component-0.0.1/andeplane_streamlit_custom_component.egg-info/PKG-INFO` & `andeplane_streamlit_custom_component-0.0.2/andeplane_streamlit_custom_component.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane-streamlit-custom-component
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component that allows you to do X
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `andeplane_streamlit_custom_component-0.0.1/my_component/__init__.py` & `andeplane_streamlit_custom_component-0.0.2/my_component/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import streamlit.components.v1 as components
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
```

### Comparing `andeplane_streamlit_custom_component-0.0.1/my_component/example.py` & `andeplane_streamlit_custom_component-0.0.2/my_component/example.py`

 * *Files identical despite different names*

### Comparing `andeplane_streamlit_custom_component-0.0.1/setup.py` & `andeplane_streamlit_custom_component-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane-streamlit-custom-component",
-    version="0.0.1",
+    version="0.0.2",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit component that allows you to do X",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

