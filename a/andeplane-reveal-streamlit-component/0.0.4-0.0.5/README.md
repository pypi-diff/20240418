# Comparing `tmp/andeplane_reveal_streamlit_component-0.0.4.tar.gz` & `tmp/andeplane_reveal_streamlit_component-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.4.tar", last modified: Thu Apr 18 18:43:34 2024, max compression
+gzip compressed data, was "andeplane_reveal_streamlit_component-0.0.5.tar", last modified: Thu Apr 18 19:49:43 2024, max compression
```

## Comparing `andeplane_reveal_streamlit_component-0.0.4.tar` & `andeplane_reveal_streamlit_component-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.881189 andeplane_reveal_streamlit_component-0.0.4/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:43:34.880830 andeplane_reveal_streamlit_component-0.0.4/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 18:18:10.000000 andeplane_reveal_streamlit_component-0.0.4/README.md
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.880009 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
--rw-r--r--   0 kvakkefly   (501) staff       (20)      354 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/requires.txt
--rw-r--r--   0 kvakkefly   (501) staff       (20)        8 2024-04-18 18:43:34.000000 andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/top_level.txt
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.878328 andeplane_reveal_streamlit_component-0.0.4/cognite/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.878400 andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/
-drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 18:43:34.879761 andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/reveal/
--rw-r--r--   0 kvakkefly   (501) staff       (20)     3705 2024-04-18 18:26:47.000000 andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/reveal/__init__.py
--rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 18:43:34.881250 andeplane_reveal_streamlit_component-0.0.4/setup.cfg
--rw-r--r--   0 kvakkefly   (501) staff       (20)     1094 2024-04-18 18:43:20.000000 andeplane_reveal_streamlit_component-0.0.4/setup.py
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 19:49:43.578328 andeplane_reveal_streamlit_component-0.0.5/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 19:49:43.578023 andeplane_reveal_streamlit_component-0.0.5/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1248 2024-04-18 18:18:10.000000 andeplane_reveal_streamlit_component-0.0.5/README.md
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 19:49:43.577243 andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1909 2024-04-18 19:49:43.000000 andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/PKG-INFO
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      354 2024-04-18 19:49:43.000000 andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/SOURCES.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 19:49:43.000000 andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/dependency_links.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)      140 2024-04-18 19:49:43.000000 andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/requires.txt
+-rw-r--r--   0 kvakkefly   (501) staff       (20)        1 2024-04-18 19:49:43.000000 andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/top_level.txt
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 19:49:43.573306 andeplane_reveal_streamlit_component-0.0.5/cognite/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 19:49:43.573375 andeplane_reveal_streamlit_component-0.0.5/cognite/streamlit/
+drwxr-xr-x   0 kvakkefly   (501) staff       (20)        0 2024-04-18 19:49:43.576301 andeplane_reveal_streamlit_component-0.0.5/cognite/streamlit/reveal/
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     3714 2024-04-18 19:49:38.000000 andeplane_reveal_streamlit_component-0.0.5/cognite/streamlit/reveal/__init__.py
+-rw-r--r--   0 kvakkefly   (501) staff       (20)       38 2024-04-18 19:49:43.578383 andeplane_reveal_streamlit_component-0.0.5/setup.cfg
+-rw-r--r--   0 kvakkefly   (501) staff       (20)     1162 2024-04-18 19:49:29.000000 andeplane_reveal_streamlit_component-0.0.5/setup.py
```

### Comparing `andeplane_reveal_streamlit_component-0.0.4/PKG-INFO` & `andeplane_reveal_streamlit_component-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.4
+Version: 0.0.5
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
```

### Comparing `andeplane_reveal_streamlit_component-0.0.4/README.md` & `andeplane_reveal_streamlit_component-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `andeplane_reveal_streamlit_component-0.0.4/andeplane_reveal_streamlit_component.egg-info/PKG-INFO` & `andeplane_reveal_streamlit_component-0.0.5/andeplane_reveal_streamlit_component.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: andeplane_reveal_streamlit_component
-Version: 0.0.4
+Version: 0.0.5
 Summary: Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion
 Home-page: 
 Author: John Smith
 Author-email: john@example.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit>=0.63
```

### Comparing `andeplane_reveal_streamlit_component-0.0.4/cognite/streamlit/reveal/__init__.py` & `andeplane_reveal_streamlit_component-0.0.5/cognite/streamlit/reveal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,17 +69,15 @@
     """
     # Call through to our private component function. Arguments we pass here
     # will be sent to the frontend, where they'll be available in an "args"
     # dictionary.
     #
     # "default" is a special argument that specifies the initial return
     # value of the component before the user has interacted with it.
-    import os 
-    token = os.getenv('COGNITE_TOKEN')
     base_url = client.config.base_url
     project = client.config.project
-
+    _, token = client.config.credentials.authorization_header()
     component_value = _component_func(model_id=model_id, revision_id=revision_id, token=token, base_url=base_url, project=project, key=key, default=0)
     
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
```

### Comparing `andeplane_reveal_streamlit_component-0.0.4/setup.py` & `andeplane_reveal_streamlit_component-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="andeplane_reveal_streamlit_component",
-    version="0.0.4",
+    version="0.0.5",
     author="John Smith",
     author_email="john@example.com",
     description="Streamlit wrapper for Cognite Reveal to view 3D content from Cognite Data Fsion",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
-    packages=['cognite.streamlit.reveal'],
+    packages=setuptools.find_packages(),
+    package_data={'cognite/streamlite/reveal': ['frontend/build/*']},
     include_package_data=True,
     classifiers=[],
     python_requires=">=3.7",
     install_requires=[
         # By definition, a Custom Component depends on Streamlit.
         # If your component has other Python dependencies, list
         # them here.
```

