# Comparing `tmp/andeplane_reveal_streamlit_component-0.0.1.tar.gz` & `tmp/andeplane_reveal_streamlit_component-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.1.tar", last modified: Thu Apr 18 17:44:44 2024, max compression
+gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.2.tar", last modified: Thu Apr 18 18:21:46 2024, max compression
```

## Comparing `andeplane_reveal_streamlit_component-0.0.1.tar` & `andeplane_reveal_streamlit_component-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 17:44:44.541372 andeplane_reveal_streamlit_component-0.0.1/
--rw-r--r--   0 kvakkefly   (501) staff       (20)      666 2024-04-18 17:44:44.541003 andeplane_reveal_streamlit_component-0.0.1/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)        4 2024-04-18 16:03:00.000000 andeplane_reveal_streamlit_component-0.0.1/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 17:44:44.540190 andeplane_reveal_streamlit_component-0.0.1/andeplane_reveal_streamlit_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)      666 2024-04-18 17:44:44.000000 andeplane_reveal_streamlit_component-0.0.1/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      342 2024-04-18 17:44:44.000000 andeplane_reveal_streamlit_component-0.0.1/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 17:44:44.000000 andeplane_reveal_streamlit_component-0.0.1/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 17:44:44.000000 andeplane_reveal_streamlit_component-0.0.1/andeplane_reveal_streamlit_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)       13 2024-04-18 17:44:44.000000 andeplane_reveal_streamlit_component-0.0.1/andeplane_reveal_streamlit_component.egg-info/top_level.txt
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 17:44:44.538898 andeplane_reveal_streamlit_component-0.0.1/my_component/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3546 2024-04-18 17:37:54.000000 andeplane_reveal_streamlit_component-0.0.1/my_component/__init__.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 17:44:44.541426 andeplane_reveal_streamlit_component-0.0.1/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1092 2024-04-18 17:44:12.000000 andeplane_reveal_streamlit_component-0.0.1/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:21:46.812760 andeplane_reveal_streamlit_component-0.0.2/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:21:46.812527 andeplane_reveal_streamlit_component-0.0.2/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 18:18:10.000000 andeplane_reveal_streamlit_component-0.0.2/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:21:46.811934 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      317 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 18:21:46.000000 andeplane_reveal_streamlit_component-0.0.2/andeplane_reveal_streamlit_component.egg-info/top_level.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 18:21:46.812802 andeplane_reveal_streamlit_component-0.0.2/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1092 2024-04-18 18:21:32.000000 andeplane_reveal_streamlit_component-0.0.2/setup.py
```

### Comparing `andeplane_reveal_streamlit_component-0.0.1/setup.py` & `andeplane_reveal_streamlit_component-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane_reveal_streamlit_component",
-    version="0.0.1",
+    version="0.0.2",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

