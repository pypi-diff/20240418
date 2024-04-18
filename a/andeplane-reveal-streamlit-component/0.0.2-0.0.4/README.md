# Comparing `tmp/andeplane_reveal_streamlit_component-0.0.2.tar.gz` & `tmp/andeplane_reveal_streamlit_component-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.2.tar", last modified: Thu Apr 18 18:21:46 2024, max compression
+gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.4.tar", last modified: Thu Apr 18 18:43:34 2024, max compression
```

## Comparing `andeplane_reveal_streamlit_component-0.0.2.tar` & `andeplane_reveal_streamlit_component-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:21:46.812760 andeplane_reveal_streamlit_component-0.0.2/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:21:46.812527 andeplane_reveal_streamlit_component-0.0.2/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 18:18:10.000000 andeplane_reveal_streamlit_component-0.0.2/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:21:46.811934 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      317 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/top_level.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 18:21:46.812802 andeplane_reveal_streamlit_component-0.0.2/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1092 2024-04-18 18:21:32.000000 andeplane_reveal_streamlit_component-0.0.2/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.881189 andeplane_reveal_streamlit_component-0.0.4/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:43:34.880830 andeplane_reveal_streamlit_component-0.0.4/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 18:18:10.000000 andeplane_reveal_streamlit_component-0.0.4/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.880009 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      354 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        8 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.878328 andeplane_reveal_streamlit_component-0.0.4/cognite/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.878400 andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.879761 andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3705 2024-04-18 18:26:47.000000 andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/reveal/__init__.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 18:43:34.881250 andeplane_reveal_streamlit_component-0.0.4/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1094 2024-04-18 18:43:20.000000 andeplane_reveal_streamlit_component-0.0.4/setup.py
```

### Comparing `andeplane_reveal_streamlit_component-0.0.2/PKG-INFO` & `andeplane_reveal_streamlit_component-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.2
+Version: 0.0.4
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
```

### Comparing `andeplane_reveal_streamlit_component-0.0.2/README.md` & `andeplane_reveal_streamlit_component-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/PKG-INFO` & `andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.2
+Version: 0.0.4
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
```

### Comparing `andeplane_reveal_streamlit_component-0.0.2/setup.py` & `andeplane_reveal_streamlit_component-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane_reveal_streamlit_component",
-    version="0.0.2",
+    version="0.0.4",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
-    packages=setuptools.find_packages(),
+    packages=['cognite.streamlit.reveal'],
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.7",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
```

