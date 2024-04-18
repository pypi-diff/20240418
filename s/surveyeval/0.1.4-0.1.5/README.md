# Comparing `tmp/surveyeval-0.1.4.tar.gz` & `tmp/surveyeval-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surveyeval-0.1.4.tar", last modified: Tue Apr 16 21:15:06 2024, max compression
+gzip compressed data, was "surveyeval-0.1.5.tar", last modified: Wed Apr 17 18:39:30 2024, max compression
```

## Comparing `surveyeval-0.1.4.tar` & `surveyeval-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.399664 surveyeval-0.1.4/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.4/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-16 21:15:06.399381 surveyeval-0.1.4/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)    10689 2024-04-16 21:14:57.000000 surveyeval-0.1.4/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-16 21:15:06.399724 surveyeval-0.1.4/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     1349 2024-04-16 21:14:57.000000 surveyeval-0.1.4/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.393694 surveyeval-0.1.4/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.397197 surveyeval-0.1.4/src/surveyeval/
--rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.4/src/surveyeval/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.4/src/surveyeval/core_evaluation_lenses.py
--rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.4/src/surveyeval/evaluation_engine.py
--rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.4/src/surveyeval/survey_parser.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 21:15:06.398980 surveyeval-0.1.4/src/surveyeval.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-16 21:15:06.000000 surveyeval-0.1.4/src/surveyeval.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.946281 surveyeval-0.1.5/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.5/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-17 18:39:30.946018 surveyeval-0.1.5/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10689 2024-04-16 21:14:57.000000 surveyeval-0.1.5/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-17 18:39:30.946342 surveyeval-0.1.5/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     1349 2024-04-17 18:39:29.000000 surveyeval-0.1.5/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.940681 surveyeval-0.1.5/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.943627 surveyeval-0.1.5/src/surveyeval/
+-rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-17 18:39:29.000000 surveyeval-0.1.5/src/surveyeval/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.5/src/surveyeval/core_evaluation_lenses.py
+-rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.5/src/surveyeval/evaluation_engine.py
+-rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.5/src/surveyeval/survey_parser.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-17 18:39:30.945609 surveyeval-0.1.5/src/surveyeval.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    11239 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)      118 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-17 18:39:30.000000 surveyeval-0.1.5/src/surveyeval.egg-info/top_level.txt
```

### Comparing `surveyeval-0.1.4/LICENSE` & `surveyeval-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.4/PKG-INFO` & `surveyeval-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
```

### Comparing `surveyeval-0.1.4/README.rst` & `surveyeval-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.4/setup.py` & `surveyeval-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='surveyeval',
-    version='0.1.4',
+    version='0.1.5',
     packages=['surveyeval'],
     python_requires='>=3.10',
     install_requires=[
         'tiktoken~=0.5.2',
         'openai~=1.10.0',
         'langchain~=0.1.15',
         'langchain-openai~=0.0.5',
```

### Comparing `surveyeval-0.1.4/src/surveyeval/__init__.py` & `surveyeval-0.1.5/src/surveyeval/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 #  limitations under the License.
 
 from .evaluation_engine import EvaluationEngine, EvaluationLens
 from .core_evaluation_lenses import (BiasEvaluationLens, PhrasingEvaluationLens, TranslationEvaluationLens,
                                      ValidatedInstrumentEvaluationLens)
 
 # report our current version, as installed
-from importlib_metadata import version
+from importlib.metadata import version
 try:
     __version__ = version("surveyeval")
 except Exception:
     # (ignore exceptions when developing and testing locally)
     pass
```

### Comparing `surveyeval-0.1.4/src/surveyeval/core_evaluation_lenses.py` & `surveyeval-0.1.5/src/surveyeval/core_evaluation_lenses.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.4/src/surveyeval/evaluation_engine.py` & `surveyeval-0.1.5/src/surveyeval/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.4/src/surveyeval/survey_parser.py` & `surveyeval-0.1.5/src/surveyeval/survey_parser.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.4/src/surveyeval.egg-info/PKG-INFO` & `surveyeval-0.1.5/src/surveyeval.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.4
+Version: 0.1.5
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
```

