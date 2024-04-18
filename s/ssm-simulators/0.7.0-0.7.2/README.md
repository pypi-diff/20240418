# Comparing `tmp/ssm-simulators-0.7.0.tar.gz` & `tmp/ssm_simulators-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssm-simulators-0.7.0.tar", last modified: Sat Feb 10 02:26:49 2024, max compression
+gzip compressed data, was "ssm_simulators-0.7.2.tar", last modified: Thu Apr 18 09:44:07 2024, max compression
```

## Comparing `ssm-simulators-0.7.0.tar` & `ssm_simulators-0.7.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.011556 ssm-simulators-0.7.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)      208 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     7676 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:48.999556 ssm-simulators-0.7.0/notebooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)    66938 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/notebooks/basic_tutorial copy.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)    91101 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/notebooks/basic_tutorial.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)   197776 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/notebooks/basic_tutorial_tmp.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)   167793 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/notebooks/essential_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   413153 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/notebooks/test_deadline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   128693 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/notebooks/test_mic2_ornstein.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (127)     1137 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-10 02:26:49.011556 ssm-simulators-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      662 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.003556 ssm-simulators-0.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)  3593863 2024-02-10 02:26:48.000000 ssm-simulators-0.7.0/src/cssm.cpp
--rwxr-xr-x   0 runner    (1001) docker     (127)   189203 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/src/cssm.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/ssm_simulators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-02-10 02:26:48.000000 ssm-simulators-0.7.0/ssm_simulators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-02-10 02:26:48.000000 ssm-simulators-0.7.0/ssm_simulators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-10 02:26:48.000000 ssm-simulators-0.7.0/ssm_simulators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-10 02:26:48.000000 ssm-simulators-0.7.0/ssm_simulators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-10 02:26:48.000000 ssm-simulators-0.7.0/ssm_simulators.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/ssms/
--rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/ssms/basic_simulators/
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/basic_simulators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/basic_simulators/boundary_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4147 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/basic_simulators/drift_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31688 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/basic_simulators/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/ssms/config/
--rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/config/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    46552 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/ssms/dataset_generators/
--rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/dataset_generators/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33081 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/dataset_generators/lan_mlp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4171 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/dataset_generators/snpe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/ssms/support_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/support_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    30771 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/ssms/support_utils/kde_class.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-10 02:26:49.007556 ssm-simulators-0.7.0/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4200 2024-02-10 02:26:36.000000 ssm-simulators-0.7.0/tests/test_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1074 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)      208 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7676 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.737729 ssm_simulators-0.7.2/notebooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    66938 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/basic_tutorial copy.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)    91101 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/basic_tutorial.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)   197776 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/basic_tutorial_tmp.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)   167793 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/essential_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   413153 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/test_deadline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   128693 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/test_mic2_ornstein.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87773 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/notebooks/test_seq2.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      662 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.741729 ssm_simulators-0.7.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)  3814438 2024-04-18 09:44:06.000000 ssm_simulators-0.7.2/src/cssm.cpp
+-rwxr-xr-x   0 runner    (1001) docker     (127)   198206 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/src/cssm.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/ssm_simulators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8828 2024-04-18 09:44:07.000000 ssm_simulators-0.7.2/ssm_simulators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-18 09:44:07.000000 ssm_simulators-0.7.2/ssm_simulators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 09:44:07.000000 ssm_simulators-0.7.2/ssm_simulators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 09:44:07.000000 ssm_simulators-0.7.2/ssm_simulators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 09:44:07.000000 ssm_simulators-0.7.2/ssm_simulators.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/ssms/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      300 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/ssms/basic_simulators/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/basic_simulators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/basic_simulators/boundary_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4147 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/basic_simulators/drift_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34181 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/basic_simulators/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/ssms/config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      297 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48172 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/ssms/dataset_generators/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       72 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/dataset_generators/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32607 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/dataset_generators/lan_mlp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4171 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/dataset_generators/snpe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/ssms/support_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       49 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/support_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30771 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/ssms/support_utils/kde_class.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 09:44:07.745729 ssm_simulators-0.7.2/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3757 2024-04-18 09:43:58.000000 ssm_simulators-0.7.2/tests/test_simulator.py
```

### Comparing `ssm-simulators-0.7.0/LICENSE` & `ssm_simulators-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/PKG-INFO` & `ssm_simulators-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: ssm-simulators
-Version: 0.7.0
+Version: 0.7.2
 Summary: SSMS is a package collecting simulators and training data generators for a bunch of generative models of interest in the cognitive science / neuroscience and approximate bayesian computation communities
 Author-email: Alexander Fenger <alexander_fengler@brown.edu>
 Project-URL: Homepage, https://github.com/AlexanderFengler/ssm-simulators
 Project-URL: Bug Tracker, https://github.com/AlexanderFengler/ssm-simulators/issues
 Keywords: simulators,generative models,cognitive science,neuroscience
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.12,>3.8
+Requires-Python: <3.12,>3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: scipy>=1.6.3
-Requires-Dist: cython>=0.29.23
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: scikit-learn>=0.24.0
 Requires-Dist: psutil>=5.0.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `ssm-simulators-0.7.0/README.md` & `ssm_simulators-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/notebooks/basic_tutorial copy.ipynb` & `ssm_simulators-0.7.2/notebooks/basic_tutorial copy.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/notebooks/basic_tutorial.ipynb` & `ssm_simulators-0.7.2/notebooks/basic_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/notebooks/basic_tutorial_tmp.ipynb` & `ssm_simulators-0.7.2/notebooks/basic_tutorial_tmp.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/notebooks/essential_tests.ipynb` & `ssm_simulators-0.7.2/notebooks/essential_tests.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/notebooks/test_deadline.ipynb` & `ssm_simulators-0.7.2/notebooks/test_deadline.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/notebooks/test_mic2_ornstein.ipynb` & `ssm_simulators-0.7.2/notebooks/test_mic2_ornstein.ipynb`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/pyproject.toml` & `ssm_simulators-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 [project.urls]
 "Homepage"= "https://github.com/AlexanderFengler/ssm-simulators"
 "Bug Tracker"= "https://github.com/AlexanderFengler/ssm-simulators/issues"
 
 [project]
 name= "ssm-simulators"
-version= "0.7.0"
+version= "0.7.2"
 authors= [{name = "Alexander Fenger", email = "alexander_fengler@brown.edu"}]
 description= "SSMS is a package collecting simulators and training data generators for a bunch of generative models of interest in the cognitive science / neuroscience and approximate bayesian computation communities"
 readme = "README.md"
-requires-python= ">3.8, <3.12"
+requires-python= ">3.9, <3.12"
 classifiers= [
     "Development Status :: 1 - Planning",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering"
 ]
-dependencies=["numpy >= 1.17.0", "scipy >=1.6.3", "cython >= 0.29.23", "pandas >= 1.0.0", "scikit-learn >= 0.24.0", "psutil >= 5.0.0"]
+dependencies=["numpy >= 1.17.0", "scipy >=1.6.3", "pandas >= 1.0.0", "scikit-learn >= 0.24.0", "psutil >= 5.0.0"]
 keywords= ["simulators", "generative models", "cognitive science", "neuroscience"]
 
 [project.optional-dependencies]
 dev = ["black", "ruff", "pytest"]
```

### Comparing `ssm-simulators-0.7.0/setup.py` & `ssm_simulators-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/src/cssm.cpp` & `ssm_simulators-0.7.2/src/cssm.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "language": "c++",
         "name": "cssm",
@@ -34,18 +34,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -129,14 +129,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -190,14 +192,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -251,60 +255,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -387,14 +414,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -746,16 +776,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1099,15 +1134,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1186,15 +1221,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1300,32 +1335,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1657,177 +1675,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1860,42 +1878,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2777,14 +2795,17 @@
 static void __Pyx_RaiseMappingExpectedError(PyObject* arg);
 
 #define __Pyx_BufPtrStrided2d(type, buf, i0, s0, i1, s1) (type)((char*)buf + i0 * s0 + i1 * s1)
 /* PyObject_Str.proto */
 #define __Pyx_PyObject_Str(obj)\
     (likely(PyString_CheckExact(obj)) ? __Pyx_NewRef(obj) : PyObject_Str(obj))
 
+/* BufferFallbackError.proto */
+static void __Pyx_RaiseBufferFallbackError(void);
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -2824,30 +2845,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -3127,14 +3148,18 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_float(PyObject *, int writable_flag);
 
+/* MemviewDtypeToObject.proto */
+static CYTHON_INLINE PyObject *__pyx_memview_get_float(const char *itemp);
+static CYTHON_INLINE int __pyx_memview_set_float(const char *itemp, PyObject *obj);
+
 /* Arithmetic.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
@@ -3347,14 +3372,15 @@
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_refcount_objects_in_slice(char *, Py_ssize_t *, Py_ssize_t *, int, int); /*proto*/
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *, int, size_t, void *, int); /*proto*/
 static void __pyx_memoryview__slice_assign_scalar(char *, Py_ssize_t *, Py_ssize_t *, int, size_t, void *); /*proto*/
 static PyObject *__pyx_unpickle_Enum__set_state(struct __pyx_MemviewEnum_obj *, PyObject *); /*proto*/
 /* #### Code section: typeinfo ### */
 static __Pyx_TypeInfo __Pyx_TypeInfo_float = { "float", NULL, sizeof(float), { 0 }, 0, 'R', 0, 0 };
+static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_int = { "int", NULL, sizeof(int), { 0 }, 0, __PYX_IS_UNSIGNED(int) ? 'U' : 'I', __PYX_IS_UNSIGNED(int), 0 };
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "cssm"
 extern int __pyx_module_is_main_cssm;
 int __pyx_module_is_main_cssm = 0;
 
 /* Implementation of "cssm" */
@@ -3392,65 +3418,77 @@
 static const char __pyx_k__3[] = "*";
 static const char __pyx_k__6[] = "'";
 static const char __pyx_k__7[] = ")";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_ix[] = "ix";
 static const char __pyx_k_np[] = "np";
+static const char __pyx_k_sd[] = "sd";
 static const char __pyx_k_st[] = "st";
 static const char __pyx_k_sv[] = "sv";
 static const char __pyx_k_sz[] = "sz";
 static const char __pyx_k_vh[] = "vh";
+static const char __pyx_k_vs[] = "vs";
 static const char __pyx_k_zh[] = "zh";
-static const char __pyx_k__60[] = "?";
+static const char __pyx_k_zs[] = "zs";
+static const char __pyx_k__66[] = "?";
 static const char __pyx_k_abc[] = "abc";
+static const char __pyx_k_abs[] = "abs";
 static const char __pyx_k_add[] = "add";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_ddm[] = "ddm";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_ix1[] = "ix1";
 static const char __pyx_k_ix2[] = "ix2";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_lca[] = "lca";
+static const char __pyx_k_min[] = "min";
+static const char __pyx_k_ndt[] = "ndt";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_rts[] = "rts";
 static const char __pyx_k_sys[] = "sys";
 static const char __pyx_k_t_h[] = "t_h";
 static const char __pyx_k_t_l[] = "t_l";
 static const char __pyx_k_t_s[] = "t_s";
+static const char __pyx_k_tan[] = "tan";
+static const char __pyx_k_v_2[] = "v_";
 static const char __pyx_k_v_l[] = "v_l";
 static const char __pyx_k_vl1[] = "vl1";
 static const char __pyx_k_vl2[] = "vl2";
+static const char __pyx_k_x_t[] = "x_t";
 static const char __pyx_k_y_h[] = "y_h";
 static const char __pyx_k_y_l[] = "y_l";
 static const char __pyx_k_zl1[] = "zl1";
 static const char __pyx_k_zl2[] = "zl2";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_cssm[] = "cssm";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_full[] = "full";
 static const char __pyx_k_intc[] = "intc";
 static const char __pyx_k_ix_l[] = "ix_l";
 static const char __pyx_k_keys[] = "keys";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
+static const char __pyx_k_nact[] = "nact";
 static const char __pyx_k_name[] = "name";
 static const char __pyx_k_ndim[] = "ndim";
 static const char __pyx_k_pack[] = "pack";
 static const char __pyx_k_sign[] = "sign";
 static const char __pyx_k_size[] = "size";
 static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_sqrt[] = "sqrt";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_t_l1[] = "t_l1";
 static const char __pyx_k_t_l2[] = "t_l2";
 static const char __pyx_k_test[] = "test";
 static const char __pyx_k_traj[] = "traj";
+static const char __pyx_k_v_RL[] = "v_RL";
+static const char __pyx_k_v_WM[] = "v_WM";
 static const char __pyx_k_v_l1[] = "v_l1";
 static const char __pyx_k_v_l2[] = "v_l2";
 static const char __pyx_k_y_l1[] = "y_l1";
 static const char __pyx_k_y_l2[] = "y_l2";
 static const char __pyx_k_ASCII[] = "ASCII";
 static const char __pyx_k_DTYPE[] = "DTYPE";
 static const char __pyx_k_alpha[] = "alpha";
@@ -3466,40 +3504,50 @@
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_t_par[] = "t_par";
 static const char __pyx_k_t_tmp[] = "t_tmp";
 static const char __pyx_k_test2[] = "test2";
+static const char __pyx_k_theta[] = "theta";
+static const char __pyx_k_vs_RL[] = "vs_RL";
+static const char __pyx_k_vs_WM[] = "vs_WM";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_a_view[] = "a_view";
 static const char __pyx_k_arange[] = "arange";
 static const char __pyx_k_argmax[] = "argmax";
+static const char __pyx_k_argmin[] = "argmin";
 static const char __pyx_k_astype[] = "astype";
 static const char __pyx_k_b_view[] = "b_view";
 static const char __pyx_k_d_view[] = "d_view";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_g_view[] = "g_view";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_ix_tmp[] = "ix_tmp";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_name_2[] = "__name__";
+static const char __pyx_k_normal[] = "normal";
 static const char __pyx_k_pickle[] = "pickle";
+static const char __pyx_k_random[] = "random";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_s_view[] = "s_view";
 static const char __pyx_k_smooth[] = "smooth";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_t_view[] = "t_view";
 static const char __pyx_k_test_2[] = "__test__";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
+static const char __pyx_k_v_RL_2[] = "v_RL_";
+static const char __pyx_k_v_WM_2[] = "v_WM_";
 static const char __pyx_k_v_dict[] = "v_dict";
 static const char __pyx_k_v_view[] = "v_view";
+static const char __pyx_k_x_t_RL[] = "x_t_RL";
+static const char __pyx_k_x_t_WM[] = "x_t_WM";
 static const char __pyx_k_z_dict[] = "z_dict";
 static const char __pyx_k_z_view[] = "z_view";
 static const char __pyx_k_choices[] = "choices";
 static const char __pyx_k_ddm_sdv[] = "ddm_sdv";
 static const char __pyx_k_delta_t[] = "delta_t";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_float32[] = "float32";
@@ -3510,14 +3558,15 @@
 static const char __pyx_k_minimal[] = "minimal";
 static const char __pyx_k_numbers[] = "numbers";
 static const char __pyx_k_rts_low[] = "rts_low";
 static const char __pyx_k_sqrt_st[] = "sqrt_st";
 static const char __pyx_k_st_view[] = "st_view";
 static const char __pyx_k_sv_view[] = "sv_view";
 static const char __pyx_k_sz_view[] = "sz_view";
+static const char __pyx_k_uniform[] = "uniform";
 static const char __pyx_k_vh_view[] = "vh_view";
 static const char __pyx_k_zh_view[] = "zh_view";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_Integral[] = "Integral";
 static const char __pyx_k_Sequence[] = "Sequence";
 static const char __pyx_k_boundary[] = "boundary";
 static const char __pyx_k_constant[] = "constant";
@@ -3539,37 +3588,42 @@
 static const char __pyx_k_vl2_view[] = "vl2_view";
 static const char __pyx_k_zl1_view[] = "zl1_view";
 static const char __pyx_k_zl2_view[] = "zl2_view";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_drift_fun[] = "drift_fun";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_isenabled[] = "isenabled";
+static const char __pyx_k_lba_angle[] = "lba_angle";
 static const char __pyx_k_n_samples[] = "n_samples";
 static const char __pyx_k_num_draws[] = "num_draws";
 static const char __pyx_k_num_steps[] = "num_steps";
 static const char __pyx_k_particles[] = "particles";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_simulator[] = "simulator";
 static const char __pyx_k_traj_view[] = "traj_view";
+static const char __pyx_k_v_RL_view[] = "v_RL_view";
+static const char __pyx_k_v_WM_view[] = "v_WM_view";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_alpha_view[] = "alpha_view";
 static const char __pyx_k_bias_trace[] = "bias_trace";
 static const char __pyx_k_drift_view[] = "drift_view";
 static const char __pyx_k_print_info[] = "print_info";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_race_model[] = "race_model";
 static const char __pyx_k_t_particle[] = "t_particle";
+static const char __pyx_k_theta_view[] = "theta_view";
 static const char __pyx_k_trajectory[] = "trajectory";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_collections[] = "collections";
+static const char __pyx_k_lba_vanilla[] = "lba_vanilla";
 static const char __pyx_k_n_particles[] = "n_particles";
 static const char __pyx_k_t_particle1[] = "t_particle1";
 static const char __pyx_k_t_particle2[] = "t_particle2";
 static const char __pyx_k_tmp_pos_dep[] = "tmp_pos_dep";
 static const char __pyx_k_boundary_fun[] = "boundary_fun";
 static const char __pyx_k_choices_view[] = "choices_view";
 static const char __pyx_k_deadline_tmp[] = "deadline_tmp";
@@ -3590,14 +3644,15 @@
 static const char __pyx_k_class_getitem[] = "__class_getitem__";
 static const char __pyx_k_ddm_flexbound[] = "ddm_flexbound";
 static const char __pyx_k_deadline_view[] = "deadline_view";
 static const char __pyx_k_delta_t_alpha[] = "delta_t_alpha";
 static const char __pyx_k_particles_sum[] = "particles_sum";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_return_option[] = "return_option";
+static const char __pyx_k_rlwm_lba_race[] = "rlwm_lba_race";
 static const char __pyx_k_rts_high_view[] = "rts_high_view";
 static const char __pyx_k_AssertionError[] = "AssertionError";
 static const char __pyx_k_drift_fun_type[] = "drift_fun_type";
 static const char __pyx_k_levy_flexbound[] = "levy_flexbound";
 static const char __pyx_k_particles_view[] = "particles_view";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
@@ -3709,44 +3764,47 @@
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_4cssm_test(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_random_state, PyObject *__pyx_v_smooth, PyObject *__pyx_v_return_option); /* proto */
 static PyObject *__pyx_pf_4cssm_2test2(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_random_state, PyObject *__pyx_v_smooth, PyObject *__pyx_v_return_option); /* proto */
 static PyObject *__pyx_pf_4cssm_4full_ddm_hddm_base(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_sz, PyArrayObject *__pyx_v_sv, PyArrayObject *__pyx_v_st, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_random_state, PyObject *__pyx_v_smooth, PyObject *__pyx_v_return_option, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_pf_4cssm_6ddm(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, PyObject *__pyx_v_max_t, float __pyx_v_s, float __pyx_v_delta_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_38__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_44__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_8ddm_flexbound(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_max_t, float __pyx_v_delta_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_40__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_46__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_10ddm_flex(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_drift_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_drift_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_42__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_48__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_12levy_flexbound(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_alpha, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_44__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_14full_ddm(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_sz, PyArrayObject *__pyx_v_sv, PyArrayObject *__pyx_v_st, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_46__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_52__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_16ddm_sdv(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_sv, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_48__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_54__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_18ornstein_uhlenbeck(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_56__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_20race_model(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_s, PyArrayObject *__pyx_v_deadline, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_52__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_58__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_22lca(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_b, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_s, PyArrayObject *__pyx_v_deadline, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_54__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_60__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_24ddm_flexbound_seq2(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_56__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_62__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_26ddm_flexbound_par2(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_58__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_64__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_28ddm_flexbound_mic2_ornstein(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, PyArrayObject *__pyx_v_s_pre_high_level_choice, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_60__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_66__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_30ddm_flexbound_mic2_multinoise(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_62__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_68__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_4cssm_32ddm_flexbound_mic2_ornstein_multinoise(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_64__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_4cssm_34ddm_flexbound_mic2_unnormalized_ornstein_multinoise(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
-static PyObject *__pyx_pf_4cssm_66__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_4cssm_36ddm_flexbound_tradeoff(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_4cssm_34lba_vanilla(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_deadline, float __pyx_v_sd, float __pyx_v_ndt, int __pyx_v_nact, int __pyx_v_n_samples, int __pyx_v_n_trials, float __pyx_v_max_t, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_4cssm_36lba_angle(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_theta, PyArrayObject *__pyx_v_deadline, float __pyx_v_sd, float __pyx_v_ndt, int __pyx_v_nact, int __pyx_v_n_samples, int __pyx_v_n_trials, float __pyx_v_max_t, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_4cssm_38rlwm_lba_race(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v_RL, PyArrayObject *__pyx_v_v_WM, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_deadline, float __pyx_v_sd, float __pyx_v_ndt, int __pyx_v_nact, int __pyx_v_n_samples, int __pyx_v_n_trials, float __pyx_v_max_t, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_4cssm_70__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_40ddm_flexbound_mic2_unnormalized_ornstein_multinoise(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
+static PyObject *__pyx_pf_4cssm_72__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_4cssm_42ddm_flexbound_tradeoff(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -3866,29 +3924,31 @@
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
   PyObject *__pyx_kp_u__2;
   PyObject *__pyx_n_s__3;
   PyObject *__pyx_kp_u__6;
-  PyObject *__pyx_n_s__60;
+  PyObject *__pyx_n_s__66;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_a;
   PyObject *__pyx_n_u_a;
   PyObject *__pyx_n_s_a_view;
   PyObject *__pyx_n_s_abc;
+  PyObject *__pyx_n_s_abs;
   PyObject *__pyx_n_s_add;
   PyObject *__pyx_n_s_allocate_buffer;
   PyObject *__pyx_n_s_alpha;
   PyObject *__pyx_n_u_alpha;
   PyObject *__pyx_n_s_alpha_stable_values;
   PyObject *__pyx_n_s_alpha_view;
   PyObject *__pyx_kp_u_and;
   PyObject *__pyx_n_s_arange;
   PyObject *__pyx_n_s_argmax;
+  PyObject *__pyx_n_s_argmin;
   PyObject *__pyx_n_s_astype;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_b;
   PyObject *__pyx_n_u_b;
   PyObject *__pyx_n_s_b_view;
   PyObject *__pyx_n_s_base;
   PyObject *__pyx_n_s_bias_trace;
@@ -4000,38 +4060,46 @@
   PyObject *__pyx_n_s_ix_l;
   PyObject *__pyx_n_s_ix_tmp;
   PyObject *__pyx_n_s_j;
   PyObject *__pyx_n_s_k;
   PyObject *__pyx_n_s_key;
   PyObject *__pyx_n_s_keys;
   PyObject *__pyx_n_s_kwargs;
+  PyObject *__pyx_n_s_lba_angle;
+  PyObject *__pyx_n_u_lba_angle;
+  PyObject *__pyx_n_s_lba_vanilla;
+  PyObject *__pyx_n_u_lba_vanilla;
   PyObject *__pyx_n_s_lca;
   PyObject *__pyx_n_u_lca;
   PyObject *__pyx_n_s_levy_flexbound;
   PyObject *__pyx_n_u_levy_flexbound;
   PyObject *__pyx_n_s_m;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_max_t;
   PyObject *__pyx_n_u_max_t;
   PyObject *__pyx_n_s_memview;
   PyObject *__pyx_n_u_metadata;
+  PyObject *__pyx_n_s_min;
   PyObject *__pyx_n_u_minimal;
   PyObject *__pyx_n_s_mode;
   PyObject *__pyx_n_s_multiply;
   PyObject *__pyx_n_s_n;
   PyObject *__pyx_n_s_n_particles;
   PyObject *__pyx_n_s_n_samples;
   PyObject *__pyx_n_u_n_samples;
   PyObject *__pyx_n_s_n_trials;
   PyObject *__pyx_n_u_n_trials;
+  PyObject *__pyx_n_s_nact;
   PyObject *__pyx_n_s_name;
   PyObject *__pyx_n_s_name_2;
   PyObject *__pyx_n_s_ndim;
+  PyObject *__pyx_n_s_ndt;
   PyObject *__pyx_n_s_new;
   PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
+  PyObject *__pyx_n_s_normal;
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_num_draws;
   PyObject *__pyx_n_s_num_steps;
   PyObject *__pyx_n_s_numbers;
   PyObject *__pyx_n_s_numpy;
   PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
   PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
@@ -4052,22 +4120,25 @@
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_Enum;
   PyObject *__pyx_n_s_pyx_vtable;
   PyObject *__pyx_n_s_race_model;
   PyObject *__pyx_n_u_race_model;
+  PyObject *__pyx_n_s_random;
   PyObject *__pyx_n_s_random_state;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_register;
   PyObject *__pyx_n_s_return_option;
   PyObject *__pyx_kp_u_return_option_must_be_either_ful;
+  PyObject *__pyx_n_s_rlwm_lba_race;
+  PyObject *__pyx_n_u_rlwm_lba_race;
   PyObject *__pyx_n_s_rts;
   PyObject *__pyx_n_u_rts;
   PyObject *__pyx_n_s_rts_high;
   PyObject *__pyx_n_u_rts_high;
   PyObject *__pyx_n_s_rts_high_view;
   PyObject *__pyx_n_s_rts_low;
   PyObject *__pyx_n_u_rts_low;
@@ -4075,14 +4146,16 @@
   PyObject *__pyx_n_s_rts_view;
   PyObject *__pyx_n_s_s;
   PyObject *__pyx_n_u_s;
   PyObject *__pyx_n_s_s_pre_high_level_choice;
   PyObject *__pyx_n_u_s_pre_high_level_choice;
   PyObject *__pyx_n_s_s_pre_high_level_choice_view;
   PyObject *__pyx_n_s_s_view;
+  PyObject *__pyx_n_s_sd;
+  PyObject *__pyx_n_u_sd;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_shape;
   PyObject *__pyx_n_s_sign;
   PyObject *__pyx_n_u_simulator;
   PyObject *__pyx_n_s_size;
   PyObject *__pyx_n_s_smooth;
@@ -4119,27 +4192,39 @@
   PyObject *__pyx_n_s_t_par;
   PyObject *__pyx_n_s_t_particle;
   PyObject *__pyx_n_s_t_particle1;
   PyObject *__pyx_n_s_t_particle2;
   PyObject *__pyx_n_s_t_s;
   PyObject *__pyx_n_s_t_tmp;
   PyObject *__pyx_n_s_t_view;
+  PyObject *__pyx_n_s_tan;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_test2;
   PyObject *__pyx_n_s_test_2;
+  PyObject *__pyx_n_s_theta;
+  PyObject *__pyx_n_u_theta;
+  PyObject *__pyx_n_s_theta_view;
   PyObject *__pyx_n_s_tmp_pos_dep;
   PyObject *__pyx_n_s_traj;
   PyObject *__pyx_n_s_traj_view;
   PyObject *__pyx_n_u_trajectory;
   PyObject *__pyx_kp_s_unable_to_allocate_array_data;
   PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
+  PyObject *__pyx_n_s_uniform;
   PyObject *__pyx_n_s_unpack;
   PyObject *__pyx_n_s_update;
   PyObject *__pyx_n_s_v;
   PyObject *__pyx_n_u_v;
+  PyObject *__pyx_n_u_v_2;
+  PyObject *__pyx_n_s_v_RL;
+  PyObject *__pyx_n_u_v_RL_2;
+  PyObject *__pyx_n_s_v_RL_view;
+  PyObject *__pyx_n_s_v_WM;
+  PyObject *__pyx_n_u_v_WM_2;
+  PyObject *__pyx_n_s_v_WM_view;
   PyObject *__pyx_n_s_v_dict;
   PyObject *__pyx_n_s_v_l;
   PyObject *__pyx_n_s_v_l1;
   PyObject *__pyx_n_s_v_l2;
   PyObject *__pyx_n_s_v_view;
   PyObject *__pyx_n_s_version_info;
   PyObject *__pyx_n_s_vh;
@@ -4147,14 +4232,20 @@
   PyObject *__pyx_n_s_vh_view;
   PyObject *__pyx_n_s_vl1;
   PyObject *__pyx_n_u_vl1;
   PyObject *__pyx_n_s_vl1_view;
   PyObject *__pyx_n_s_vl2;
   PyObject *__pyx_n_u_vl2;
   PyObject *__pyx_n_s_vl2_view;
+  PyObject *__pyx_n_s_vs;
+  PyObject *__pyx_n_s_vs_RL;
+  PyObject *__pyx_n_s_vs_WM;
+  PyObject *__pyx_n_s_x_t;
+  PyObject *__pyx_n_s_x_t_RL;
+  PyObject *__pyx_n_s_x_t_WM;
   PyObject *__pyx_n_s_y;
   PyObject *__pyx_n_s_y_h;
   PyObject *__pyx_n_s_y_l;
   PyObject *__pyx_n_s_y_l1;
   PyObject *__pyx_n_s_y_l2;
   PyObject *__pyx_n_s_z;
   PyObject *__pyx_n_u_z;
@@ -4166,14 +4257,15 @@
   PyObject *__pyx_n_s_zh_view;
   PyObject *__pyx_n_s_zl1;
   PyObject *__pyx_n_u_zl1;
   PyObject *__pyx_n_s_zl1_view;
   PyObject *__pyx_n_s_zl2;
   PyObject *__pyx_n_u_zl2;
   PyObject *__pyx_n_s_zl2_view;
+  PyObject *__pyx_n_s_zs;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_1;
   PyObject *__pyx_int_2;
   PyObject *__pyx_int_3;
   PyObject *__pyx_int_20;
   PyObject *__pyx_int_112105877;
   PyObject *__pyx_int_136983863;
@@ -4209,15 +4301,18 @@
   PyObject *__pyx_tuple__43;
   PyObject *__pyx_tuple__45;
   PyObject *__pyx_tuple__47;
   PyObject *__pyx_tuple__49;
   PyObject *__pyx_tuple__51;
   PyObject *__pyx_tuple__53;
   PyObject *__pyx_tuple__55;
-  PyObject *__pyx_tuple__58;
+  PyObject *__pyx_tuple__57;
+  PyObject *__pyx_tuple__59;
+  PyObject *__pyx_tuple__61;
+  PyObject *__pyx_tuple__64;
   PyObject *__pyx_codeobj__23;
   PyObject *__pyx_codeobj__25;
   PyObject *__pyx_codeobj__26;
   PyObject *__pyx_codeobj__28;
   PyObject *__pyx_codeobj__30;
   PyObject *__pyx_codeobj__32;
   PyObject *__pyx_codeobj__34;
@@ -4228,16 +4323,19 @@
   PyObject *__pyx_codeobj__44;
   PyObject *__pyx_codeobj__46;
   PyObject *__pyx_codeobj__48;
   PyObject *__pyx_codeobj__50;
   PyObject *__pyx_codeobj__52;
   PyObject *__pyx_codeobj__54;
   PyObject *__pyx_codeobj__56;
-  PyObject *__pyx_codeobj__57;
-  PyObject *__pyx_codeobj__59;
+  PyObject *__pyx_codeobj__58;
+  PyObject *__pyx_codeobj__60;
+  PyObject *__pyx_codeobj__62;
+  PyObject *__pyx_codeobj__63;
+  PyObject *__pyx_codeobj__65;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -4334,29 +4432,31 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
-  Py_CLEAR(clear_module_state->__pyx_n_s__60);
+  Py_CLEAR(clear_module_state->__pyx_n_s__66);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_a);
   Py_CLEAR(clear_module_state->__pyx_n_u_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_a_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_abc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_abs);
   Py_CLEAR(clear_module_state->__pyx_n_s_add);
   Py_CLEAR(clear_module_state->__pyx_n_s_allocate_buffer);
   Py_CLEAR(clear_module_state->__pyx_n_s_alpha);
   Py_CLEAR(clear_module_state->__pyx_n_u_alpha);
   Py_CLEAR(clear_module_state->__pyx_n_s_alpha_stable_values);
   Py_CLEAR(clear_module_state->__pyx_n_s_alpha_view);
   Py_CLEAR(clear_module_state->__pyx_kp_u_and);
   Py_CLEAR(clear_module_state->__pyx_n_s_arange);
   Py_CLEAR(clear_module_state->__pyx_n_s_argmax);
+  Py_CLEAR(clear_module_state->__pyx_n_s_argmin);
   Py_CLEAR(clear_module_state->__pyx_n_s_astype);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_b);
   Py_CLEAR(clear_module_state->__pyx_n_u_b);
   Py_CLEAR(clear_module_state->__pyx_n_s_b_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_base);
   Py_CLEAR(clear_module_state->__pyx_n_s_bias_trace);
@@ -4468,38 +4568,46 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_ix_l);
   Py_CLEAR(clear_module_state->__pyx_n_s_ix_tmp);
   Py_CLEAR(clear_module_state->__pyx_n_s_j);
   Py_CLEAR(clear_module_state->__pyx_n_s_k);
   Py_CLEAR(clear_module_state->__pyx_n_s_key);
   Py_CLEAR(clear_module_state->__pyx_n_s_keys);
   Py_CLEAR(clear_module_state->__pyx_n_s_kwargs);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lba_angle);
+  Py_CLEAR(clear_module_state->__pyx_n_u_lba_angle);
+  Py_CLEAR(clear_module_state->__pyx_n_s_lba_vanilla);
+  Py_CLEAR(clear_module_state->__pyx_n_u_lba_vanilla);
   Py_CLEAR(clear_module_state->__pyx_n_s_lca);
   Py_CLEAR(clear_module_state->__pyx_n_u_lca);
   Py_CLEAR(clear_module_state->__pyx_n_s_levy_flexbound);
   Py_CLEAR(clear_module_state->__pyx_n_u_levy_flexbound);
   Py_CLEAR(clear_module_state->__pyx_n_s_m);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_max_t);
   Py_CLEAR(clear_module_state->__pyx_n_u_max_t);
   Py_CLEAR(clear_module_state->__pyx_n_s_memview);
   Py_CLEAR(clear_module_state->__pyx_n_u_metadata);
+  Py_CLEAR(clear_module_state->__pyx_n_s_min);
   Py_CLEAR(clear_module_state->__pyx_n_u_minimal);
   Py_CLEAR(clear_module_state->__pyx_n_s_mode);
   Py_CLEAR(clear_module_state->__pyx_n_s_multiply);
   Py_CLEAR(clear_module_state->__pyx_n_s_n);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_particles);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_samples);
   Py_CLEAR(clear_module_state->__pyx_n_u_n_samples);
   Py_CLEAR(clear_module_state->__pyx_n_s_n_trials);
   Py_CLEAR(clear_module_state->__pyx_n_u_n_trials);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nact);
   Py_CLEAR(clear_module_state->__pyx_n_s_name);
   Py_CLEAR(clear_module_state->__pyx_n_s_name_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_ndim);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ndt);
   Py_CLEAR(clear_module_state->__pyx_n_s_new);
   Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
+  Py_CLEAR(clear_module_state->__pyx_n_s_normal);
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_num_draws);
   Py_CLEAR(clear_module_state->__pyx_n_s_num_steps);
   Py_CLEAR(clear_module_state->__pyx_n_s_numbers);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
   Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
   Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
@@ -4520,22 +4628,25 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
   Py_CLEAR(clear_module_state->__pyx_n_s_race_model);
   Py_CLEAR(clear_module_state->__pyx_n_u_race_model);
+  Py_CLEAR(clear_module_state->__pyx_n_s_random);
   Py_CLEAR(clear_module_state->__pyx_n_s_random_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_register);
   Py_CLEAR(clear_module_state->__pyx_n_s_return_option);
   Py_CLEAR(clear_module_state->__pyx_kp_u_return_option_must_be_either_ful);
+  Py_CLEAR(clear_module_state->__pyx_n_s_rlwm_lba_race);
+  Py_CLEAR(clear_module_state->__pyx_n_u_rlwm_lba_race);
   Py_CLEAR(clear_module_state->__pyx_n_s_rts);
   Py_CLEAR(clear_module_state->__pyx_n_u_rts);
   Py_CLEAR(clear_module_state->__pyx_n_s_rts_high);
   Py_CLEAR(clear_module_state->__pyx_n_u_rts_high);
   Py_CLEAR(clear_module_state->__pyx_n_s_rts_high_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_rts_low);
   Py_CLEAR(clear_module_state->__pyx_n_u_rts_low);
@@ -4543,14 +4654,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_rts_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_s);
   Py_CLEAR(clear_module_state->__pyx_n_u_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_s_pre_high_level_choice);
   Py_CLEAR(clear_module_state->__pyx_n_u_s_pre_high_level_choice);
   Py_CLEAR(clear_module_state->__pyx_n_s_s_pre_high_level_choice_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_s_view);
+  Py_CLEAR(clear_module_state->__pyx_n_s_sd);
+  Py_CLEAR(clear_module_state->__pyx_n_u_sd);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_shape);
   Py_CLEAR(clear_module_state->__pyx_n_s_sign);
   Py_CLEAR(clear_module_state->__pyx_n_u_simulator);
   Py_CLEAR(clear_module_state->__pyx_n_s_size);
   Py_CLEAR(clear_module_state->__pyx_n_s_smooth);
@@ -4587,27 +4700,39 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_t_par);
   Py_CLEAR(clear_module_state->__pyx_n_s_t_particle);
   Py_CLEAR(clear_module_state->__pyx_n_s_t_particle1);
   Py_CLEAR(clear_module_state->__pyx_n_s_t_particle2);
   Py_CLEAR(clear_module_state->__pyx_n_s_t_s);
   Py_CLEAR(clear_module_state->__pyx_n_s_t_tmp);
   Py_CLEAR(clear_module_state->__pyx_n_s_t_view);
+  Py_CLEAR(clear_module_state->__pyx_n_s_tan);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_test2);
   Py_CLEAR(clear_module_state->__pyx_n_s_test_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_theta);
+  Py_CLEAR(clear_module_state->__pyx_n_u_theta);
+  Py_CLEAR(clear_module_state->__pyx_n_s_theta_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_tmp_pos_dep);
   Py_CLEAR(clear_module_state->__pyx_n_s_traj);
   Py_CLEAR(clear_module_state->__pyx_n_s_traj_view);
   Py_CLEAR(clear_module_state->__pyx_n_u_trajectory);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_CLEAR(clear_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
+  Py_CLEAR(clear_module_state->__pyx_n_s_uniform);
   Py_CLEAR(clear_module_state->__pyx_n_s_unpack);
   Py_CLEAR(clear_module_state->__pyx_n_s_update);
   Py_CLEAR(clear_module_state->__pyx_n_s_v);
   Py_CLEAR(clear_module_state->__pyx_n_u_v);
+  Py_CLEAR(clear_module_state->__pyx_n_u_v_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_v_RL);
+  Py_CLEAR(clear_module_state->__pyx_n_u_v_RL_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_v_RL_view);
+  Py_CLEAR(clear_module_state->__pyx_n_s_v_WM);
+  Py_CLEAR(clear_module_state->__pyx_n_u_v_WM_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_v_WM_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_v_dict);
   Py_CLEAR(clear_module_state->__pyx_n_s_v_l);
   Py_CLEAR(clear_module_state->__pyx_n_s_v_l1);
   Py_CLEAR(clear_module_state->__pyx_n_s_v_l2);
   Py_CLEAR(clear_module_state->__pyx_n_s_v_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_version_info);
   Py_CLEAR(clear_module_state->__pyx_n_s_vh);
@@ -4615,14 +4740,20 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_vh_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_vl1);
   Py_CLEAR(clear_module_state->__pyx_n_u_vl1);
   Py_CLEAR(clear_module_state->__pyx_n_s_vl1_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_vl2);
   Py_CLEAR(clear_module_state->__pyx_n_u_vl2);
   Py_CLEAR(clear_module_state->__pyx_n_s_vl2_view);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vs);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vs_RL);
+  Py_CLEAR(clear_module_state->__pyx_n_s_vs_WM);
+  Py_CLEAR(clear_module_state->__pyx_n_s_x_t);
+  Py_CLEAR(clear_module_state->__pyx_n_s_x_t_RL);
+  Py_CLEAR(clear_module_state->__pyx_n_s_x_t_WM);
   Py_CLEAR(clear_module_state->__pyx_n_s_y);
   Py_CLEAR(clear_module_state->__pyx_n_s_y_h);
   Py_CLEAR(clear_module_state->__pyx_n_s_y_l);
   Py_CLEAR(clear_module_state->__pyx_n_s_y_l1);
   Py_CLEAR(clear_module_state->__pyx_n_s_y_l2);
   Py_CLEAR(clear_module_state->__pyx_n_s_z);
   Py_CLEAR(clear_module_state->__pyx_n_u_z);
@@ -4634,14 +4765,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_zh_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_zl1);
   Py_CLEAR(clear_module_state->__pyx_n_u_zl1);
   Py_CLEAR(clear_module_state->__pyx_n_s_zl1_view);
   Py_CLEAR(clear_module_state->__pyx_n_s_zl2);
   Py_CLEAR(clear_module_state->__pyx_n_u_zl2);
   Py_CLEAR(clear_module_state->__pyx_n_s_zl2_view);
+  Py_CLEAR(clear_module_state->__pyx_n_s_zs);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_1);
   Py_CLEAR(clear_module_state->__pyx_int_2);
   Py_CLEAR(clear_module_state->__pyx_int_3);
   Py_CLEAR(clear_module_state->__pyx_int_20);
   Py_CLEAR(clear_module_state->__pyx_int_112105877);
   Py_CLEAR(clear_module_state->__pyx_int_136983863);
@@ -4677,15 +4809,18 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__43);
   Py_CLEAR(clear_module_state->__pyx_tuple__45);
   Py_CLEAR(clear_module_state->__pyx_tuple__47);
   Py_CLEAR(clear_module_state->__pyx_tuple__49);
   Py_CLEAR(clear_module_state->__pyx_tuple__51);
   Py_CLEAR(clear_module_state->__pyx_tuple__53);
   Py_CLEAR(clear_module_state->__pyx_tuple__55);
-  Py_CLEAR(clear_module_state->__pyx_tuple__58);
+  Py_CLEAR(clear_module_state->__pyx_tuple__57);
+  Py_CLEAR(clear_module_state->__pyx_tuple__59);
+  Py_CLEAR(clear_module_state->__pyx_tuple__61);
+  Py_CLEAR(clear_module_state->__pyx_tuple__64);
   Py_CLEAR(clear_module_state->__pyx_codeobj__23);
   Py_CLEAR(clear_module_state->__pyx_codeobj__25);
   Py_CLEAR(clear_module_state->__pyx_codeobj__26);
   Py_CLEAR(clear_module_state->__pyx_codeobj__28);
   Py_CLEAR(clear_module_state->__pyx_codeobj__30);
   Py_CLEAR(clear_module_state->__pyx_codeobj__32);
   Py_CLEAR(clear_module_state->__pyx_codeobj__34);
@@ -4696,16 +4831,19 @@
   Py_CLEAR(clear_module_state->__pyx_codeobj__44);
   Py_CLEAR(clear_module_state->__pyx_codeobj__46);
   Py_CLEAR(clear_module_state->__pyx_codeobj__48);
   Py_CLEAR(clear_module_state->__pyx_codeobj__50);
   Py_CLEAR(clear_module_state->__pyx_codeobj__52);
   Py_CLEAR(clear_module_state->__pyx_codeobj__54);
   Py_CLEAR(clear_module_state->__pyx_codeobj__56);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__57);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__59);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__58);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__60);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__62);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__63);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__65);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -4780,29 +4918,31 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
-  Py_VISIT(traverse_module_state->__pyx_n_s__60);
+  Py_VISIT(traverse_module_state->__pyx_n_s__66);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_a);
   Py_VISIT(traverse_module_state->__pyx_n_u_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_a_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_abc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_abs);
   Py_VISIT(traverse_module_state->__pyx_n_s_add);
   Py_VISIT(traverse_module_state->__pyx_n_s_allocate_buffer);
   Py_VISIT(traverse_module_state->__pyx_n_s_alpha);
   Py_VISIT(traverse_module_state->__pyx_n_u_alpha);
   Py_VISIT(traverse_module_state->__pyx_n_s_alpha_stable_values);
   Py_VISIT(traverse_module_state->__pyx_n_s_alpha_view);
   Py_VISIT(traverse_module_state->__pyx_kp_u_and);
   Py_VISIT(traverse_module_state->__pyx_n_s_arange);
   Py_VISIT(traverse_module_state->__pyx_n_s_argmax);
+  Py_VISIT(traverse_module_state->__pyx_n_s_argmin);
   Py_VISIT(traverse_module_state->__pyx_n_s_astype);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_b);
   Py_VISIT(traverse_module_state->__pyx_n_u_b);
   Py_VISIT(traverse_module_state->__pyx_n_s_b_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_base);
   Py_VISIT(traverse_module_state->__pyx_n_s_bias_trace);
@@ -4914,38 +5054,46 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_ix_l);
   Py_VISIT(traverse_module_state->__pyx_n_s_ix_tmp);
   Py_VISIT(traverse_module_state->__pyx_n_s_j);
   Py_VISIT(traverse_module_state->__pyx_n_s_k);
   Py_VISIT(traverse_module_state->__pyx_n_s_key);
   Py_VISIT(traverse_module_state->__pyx_n_s_keys);
   Py_VISIT(traverse_module_state->__pyx_n_s_kwargs);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lba_angle);
+  Py_VISIT(traverse_module_state->__pyx_n_u_lba_angle);
+  Py_VISIT(traverse_module_state->__pyx_n_s_lba_vanilla);
+  Py_VISIT(traverse_module_state->__pyx_n_u_lba_vanilla);
   Py_VISIT(traverse_module_state->__pyx_n_s_lca);
   Py_VISIT(traverse_module_state->__pyx_n_u_lca);
   Py_VISIT(traverse_module_state->__pyx_n_s_levy_flexbound);
   Py_VISIT(traverse_module_state->__pyx_n_u_levy_flexbound);
   Py_VISIT(traverse_module_state->__pyx_n_s_m);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_max_t);
   Py_VISIT(traverse_module_state->__pyx_n_u_max_t);
   Py_VISIT(traverse_module_state->__pyx_n_s_memview);
   Py_VISIT(traverse_module_state->__pyx_n_u_metadata);
+  Py_VISIT(traverse_module_state->__pyx_n_s_min);
   Py_VISIT(traverse_module_state->__pyx_n_u_minimal);
   Py_VISIT(traverse_module_state->__pyx_n_s_mode);
   Py_VISIT(traverse_module_state->__pyx_n_s_multiply);
   Py_VISIT(traverse_module_state->__pyx_n_s_n);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_particles);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_samples);
   Py_VISIT(traverse_module_state->__pyx_n_u_n_samples);
   Py_VISIT(traverse_module_state->__pyx_n_s_n_trials);
   Py_VISIT(traverse_module_state->__pyx_n_u_n_trials);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nact);
   Py_VISIT(traverse_module_state->__pyx_n_s_name);
   Py_VISIT(traverse_module_state->__pyx_n_s_name_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_ndim);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ndt);
   Py_VISIT(traverse_module_state->__pyx_n_s_new);
   Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
+  Py_VISIT(traverse_module_state->__pyx_n_s_normal);
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_num_draws);
   Py_VISIT(traverse_module_state->__pyx_n_s_num_steps);
   Py_VISIT(traverse_module_state->__pyx_n_s_numbers);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
   Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
   Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
@@ -4966,22 +5114,25 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
   Py_VISIT(traverse_module_state->__pyx_n_s_race_model);
   Py_VISIT(traverse_module_state->__pyx_n_u_race_model);
+  Py_VISIT(traverse_module_state->__pyx_n_s_random);
   Py_VISIT(traverse_module_state->__pyx_n_s_random_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_register);
   Py_VISIT(traverse_module_state->__pyx_n_s_return_option);
   Py_VISIT(traverse_module_state->__pyx_kp_u_return_option_must_be_either_ful);
+  Py_VISIT(traverse_module_state->__pyx_n_s_rlwm_lba_race);
+  Py_VISIT(traverse_module_state->__pyx_n_u_rlwm_lba_race);
   Py_VISIT(traverse_module_state->__pyx_n_s_rts);
   Py_VISIT(traverse_module_state->__pyx_n_u_rts);
   Py_VISIT(traverse_module_state->__pyx_n_s_rts_high);
   Py_VISIT(traverse_module_state->__pyx_n_u_rts_high);
   Py_VISIT(traverse_module_state->__pyx_n_s_rts_high_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_rts_low);
   Py_VISIT(traverse_module_state->__pyx_n_u_rts_low);
@@ -4989,14 +5140,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_rts_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_s);
   Py_VISIT(traverse_module_state->__pyx_n_u_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_s_pre_high_level_choice);
   Py_VISIT(traverse_module_state->__pyx_n_u_s_pre_high_level_choice);
   Py_VISIT(traverse_module_state->__pyx_n_s_s_pre_high_level_choice_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_s_view);
+  Py_VISIT(traverse_module_state->__pyx_n_s_sd);
+  Py_VISIT(traverse_module_state->__pyx_n_u_sd);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_shape);
   Py_VISIT(traverse_module_state->__pyx_n_s_sign);
   Py_VISIT(traverse_module_state->__pyx_n_u_simulator);
   Py_VISIT(traverse_module_state->__pyx_n_s_size);
   Py_VISIT(traverse_module_state->__pyx_n_s_smooth);
@@ -5033,27 +5186,39 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_t_par);
   Py_VISIT(traverse_module_state->__pyx_n_s_t_particle);
   Py_VISIT(traverse_module_state->__pyx_n_s_t_particle1);
   Py_VISIT(traverse_module_state->__pyx_n_s_t_particle2);
   Py_VISIT(traverse_module_state->__pyx_n_s_t_s);
   Py_VISIT(traverse_module_state->__pyx_n_s_t_tmp);
   Py_VISIT(traverse_module_state->__pyx_n_s_t_view);
+  Py_VISIT(traverse_module_state->__pyx_n_s_tan);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_test2);
   Py_VISIT(traverse_module_state->__pyx_n_s_test_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_theta);
+  Py_VISIT(traverse_module_state->__pyx_n_u_theta);
+  Py_VISIT(traverse_module_state->__pyx_n_s_theta_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_tmp_pos_dep);
   Py_VISIT(traverse_module_state->__pyx_n_s_traj);
   Py_VISIT(traverse_module_state->__pyx_n_s_traj_view);
   Py_VISIT(traverse_module_state->__pyx_n_u_trajectory);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_array_data);
   Py_VISIT(traverse_module_state->__pyx_kp_s_unable_to_allocate_shape_and_str);
+  Py_VISIT(traverse_module_state->__pyx_n_s_uniform);
   Py_VISIT(traverse_module_state->__pyx_n_s_unpack);
   Py_VISIT(traverse_module_state->__pyx_n_s_update);
   Py_VISIT(traverse_module_state->__pyx_n_s_v);
   Py_VISIT(traverse_module_state->__pyx_n_u_v);
+  Py_VISIT(traverse_module_state->__pyx_n_u_v_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_v_RL);
+  Py_VISIT(traverse_module_state->__pyx_n_u_v_RL_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_v_RL_view);
+  Py_VISIT(traverse_module_state->__pyx_n_s_v_WM);
+  Py_VISIT(traverse_module_state->__pyx_n_u_v_WM_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_v_WM_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_v_dict);
   Py_VISIT(traverse_module_state->__pyx_n_s_v_l);
   Py_VISIT(traverse_module_state->__pyx_n_s_v_l1);
   Py_VISIT(traverse_module_state->__pyx_n_s_v_l2);
   Py_VISIT(traverse_module_state->__pyx_n_s_v_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_version_info);
   Py_VISIT(traverse_module_state->__pyx_n_s_vh);
@@ -5061,14 +5226,20 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_vh_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_vl1);
   Py_VISIT(traverse_module_state->__pyx_n_u_vl1);
   Py_VISIT(traverse_module_state->__pyx_n_s_vl1_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_vl2);
   Py_VISIT(traverse_module_state->__pyx_n_u_vl2);
   Py_VISIT(traverse_module_state->__pyx_n_s_vl2_view);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vs);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vs_RL);
+  Py_VISIT(traverse_module_state->__pyx_n_s_vs_WM);
+  Py_VISIT(traverse_module_state->__pyx_n_s_x_t);
+  Py_VISIT(traverse_module_state->__pyx_n_s_x_t_RL);
+  Py_VISIT(traverse_module_state->__pyx_n_s_x_t_WM);
   Py_VISIT(traverse_module_state->__pyx_n_s_y);
   Py_VISIT(traverse_module_state->__pyx_n_s_y_h);
   Py_VISIT(traverse_module_state->__pyx_n_s_y_l);
   Py_VISIT(traverse_module_state->__pyx_n_s_y_l1);
   Py_VISIT(traverse_module_state->__pyx_n_s_y_l2);
   Py_VISIT(traverse_module_state->__pyx_n_s_z);
   Py_VISIT(traverse_module_state->__pyx_n_u_z);
@@ -5080,14 +5251,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_zh_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_zl1);
   Py_VISIT(traverse_module_state->__pyx_n_u_zl1);
   Py_VISIT(traverse_module_state->__pyx_n_s_zl1_view);
   Py_VISIT(traverse_module_state->__pyx_n_s_zl2);
   Py_VISIT(traverse_module_state->__pyx_n_u_zl2);
   Py_VISIT(traverse_module_state->__pyx_n_s_zl2_view);
+  Py_VISIT(traverse_module_state->__pyx_n_s_zs);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_1);
   Py_VISIT(traverse_module_state->__pyx_int_2);
   Py_VISIT(traverse_module_state->__pyx_int_3);
   Py_VISIT(traverse_module_state->__pyx_int_20);
   Py_VISIT(traverse_module_state->__pyx_int_112105877);
   Py_VISIT(traverse_module_state->__pyx_int_136983863);
@@ -5123,15 +5295,18 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__43);
   Py_VISIT(traverse_module_state->__pyx_tuple__45);
   Py_VISIT(traverse_module_state->__pyx_tuple__47);
   Py_VISIT(traverse_module_state->__pyx_tuple__49);
   Py_VISIT(traverse_module_state->__pyx_tuple__51);
   Py_VISIT(traverse_module_state->__pyx_tuple__53);
   Py_VISIT(traverse_module_state->__pyx_tuple__55);
-  Py_VISIT(traverse_module_state->__pyx_tuple__58);
+  Py_VISIT(traverse_module_state->__pyx_tuple__57);
+  Py_VISIT(traverse_module_state->__pyx_tuple__59);
+  Py_VISIT(traverse_module_state->__pyx_tuple__61);
+  Py_VISIT(traverse_module_state->__pyx_tuple__64);
   Py_VISIT(traverse_module_state->__pyx_codeobj__23);
   Py_VISIT(traverse_module_state->__pyx_codeobj__25);
   Py_VISIT(traverse_module_state->__pyx_codeobj__26);
   Py_VISIT(traverse_module_state->__pyx_codeobj__28);
   Py_VISIT(traverse_module_state->__pyx_codeobj__30);
   Py_VISIT(traverse_module_state->__pyx_codeobj__32);
   Py_VISIT(traverse_module_state->__pyx_codeobj__34);
@@ -5142,16 +5317,19 @@
   Py_VISIT(traverse_module_state->__pyx_codeobj__44);
   Py_VISIT(traverse_module_state->__pyx_codeobj__46);
   Py_VISIT(traverse_module_state->__pyx_codeobj__48);
   Py_VISIT(traverse_module_state->__pyx_codeobj__50);
   Py_VISIT(traverse_module_state->__pyx_codeobj__52);
   Py_VISIT(traverse_module_state->__pyx_codeobj__54);
   Py_VISIT(traverse_module_state->__pyx_codeobj__56);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__57);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__59);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__58);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__60);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__62);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__63);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__65);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -5268,29 +5446,31 @@
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
-#define __pyx_n_s__60 __pyx_mstate_global->__pyx_n_s__60
+#define __pyx_n_s__66 __pyx_mstate_global->__pyx_n_s__66
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_a __pyx_mstate_global->__pyx_n_s_a
 #define __pyx_n_u_a __pyx_mstate_global->__pyx_n_u_a
 #define __pyx_n_s_a_view __pyx_mstate_global->__pyx_n_s_a_view
 #define __pyx_n_s_abc __pyx_mstate_global->__pyx_n_s_abc
+#define __pyx_n_s_abs __pyx_mstate_global->__pyx_n_s_abs
 #define __pyx_n_s_add __pyx_mstate_global->__pyx_n_s_add
 #define __pyx_n_s_allocate_buffer __pyx_mstate_global->__pyx_n_s_allocate_buffer
 #define __pyx_n_s_alpha __pyx_mstate_global->__pyx_n_s_alpha
 #define __pyx_n_u_alpha __pyx_mstate_global->__pyx_n_u_alpha
 #define __pyx_n_s_alpha_stable_values __pyx_mstate_global->__pyx_n_s_alpha_stable_values
 #define __pyx_n_s_alpha_view __pyx_mstate_global->__pyx_n_s_alpha_view
 #define __pyx_kp_u_and __pyx_mstate_global->__pyx_kp_u_and
 #define __pyx_n_s_arange __pyx_mstate_global->__pyx_n_s_arange
 #define __pyx_n_s_argmax __pyx_mstate_global->__pyx_n_s_argmax
+#define __pyx_n_s_argmin __pyx_mstate_global->__pyx_n_s_argmin
 #define __pyx_n_s_astype __pyx_mstate_global->__pyx_n_s_astype
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_b __pyx_mstate_global->__pyx_n_s_b
 #define __pyx_n_u_b __pyx_mstate_global->__pyx_n_u_b
 #define __pyx_n_s_b_view __pyx_mstate_global->__pyx_n_s_b_view
 #define __pyx_n_s_base __pyx_mstate_global->__pyx_n_s_base
 #define __pyx_n_s_bias_trace __pyx_mstate_global->__pyx_n_s_bias_trace
@@ -5402,38 +5582,46 @@
 #define __pyx_n_s_ix_l __pyx_mstate_global->__pyx_n_s_ix_l
 #define __pyx_n_s_ix_tmp __pyx_mstate_global->__pyx_n_s_ix_tmp
 #define __pyx_n_s_j __pyx_mstate_global->__pyx_n_s_j
 #define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
 #define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
 #define __pyx_n_s_keys __pyx_mstate_global->__pyx_n_s_keys
 #define __pyx_n_s_kwargs __pyx_mstate_global->__pyx_n_s_kwargs
+#define __pyx_n_s_lba_angle __pyx_mstate_global->__pyx_n_s_lba_angle
+#define __pyx_n_u_lba_angle __pyx_mstate_global->__pyx_n_u_lba_angle
+#define __pyx_n_s_lba_vanilla __pyx_mstate_global->__pyx_n_s_lba_vanilla
+#define __pyx_n_u_lba_vanilla __pyx_mstate_global->__pyx_n_u_lba_vanilla
 #define __pyx_n_s_lca __pyx_mstate_global->__pyx_n_s_lca
 #define __pyx_n_u_lca __pyx_mstate_global->__pyx_n_u_lca
 #define __pyx_n_s_levy_flexbound __pyx_mstate_global->__pyx_n_s_levy_flexbound
 #define __pyx_n_u_levy_flexbound __pyx_mstate_global->__pyx_n_u_levy_flexbound
 #define __pyx_n_s_m __pyx_mstate_global->__pyx_n_s_m
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_max_t __pyx_mstate_global->__pyx_n_s_max_t
 #define __pyx_n_u_max_t __pyx_mstate_global->__pyx_n_u_max_t
 #define __pyx_n_s_memview __pyx_mstate_global->__pyx_n_s_memview
 #define __pyx_n_u_metadata __pyx_mstate_global->__pyx_n_u_metadata
+#define __pyx_n_s_min __pyx_mstate_global->__pyx_n_s_min
 #define __pyx_n_u_minimal __pyx_mstate_global->__pyx_n_u_minimal
 #define __pyx_n_s_mode __pyx_mstate_global->__pyx_n_s_mode
 #define __pyx_n_s_multiply __pyx_mstate_global->__pyx_n_s_multiply
 #define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
 #define __pyx_n_s_n_particles __pyx_mstate_global->__pyx_n_s_n_particles
 #define __pyx_n_s_n_samples __pyx_mstate_global->__pyx_n_s_n_samples
 #define __pyx_n_u_n_samples __pyx_mstate_global->__pyx_n_u_n_samples
 #define __pyx_n_s_n_trials __pyx_mstate_global->__pyx_n_s_n_trials
 #define __pyx_n_u_n_trials __pyx_mstate_global->__pyx_n_u_n_trials
+#define __pyx_n_s_nact __pyx_mstate_global->__pyx_n_s_nact
 #define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
 #define __pyx_n_s_name_2 __pyx_mstate_global->__pyx_n_s_name_2
 #define __pyx_n_s_ndim __pyx_mstate_global->__pyx_n_s_ndim
+#define __pyx_n_s_ndt __pyx_mstate_global->__pyx_n_s_ndt
 #define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
 #define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
+#define __pyx_n_s_normal __pyx_mstate_global->__pyx_n_s_normal
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_num_draws __pyx_mstate_global->__pyx_n_s_num_draws
 #define __pyx_n_s_num_steps __pyx_mstate_global->__pyx_n_s_num_steps
 #define __pyx_n_s_numbers __pyx_mstate_global->__pyx_n_s_numbers
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
 #define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
 #define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
@@ -5454,22 +5642,25 @@
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_Enum __pyx_mstate_global->__pyx_n_s_pyx_unpickle_Enum
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
 #define __pyx_n_s_race_model __pyx_mstate_global->__pyx_n_s_race_model
 #define __pyx_n_u_race_model __pyx_mstate_global->__pyx_n_u_race_model
+#define __pyx_n_s_random __pyx_mstate_global->__pyx_n_s_random
 #define __pyx_n_s_random_state __pyx_mstate_global->__pyx_n_s_random_state
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_register __pyx_mstate_global->__pyx_n_s_register
 #define __pyx_n_s_return_option __pyx_mstate_global->__pyx_n_s_return_option
 #define __pyx_kp_u_return_option_must_be_either_ful __pyx_mstate_global->__pyx_kp_u_return_option_must_be_either_ful
+#define __pyx_n_s_rlwm_lba_race __pyx_mstate_global->__pyx_n_s_rlwm_lba_race
+#define __pyx_n_u_rlwm_lba_race __pyx_mstate_global->__pyx_n_u_rlwm_lba_race
 #define __pyx_n_s_rts __pyx_mstate_global->__pyx_n_s_rts
 #define __pyx_n_u_rts __pyx_mstate_global->__pyx_n_u_rts
 #define __pyx_n_s_rts_high __pyx_mstate_global->__pyx_n_s_rts_high
 #define __pyx_n_u_rts_high __pyx_mstate_global->__pyx_n_u_rts_high
 #define __pyx_n_s_rts_high_view __pyx_mstate_global->__pyx_n_s_rts_high_view
 #define __pyx_n_s_rts_low __pyx_mstate_global->__pyx_n_s_rts_low
 #define __pyx_n_u_rts_low __pyx_mstate_global->__pyx_n_u_rts_low
@@ -5477,14 +5668,16 @@
 #define __pyx_n_s_rts_view __pyx_mstate_global->__pyx_n_s_rts_view
 #define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
 #define __pyx_n_u_s __pyx_mstate_global->__pyx_n_u_s
 #define __pyx_n_s_s_pre_high_level_choice __pyx_mstate_global->__pyx_n_s_s_pre_high_level_choice
 #define __pyx_n_u_s_pre_high_level_choice __pyx_mstate_global->__pyx_n_u_s_pre_high_level_choice
 #define __pyx_n_s_s_pre_high_level_choice_view __pyx_mstate_global->__pyx_n_s_s_pre_high_level_choice_view
 #define __pyx_n_s_s_view __pyx_mstate_global->__pyx_n_s_s_view
+#define __pyx_n_s_sd __pyx_mstate_global->__pyx_n_s_sd
+#define __pyx_n_u_sd __pyx_mstate_global->__pyx_n_u_sd
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_shape __pyx_mstate_global->__pyx_n_s_shape
 #define __pyx_n_s_sign __pyx_mstate_global->__pyx_n_s_sign
 #define __pyx_n_u_simulator __pyx_mstate_global->__pyx_n_u_simulator
 #define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
 #define __pyx_n_s_smooth __pyx_mstate_global->__pyx_n_s_smooth
@@ -5521,27 +5714,39 @@
 #define __pyx_n_s_t_par __pyx_mstate_global->__pyx_n_s_t_par
 #define __pyx_n_s_t_particle __pyx_mstate_global->__pyx_n_s_t_particle
 #define __pyx_n_s_t_particle1 __pyx_mstate_global->__pyx_n_s_t_particle1
 #define __pyx_n_s_t_particle2 __pyx_mstate_global->__pyx_n_s_t_particle2
 #define __pyx_n_s_t_s __pyx_mstate_global->__pyx_n_s_t_s
 #define __pyx_n_s_t_tmp __pyx_mstate_global->__pyx_n_s_t_tmp
 #define __pyx_n_s_t_view __pyx_mstate_global->__pyx_n_s_t_view
+#define __pyx_n_s_tan __pyx_mstate_global->__pyx_n_s_tan
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_test2 __pyx_mstate_global->__pyx_n_s_test2
 #define __pyx_n_s_test_2 __pyx_mstate_global->__pyx_n_s_test_2
+#define __pyx_n_s_theta __pyx_mstate_global->__pyx_n_s_theta
+#define __pyx_n_u_theta __pyx_mstate_global->__pyx_n_u_theta
+#define __pyx_n_s_theta_view __pyx_mstate_global->__pyx_n_s_theta_view
 #define __pyx_n_s_tmp_pos_dep __pyx_mstate_global->__pyx_n_s_tmp_pos_dep
 #define __pyx_n_s_traj __pyx_mstate_global->__pyx_n_s_traj
 #define __pyx_n_s_traj_view __pyx_mstate_global->__pyx_n_s_traj_view
 #define __pyx_n_u_trajectory __pyx_mstate_global->__pyx_n_u_trajectory
 #define __pyx_kp_s_unable_to_allocate_array_data __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_array_data
 #define __pyx_kp_s_unable_to_allocate_shape_and_str __pyx_mstate_global->__pyx_kp_s_unable_to_allocate_shape_and_str
+#define __pyx_n_s_uniform __pyx_mstate_global->__pyx_n_s_uniform
 #define __pyx_n_s_unpack __pyx_mstate_global->__pyx_n_s_unpack
 #define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
 #define __pyx_n_s_v __pyx_mstate_global->__pyx_n_s_v
 #define __pyx_n_u_v __pyx_mstate_global->__pyx_n_u_v
+#define __pyx_n_u_v_2 __pyx_mstate_global->__pyx_n_u_v_2
+#define __pyx_n_s_v_RL __pyx_mstate_global->__pyx_n_s_v_RL
+#define __pyx_n_u_v_RL_2 __pyx_mstate_global->__pyx_n_u_v_RL_2
+#define __pyx_n_s_v_RL_view __pyx_mstate_global->__pyx_n_s_v_RL_view
+#define __pyx_n_s_v_WM __pyx_mstate_global->__pyx_n_s_v_WM
+#define __pyx_n_u_v_WM_2 __pyx_mstate_global->__pyx_n_u_v_WM_2
+#define __pyx_n_s_v_WM_view __pyx_mstate_global->__pyx_n_s_v_WM_view
 #define __pyx_n_s_v_dict __pyx_mstate_global->__pyx_n_s_v_dict
 #define __pyx_n_s_v_l __pyx_mstate_global->__pyx_n_s_v_l
 #define __pyx_n_s_v_l1 __pyx_mstate_global->__pyx_n_s_v_l1
 #define __pyx_n_s_v_l2 __pyx_mstate_global->__pyx_n_s_v_l2
 #define __pyx_n_s_v_view __pyx_mstate_global->__pyx_n_s_v_view
 #define __pyx_n_s_version_info __pyx_mstate_global->__pyx_n_s_version_info
 #define __pyx_n_s_vh __pyx_mstate_global->__pyx_n_s_vh
@@ -5549,14 +5754,20 @@
 #define __pyx_n_s_vh_view __pyx_mstate_global->__pyx_n_s_vh_view
 #define __pyx_n_s_vl1 __pyx_mstate_global->__pyx_n_s_vl1
 #define __pyx_n_u_vl1 __pyx_mstate_global->__pyx_n_u_vl1
 #define __pyx_n_s_vl1_view __pyx_mstate_global->__pyx_n_s_vl1_view
 #define __pyx_n_s_vl2 __pyx_mstate_global->__pyx_n_s_vl2
 #define __pyx_n_u_vl2 __pyx_mstate_global->__pyx_n_u_vl2
 #define __pyx_n_s_vl2_view __pyx_mstate_global->__pyx_n_s_vl2_view
+#define __pyx_n_s_vs __pyx_mstate_global->__pyx_n_s_vs
+#define __pyx_n_s_vs_RL __pyx_mstate_global->__pyx_n_s_vs_RL
+#define __pyx_n_s_vs_WM __pyx_mstate_global->__pyx_n_s_vs_WM
+#define __pyx_n_s_x_t __pyx_mstate_global->__pyx_n_s_x_t
+#define __pyx_n_s_x_t_RL __pyx_mstate_global->__pyx_n_s_x_t_RL
+#define __pyx_n_s_x_t_WM __pyx_mstate_global->__pyx_n_s_x_t_WM
 #define __pyx_n_s_y __pyx_mstate_global->__pyx_n_s_y
 #define __pyx_n_s_y_h __pyx_mstate_global->__pyx_n_s_y_h
 #define __pyx_n_s_y_l __pyx_mstate_global->__pyx_n_s_y_l
 #define __pyx_n_s_y_l1 __pyx_mstate_global->__pyx_n_s_y_l1
 #define __pyx_n_s_y_l2 __pyx_mstate_global->__pyx_n_s_y_l2
 #define __pyx_n_s_z __pyx_mstate_global->__pyx_n_s_z
 #define __pyx_n_u_z __pyx_mstate_global->__pyx_n_u_z
@@ -5568,14 +5779,15 @@
 #define __pyx_n_s_zh_view __pyx_mstate_global->__pyx_n_s_zh_view
 #define __pyx_n_s_zl1 __pyx_mstate_global->__pyx_n_s_zl1
 #define __pyx_n_u_zl1 __pyx_mstate_global->__pyx_n_u_zl1
 #define __pyx_n_s_zl1_view __pyx_mstate_global->__pyx_n_s_zl1_view
 #define __pyx_n_s_zl2 __pyx_mstate_global->__pyx_n_s_zl2
 #define __pyx_n_u_zl2 __pyx_mstate_global->__pyx_n_u_zl2
 #define __pyx_n_s_zl2_view __pyx_mstate_global->__pyx_n_s_zl2_view
+#define __pyx_n_s_zs __pyx_mstate_global->__pyx_n_s_zs
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_1 __pyx_mstate_global->__pyx_int_1
 #define __pyx_int_2 __pyx_mstate_global->__pyx_int_2
 #define __pyx_int_3 __pyx_mstate_global->__pyx_int_3
 #define __pyx_int_20 __pyx_mstate_global->__pyx_int_20
 #define __pyx_int_112105877 __pyx_mstate_global->__pyx_int_112105877
 #define __pyx_int_136983863 __pyx_mstate_global->__pyx_int_136983863
@@ -5611,15 +5823,18 @@
 #define __pyx_tuple__43 __pyx_mstate_global->__pyx_tuple__43
 #define __pyx_tuple__45 __pyx_mstate_global->__pyx_tuple__45
 #define __pyx_tuple__47 __pyx_mstate_global->__pyx_tuple__47
 #define __pyx_tuple__49 __pyx_mstate_global->__pyx_tuple__49
 #define __pyx_tuple__51 __pyx_mstate_global->__pyx_tuple__51
 #define __pyx_tuple__53 __pyx_mstate_global->__pyx_tuple__53
 #define __pyx_tuple__55 __pyx_mstate_global->__pyx_tuple__55
-#define __pyx_tuple__58 __pyx_mstate_global->__pyx_tuple__58
+#define __pyx_tuple__57 __pyx_mstate_global->__pyx_tuple__57
+#define __pyx_tuple__59 __pyx_mstate_global->__pyx_tuple__59
+#define __pyx_tuple__61 __pyx_mstate_global->__pyx_tuple__61
+#define __pyx_tuple__64 __pyx_mstate_global->__pyx_tuple__64
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
 #define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
 #define __pyx_codeobj__30 __pyx_mstate_global->__pyx_codeobj__30
 #define __pyx_codeobj__32 __pyx_mstate_global->__pyx_codeobj__32
 #define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
@@ -5630,16 +5845,19 @@
 #define __pyx_codeobj__44 __pyx_mstate_global->__pyx_codeobj__44
 #define __pyx_codeobj__46 __pyx_mstate_global->__pyx_codeobj__46
 #define __pyx_codeobj__48 __pyx_mstate_global->__pyx_codeobj__48
 #define __pyx_codeobj__50 __pyx_mstate_global->__pyx_codeobj__50
 #define __pyx_codeobj__52 __pyx_mstate_global->__pyx_codeobj__52
 #define __pyx_codeobj__54 __pyx_mstate_global->__pyx_codeobj__54
 #define __pyx_codeobj__56 __pyx_mstate_global->__pyx_codeobj__56
-#define __pyx_codeobj__57 __pyx_mstate_global->__pyx_codeobj__57
-#define __pyx_codeobj__59 __pyx_mstate_global->__pyx_codeobj__59
+#define __pyx_codeobj__58 __pyx_mstate_global->__pyx_codeobj__58
+#define __pyx_codeobj__60 __pyx_mstate_global->__pyx_codeobj__60
+#define __pyx_codeobj__62 __pyx_mstate_global->__pyx_codeobj__62
+#define __pyx_codeobj__63 __pyx_mstate_global->__pyx_codeobj__63
+#define __pyx_codeobj__65 __pyx_mstate_global->__pyx_codeobj__65
 /* #### Code section: module_code ### */
 
 /* "View.MemoryView":131
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
@@ -19260,261 +19478,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19523,29 +19741,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19556,15 +19774,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19573,29 +19791,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19606,15 +19824,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19623,29 +19841,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19656,15 +19874,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19673,29 +19891,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19706,15 +19924,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19723,29 +19941,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19756,217 +19974,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19982,15 +20200,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19998,68 +20216,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20067,15 +20285,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -20090,15 +20308,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20114,15 +20332,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20130,68 +20348,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20199,15 +20417,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20222,15 +20440,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20246,15 +20464,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -20262,68 +20480,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -20331,15 +20549,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -20354,170 +20572,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -27209,15 +27427,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
  *                   np.ndarray[float, ndim = 1] a,
  *                   np.ndarray[float, ndim = 1] z,
  */
 
-static PyObject *__pyx_pf_4cssm_38__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_44__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -29303,15 +29521,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flex(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
  *              np.ndarray[float, ndim = 1] a,
  *              np.ndarray[float, ndim = 1] z,
  */
 
-static PyObject *__pyx_pf_4cssm_40__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_46__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -31666,15 +31884,15 @@
  * # @cythonwraparound(False)
  * 
  * def levy_flexbound(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
  *                    np.ndarray[float, ndim = 1] a,
  *                    np.ndarray[float, ndim = 1] z,
  */
 
-static PyObject *__pyx_pf_4cssm_42__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_48__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -33796,15 +34014,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def full_ddm(np.ndarray[float, ndim = 1] v, # = 0,             # <<<<<<<<<<<<<<
  *              np.ndarray[float, ndim = 1] a, # = 1,
  *              np.ndarray[float, ndim = 1] z, # = 0.5,
  */
 
-static PyObject *__pyx_pf_4cssm_44__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -36171,15 +36389,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_sdv(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
  *             np.ndarray[float, ndim = 1] a,
  *             np.ndarray[float, ndim = 1] z,
  */
 
-static PyObject *__pyx_pf_4cssm_46__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_52__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -38419,15 +38637,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ornstein_uhlenbeck(np.ndarray[float, ndim = 1] v, # drift parameter             # <<<<<<<<<<<<<<
  *                        np.ndarray[float, ndim = 1] a, # initial boundary separation
  *                        np.ndarray[float, ndim = 1] z, # starting point bias
  */
 
-static PyObject *__pyx_pf_4cssm_48__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_54__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -40681,15 +40899,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def race_model(np.ndarray[float, ndim = 2] v,  # np.array expected, one column of floats             # <<<<<<<<<<<<<<
  *                np.ndarray[float, ndim = 2] a, # initial boundary separation
  *                np.ndarray[float, ndim = 2] z, # np.array expected, one column of floats
  */
 
-static PyObject *__pyx_pf_4cssm_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_56__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -43172,15 +43390,15 @@
  * 
  * # Simulate (rt, choice) tuples from: Leaky Competing Accumulator Model -----------------------------
  * def lca(np.ndarray[float, ndim = 2] v, # drift parameters (np.array expect: one column of floats)             # <<<<<<<<<<<<<<
  *         np.ndarray[float, ndim = 2] a, # criterion height
  *         np.ndarray[float, ndim = 2] z, # initial bias parameters (np.array expect: one column of floats)
  */
 
-static PyObject *__pyx_pf_4cssm_52__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_58__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -45822,15 +46040,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_seq2(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                        np.ndarray[float, ndim = 1] vl1,
  *                        np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_54__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_60__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -48693,124 +48911,124 @@
       }
 
       /* "cssm.pyx":2183
  *                     smooth_u = 0.0
  *             else:
  *                 smooth_u = 0.0             # <<<<<<<<<<<<<<
  * 
- *                 rts_view[n, k, 0] = t_particle + t_view[k] + smooth_u
+ *             rts_view[n, k, 0] = t_particle + t_view[k] + smooth_u
  */
       /*else*/ {
         __pyx_v_smooth_u = 0.0;
+      }
+      __pyx_L64:;
 
-        /* "cssm.pyx":2185
+      /* "cssm.pyx":2185
  *                 smooth_u = 0.0
  * 
- *                 rts_view[n, k, 0] = t_particle + t_view[k] + smooth_u             # <<<<<<<<<<<<<<
+ *             rts_view[n, k, 0] = t_particle + t_view[k] + smooth_u             # <<<<<<<<<<<<<<
  * 
- *                 # The probability of making a 'mistake' 1 - (relative y position)
+ *             # The probability of making a 'mistake' 1 - (relative y position)
  */
-        __pyx_t_24 = __pyx_v_k;
-        __pyx_t_20 = __pyx_v_n;
-        __pyx_t_19 = __pyx_v_k;
-        __pyx_t_26 = 0;
-        *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_20 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_26 * __pyx_v_rts_view.strides[2]) )) = ((__pyx_v_t_particle + (*((float *) ( /* dim=0 */ (__pyx_v_t_view.data + __pyx_t_24 * __pyx_v_t_view.strides[0]) )))) + __pyx_v_smooth_u);
+      __pyx_t_24 = __pyx_v_k;
+      __pyx_t_20 = __pyx_v_n;
+      __pyx_t_19 = __pyx_v_k;
+      __pyx_t_26 = 0;
+      *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_20 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_26 * __pyx_v_rts_view.strides[2]) )) = ((__pyx_v_t_particle + (*((float *) ( /* dim=0 */ (__pyx_v_t_view.data + __pyx_t_24 * __pyx_v_t_view.strides[0]) )))) + __pyx_v_smooth_u);
 
-        /* "cssm.pyx":2192
+      /* "cssm.pyx":2192
  * 
- *                 # If boundary is negative (or 0) already, we flip a coin
- *                 if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
- *                     if random_uniform() <= 0.5:
- *                         choices_view[n, k, 0] += 1
+ *             # If boundary is negative (or 0) already, we flip a coin
+ *             if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
+ *                 if random_uniform() <= 0.5:
+ *                     choices_view[n, k, 0] += 1
  */
-        __pyx_t_24 = __pyx_v_ix;
-        __pyx_t_18 = ((*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_24 * __pyx_v_boundary_view.strides[0]) ))) <= 0.0);
-        if (__pyx_t_18) {
+      __pyx_t_24 = __pyx_v_ix;
+      __pyx_t_18 = ((*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_24 * __pyx_v_boundary_view.strides[0]) ))) <= 0.0);
+      if (__pyx_t_18) {
 
-          /* "cssm.pyx":2193
- *                 # If boundary is negative (or 0) already, we flip a coin
- *                 if boundary_view[ix] <= 0:
- *                     if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
- *                         choices_view[n, k, 0] += 1
- *                 # Otherwise apply rule from above
+        /* "cssm.pyx":2193
+ *             # If boundary is negative (or 0) already, we flip a coin
+ *             if boundary_view[ix] <= 0:
+ *                 if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
+ *                     choices_view[n, k, 0] += 1
+ *             # Otherwise apply rule from above
  */
-          __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2193, __pyx_L1_error)
-          __pyx_t_18 = (__pyx_t_23 <= 0.5);
-          if (__pyx_t_18) {
+        __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2193, __pyx_L1_error)
+        __pyx_t_18 = (__pyx_t_23 <= 0.5);
+        if (__pyx_t_18) {
 
-            /* "cssm.pyx":2194
- *                 if boundary_view[ix] <= 0:
- *                     if random_uniform() <= 0.5:
- *                         choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
- *                 # Otherwise apply rule from above
- *                 elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
+          /* "cssm.pyx":2194
+ *             if boundary_view[ix] <= 0:
+ *                 if random_uniform() <= 0.5:
+ *                     choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
+ *             # Otherwise apply rule from above
+ *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
  */
-            __pyx_t_24 = __pyx_v_n;
-            __pyx_t_26 = __pyx_v_k;
-            __pyx_t_19 = 0;
-            *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_24 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_26 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[2]) )) += 1;
+          __pyx_t_24 = __pyx_v_n;
+          __pyx_t_26 = __pyx_v_k;
+          __pyx_t_19 = 0;
+          *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_24 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_26 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[2]) )) += 1;
 
-            /* "cssm.pyx":2193
- *                 # If boundary is negative (or 0) already, we flip a coin
- *                 if boundary_view[ix] <= 0:
- *                     if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
- *                         choices_view[n, k, 0] += 1
- *                 # Otherwise apply rule from above
+          /* "cssm.pyx":2193
+ *             # If boundary is negative (or 0) already, we flip a coin
+ *             if boundary_view[ix] <= 0:
+ *                 if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
+ *                     choices_view[n, k, 0] += 1
+ *             # Otherwise apply rule from above
  */
-          }
+        }
 
-          /* "cssm.pyx":2192
+        /* "cssm.pyx":2192
  * 
- *                 # If boundary is negative (or 0) already, we flip a coin
- *                 if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
- *                     if random_uniform() <= 0.5:
- *                         choices_view[n, k, 0] += 1
+ *             # If boundary is negative (or 0) already, we flip a coin
+ *             if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
+ *                 if random_uniform() <= 0.5:
+ *                     choices_view[n, k, 0] += 1
  */
-          goto __pyx_L66;
-        }
+        goto __pyx_L66;
+      }
 
-        /* "cssm.pyx":2196
- *                         choices_view[n, k, 0] += 1
- *                 # Otherwise apply rule from above
- *                 elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
+      /* "cssm.pyx":2196
  *                     choices_view[n, k, 0] += 1
+ *             # Otherwise apply rule from above
+ *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
+ *                 choices_view[n, k, 0] += 1
  * 
  */
-        __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2196, __pyx_L1_error)
-        __pyx_t_19 = __pyx_v_ix;
-        __pyx_t_26 = __pyx_v_ix;
-        __pyx_t_18 = (__pyx_t_23 <= ((__pyx_v_y_l + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_26 * __pyx_v_boundary_view.strides[0]) ))))));
-        if (__pyx_t_18) {
+      __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 2196, __pyx_L1_error)
+      __pyx_t_19 = __pyx_v_ix;
+      __pyx_t_26 = __pyx_v_ix;
+      __pyx_t_18 = (__pyx_t_23 <= ((__pyx_v_y_l + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_26 * __pyx_v_boundary_view.strides[0]) ))))));
+      if (__pyx_t_18) {
 
-          /* "cssm.pyx":2197
- *                 # Otherwise apply rule from above
- *                 elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
- *                     choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
+        /* "cssm.pyx":2197
+ *             # Otherwise apply rule from above
+ *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
+ *                 choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):
  */
-          __pyx_t_26 = __pyx_v_n;
-          __pyx_t_19 = __pyx_v_k;
-          __pyx_t_24 = 0;
-          *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_26 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[2]) )) += 1;
+        __pyx_t_26 = __pyx_v_n;
+        __pyx_t_19 = __pyx_v_k;
+        __pyx_t_24 = 0;
+        *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_26 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[2]) )) += 1;
 
-          /* "cssm.pyx":2196
- *                         choices_view[n, k, 0] += 1
- *                 # Otherwise apply rule from above
- *                 elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
+        /* "cssm.pyx":2196
  *                     choices_view[n, k, 0] += 1
+ *             # Otherwise apply rule from above
+ *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
+ *                 choices_view[n, k, 0] += 1
  * 
  */
-        }
-        __pyx_L66:;
       }
-      __pyx_L64:;
+      __pyx_L66:;
 
       /* "cssm.pyx":2199
- *                     choices_view[n, k, 0] += 1
+ *                 choices_view[n, k, 0] += 1
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):             # <<<<<<<<<<<<<<
  *                     rts_view[n, k, 0] = -999
  * 
  */
       __pyx_t_24 = __pyx_v_n;
       __pyx_t_19 = __pyx_v_k;
@@ -48829,15 +49047,15 @@
  */
         __pyx_t_27 = __pyx_v_n;
         __pyx_t_20 = __pyx_v_k;
         __pyx_t_26 = 0;
         *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_27 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_20 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_26 * __pyx_v_rts_view.strides[2]) )) = -999.0;
 
         /* "cssm.pyx":2199
- *                     choices_view[n, k, 0] += 1
+ *                 choices_view[n, k, 0] += 1
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):             # <<<<<<<<<<<<<<
  *                     rts_view[n, k, 0] = -999
  * 
  */
       }
     }
@@ -49281,15 +49499,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_par2(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                        np.ndarray[float, ndim = 1] vl1,
  *                        np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_56__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_62__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -52457,15 +52675,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_ornstein(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                 np.ndarray[float, ndim = 1] vl1,
  *                                 np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_58__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_64__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -56197,15 +56415,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                   np.ndarray[float, ndim = 1] vl1,
  *                                   np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_60__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_66__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -59840,15 +60058,15 @@
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                            np.ndarray[float, ndim = 1] vl1,
  *                                            np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_62__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_68__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -63471,139 +63689,4095 @@
   __Pyx_XDECREF(__pyx_v_boundary_params_tmp);
   __Pyx_XDECREF(__pyx_9genexpr13__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cssm.pyx":3328
+/* "cssm.pyx":3327
+ * 
+ * # Simulate (rt, choice) tuples from: Vanilla LBA Model without ndt -----------------------------
+ * def lba_vanilla(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4cssm_35lba_vanilla(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_4cssm_35lba_vanilla = {"lba_vanilla", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_35lba_vanilla, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cssm_35lba_vanilla(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_v = 0;
+  PyArrayObject *__pyx_v_a = 0;
+  PyArrayObject *__pyx_v_z = 0;
+  PyArrayObject *__pyx_v_deadline = 0;
+  float __pyx_v_sd;
+  float __pyx_v_ndt;
+  int __pyx_v_nact;
+  int __pyx_v_n_samples;
+  int __pyx_v_n_trials;
+  float __pyx_v_max_t;
+  CYTHON_UNUSED PyObject *__pyx_v_kwargs = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("lba_vanilla (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kwargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_v,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_deadline,&__pyx_n_s_sd,&__pyx_n_s_ndt,&__pyx_n_s_nact,&__pyx_n_s_n_samples,&__pyx_n_s_n_trials,&__pyx_n_s_max_t,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_v)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_a)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_vanilla", 0, 5, 10, 1); __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_z)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_vanilla", 0, 5, 10, 2); __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_deadline)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_vanilla", 0, 5, 10, 3); __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sd)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_vanilla", 0, 5, 10, 4); __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ndt);
+          if (value) { values[5] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nact);
+          if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_samples);
+          if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_trials);
+          if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  9:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_t);
+          if (value) { values[9] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3327, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "lba_vanilla") < 0)) __PYX_ERR(0, 3327, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_v = ((PyArrayObject *)values[0]);
+    __pyx_v_a = ((PyArrayObject *)values[1]);
+    __pyx_v_z = ((PyArrayObject *)values[2]);
+    __pyx_v_deadline = ((PyArrayObject *)values[3]);
+    __pyx_v_sd = __pyx_PyFloat_AsFloat(values[4]); if (unlikely((__pyx_v_sd == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3331, __pyx_L3_error)
+    if (values[5]) {
+      __pyx_v_ndt = __pyx_PyFloat_AsFloat(values[5]); if (unlikely((__pyx_v_ndt == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3332, __pyx_L3_error)
+    } else {
+      __pyx_v_ndt = ((float)((float)0.0));
+    }
+    if (values[6]) {
+      __pyx_v_nact = __Pyx_PyInt_As_int(values[6]); if (unlikely((__pyx_v_nact == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3333, __pyx_L3_error)
+    } else {
+      __pyx_v_nact = ((int)((int)3));
+    }
+    if (values[7]) {
+      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3334, __pyx_L3_error)
+    } else {
+      __pyx_v_n_samples = ((int)((int)0x7D0));
+    }
+    if (values[8]) {
+      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3335, __pyx_L3_error)
+    } else {
+      __pyx_v_n_trials = ((int)((int)1));
+    }
+    if (values[9]) {
+      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[9]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3336, __pyx_L3_error)
+    } else {
+      __pyx_v_max_t = ((float)((float)20.0));
+    }
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("lba_vanilla", 0, 5, 10, __pyx_nargs); __PYX_ERR(0, 3327, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+  __Pyx_AddTraceback("cssm.lba_vanilla", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_v), __pyx_ptype_5numpy_ndarray, 1, "v", 0))) __PYX_ERR(0, 3327, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 3328, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_z), __pyx_ptype_5numpy_ndarray, 1, "z", 0))) __PYX_ERR(0, 3329, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 3330, __pyx_L1_error)
+  __pyx_r = __pyx_pf_4cssm_34lba_vanilla(__pyx_self, __pyx_v_v, __pyx_v_a, __pyx_v_z, __pyx_v_deadline, __pyx_v_sd, __pyx_v_ndt, __pyx_v_nact, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_max_t, __pyx_v_kwargs);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_DECREF(__pyx_v_kwargs);
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4cssm_34lba_vanilla(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_deadline, float __pyx_v_sd, float __pyx_v_ndt, int __pyx_v_nact, int __pyx_v_n_samples, int __pyx_v_n_trials, float __pyx_v_max_t, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
+  __Pyx_memviewslice __pyx_v_v_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_a_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_z_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_deadline_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_rts = NULL;
+  __Pyx_memviewslice __pyx_v_rts_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_choices = NULL;
+  __Pyx_memviewslice __pyx_v_choices_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_v_n;
+  Py_ssize_t __pyx_v_k;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_zs = NULL;
+  PyObject *__pyx_v_vs = NULL;
+  PyObject *__pyx_v_x_t = NULL;
+  PyObject *__pyx_v_v_dict = NULL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_a;
+  __Pyx_Buffer __pyx_pybuffer_a;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_deadline;
+  __Pyx_Buffer __pyx_pybuffer_deadline;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_v;
+  __Pyx_Buffer __pyx_pybuffer_v;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_z;
+  __Pyx_Buffer __pyx_pybuffer_z;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_memviewslice __pyx_t_1 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_t_2 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_t_8 = NULL;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_t_10;
+  int __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  int __pyx_t_13;
+  int __pyx_t_14;
+  Py_ssize_t __pyx_t_15;
+  int __pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  Py_ssize_t __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  Py_ssize_t __pyx_t_21;
+  float __pyx_t_22;
+  Py_ssize_t __pyx_t_23;
+  int __pyx_t_24;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("lba_vanilla", 1);
+  __pyx_pybuffer_v.pybuffer.buf = NULL;
+  __pyx_pybuffer_v.refcount = 0;
+  __pyx_pybuffernd_v.data = NULL;
+  __pyx_pybuffernd_v.rcbuffer = &__pyx_pybuffer_v;
+  __pyx_pybuffer_a.pybuffer.buf = NULL;
+  __pyx_pybuffer_a.refcount = 0;
+  __pyx_pybuffernd_a.data = NULL;
+  __pyx_pybuffernd_a.rcbuffer = &__pyx_pybuffer_a;
+  __pyx_pybuffer_z.pybuffer.buf = NULL;
+  __pyx_pybuffer_z.refcount = 0;
+  __pyx_pybuffernd_z.data = NULL;
+  __pyx_pybuffernd_z.rcbuffer = &__pyx_pybuffer_z;
+  __pyx_pybuffer_deadline.pybuffer.buf = NULL;
+  __pyx_pybuffer_deadline.refcount = 0;
+  __pyx_pybuffernd_deadline.data = NULL;
+  __pyx_pybuffernd_deadline.rcbuffer = &__pyx_pybuffer_deadline;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_v.rcbuffer->pybuffer, (PyObject*)__pyx_v_v, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_v.diminfo[0].strides = __pyx_pybuffernd_v.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_v.diminfo[0].shape = __pyx_pybuffernd_v.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_v.diminfo[1].strides = __pyx_pybuffernd_v.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_v.diminfo[1].shape = __pyx_pybuffernd_v.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_a.diminfo[1].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_a.diminfo[1].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_z.rcbuffer->pybuffer, (PyObject*)__pyx_v_z, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_z.diminfo[0].strides = __pyx_pybuffernd_z.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_z.diminfo[0].shape = __pyx_pybuffernd_z.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_z.diminfo[1].strides = __pyx_pybuffernd_z.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_z.diminfo[1].shape = __pyx_pybuffernd_z.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_deadline.diminfo[0].strides = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_deadline.diminfo[0].shape = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.shape[0];
+
+  /* "cssm.pyx":3345
+ * 
+ *     # Param views
+ *     cdef float[:, :] v_view = v             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_v), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3345, __pyx_L1_error)
+  __pyx_v_v_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3346
+ *     # Param views
+ *     cdef float[:, :] v_view = v
+ *     cdef float[:, :] a_view = a             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] z_view = z
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3346, __pyx_L1_error)
+  __pyx_v_a_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3347
+ *     cdef float[:, :] v_view = v
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z             # <<<<<<<<<<<<<<
+ * 
+ *     cdef float[:] deadline_view = deadline
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_z), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3347, __pyx_L1_error)
+  __pyx_v_z_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3349
+ *     cdef float[:, :] z_view = z
+ * 
+ *     cdef float[:] deadline_view = deadline             # <<<<<<<<<<<<<<
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+ */
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3349, __pyx_L1_error)
+  __pyx_v_deadline_view = __pyx_t_2;
+  __pyx_t_2.memview = NULL;
+  __pyx_t_2.data = NULL;
+
+  /* "cssm.pyx":3351
+ *     cdef float[:] deadline_view = deadline
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
+ *     cdef float[:, :, :] rts_view = rts
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 3351, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 3351, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_int_1);
+  __Pyx_GIVEREF(__pyx_int_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_int_1)) __PYX_ERR(0, 3351, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3351, __pyx_L1_error);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3351, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_v_rts = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "cssm.pyx":3352
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+ *     cdef float[:, :, :] rts_view = rts             # <<<<<<<<<<<<<<
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+ */
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3352, __pyx_L1_error)
+  __pyx_v_rts_view = __pyx_t_7;
+  __pyx_t_7.memview = NULL;
+  __pyx_t_7.data = NULL;
+
+  /* "cssm.pyx":3354
+ *     cdef float[:, :, :] rts_view = rts
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)             # <<<<<<<<<<<<<<
+ *     cdef int[:, :, :] choices_view = choices
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3354, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5)) __PYX_ERR(0, 3354, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_int_1);
+  __Pyx_GIVEREF(__pyx_int_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_1)) __PYX_ERR(0, 3354, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 3354, __pyx_L1_error);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_intc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3354, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_choices = __pyx_t_8;
+  __pyx_t_8 = 0;
+
+  /* "cssm.pyx":3355
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+ *     cdef int[:, :, :] choices_view = choices             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t n, k, i
+ */
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 3355, __pyx_L1_error)
+  __pyx_v_choices_view = __pyx_t_9;
+  __pyx_t_9.memview = NULL;
+  __pyx_t_9.data = NULL;
+
+  /* "cssm.pyx":3359
+ *     cdef Py_ssize_t n, k, i
+ * 
+ *     for k in range(n_trials):             # <<<<<<<<<<<<<<
+ * 
+ *         for n in range(n_samples):
+ */
+  __pyx_t_10 = __pyx_v_n_trials;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_k = __pyx_t_12;
+
+    /* "cssm.pyx":3361
+ *     for k in range(n_trials):
+ * 
+ *         for n in range(n_samples):             # <<<<<<<<<<<<<<
+ *             zs = np.random.uniform(0, z_view[k], nact)
+ * 
+ */
+    __pyx_t_13 = __pyx_v_n_samples;
+    __pyx_t_14 = __pyx_t_13;
+    for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
+      __pyx_v_n = __pyx_t_15;
+
+      /* "cssm.pyx":3362
+ * 
+ *         for n in range(n_samples):
+ *             zs = np.random.uniform(0, z_view[k], nact)             # <<<<<<<<<<<<<<
+ * 
+ *             vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3362, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_random); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3362, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uniform); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3362, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_2.data = __pyx_v_z_view.data;
+      __pyx_t_2.memview = __pyx_v_z_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_z_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_z_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_z_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_5 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3362, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_nact); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3362, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_3 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_int_0, __pyx_t_5, __pyx_t_6};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_16, 3+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3362, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      __Pyx_XDECREF_SET(__pyx_v_zs, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3364
+ *             zs = np.random.uniform(0, z_view[k], nact)
+ * 
+ *             vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs             # <<<<<<<<<<<<<<
+ * 
+ *             x_t = ([a_view[k]]*nact - zs)/vs
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_abs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_normal); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_2.data = __pyx_v_v_view.data;
+      __pyx_t_2.memview = __pyx_v_v_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_v_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_v_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_v_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_3 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_17 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3364, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_17);
+      __pyx_t_18 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_18)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_18);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[3] = {__pyx_t_18, __pyx_t_3, __pyx_t_17};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_16, 2+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3364, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_5 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3364, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      }
+      __Pyx_XDECREF_SET(__pyx_v_vs, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3366
+ *             vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs
+ * 
+ *             x_t = ([a_view[k]]*nact - zs)/vs             # <<<<<<<<<<<<<<
+ * 
+ *             choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n
+ */
+      __pyx_t_2.data = __pyx_v_a_view.data;
+      __pyx_t_2.memview = __pyx_v_a_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_a_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_a_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_a_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_8 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3366, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_6 = PyList_New(1 * ((__pyx_v_nact<0) ? 0:__pyx_v_nact)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3366, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      { Py_ssize_t __pyx_temp;
+        for (__pyx_temp=0; __pyx_temp < __pyx_v_nact; __pyx_temp++) {
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_GIVEREF(__pyx_t_8);
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_6, __pyx_temp, __pyx_t_8)) __PYX_ERR(0, 3366, __pyx_L1_error);
+        }
+      }
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = PyNumber_Subtract(__pyx_t_6, __pyx_v_zs); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3366, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_t_8, __pyx_v_vs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3366, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_x_t, __pyx_t_6);
+      __pyx_t_6 = 0;
+
+      /* "cssm.pyx":3368
+ *             x_t = ([a_view[k]]*nact - zs)/vs
+ * 
+ *             choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n             # <<<<<<<<<<<<<<
+ *             rts_view[n, k, 0] = np.min(x_t) + ndt  # store reaction time for sample n
+ * 
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3368, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_argmin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3368, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_8)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_v_x_t};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3368, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      __pyx_t_16 = __Pyx_PyInt_As_int(__pyx_t_6); if (unlikely((__pyx_t_16 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3368, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_19 = __pyx_v_n;
+      __pyx_t_20 = __pyx_v_k;
+      __pyx_t_21 = 0;
+      *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_19 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_20 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_21 * __pyx_v_choices_view.strides[2]) )) = __pyx_t_16;
+
+      /* "cssm.pyx":3369
+ * 
+ *             choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n
+ *             rts_view[n, k, 0] = np.min(x_t) + ndt  # store reaction time for sample n             # <<<<<<<<<<<<<<
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3369, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_min); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3369, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_8))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+          __Pyx_INCREF(__pyx_t_4);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_8, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v_x_t};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3369, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      }
+      __pyx_t_8 = PyFloat_FromDouble(__pyx_v_ndt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3369, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_4 = PyNumber_Add(__pyx_t_6, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3369, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_22 = __pyx_PyFloat_AsFloat(__pyx_t_4); if (unlikely((__pyx_t_22 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3369, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_21 = __pyx_v_n;
+      __pyx_t_20 = __pyx_v_k;
+      __pyx_t_19 = 0;
+      *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_21 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_20 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[2]) )) = __pyx_t_22;
+
+      /* "cssm.pyx":3372
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = -999
+ * 
+ */
+      __pyx_t_19 = __pyx_v_n;
+      __pyx_t_20 = __pyx_v_k;
+      __pyx_t_21 = 0;
+      __pyx_t_23 = __pyx_v_k;
+      __pyx_t_24 = ((*((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_19 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_20 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_21 * __pyx_v_rts_view.strides[2]) ))) >= (*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_23 * __pyx_v_deadline_view.strides[0]) ))));
+      if (__pyx_t_24) {
+
+        /* "cssm.pyx":3373
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:
+ *                 rts_view[n, k, 0] = -999             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+        __pyx_t_23 = __pyx_v_n;
+        __pyx_t_21 = __pyx_v_k;
+        __pyx_t_20 = 0;
+        *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_23 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_21 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_20 * __pyx_v_rts_view.strides[2]) )) = -999.0;
+
+        /* "cssm.pyx":3372
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = -999
+ * 
+ */
+      }
+    }
+  }
+
+  /* "cssm.pyx":3376
+ * 
+ * 
+ *     v_dict = {}             # <<<<<<<<<<<<<<
+ *     for i in range(nact):
+ *         v_dict['v_' + str(i)] = v[:, i]
+ */
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3376, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_v_v_dict = ((PyObject*)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cssm.pyx":3377
+ * 
+ *     v_dict = {}
+ *     for i in range(nact):             # <<<<<<<<<<<<<<
+ *         v_dict['v_' + str(i)] = v[:, i]
+ * 
+ */
+  __pyx_t_10 = __pyx_v_nact;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_i = __pyx_t_12;
+
+    /* "cssm.pyx":3378
+ *     v_dict = {}
+ *     for i in range(nact):
+ *         v_dict['v_' + str(i)] = v[:, i]             # <<<<<<<<<<<<<<
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ */
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_INCREF(__pyx_slice__5);
+    __Pyx_GIVEREF(__pyx_slice__5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_slice__5)) __PYX_ERR(0, 3378, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_4)) __PYX_ERR(0, 3378, __pyx_L1_error);
+    __pyx_t_4 = 0;
+    __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_v), __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_6 = __Pyx_PyObject_Str(__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __pyx_t_8 = PyNumber_Add(__pyx_n_u_v_2, __pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely((PyDict_SetItem(__pyx_v_v_dict, __pyx_t_8, __pyx_t_4) < 0))) __PYX_ERR(0, 3378, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  }
+
+  /* "cssm.pyx":3380
+ *         v_dict['v_' + str(i)] = v[:, i]
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,             # <<<<<<<<<<<<<<
+ *                                                          'a': a,
+ *                                                          'z': z,
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3380, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3380, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3380, __pyx_L1_error)
+  __pyx_t_8 = PyDict_Copy(__pyx_v_v_dict); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3380, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+
+  /* "cssm.pyx":3381
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ *                                                          'a': a,             # <<<<<<<<<<<<<<
+ *                                                          'z': z,
+ *                                                          'deadline': deadline,
+ */
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 3381, __pyx_L1_error)
+
+  /* "cssm.pyx":3382
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ *                                                          'a': a,
+ *                                                          'z': z,             # <<<<<<<<<<<<<<
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,
+ */
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_z, ((PyObject *)__pyx_v_z)) < 0) __PYX_ERR(0, 3382, __pyx_L1_error)
+
+  /* "cssm.pyx":3383
+ *                                                          'a': a,
+ *                                                          'z': z,
+ *                                                          'deadline': deadline,             # <<<<<<<<<<<<<<
+ *                                                          'sd': sd,
+ *                                                          'n_samples': n_samples,
+ */
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 3383, __pyx_L1_error)
+
+  /* "cssm.pyx":3384
+ *                                                          'z': z,
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,             # <<<<<<<<<<<<<<
+ *                                                          'n_samples': n_samples,
+ *                                                          'simulator' : 'lba_vanilla',
+ */
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3384, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_sd, __pyx_t_6) < 0) __PYX_ERR(0, 3384, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+  /* "cssm.pyx":3385
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,
+ *                                                          'n_samples': n_samples,             # <<<<<<<<<<<<<<
+ *                                                          'simulator' : 'lba_vanilla',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),
+ */
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3385, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_n_samples, __pyx_t_6) < 0) __PYX_ERR(0, 3385, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_simulator, __pyx_n_u_lba_vanilla) < 0) __PYX_ERR(0, 3386, __pyx_L1_error)
+
+  /* "cssm.pyx":3387
+ *                                                          'n_samples': n_samples,
+ *                                                          'simulator' : 'lba_vanilla',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),             # <<<<<<<<<<<<<<
+ *                                                          'max_t': max_t,
+ *                                                          }}
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_17);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nact); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_3 = NULL;
+  __pyx_t_10 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_17))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_17);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_17);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_17, function);
+      __pyx_t_10 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_int_0, __pyx_t_5, __pyx_int_1};
+    __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_10, 3+__pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3387, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  }
+  __pyx_t_17 = __Pyx_PySequence_ListKeepNew(__pyx_t_6); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_17);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_possible_choices, __pyx_t_17) < 0) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+
+  /* "cssm.pyx":3388
+ *                                                          'simulator' : 'lba_vanilla',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),
+ *                                                          'max_t': max_t,             # <<<<<<<<<<<<<<
+ *                                                          }}
+ * 
+ */
+  __pyx_t_17 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_17);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_max_t, __pyx_t_17) < 0) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_metadata, __pyx_t_8) < 0) __PYX_ERR(0, 3380, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_r = __pyx_t_4;
+  __pyx_t_4 = 0;
+  goto __pyx_L0;
+
+  /* "cssm.pyx":3327
+ * 
+ * # Simulate (rt, choice) tuples from: Vanilla LBA Model without ndt -----------------------------
+ * def lba_vanilla(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_1, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
+  __Pyx_XDECREF(__pyx_t_8);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_XDECREF(__pyx_t_17);
+  __Pyx_XDECREF(__pyx_t_18);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("cssm.lba_vanilla", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_v_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_a_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_z_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_deadline_view, 1);
+  __Pyx_XDECREF(__pyx_v_rts);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_rts_view, 1);
+  __Pyx_XDECREF(__pyx_v_choices);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_choices_view, 1);
+  __Pyx_XDECREF(__pyx_v_zs);
+  __Pyx_XDECREF(__pyx_v_vs);
+  __Pyx_XDECREF(__pyx_v_x_t);
+  __Pyx_XDECREF(__pyx_v_v_dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "cssm.pyx":3394
+ * 
+ * # Simulate (rt, choice) tuples from: Collapsing bound angle LBA Model -----------------------------
+ * def lba_angle(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4cssm_37lba_angle(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_4cssm_37lba_angle = {"lba_angle", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_37lba_angle, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cssm_37lba_angle(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_v = 0;
+  PyArrayObject *__pyx_v_a = 0;
+  PyArrayObject *__pyx_v_z = 0;
+  PyArrayObject *__pyx_v_theta = 0;
+  PyArrayObject *__pyx_v_deadline = 0;
+  float __pyx_v_sd;
+  float __pyx_v_ndt;
+  int __pyx_v_nact;
+  int __pyx_v_n_samples;
+  int __pyx_v_n_trials;
+  float __pyx_v_max_t;
+  CYTHON_UNUSED PyObject *__pyx_v_kwargs = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("lba_angle (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kwargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_v,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_theta,&__pyx_n_s_deadline,&__pyx_n_s_sd,&__pyx_n_s_ndt,&__pyx_n_s_nact,&__pyx_n_s_n_samples,&__pyx_n_s_n_trials,&__pyx_n_s_max_t,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_v)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_a)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_angle", 0, 6, 11, 1); __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_z)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_angle", 0, 6, 11, 2); __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_theta)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_angle", 0, 6, 11, 3); __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_deadline)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_angle", 0, 6, 11, 4); __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sd)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("lba_angle", 0, 6, 11, 5); __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ndt);
+          if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nact);
+          if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_samples);
+          if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  9:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_trials);
+          if (value) { values[9] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case 10:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_t);
+          if (value) { values[10] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3394, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "lba_angle") < 0)) __PYX_ERR(0, 3394, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+        values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_v = ((PyArrayObject *)values[0]);
+    __pyx_v_a = ((PyArrayObject *)values[1]);
+    __pyx_v_z = ((PyArrayObject *)values[2]);
+    __pyx_v_theta = ((PyArrayObject *)values[3]);
+    __pyx_v_deadline = ((PyArrayObject *)values[4]);
+    __pyx_v_sd = __pyx_PyFloat_AsFloat(values[5]); if (unlikely((__pyx_v_sd == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3399, __pyx_L3_error)
+    if (values[6]) {
+      __pyx_v_ndt = __pyx_PyFloat_AsFloat(values[6]); if (unlikely((__pyx_v_ndt == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3400, __pyx_L3_error)
+    } else {
+      __pyx_v_ndt = ((float)((float)0.0));
+    }
+    if (values[7]) {
+      __pyx_v_nact = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_nact == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3401, __pyx_L3_error)
+    } else {
+      __pyx_v_nact = ((int)((int)3));
+    }
+    if (values[8]) {
+      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3402, __pyx_L3_error)
+    } else {
+      __pyx_v_n_samples = ((int)((int)0x7D0));
+    }
+    if (values[9]) {
+      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[9]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3403, __pyx_L3_error)
+    } else {
+      __pyx_v_n_trials = ((int)((int)1));
+    }
+    if (values[10]) {
+      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[10]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3404, __pyx_L3_error)
+    } else {
+      __pyx_v_max_t = ((float)((float)20.0));
+    }
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("lba_angle", 0, 6, 11, __pyx_nargs); __PYX_ERR(0, 3394, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+  __Pyx_AddTraceback("cssm.lba_angle", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_v), __pyx_ptype_5numpy_ndarray, 1, "v", 0))) __PYX_ERR(0, 3394, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 3395, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_z), __pyx_ptype_5numpy_ndarray, 1, "z", 0))) __PYX_ERR(0, 3396, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_theta), __pyx_ptype_5numpy_ndarray, 1, "theta", 0))) __PYX_ERR(0, 3397, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 3398, __pyx_L1_error)
+  __pyx_r = __pyx_pf_4cssm_36lba_angle(__pyx_self, __pyx_v_v, __pyx_v_a, __pyx_v_z, __pyx_v_theta, __pyx_v_deadline, __pyx_v_sd, __pyx_v_ndt, __pyx_v_nact, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_max_t, __pyx_v_kwargs);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_DECREF(__pyx_v_kwargs);
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4cssm_36lba_angle(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_theta, PyArrayObject *__pyx_v_deadline, float __pyx_v_sd, float __pyx_v_ndt, int __pyx_v_nact, int __pyx_v_n_samples, int __pyx_v_n_trials, float __pyx_v_max_t, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
+  __Pyx_memviewslice __pyx_v_v_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_a_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_z_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_theta_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_deadline_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_rts = NULL;
+  __Pyx_memviewslice __pyx_v_rts_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_choices = NULL;
+  __Pyx_memviewslice __pyx_v_choices_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_v_n;
+  Py_ssize_t __pyx_v_k;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_zs = NULL;
+  PyObject *__pyx_v_vs = NULL;
+  PyObject *__pyx_v_x_t = NULL;
+  PyObject *__pyx_v_v_dict = NULL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_a;
+  __Pyx_Buffer __pyx_pybuffer_a;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_deadline;
+  __Pyx_Buffer __pyx_pybuffer_deadline;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_theta;
+  __Pyx_Buffer __pyx_pybuffer_theta;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_v;
+  __Pyx_Buffer __pyx_pybuffer_v;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_z;
+  __Pyx_Buffer __pyx_pybuffer_z;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_memviewslice __pyx_t_1 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_t_2 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_t_8 = NULL;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_t_10;
+  int __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  int __pyx_t_13;
+  int __pyx_t_14;
+  Py_ssize_t __pyx_t_15;
+  int __pyx_t_16;
+  PyObject *__pyx_t_17 = NULL;
+  PyObject *__pyx_t_18 = NULL;
+  Py_ssize_t __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  Py_ssize_t __pyx_t_21;
+  float __pyx_t_22;
+  Py_ssize_t __pyx_t_23;
+  int __pyx_t_24;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("lba_angle", 1);
+  __pyx_pybuffer_v.pybuffer.buf = NULL;
+  __pyx_pybuffer_v.refcount = 0;
+  __pyx_pybuffernd_v.data = NULL;
+  __pyx_pybuffernd_v.rcbuffer = &__pyx_pybuffer_v;
+  __pyx_pybuffer_a.pybuffer.buf = NULL;
+  __pyx_pybuffer_a.refcount = 0;
+  __pyx_pybuffernd_a.data = NULL;
+  __pyx_pybuffernd_a.rcbuffer = &__pyx_pybuffer_a;
+  __pyx_pybuffer_z.pybuffer.buf = NULL;
+  __pyx_pybuffer_z.refcount = 0;
+  __pyx_pybuffernd_z.data = NULL;
+  __pyx_pybuffernd_z.rcbuffer = &__pyx_pybuffer_z;
+  __pyx_pybuffer_theta.pybuffer.buf = NULL;
+  __pyx_pybuffer_theta.refcount = 0;
+  __pyx_pybuffernd_theta.data = NULL;
+  __pyx_pybuffernd_theta.rcbuffer = &__pyx_pybuffer_theta;
+  __pyx_pybuffer_deadline.pybuffer.buf = NULL;
+  __pyx_pybuffer_deadline.refcount = 0;
+  __pyx_pybuffernd_deadline.data = NULL;
+  __pyx_pybuffernd_deadline.rcbuffer = &__pyx_pybuffer_deadline;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_v.rcbuffer->pybuffer, (PyObject*)__pyx_v_v, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_v.diminfo[0].strides = __pyx_pybuffernd_v.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_v.diminfo[0].shape = __pyx_pybuffernd_v.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_v.diminfo[1].strides = __pyx_pybuffernd_v.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_v.diminfo[1].shape = __pyx_pybuffernd_v.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_a.diminfo[1].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_a.diminfo[1].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_z.rcbuffer->pybuffer, (PyObject*)__pyx_v_z, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_z.diminfo[0].strides = __pyx_pybuffernd_z.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_z.diminfo[0].shape = __pyx_pybuffernd_z.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_z.diminfo[1].strides = __pyx_pybuffernd_z.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_z.diminfo[1].shape = __pyx_pybuffernd_z.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_theta.rcbuffer->pybuffer, (PyObject*)__pyx_v_theta, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_theta.diminfo[0].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_theta.diminfo[0].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_theta.diminfo[1].strides = __pyx_pybuffernd_theta.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_theta.diminfo[1].shape = __pyx_pybuffernd_theta.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_deadline.diminfo[0].strides = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_deadline.diminfo[0].shape = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.shape[0];
+
+  /* "cssm.pyx":3409
+ * 
+ *     # Param views
+ *     cdef float[:, :] v_view = v             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_v), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3409, __pyx_L1_error)
+  __pyx_v_v_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3410
+ *     # Param views
+ *     cdef float[:, :] v_view = v
+ *     cdef float[:, :] a_view = a             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] z_view = z
+ *     cdef float[:, :] theta_view = theta
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3410, __pyx_L1_error)
+  __pyx_v_a_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3411
+ *     cdef float[:, :] v_view = v
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] theta_view = theta
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_z), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3411, __pyx_L1_error)
+  __pyx_v_z_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3412
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z
+ *     cdef float[:, :] theta_view = theta             # <<<<<<<<<<<<<<
+ * 
+ *     cdef float[:] deadline_view = deadline
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_theta), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3412, __pyx_L1_error)
+  __pyx_v_theta_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3414
+ *     cdef float[:, :] theta_view = theta
+ * 
+ *     cdef float[:] deadline_view = deadline             # <<<<<<<<<<<<<<
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+ */
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3414, __pyx_L1_error)
+  __pyx_v_deadline_view = __pyx_t_2;
+  __pyx_t_2.memview = NULL;
+  __pyx_t_2.data = NULL;
+
+  /* "cssm.pyx":3416
+ *     cdef float[:] deadline_view = deadline
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
+ *     cdef float[:, :, :] rts_view = rts
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 3416, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 3416, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_int_1);
+  __Pyx_GIVEREF(__pyx_int_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_int_1)) __PYX_ERR(0, 3416, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3416, __pyx_L1_error);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3416, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_v_rts = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "cssm.pyx":3417
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+ *     cdef float[:, :, :] rts_view = rts             # <<<<<<<<<<<<<<
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+ */
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3417, __pyx_L1_error)
+  __pyx_v_rts_view = __pyx_t_7;
+  __pyx_t_7.memview = NULL;
+  __pyx_t_7.data = NULL;
+
+  /* "cssm.pyx":3419
+ *     cdef float[:, :, :] rts_view = rts
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)             # <<<<<<<<<<<<<<
+ *     cdef int[:, :, :] choices_view = choices
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3419, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5)) __PYX_ERR(0, 3419, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_int_1);
+  __Pyx_GIVEREF(__pyx_int_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_1)) __PYX_ERR(0, 3419, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 3419, __pyx_L1_error);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_intc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3419, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_choices = __pyx_t_8;
+  __pyx_t_8 = 0;
+
+  /* "cssm.pyx":3420
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+ *     cdef int[:, :, :] choices_view = choices             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t n, k, i
+ */
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 3420, __pyx_L1_error)
+  __pyx_v_choices_view = __pyx_t_9;
+  __pyx_t_9.memview = NULL;
+  __pyx_t_9.data = NULL;
+
+  /* "cssm.pyx":3424
+ *     cdef Py_ssize_t n, k, i
+ * 
+ *     for k in range(n_trials):             # <<<<<<<<<<<<<<
+ * 
+ *         for n in range(n_samples):
+ */
+  __pyx_t_10 = __pyx_v_n_trials;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_k = __pyx_t_12;
+
+    /* "cssm.pyx":3426
+ *     for k in range(n_trials):
+ * 
+ *         for n in range(n_samples):             # <<<<<<<<<<<<<<
+ *             zs = np.random.uniform(0, z_view[k], nact)
+ * 
+ */
+    __pyx_t_13 = __pyx_v_n_samples;
+    __pyx_t_14 = __pyx_t_13;
+    for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
+      __pyx_v_n = __pyx_t_15;
+
+      /* "cssm.pyx":3427
+ * 
+ *         for n in range(n_samples):
+ *             zs = np.random.uniform(0, z_view[k], nact)             # <<<<<<<<<<<<<<
+ * 
+ *             vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_random); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_uniform); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_2.data = __pyx_v_z_view.data;
+      __pyx_t_2.memview = __pyx_v_z_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_z_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_z_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_z_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_5 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_nact); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3427, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_3 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_int_0, __pyx_t_5, __pyx_t_6};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_16, 3+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3427, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      __Pyx_XDECREF_SET(__pyx_v_zs, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3429
+ *             zs = np.random.uniform(0, z_view[k], nact)
+ * 
+ *             vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs             # <<<<<<<<<<<<<<
+ *             x_t = ([a_view[k]]*nact - zs)/(vs + np.tan(theta_view[k, 0]))
+ * 
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_abs); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_random); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_normal); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_2.data = __pyx_v_v_view.data;
+      __pyx_t_2.memview = __pyx_v_v_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_v_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_v_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_v_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_3 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_17 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3429, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_17);
+      __pyx_t_18 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_18 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_18)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_18);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[3] = {__pyx_t_18, __pyx_t_3, __pyx_t_17};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_16, 2+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_18); __pyx_t_18 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3429, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_5 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_6))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_6, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_t_4};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3429, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      }
+      __Pyx_XDECREF_SET(__pyx_v_vs, __pyx_t_8);
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3430
+ * 
+ *             vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs
+ *             x_t = ([a_view[k]]*nact - zs)/(vs + np.tan(theta_view[k, 0]))             # <<<<<<<<<<<<<<
+ * 
+ *             choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n
+ */
+      __pyx_t_2.data = __pyx_v_a_view.data;
+      __pyx_t_2.memview = __pyx_v_a_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_a_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_a_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_a_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_8 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_6 = PyList_New(1 * ((__pyx_v_nact<0) ? 0:__pyx_v_nact)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      { Py_ssize_t __pyx_temp;
+        for (__pyx_temp=0; __pyx_temp < __pyx_v_nact; __pyx_temp++) {
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_GIVEREF(__pyx_t_8);
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_6, __pyx_temp, __pyx_t_8)) __PYX_ERR(0, 3430, __pyx_L1_error);
+        }
+      }
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = PyNumber_Subtract(__pyx_t_6, __pyx_v_zs); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_tan); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_19 = __pyx_v_k;
+      __pyx_t_20 = 0;
+      __pyx_t_4 = PyFloat_FromDouble((*((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_theta_view.data + __pyx_t_19 * __pyx_v_theta_view.strides[0]) ) + __pyx_t_20 * __pyx_v_theta_view.strides[1]) )))); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_17 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_17 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_17)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_17);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_17, __pyx_t_4};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_17); __pyx_t_17 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3430, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_5 = PyNumber_Add(__pyx_v_vs, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_6 = __Pyx_PyNumber_Divide(__pyx_t_8, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3430, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_x_t, __pyx_t_6);
+      __pyx_t_6 = 0;
+
+      /* "cssm.pyx":3432
+ *             x_t = ([a_view[k]]*nact - zs)/(vs + np.tan(theta_view[k, 0]))
+ * 
+ *             choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n             # <<<<<<<<<<<<<<
+ *             rts_view[n, k, 0] = np.min(x_t) + ndt # store reaction time for sample n
+ * 
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3432, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_argmin); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3432, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_8))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_8);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_8, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, __pyx_v_x_t};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3432, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      }
+      __pyx_t_16 = __Pyx_PyInt_As_int(__pyx_t_6); if (unlikely((__pyx_t_16 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3432, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_20 = __pyx_v_n;
+      __pyx_t_19 = __pyx_v_k;
+      __pyx_t_21 = 0;
+      *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_20 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_21 * __pyx_v_choices_view.strides[2]) )) = __pyx_t_16;
+
+      /* "cssm.pyx":3433
+ * 
+ *             choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n
+ *             rts_view[n, k, 0] = np.min(x_t) + ndt # store reaction time for sample n             # <<<<<<<<<<<<<<
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3433, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_min); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3433, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = NULL;
+      __pyx_t_16 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_8)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_16 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_v_x_t};
+        __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3433, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_6);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_5 = PyFloat_FromDouble(__pyx_v_ndt); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3433, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_8 = PyNumber_Add(__pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3433, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_22 = __pyx_PyFloat_AsFloat(__pyx_t_8); if (unlikely((__pyx_t_22 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3433, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_21 = __pyx_v_n;
+      __pyx_t_19 = __pyx_v_k;
+      __pyx_t_20 = 0;
+      *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_21 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_20 * __pyx_v_rts_view.strides[2]) )) = __pyx_t_22;
+
+      /* "cssm.pyx":3436
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = -999
+ * 
+ */
+      __pyx_t_20 = __pyx_v_n;
+      __pyx_t_19 = __pyx_v_k;
+      __pyx_t_21 = 0;
+      __pyx_t_23 = __pyx_v_k;
+      __pyx_t_24 = ((*((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_20 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_21 * __pyx_v_rts_view.strides[2]) ))) >= (*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_23 * __pyx_v_deadline_view.strides[0]) ))));
+      if (__pyx_t_24) {
+
+        /* "cssm.pyx":3437
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:
+ *                 rts_view[n, k, 0] = -999             # <<<<<<<<<<<<<<
+ * 
+ *             # if np.min(x_t) <= 0:
+ */
+        __pyx_t_23 = __pyx_v_n;
+        __pyx_t_21 = __pyx_v_k;
+        __pyx_t_19 = 0;
+        *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_23 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_21 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[2]) )) = -999.0;
+
+        /* "cssm.pyx":3436
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = -999
+ * 
+ */
+      }
+    }
+  }
+
+  /* "cssm.pyx":3442
+ *             #     print("\n ssms sim error: ", a[k], zs, vs, np.tan(theta[k]))
+ * 
+ *     v_dict = {}             # <<<<<<<<<<<<<<
+ *     for i in range(nact):
+ *         v_dict['v_' + str(i)] = v[:, i]
+ */
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3442, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __pyx_v_v_dict = ((PyObject*)__pyx_t_8);
+  __pyx_t_8 = 0;
+
+  /* "cssm.pyx":3443
+ * 
+ *     v_dict = {}
+ *     for i in range(nact):             # <<<<<<<<<<<<<<
+ *         v_dict['v_' + str(i)] = v[:, i]
+ * 
+ */
+  __pyx_t_10 = __pyx_v_nact;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_i = __pyx_t_12;
+
+    /* "cssm.pyx":3444
+ *     v_dict = {}
+ *     for i in range(nact):
+ *         v_dict['v_' + str(i)] = v[:, i]             # <<<<<<<<<<<<<<
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ */
+    __pyx_t_8 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_INCREF(__pyx_slice__5);
+    __Pyx_GIVEREF(__pyx_slice__5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_slice__5)) __PYX_ERR(0, 3444, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_8);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_8)) __PYX_ERR(0, 3444, __pyx_L1_error);
+    __pyx_t_8 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_v), __pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = __Pyx_PyObject_Str(__pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = PyNumber_Add(__pyx_n_u_v_2, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely((PyDict_SetItem(__pyx_v_v_dict, __pyx_t_5, __pyx_t_8) < 0))) __PYX_ERR(0, 3444, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  }
+
+  /* "cssm.pyx":3446
+ *         v_dict['v_' + str(i)] = v[:, i]
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,             # <<<<<<<<<<<<<<
+ *                                                          'a': a,
+ *                                                          'z': z,
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3446, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3446, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3446, __pyx_L1_error)
+  __pyx_t_5 = PyDict_Copy(__pyx_v_v_dict); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3446, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "cssm.pyx":3447
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ *                                                          'a': a,             # <<<<<<<<<<<<<<
+ *                                                          'z': z,
+ *                                                          'theta': theta,
+ */
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 3447, __pyx_L1_error)
+
+  /* "cssm.pyx":3448
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ *                                                          'a': a,
+ *                                                          'z': z,             # <<<<<<<<<<<<<<
+ *                                                          'theta': theta,
+ *                                                          'deadline': deadline,
+ */
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_z, ((PyObject *)__pyx_v_z)) < 0) __PYX_ERR(0, 3448, __pyx_L1_error)
+
+  /* "cssm.pyx":3449
+ *                                                          'a': a,
+ *                                                          'z': z,
+ *                                                          'theta': theta,             # <<<<<<<<<<<<<<
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,
+ */
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_theta, ((PyObject *)__pyx_v_theta)) < 0) __PYX_ERR(0, 3449, __pyx_L1_error)
+
+  /* "cssm.pyx":3450
+ *                                                          'z': z,
+ *                                                          'theta': theta,
+ *                                                          'deadline': deadline,             # <<<<<<<<<<<<<<
+ *                                                          'sd': sd,
+ *                                                          'n_samples': n_samples,
+ */
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 3450, __pyx_L1_error)
+
+  /* "cssm.pyx":3451
+ *                                                          'theta': theta,
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,             # <<<<<<<<<<<<<<
+ *                                                          'n_samples': n_samples,
+ *                                                          'simulator' : 'lba_angle',
+ */
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3451, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_sd, __pyx_t_6) < 0) __PYX_ERR(0, 3451, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+  /* "cssm.pyx":3452
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,
+ *                                                          'n_samples': n_samples,             # <<<<<<<<<<<<<<
+ *                                                          'simulator' : 'lba_angle',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),
+ */
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3452, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_n_samples, __pyx_t_6) < 0) __PYX_ERR(0, 3452, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_simulator, __pyx_n_u_lba_angle) < 0) __PYX_ERR(0, 3453, __pyx_L1_error)
+
+  /* "cssm.pyx":3454
+ *                                                          'n_samples': n_samples,
+ *                                                          'simulator' : 'lba_angle',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),             # <<<<<<<<<<<<<<
+ *                                                          'max_t': max_t,
+ *                                                          }}
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3454, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_17 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_arange); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3454, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_17);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_nact); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3454, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = NULL;
+  __pyx_t_10 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_17))) {
+    __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_17);
+    if (likely(__pyx_t_3)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_17);
+      __Pyx_INCREF(__pyx_t_3);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_17, function);
+      __pyx_t_10 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[4] = {__pyx_t_3, __pyx_int_0, __pyx_t_4, __pyx_int_1};
+    __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_17, __pyx_callargs+1-__pyx_t_10, 3+__pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3454, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  }
+  __pyx_t_17 = __Pyx_PySequence_ListKeepNew(__pyx_t_6); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3454, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_17);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_possible_choices, __pyx_t_17) < 0) __PYX_ERR(0, 3454, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+
+  /* "cssm.pyx":3455
+ *                                                          'simulator' : 'lba_angle',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),
+ *                                                          'max_t': max_t,             # <<<<<<<<<<<<<<
+ *                                                          }}
+ * 
+ */
+  __pyx_t_17 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 3455, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_17);
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_max_t, __pyx_t_17) < 0) __PYX_ERR(0, 3455, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_u_metadata, __pyx_t_5) < 0) __PYX_ERR(0, 3446, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_r = __pyx_t_8;
+  __pyx_t_8 = 0;
+  goto __pyx_L0;
+
+  /* "cssm.pyx":3394
+ * 
+ * # Simulate (rt, choice) tuples from: Collapsing bound angle LBA Model -----------------------------
+ * def lba_angle(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_1, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
+  __Pyx_XDECREF(__pyx_t_8);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_XDECREF(__pyx_t_17);
+  __Pyx_XDECREF(__pyx_t_18);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_theta.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("cssm.lba_angle", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_theta.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_v_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_a_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_z_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_theta_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_deadline_view, 1);
+  __Pyx_XDECREF(__pyx_v_rts);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_rts_view, 1);
+  __Pyx_XDECREF(__pyx_v_choices);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_choices_view, 1);
+  __Pyx_XDECREF(__pyx_v_zs);
+  __Pyx_XDECREF(__pyx_v_vs);
+  __Pyx_XDECREF(__pyx_v_x_t);
+  __Pyx_XDECREF(__pyx_v_v_dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "cssm.pyx":3460
+ * 
+ * # Simulate (rt, choice) tuples from: RLWM LBA Race Model without ndt -----------------------------
+ * def rlwm_lba_race(np.ndarray[float, ndim = 2] v_RL, # RL drift parameters (np.array expect: one column of floats)             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] v_WM, # WM drift parameters (np.array expect: one column of floats)
+ *         np.ndarray[float, ndim = 2] a, # criterion height
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4cssm_39rlwm_lba_race(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_4cssm_39rlwm_lba_race = {"rlwm_lba_race", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_39rlwm_lba_race, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cssm_39rlwm_lba_race(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  PyArrayObject *__pyx_v_v_RL = 0;
+  PyArrayObject *__pyx_v_v_WM = 0;
+  PyArrayObject *__pyx_v_a = 0;
+  PyArrayObject *__pyx_v_z = 0;
+  PyArrayObject *__pyx_v_deadline = 0;
+  float __pyx_v_sd;
+  float __pyx_v_ndt;
+  int __pyx_v_nact;
+  int __pyx_v_n_samples;
+  int __pyx_v_n_trials;
+  float __pyx_v_max_t;
+  CYTHON_UNUSED PyObject *__pyx_v_kwargs = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("rlwm_lba_race (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
+  __Pyx_GOTREF(__pyx_v_kwargs);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_v_RL,&__pyx_n_s_v_WM,&__pyx_n_s_a,&__pyx_n_s_z,&__pyx_n_s_deadline,&__pyx_n_s_sd,&__pyx_n_s_ndt,&__pyx_n_s_nact,&__pyx_n_s_n_samples,&__pyx_n_s_n_trials,&__pyx_n_s_max_t,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_v_RL)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_v_WM)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("rlwm_lba_race", 0, 6, 11, 1); __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_a)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("rlwm_lba_race", 0, 6, 11, 2); __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_z)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("rlwm_lba_race", 0, 6, 11, 3); __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_deadline)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("rlwm_lba_race", 0, 6, 11, 4); __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_sd)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
+          kw_args--;
+        }
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("rlwm_lba_race", 0, 6, 11, 5); __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  6:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ndt);
+          if (value) { values[6] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  7:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_nact);
+          if (value) { values[7] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  8:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_samples);
+          if (value) { values[8] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  9:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_trials);
+          if (value) { values[9] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case 10:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_t);
+          if (value) { values[10] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3460, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "rlwm_lba_race") < 0)) __PYX_ERR(0, 3460, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case 11: values[10] = __Pyx_Arg_FASTCALL(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
+        case 10: values[9] = __Pyx_Arg_FASTCALL(__pyx_args, 9);
+        CYTHON_FALLTHROUGH;
+        case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
+        CYTHON_FALLTHROUGH;
+        case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
+        CYTHON_FALLTHROUGH;
+        case  7: values[6] = __Pyx_Arg_FASTCALL(__pyx_args, 6);
+        CYTHON_FALLTHROUGH;
+        case  6: values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
+        values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
+        values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_v_RL = ((PyArrayObject *)values[0]);
+    __pyx_v_v_WM = ((PyArrayObject *)values[1]);
+    __pyx_v_a = ((PyArrayObject *)values[2]);
+    __pyx_v_z = ((PyArrayObject *)values[3]);
+    __pyx_v_deadline = ((PyArrayObject *)values[4]);
+    __pyx_v_sd = __pyx_PyFloat_AsFloat(values[5]); if (unlikely((__pyx_v_sd == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3465, __pyx_L3_error)
+    if (values[6]) {
+      __pyx_v_ndt = __pyx_PyFloat_AsFloat(values[6]); if (unlikely((__pyx_v_ndt == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3466, __pyx_L3_error)
+    } else {
+      __pyx_v_ndt = ((float)((float)0.0));
+    }
+    if (values[7]) {
+      __pyx_v_nact = __Pyx_PyInt_As_int(values[7]); if (unlikely((__pyx_v_nact == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3467, __pyx_L3_error)
+    } else {
+      __pyx_v_nact = ((int)((int)3));
+    }
+    if (values[8]) {
+      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[8]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3468, __pyx_L3_error)
+    } else {
+      __pyx_v_n_samples = ((int)((int)0x7D0));
+    }
+    if (values[9]) {
+      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[9]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3469, __pyx_L3_error)
+    } else {
+      __pyx_v_n_trials = ((int)((int)1));
+    }
+    if (values[10]) {
+      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[10]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3470, __pyx_L3_error)
+    } else {
+      __pyx_v_max_t = ((float)((float)20.0));
+    }
+  }
+  goto __pyx_L6_skip;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("rlwm_lba_race", 0, 6, 11, __pyx_nargs); __PYX_ERR(0, 3460, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
+  __Pyx_AddTraceback("cssm.rlwm_lba_race", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_v_RL), __pyx_ptype_5numpy_ndarray, 1, "v_RL", 0))) __PYX_ERR(0, 3460, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_v_WM), __pyx_ptype_5numpy_ndarray, 1, "v_WM", 0))) __PYX_ERR(0, 3461, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 3462, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_z), __pyx_ptype_5numpy_ndarray, 1, "z", 0))) __PYX_ERR(0, 3463, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 3464, __pyx_L1_error)
+  __pyx_r = __pyx_pf_4cssm_38rlwm_lba_race(__pyx_self, __pyx_v_v_RL, __pyx_v_v_WM, __pyx_v_a, __pyx_v_z, __pyx_v_deadline, __pyx_v_sd, __pyx_v_ndt, __pyx_v_nact, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_max_t, __pyx_v_kwargs);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_DECREF(__pyx_v_kwargs);
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4cssm_38rlwm_lba_race(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_v_RL, PyArrayObject *__pyx_v_v_WM, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_z, PyArrayObject *__pyx_v_deadline, float __pyx_v_sd, float __pyx_v_ndt, int __pyx_v_nact, int __pyx_v_n_samples, int __pyx_v_n_trials, float __pyx_v_max_t, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
+  __Pyx_memviewslice __pyx_v_v_RL_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_v_WM_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_a_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_z_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_deadline_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyArrayObject *__pyx_v_zs = 0;
+  PyArrayObject *__pyx_v_x_t_RL = 0;
+  PyArrayObject *__pyx_v_x_t_WM = 0;
+  PyArrayObject *__pyx_v_vs_RL = 0;
+  PyArrayObject *__pyx_v_vs_WM = 0;
+  PyObject *__pyx_v_rts = NULL;
+  __Pyx_memviewslice __pyx_v_rts_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_choices = NULL;
+  __Pyx_memviewslice __pyx_v_choices_view = { 0, 0, { 0 }, { 0 }, { 0 } };
+  Py_ssize_t __pyx_v_n;
+  Py_ssize_t __pyx_v_k;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_v_dict = NULL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_a;
+  __Pyx_Buffer __pyx_pybuffer_a;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_deadline;
+  __Pyx_Buffer __pyx_pybuffer_deadline;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_v_RL;
+  __Pyx_Buffer __pyx_pybuffer_v_RL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_v_WM;
+  __Pyx_Buffer __pyx_pybuffer_v_WM;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_vs_RL;
+  __Pyx_Buffer __pyx_pybuffer_vs_RL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_vs_WM;
+  __Pyx_Buffer __pyx_pybuffer_vs_WM;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_x_t_RL;
+  __Pyx_Buffer __pyx_pybuffer_x_t_RL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_x_t_WM;
+  __Pyx_Buffer __pyx_pybuffer_x_t_WM;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_z;
+  __Pyx_Buffer __pyx_pybuffer_z;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_zs;
+  __Pyx_Buffer __pyx_pybuffer_zs;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_memviewslice __pyx_t_1 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_t_2 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  __Pyx_memviewslice __pyx_t_7 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_t_8 = NULL;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_t_10;
+  int __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  int __pyx_t_13;
+  int __pyx_t_14;
+  Py_ssize_t __pyx_t_15;
+  PyObject *__pyx_t_16 = NULL;
+  int __pyx_t_17;
+  PyArrayObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
+  PyObject *__pyx_t_21 = NULL;
+  PyObject *__pyx_t_22 = NULL;
+  PyArrayObject *__pyx_t_23 = NULL;
+  PyArrayObject *__pyx_t_24 = NULL;
+  PyArrayObject *__pyx_t_25 = NULL;
+  PyArrayObject *__pyx_t_26 = NULL;
+  int __pyx_t_27;
+  float __pyx_t_28;
+  Py_ssize_t __pyx_t_29;
+  Py_ssize_t __pyx_t_30;
+  Py_ssize_t __pyx_t_31;
+  Py_ssize_t __pyx_t_32;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("rlwm_lba_race", 1);
+  __pyx_pybuffer_zs.pybuffer.buf = NULL;
+  __pyx_pybuffer_zs.refcount = 0;
+  __pyx_pybuffernd_zs.data = NULL;
+  __pyx_pybuffernd_zs.rcbuffer = &__pyx_pybuffer_zs;
+  __pyx_pybuffer_x_t_RL.pybuffer.buf = NULL;
+  __pyx_pybuffer_x_t_RL.refcount = 0;
+  __pyx_pybuffernd_x_t_RL.data = NULL;
+  __pyx_pybuffernd_x_t_RL.rcbuffer = &__pyx_pybuffer_x_t_RL;
+  __pyx_pybuffer_x_t_WM.pybuffer.buf = NULL;
+  __pyx_pybuffer_x_t_WM.refcount = 0;
+  __pyx_pybuffernd_x_t_WM.data = NULL;
+  __pyx_pybuffernd_x_t_WM.rcbuffer = &__pyx_pybuffer_x_t_WM;
+  __pyx_pybuffer_vs_RL.pybuffer.buf = NULL;
+  __pyx_pybuffer_vs_RL.refcount = 0;
+  __pyx_pybuffernd_vs_RL.data = NULL;
+  __pyx_pybuffernd_vs_RL.rcbuffer = &__pyx_pybuffer_vs_RL;
+  __pyx_pybuffer_vs_WM.pybuffer.buf = NULL;
+  __pyx_pybuffer_vs_WM.refcount = 0;
+  __pyx_pybuffernd_vs_WM.data = NULL;
+  __pyx_pybuffernd_vs_WM.rcbuffer = &__pyx_pybuffer_vs_WM;
+  __pyx_pybuffer_v_RL.pybuffer.buf = NULL;
+  __pyx_pybuffer_v_RL.refcount = 0;
+  __pyx_pybuffernd_v_RL.data = NULL;
+  __pyx_pybuffernd_v_RL.rcbuffer = &__pyx_pybuffer_v_RL;
+  __pyx_pybuffer_v_WM.pybuffer.buf = NULL;
+  __pyx_pybuffer_v_WM.refcount = 0;
+  __pyx_pybuffernd_v_WM.data = NULL;
+  __pyx_pybuffernd_v_WM.rcbuffer = &__pyx_pybuffer_v_WM;
+  __pyx_pybuffer_a.pybuffer.buf = NULL;
+  __pyx_pybuffer_a.refcount = 0;
+  __pyx_pybuffernd_a.data = NULL;
+  __pyx_pybuffernd_a.rcbuffer = &__pyx_pybuffer_a;
+  __pyx_pybuffer_z.pybuffer.buf = NULL;
+  __pyx_pybuffer_z.refcount = 0;
+  __pyx_pybuffernd_z.data = NULL;
+  __pyx_pybuffernd_z.rcbuffer = &__pyx_pybuffer_z;
+  __pyx_pybuffer_deadline.pybuffer.buf = NULL;
+  __pyx_pybuffer_deadline.refcount = 0;
+  __pyx_pybuffernd_deadline.data = NULL;
+  __pyx_pybuffernd_deadline.rcbuffer = &__pyx_pybuffer_deadline;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_v_RL.rcbuffer->pybuffer, (PyObject*)__pyx_v_v_RL, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_v_RL.diminfo[0].strides = __pyx_pybuffernd_v_RL.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_v_RL.diminfo[0].shape = __pyx_pybuffernd_v_RL.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_v_RL.diminfo[1].strides = __pyx_pybuffernd_v_RL.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_v_RL.diminfo[1].shape = __pyx_pybuffernd_v_RL.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_v_WM.rcbuffer->pybuffer, (PyObject*)__pyx_v_v_WM, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_v_WM.diminfo[0].strides = __pyx_pybuffernd_v_WM.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_v_WM.diminfo[0].shape = __pyx_pybuffernd_v_WM.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_v_WM.diminfo[1].strides = __pyx_pybuffernd_v_WM.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_v_WM.diminfo[1].shape = __pyx_pybuffernd_v_WM.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_a.diminfo[1].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_a.diminfo[1].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_z.rcbuffer->pybuffer, (PyObject*)__pyx_v_z, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_z.diminfo[0].strides = __pyx_pybuffernd_z.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_z.diminfo[0].shape = __pyx_pybuffernd_z.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_z.diminfo[1].strides = __pyx_pybuffernd_z.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_z.diminfo[1].shape = __pyx_pybuffernd_z.rcbuffer->pybuffer.shape[1];
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_deadline.diminfo[0].strides = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_deadline.diminfo[0].shape = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.shape[0];
+
+  /* "cssm.pyx":3479
+ * 
+ *     # Param views
+ *     cdef float[:, :] v_RL_view = v_RL             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] v_WM_view = v_WM
+ *     cdef float[:, :] a_view = a
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_v_RL), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3479, __pyx_L1_error)
+  __pyx_v_v_RL_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3480
+ *     # Param views
+ *     cdef float[:, :] v_RL_view = v_RL
+ *     cdef float[:, :] v_WM_view = v_WM             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_v_WM), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3480, __pyx_L1_error)
+  __pyx_v_v_WM_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3481
+ *     cdef float[:, :] v_RL_view = v_RL
+ *     cdef float[:, :] v_WM_view = v_WM
+ *     cdef float[:, :] a_view = a             # <<<<<<<<<<<<<<
+ *     cdef float[:, :] z_view = z
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3481, __pyx_L1_error)
+  __pyx_v_a_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3482
+ *     cdef float[:, :] v_WM_view = v_WM
+ *     cdef float[:, :] a_view = a
+ *     cdef float[:, :] z_view = z             # <<<<<<<<<<<<<<
+ * 
+ *     cdef float[:] deadline_view = deadline
+ */
+  __pyx_t_1 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(((PyObject *)__pyx_v_z), PyBUF_WRITABLE); if (unlikely(!__pyx_t_1.memview)) __PYX_ERR(0, 3482, __pyx_L1_error)
+  __pyx_v_z_view = __pyx_t_1;
+  __pyx_t_1.memview = NULL;
+  __pyx_t_1.data = NULL;
+
+  /* "cssm.pyx":3484
+ *     cdef float[:, :] z_view = z
+ * 
+ *     cdef float[:] deadline_view = deadline             # <<<<<<<<<<<<<<
+ * 
+ *     cdef np.ndarray[float, ndim = 1] zs
+ */
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3484, __pyx_L1_error)
+  __pyx_v_deadline_view = __pyx_t_2;
+  __pyx_t_2.memview = NULL;
+  __pyx_t_2.data = NULL;
+
+  /* "cssm.pyx":3492
+ *     cdef np.ndarray[double, ndim = 1] vs_WM
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
+ *     cdef float[:, :, :] rts_view = rts
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 3492, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_5)) __PYX_ERR(0, 3492, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_int_1);
+  __Pyx_GIVEREF(__pyx_int_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_int_1)) __PYX_ERR(0, 3492, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3492, __pyx_L1_error);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3492, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_v_rts = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "cssm.pyx":3493
+ * 
+ *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+ *     cdef float[:, :, :] rts_view = rts             # <<<<<<<<<<<<<<
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+ */
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3493, __pyx_L1_error)
+  __pyx_v_rts_view = __pyx_t_7;
+  __pyx_t_7.memview = NULL;
+  __pyx_t_7.data = NULL;
+
+  /* "cssm.pyx":3495
+ *     cdef float[:, :, :] rts_view = rts
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)             # <<<<<<<<<<<<<<
+ *     cdef int[:, :, :] choices_view = choices
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_3);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3495, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_5)) __PYX_ERR(0, 3495, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_int_1);
+  __Pyx_GIVEREF(__pyx_int_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_int_1)) __PYX_ERR(0, 3495, __pyx_L1_error);
+  __pyx_t_3 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4)) __PYX_ERR(0, 3495, __pyx_L1_error);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_intc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_8) < 0) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3495, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_choices = __pyx_t_8;
+  __pyx_t_8 = 0;
+
+  /* "cssm.pyx":3496
+ * 
+ *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+ *     cdef int[:, :, :] choices_view = choices             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t n, k, i
+ */
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 3496, __pyx_L1_error)
+  __pyx_v_choices_view = __pyx_t_9;
+  __pyx_t_9.memview = NULL;
+  __pyx_t_9.data = NULL;
+
+  /* "cssm.pyx":3500
+ *     cdef Py_ssize_t n, k, i
+ * 
+ *     for k in range(n_trials):             # <<<<<<<<<<<<<<
+ * 
+ *         for n in range(n_samples):
+ */
+  __pyx_t_10 = __pyx_v_n_trials;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_k = __pyx_t_12;
+
+    /* "cssm.pyx":3502
+ *     for k in range(n_trials):
+ * 
+ *         for n in range(n_samples):             # <<<<<<<<<<<<<<
+ *             zs = np.random.uniform(0, z_view[k], nact).astype(DTYPE)
+ * 
+ */
+    __pyx_t_13 = __pyx_v_n_samples;
+    __pyx_t_14 = __pyx_t_13;
+    for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_14; __pyx_t_15+=1) {
+      __pyx_v_n = __pyx_t_15;
+
+      /* "cssm.pyx":3503
+ * 
+ *         for n in range(n_samples):
+ *             zs = np.random.uniform(0, z_view[k], nact).astype(DTYPE)             # <<<<<<<<<<<<<<
+ * 
+ *             vs_RL = np.abs(np.random.normal(v_RL_view[k], sd)) # np.abs() to avoid negative vs
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_random); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_uniform); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_2.data = __pyx_v_z_view.data;
+      __pyx_t_2.memview = __pyx_v_z_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_z_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_z_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_z_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_6 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_nact); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_16 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_16)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_16);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[4] = {__pyx_t_16, __pyx_int_0, __pyx_t_6, __pyx_t_3};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_17, 3+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3503, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_astype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_3 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3503, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 3503, __pyx_L1_error)
+      __pyx_t_18 = ((PyArrayObject *)__pyx_t_8);
+      {
+        __Pyx_BufFmt_StackElem __pyx_stack[1];
+        __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_zs.rcbuffer->pybuffer);
+        __pyx_t_17 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zs.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+        if (unlikely(__pyx_t_17 < 0)) {
+          PyErr_Fetch(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21);
+          if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zs.rcbuffer->pybuffer, (PyObject*)__pyx_v_zs, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+            Py_XDECREF(__pyx_t_19); Py_XDECREF(__pyx_t_20); Py_XDECREF(__pyx_t_21);
+            __Pyx_RaiseBufferFallbackError();
+          } else {
+            PyErr_Restore(__pyx_t_19, __pyx_t_20, __pyx_t_21);
+          }
+          __pyx_t_19 = __pyx_t_20 = __pyx_t_21 = 0;
+        }
+        __pyx_pybuffernd_zs.diminfo[0].strides = __pyx_pybuffernd_zs.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zs.diminfo[0].shape = __pyx_pybuffernd_zs.rcbuffer->pybuffer.shape[0];
+        if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3503, __pyx_L1_error)
+      }
+      __pyx_t_18 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_zs, ((PyArrayObject *)__pyx_t_8));
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3505
+ *             zs = np.random.uniform(0, z_view[k], nact).astype(DTYPE)
+ * 
+ *             vs_RL = np.abs(np.random.normal(v_RL_view[k], sd)) # np.abs() to avoid negative vs             # <<<<<<<<<<<<<<
+ *             vs_WM = np.abs(np.random.normal(v_WM_view[k], sd)) # np.abs() to avoid negative vs
+ * 
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_abs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_normal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+      __pyx_t_2.data = __pyx_v_v_RL_view.data;
+      __pyx_t_2.memview = __pyx_v_v_RL_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_v_RL_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_v_RL_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_v_RL_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_6 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_16 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_16);
+      __pyx_t_22 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_22)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_22);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[3] = {__pyx_t_22, __pyx_t_6, __pyx_t_16};
+        __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_17, 2+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3505, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
+      __pyx_t_3 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_5};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3505, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 3505, __pyx_L1_error)
+      __pyx_t_23 = ((PyArrayObject *)__pyx_t_8);
+      {
+        __Pyx_BufFmt_StackElem __pyx_stack[1];
+        __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vs_RL.rcbuffer->pybuffer);
+        __pyx_t_17 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vs_RL.rcbuffer->pybuffer, (PyObject*)__pyx_t_23, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+        if (unlikely(__pyx_t_17 < 0)) {
+          PyErr_Fetch(&__pyx_t_21, &__pyx_t_20, &__pyx_t_19);
+          if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vs_RL.rcbuffer->pybuffer, (PyObject*)__pyx_v_vs_RL, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+            Py_XDECREF(__pyx_t_21); Py_XDECREF(__pyx_t_20); Py_XDECREF(__pyx_t_19);
+            __Pyx_RaiseBufferFallbackError();
+          } else {
+            PyErr_Restore(__pyx_t_21, __pyx_t_20, __pyx_t_19);
+          }
+          __pyx_t_21 = __pyx_t_20 = __pyx_t_19 = 0;
+        }
+        __pyx_pybuffernd_vs_RL.diminfo[0].strides = __pyx_pybuffernd_vs_RL.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vs_RL.diminfo[0].shape = __pyx_pybuffernd_vs_RL.rcbuffer->pybuffer.shape[0];
+        if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3505, __pyx_L1_error)
+      }
+      __pyx_t_23 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_vs_RL, ((PyArrayObject *)__pyx_t_8));
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3506
+ * 
+ *             vs_RL = np.abs(np.random.normal(v_RL_view[k], sd)) # np.abs() to avoid negative vs
+ *             vs_WM = np.abs(np.random.normal(v_WM_view[k], sd)) # np.abs() to avoid negative vs             # <<<<<<<<<<<<<<
+ * 
+ *             x_t_RL = ([a_view[k]]*nact - zs)/vs_RL
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_abs); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_16 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_random); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_16);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_16, __pyx_n_s_normal); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+      __pyx_t_2.data = __pyx_v_v_WM_view.data;
+      __pyx_t_2.memview = __pyx_v_v_WM_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_v_WM_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_v_WM_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_v_WM_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_16 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_16);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_6 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __pyx_t_22 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_22 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_22)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_22);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[3] = {__pyx_t_22, __pyx_t_16, __pyx_t_6};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_17, 2+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_22); __pyx_t_22 = 0;
+        __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
+        __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3506, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
+      __pyx_t_3 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3506, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      }
+      if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 3506, __pyx_L1_error)
+      __pyx_t_24 = ((PyArrayObject *)__pyx_t_8);
+      {
+        __Pyx_BufFmt_StackElem __pyx_stack[1];
+        __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vs_WM.rcbuffer->pybuffer);
+        __pyx_t_17 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vs_WM.rcbuffer->pybuffer, (PyObject*)__pyx_t_24, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack);
+        if (unlikely(__pyx_t_17 < 0)) {
+          PyErr_Fetch(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21);
+          if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vs_WM.rcbuffer->pybuffer, (PyObject*)__pyx_v_vs_WM, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) {
+            Py_XDECREF(__pyx_t_19); Py_XDECREF(__pyx_t_20); Py_XDECREF(__pyx_t_21);
+            __Pyx_RaiseBufferFallbackError();
+          } else {
+            PyErr_Restore(__pyx_t_19, __pyx_t_20, __pyx_t_21);
+          }
+          __pyx_t_19 = __pyx_t_20 = __pyx_t_21 = 0;
+        }
+        __pyx_pybuffernd_vs_WM.diminfo[0].strides = __pyx_pybuffernd_vs_WM.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vs_WM.diminfo[0].shape = __pyx_pybuffernd_vs_WM.rcbuffer->pybuffer.shape[0];
+        if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3506, __pyx_L1_error)
+      }
+      __pyx_t_24 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_vs_WM, ((PyArrayObject *)__pyx_t_8));
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3508
+ *             vs_WM = np.abs(np.random.normal(v_WM_view[k], sd)) # np.abs() to avoid negative vs
+ * 
+ *             x_t_RL = ([a_view[k]]*nact - zs)/vs_RL             # <<<<<<<<<<<<<<
+ *             x_t_WM = ([a_view[k]]*nact - zs)/vs_WM
+ * 
+ */
+      __pyx_t_2.data = __pyx_v_a_view.data;
+      __pyx_t_2.memview = __pyx_v_a_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_a_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_a_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_a_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_8 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3508, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_5 = PyList_New(1 * ((__pyx_v_nact<0) ? 0:__pyx_v_nact)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3508, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      { Py_ssize_t __pyx_temp;
+        for (__pyx_temp=0; __pyx_temp < __pyx_v_nact; __pyx_temp++) {
+          __Pyx_INCREF(__pyx_t_8);
+          __Pyx_GIVEREF(__pyx_t_8);
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_5, __pyx_temp, __pyx_t_8)) __PYX_ERR(0, 3508, __pyx_L1_error);
+        }
+      }
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = PyNumber_Subtract(__pyx_t_5, ((PyObject *)__pyx_v_zs)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3508, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = __Pyx_PyNumber_Divide(__pyx_t_8, ((PyObject *)__pyx_v_vs_RL)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3508, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 3508, __pyx_L1_error)
+      __pyx_t_25 = ((PyArrayObject *)__pyx_t_5);
+      {
+        __Pyx_BufFmt_StackElem __pyx_stack[1];
+        __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer);
+        __pyx_t_17 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer, (PyObject*)__pyx_t_25, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
+        if (unlikely(__pyx_t_17 < 0)) {
+          PyErr_Fetch(&__pyx_t_21, &__pyx_t_20, &__pyx_t_19);
+          if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer, (PyObject*)__pyx_v_x_t_RL, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+            Py_XDECREF(__pyx_t_21); Py_XDECREF(__pyx_t_20); Py_XDECREF(__pyx_t_19);
+            __Pyx_RaiseBufferFallbackError();
+          } else {
+            PyErr_Restore(__pyx_t_21, __pyx_t_20, __pyx_t_19);
+          }
+          __pyx_t_21 = __pyx_t_20 = __pyx_t_19 = 0;
+        }
+        __pyx_pybuffernd_x_t_RL.diminfo[0].strides = __pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_t_RL.diminfo[0].shape = __pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_x_t_RL.diminfo[1].strides = __pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_x_t_RL.diminfo[1].shape = __pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer.shape[1];
+        if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3508, __pyx_L1_error)
+      }
+      __pyx_t_25 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_x_t_RL, ((PyArrayObject *)__pyx_t_5));
+      __pyx_t_5 = 0;
+
+      /* "cssm.pyx":3509
+ * 
+ *             x_t_RL = ([a_view[k]]*nact - zs)/vs_RL
+ *             x_t_WM = ([a_view[k]]*nact - zs)/vs_WM             # <<<<<<<<<<<<<<
+ * 
+ *             if np.min(x_t_RL) <= np.min(x_t_WM):
+ */
+      __pyx_t_2.data = __pyx_v_a_view.data;
+      __pyx_t_2.memview = __pyx_v_a_view.memview;
+      __PYX_INC_MEMVIEW(&__pyx_t_2, 1);
+      {
+    Py_ssize_t __pyx_tmp_idx = __pyx_v_k;
+    Py_ssize_t __pyx_tmp_stride = __pyx_v_a_view.strides[0];
+        __pyx_t_2.data += __pyx_tmp_idx * __pyx_tmp_stride;
+}
+
+__pyx_t_2.shape[0] = __pyx_v_a_view.shape[1];
+__pyx_t_2.strides[0] = __pyx_v_a_view.strides[1];
+    __pyx_t_2.suboffsets[0] = -1;
+
+__pyx_t_5 = __pyx_memoryview_fromslice(__pyx_t_2, 1, (PyObject *(*)(char *)) __pyx_memview_get_float, (int (*)(char *, PyObject *)) __pyx_memview_set_float, 0);; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3509, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+      __pyx_t_2.memview = NULL; __pyx_t_2.data = NULL;
+      __pyx_t_8 = PyList_New(1 * ((__pyx_v_nact<0) ? 0:__pyx_v_nact)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3509, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      { Py_ssize_t __pyx_temp;
+        for (__pyx_temp=0; __pyx_temp < __pyx_v_nact; __pyx_temp++) {
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_GIVEREF(__pyx_t_5);
+          if (__Pyx_PyList_SET_ITEM(__pyx_t_8, __pyx_temp, __pyx_t_5)) __PYX_ERR(0, 3509, __pyx_L1_error);
+        }
+      }
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = PyNumber_Subtract(__pyx_t_8, ((PyObject *)__pyx_v_zs)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3509, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __pyx_t_8 = __Pyx_PyNumber_Divide(__pyx_t_5, ((PyObject *)__pyx_v_vs_WM)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3509, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (!(likely(((__pyx_t_8) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_8, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 3509, __pyx_L1_error)
+      __pyx_t_26 = ((PyArrayObject *)__pyx_t_8);
+      {
+        __Pyx_BufFmt_StackElem __pyx_stack[1];
+        __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer);
+        __pyx_t_17 = __Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer, (PyObject*)__pyx_t_26, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack);
+        if (unlikely(__pyx_t_17 < 0)) {
+          PyErr_Fetch(&__pyx_t_19, &__pyx_t_20, &__pyx_t_21);
+          if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer, (PyObject*)__pyx_v_x_t_WM, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) {
+            Py_XDECREF(__pyx_t_19); Py_XDECREF(__pyx_t_20); Py_XDECREF(__pyx_t_21);
+            __Pyx_RaiseBufferFallbackError();
+          } else {
+            PyErr_Restore(__pyx_t_19, __pyx_t_20, __pyx_t_21);
+          }
+          __pyx_t_19 = __pyx_t_20 = __pyx_t_21 = 0;
+        }
+        __pyx_pybuffernd_x_t_WM.diminfo[0].strides = __pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_t_WM.diminfo[0].shape = __pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_x_t_WM.diminfo[1].strides = __pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_x_t_WM.diminfo[1].shape = __pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer.shape[1];
+        if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3509, __pyx_L1_error)
+      }
+      __pyx_t_26 = 0;
+      __Pyx_XDECREF_SET(__pyx_v_x_t_WM, ((PyArrayObject *)__pyx_t_8));
+      __pyx_t_8 = 0;
+
+      /* "cssm.pyx":3511
+ *             x_t_WM = ([a_view[k]]*nact - zs)/vs_WM
+ * 
+ *             if np.min(x_t_RL) <= np.min(x_t_WM):             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = np.min(x_t_RL) + ndt  # store reaction time for sample n
+ *                 choices_view[n, k, 0] = np.argmin(x_t_RL) # store choices for sample n
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3511, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_min); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3511, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_4))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_4, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, ((PyObject *)__pyx_v_x_t_RL)};
+        __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3511, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      }
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3511, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_min); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3511, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      __pyx_t_17 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+          __pyx_t_17 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_5, ((PyObject *)__pyx_v_x_t_WM)};
+        __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+        __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3511, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      }
+      __pyx_t_3 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_LE); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3511, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_27 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_27 < 0))) __PYX_ERR(0, 3511, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (__pyx_t_27) {
+
+        /* "cssm.pyx":3512
+ * 
+ *             if np.min(x_t_RL) <= np.min(x_t_WM):
+ *                 rts_view[n, k, 0] = np.min(x_t_RL) + ndt  # store reaction time for sample n             # <<<<<<<<<<<<<<
+ *                 choices_view[n, k, 0] = np.argmin(x_t_RL) # store choices for sample n
+ *             else:
+ */
+        __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3512, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_min); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3512, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_4 = NULL;
+        __pyx_t_17 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_8))) {
+          __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_8);
+          if (likely(__pyx_t_4)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+            __Pyx_INCREF(__pyx_t_4);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_8, function);
+            __pyx_t_17 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_4, ((PyObject *)__pyx_v_x_t_RL)};
+          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+          __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3512, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        }
+        __pyx_t_8 = PyFloat_FromDouble(__pyx_v_ndt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3512, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_4 = PyNumber_Add(__pyx_t_3, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3512, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_28 = __pyx_PyFloat_AsFloat(__pyx_t_4); if (unlikely((__pyx_t_28 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3512, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_29 = __pyx_v_n;
+        __pyx_t_30 = __pyx_v_k;
+        __pyx_t_31 = 0;
+        *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_29 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_30 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_31 * __pyx_v_rts_view.strides[2]) )) = __pyx_t_28;
+
+        /* "cssm.pyx":3513
+ *             if np.min(x_t_RL) <= np.min(x_t_WM):
+ *                 rts_view[n, k, 0] = np.min(x_t_RL) + ndt  # store reaction time for sample n
+ *                 choices_view[n, k, 0] = np.argmin(x_t_RL) # store choices for sample n             # <<<<<<<<<<<<<<
+ *             else:
+ *                 rts_view[n, k, 0] = np.min(x_t_WM) + ndt  # store reaction time for sample n
+ */
+        __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3513, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_argmin); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3513, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = NULL;
+        __pyx_t_17 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_3))) {
+          __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
+          if (likely(__pyx_t_8)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+            __Pyx_INCREF(__pyx_t_8);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_3, function);
+            __pyx_t_17 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_8, ((PyObject *)__pyx_v_x_t_RL)};
+          __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3513, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        }
+        __pyx_t_17 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_17 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3513, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __pyx_t_31 = __pyx_v_n;
+        __pyx_t_30 = __pyx_v_k;
+        __pyx_t_29 = 0;
+        *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_31 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_30 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_29 * __pyx_v_choices_view.strides[2]) )) = __pyx_t_17;
+
+        /* "cssm.pyx":3511
+ *             x_t_WM = ([a_view[k]]*nact - zs)/vs_WM
+ * 
+ *             if np.min(x_t_RL) <= np.min(x_t_WM):             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = np.min(x_t_RL) + ndt  # store reaction time for sample n
+ *                 choices_view[n, k, 0] = np.argmin(x_t_RL) # store choices for sample n
+ */
+        goto __pyx_L7;
+      }
+
+      /* "cssm.pyx":3515
+ *                 choices_view[n, k, 0] = np.argmin(x_t_RL) # store choices for sample n
+ *             else:
+ *                 rts_view[n, k, 0] = np.min(x_t_WM) + ndt  # store reaction time for sample n             # <<<<<<<<<<<<<<
+ *                 choices_view[n, k, 0] = np.argmin(x_t_WM) # store choices for sample n
+ * 
+ */
+      /*else*/ {
+        __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3515, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_min); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3515, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_3 = NULL;
+        __pyx_t_17 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_8))) {
+          __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_8);
+          if (likely(__pyx_t_3)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+            __Pyx_INCREF(__pyx_t_3);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_8, function);
+            __pyx_t_17 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_3, ((PyObject *)__pyx_v_x_t_WM)};
+          __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+          __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3515, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_4);
+          __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        }
+        __pyx_t_8 = PyFloat_FromDouble(__pyx_v_ndt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3515, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_3 = PyNumber_Add(__pyx_t_4, __pyx_t_8); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3515, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_28 = __pyx_PyFloat_AsFloat(__pyx_t_3); if (unlikely((__pyx_t_28 == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3515, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_29 = __pyx_v_n;
+        __pyx_t_30 = __pyx_v_k;
+        __pyx_t_31 = 0;
+        *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_29 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_30 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_31 * __pyx_v_rts_view.strides[2]) )) = __pyx_t_28;
+
+        /* "cssm.pyx":3516
+ *             else:
+ *                 rts_view[n, k, 0] = np.min(x_t_WM) + ndt  # store reaction time for sample n
+ *                 choices_view[n, k, 0] = np.argmin(x_t_WM) # store choices for sample n             # <<<<<<<<<<<<<<
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ */
+        __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_np); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_argmin); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3516, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+        __pyx_t_8 = NULL;
+        __pyx_t_17 = 0;
+        #if CYTHON_UNPACK_METHODS
+        if (unlikely(PyMethod_Check(__pyx_t_4))) {
+          __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_4);
+          if (likely(__pyx_t_8)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+            __Pyx_INCREF(__pyx_t_8);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_4, function);
+            __pyx_t_17 = 1;
+          }
+        }
+        #endif
+        {
+          PyObject *__pyx_callargs[2] = {__pyx_t_8, ((PyObject *)__pyx_v_x_t_WM)};
+          __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_17, 1+__pyx_t_17);
+          __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+          if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3516, __pyx_L1_error)
+          __Pyx_GOTREF(__pyx_t_3);
+          __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+        }
+        __pyx_t_17 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_17 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3516, __pyx_L1_error)
+        __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+        __pyx_t_31 = __pyx_v_n;
+        __pyx_t_30 = __pyx_v_k;
+        __pyx_t_29 = 0;
+        *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_31 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_30 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_29 * __pyx_v_choices_view.strides[2]) )) = __pyx_t_17;
+      }
+      __pyx_L7:;
+
+      /* "cssm.pyx":3519
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = -999
+ * 
+ */
+      __pyx_t_29 = __pyx_v_n;
+      __pyx_t_30 = __pyx_v_k;
+      __pyx_t_31 = 0;
+      __pyx_t_32 = __pyx_v_k;
+      __pyx_t_27 = ((*((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_29 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_30 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_31 * __pyx_v_rts_view.strides[2]) ))) >= (*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_32 * __pyx_v_deadline_view.strides[0]) ))));
+      if (__pyx_t_27) {
+
+        /* "cssm.pyx":3520
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:
+ *                 rts_view[n, k, 0] = -999             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+        __pyx_t_32 = __pyx_v_n;
+        __pyx_t_31 = __pyx_v_k;
+        __pyx_t_30 = 0;
+        *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_32 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_31 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_30 * __pyx_v_rts_view.strides[2]) )) = -999.0;
+
+        /* "cssm.pyx":3519
+ * 
+ *             # If the rt exceeds the deadline, set rt to -999
+ *             if rts_view[n, k, 0] >= deadline_view[k]:             # <<<<<<<<<<<<<<
+ *                 rts_view[n, k, 0] = -999
+ * 
+ */
+      }
+    }
+  }
+
+  /* "cssm.pyx":3523
+ * 
+ * 
+ *     v_dict = {}             # <<<<<<<<<<<<<<
+ *     for i in range(nact):
+ *         v_dict['v_RL_' + str(i)] = v_RL[:, i]
+ */
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3523, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_v_v_dict = ((PyObject*)__pyx_t_3);
+  __pyx_t_3 = 0;
+
+  /* "cssm.pyx":3524
+ * 
+ *     v_dict = {}
+ *     for i in range(nact):             # <<<<<<<<<<<<<<
+ *         v_dict['v_RL_' + str(i)] = v_RL[:, i]
+ *         v_dict['v_WM_' + str(i)] = v_WM[:, i]
+ */
+  __pyx_t_10 = __pyx_v_nact;
+  __pyx_t_11 = __pyx_t_10;
+  for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+    __pyx_v_i = __pyx_t_12;
+
+    /* "cssm.pyx":3525
+ *     v_dict = {}
+ *     for i in range(nact):
+ *         v_dict['v_RL_' + str(i)] = v_RL[:, i]             # <<<<<<<<<<<<<<
+ *         v_dict['v_WM_' + str(i)] = v_WM[:, i]
+ * 
+ */
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_slice__5);
+    __Pyx_GIVEREF(__pyx_slice__5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__5)) __PYX_ERR(0, 3525, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3)) __PYX_ERR(0, 3525, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_v_RL), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_8 = __Pyx_PyObject_Str(__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyNumber_Add(__pyx_n_u_v_RL_2, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely((PyDict_SetItem(__pyx_v_v_dict, __pyx_t_4, __pyx_t_3) < 0))) __PYX_ERR(0, 3525, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+
+    /* "cssm.pyx":3526
+ *     for i in range(nact):
+ *         v_dict['v_RL_' + str(i)] = v_RL[:, i]
+ *         v_dict['v_WM_' + str(i)] = v_WM[:, i]             # <<<<<<<<<<<<<<
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ */
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_slice__5);
+    __Pyx_GIVEREF(__pyx_slice__5);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_slice__5)) __PYX_ERR(0, 3526, __pyx_L1_error);
+    __Pyx_GIVEREF(__pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3)) __PYX_ERR(0, 3526, __pyx_L1_error);
+    __pyx_t_3 = 0;
+    __pyx_t_3 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_v_WM), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_8 = __Pyx_PyObject_Str(__pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = PyNumber_Add(__pyx_n_u_v_WM_2, __pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely((PyDict_SetItem(__pyx_v_v_dict, __pyx_t_4, __pyx_t_3) < 0))) __PYX_ERR(0, 3526, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  }
+
+  /* "cssm.pyx":3528
+ *         v_dict['v_WM_' + str(i)] = v_WM[:, i]
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,             # <<<<<<<<<<<<<<
+ *                                                          'a': a,
+ *                                                          'z': z,
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3528, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3528, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3528, __pyx_L1_error)
+  __pyx_t_4 = PyDict_Copy(__pyx_v_v_dict); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3528, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+
+  /* "cssm.pyx":3529
+ * 
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ *                                                          'a': a,             # <<<<<<<<<<<<<<
+ *                                                          'z': z,
+ *                                                          'deadline': deadline,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 3529, __pyx_L1_error)
+
+  /* "cssm.pyx":3530
+ *     return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+ *                                                          'a': a,
+ *                                                          'z': z,             # <<<<<<<<<<<<<<
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_z, ((PyObject *)__pyx_v_z)) < 0) __PYX_ERR(0, 3530, __pyx_L1_error)
+
+  /* "cssm.pyx":3531
+ *                                                          'a': a,
+ *                                                          'z': z,
+ *                                                          'deadline': deadline,             # <<<<<<<<<<<<<<
+ *                                                          'sd': sd,
+ *                                                          'n_samples': n_samples,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 3531, __pyx_L1_error)
+
+  /* "cssm.pyx":3532
+ *                                                          'z': z,
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,             # <<<<<<<<<<<<<<
+ *                                                          'n_samples': n_samples,
+ *                                                          'simulator' : 'rlwm_lba_race',
+ */
+  __pyx_t_8 = PyFloat_FromDouble(__pyx_v_sd); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3532, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_sd, __pyx_t_8) < 0) __PYX_ERR(0, 3532, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+
+  /* "cssm.pyx":3533
+ *                                                          'deadline': deadline,
+ *                                                          'sd': sd,
+ *                                                          'n_samples': n_samples,             # <<<<<<<<<<<<<<
+ *                                                          'simulator' : 'rlwm_lba_race',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),
+ */
+  __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3533, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_8);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_n_samples, __pyx_t_8) < 0) __PYX_ERR(0, 3533, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_simulator, __pyx_n_u_rlwm_lba_race) < 0) __PYX_ERR(0, 3534, __pyx_L1_error)
+
+  /* "cssm.pyx":3535
+ *                                                          'n_samples': n_samples,
+ *                                                          'simulator' : 'rlwm_lba_race',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),             # <<<<<<<<<<<<<<
+ *                                                          'max_t': max_t,
+ *                                                          }}
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3535, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_arange); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3535, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_nact); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3535, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __pyx_t_16 = NULL;
+  __pyx_t_10 = 0;
+  #if CYTHON_UNPACK_METHODS
+  if (unlikely(PyMethod_Check(__pyx_t_6))) {
+    __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_6);
+    if (likely(__pyx_t_16)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_16);
+      __Pyx_INCREF(function);
+      __Pyx_DECREF_SET(__pyx_t_6, function);
+      __pyx_t_10 = 1;
+    }
+  }
+  #endif
+  {
+    PyObject *__pyx_callargs[4] = {__pyx_t_16, __pyx_int_0, __pyx_t_5, __pyx_int_1};
+    __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_10, 3+__pyx_t_10);
+    __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 3535, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  }
+  __pyx_t_6 = __Pyx_PySequence_ListKeepNew(__pyx_t_8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3535, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_possible_choices, __pyx_t_6) < 0) __PYX_ERR(0, 3535, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+
+  /* "cssm.pyx":3536
+ *                                                          'simulator' : 'rlwm_lba_race',
+ *                                                          'possible_choices': list(np.arange(0, nact, 1)),
+ *                                                          'max_t': max_t,             # <<<<<<<<<<<<<<
+ *                                                          }}
+ * # ----------------------------------------------------------------------------------------------------
+ */
+  __pyx_t_6 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3536, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_max_t, __pyx_t_6) < 0) __PYX_ERR(0, 3536, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_metadata, __pyx_t_4) < 0) __PYX_ERR(0, 3528, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "cssm.pyx":3460
+ * 
+ * # Simulate (rt, choice) tuples from: RLWM LBA Race Model without ndt -----------------------------
+ * def rlwm_lba_race(np.ndarray[float, ndim = 2] v_RL, # RL drift parameters (np.array expect: one column of floats)             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] v_WM, # WM drift parameters (np.array expect: one column of floats)
+ *         np.ndarray[float, ndim = 2] a, # criterion height
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_1, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_2, 1);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_7, 1);
+  __Pyx_XDECREF(__pyx_t_8);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_XDECREF(__pyx_t_16);
+  __Pyx_XDECREF(__pyx_t_22);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v_RL.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v_WM.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vs_RL.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vs_WM.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_zs.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("cssm.rlwm_lba_race", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_a.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v_RL.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_v_WM.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vs_RL.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_vs_WM.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_t_RL.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_t_WM.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_zs.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_v_RL_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_v_WM_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_a_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_z_view, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_deadline_view, 1);
+  __Pyx_XDECREF((PyObject *)__pyx_v_zs);
+  __Pyx_XDECREF((PyObject *)__pyx_v_x_t_RL);
+  __Pyx_XDECREF((PyObject *)__pyx_v_x_t_WM);
+  __Pyx_XDECREF((PyObject *)__pyx_v_vs_RL);
+  __Pyx_XDECREF((PyObject *)__pyx_v_vs_WM);
+  __Pyx_XDECREF(__pyx_v_rts);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_rts_view, 1);
+  __Pyx_XDECREF(__pyx_v_choices);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_choices_view, 1);
+  __Pyx_XDECREF(__pyx_v_v_dict);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "cssm.pyx":3543
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                                         np.ndarray[float, ndim = 1] vl1,
  *                                                         np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_64__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_70__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
 
-  /* "cssm.pyx":3339
+  /* "cssm.pyx":3554
  *                                                         np.ndarray[float, ndim = 1] t,
  *                                                         np.ndarray[float, ndim = 1] deadline,
  *                                                         float s = 1.0,             # <<<<<<<<<<<<<<
  *                                                         float delta_t = 0.001,
  *                                                         float max_t = 20,
  */
-  __pyx_t_1 = PyFloat_FromDouble(((double)1.0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3339, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(((double)1.0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "cssm.pyx":3340
+  /* "cssm.pyx":3555
  *                                                         np.ndarray[float, ndim = 1] deadline,
  *                                                         float s = 1.0,
  *                                                         float delta_t = 0.001,             # <<<<<<<<<<<<<<
  *                                                         float max_t = 20,
  *                                                         int n_samples = 20000,
  */
-  __pyx_t_2 = PyFloat_FromDouble(((double)0.001)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3340, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)0.001)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3555, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "cssm.pyx":3341
+  /* "cssm.pyx":3556
  *                                                         float s = 1.0,
  *                                                         float delta_t = 0.001,
  *                                                         float max_t = 20,             # <<<<<<<<<<<<<<
  *                                                         int n_samples = 20000,
  *                                                         int n_trials = 1,
  */
-  __pyx_t_3 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3341, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3556, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "cssm.pyx":3342
+  /* "cssm.pyx":3557
  *                                                         float delta_t = 0.001,
  *                                                         float max_t = 20,
  *                                                         int n_samples = 20000,             # <<<<<<<<<<<<<<
  *                                                         int n_trials = 1,
  *                                                         print_info = True,
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(((int)0x4E20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3342, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(((int)0x4E20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3557, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "cssm.pyx":3343
+  /* "cssm.pyx":3558
  *                                                         float max_t = 20,
  *                                                         int n_samples = 20000,
  *                                                         int n_trials = 1,             # <<<<<<<<<<<<<<
  *                                                         print_info = True,
  *                                                         boundary_fun = None, # function of t (and potentially other parameters) that takes in (t, *args)
  */
-  __pyx_t_5 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3343, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3558, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "cssm.pyx":3328
+  /* "cssm.pyx":3543
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                                         np.ndarray[float, ndim = 1] vl1,
  *                                                         np.ndarray[float, ndim = 1] vl2,
  */
-  __pyx_t_6 = PyTuple_New(12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3328, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_3)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_3)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_4)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_4)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_t_5)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_t_5)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_True));
   __Pyx_GIVEREF(((PyObject *)Py_True));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, ((PyObject *)Py_True))) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, ((PyObject *)Py_True))) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 6, Py_None)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 6, Py_None)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_True));
   __Pyx_GIVEREF(((PyObject *)Py_True));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 7, ((PyObject *)Py_True))) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 7, ((PyObject *)Py_True))) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_self)->__pyx_arg_boundary_params);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_self)->__pyx_arg_boundary_params);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 8, __Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_self)->__pyx_arg_boundary_params)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 8, __Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_self)->__pyx_arg_boundary_params)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 9, Py_None)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 9, Py_None)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_n_u_full));
   __Pyx_GIVEREF(((PyObject*)__pyx_n_u_full));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 10, ((PyObject*)__pyx_n_u_full))) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 10, ((PyObject*)__pyx_n_u_full))) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_False));
   __Pyx_GIVEREF(((PyObject *)Py_False));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 11, ((PyObject *)Py_False))) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 11, ((PyObject *)Py_False))) __PYX_ERR(0, 3543, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3328, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3543, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, Py_None)) __PYX_ERR(0, 3328, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, Py_None)) __PYX_ERR(0, 3543, __pyx_L1_error);
   __pyx_t_6 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -63618,23 +67792,23 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4cssm_35ddm_flexbound_mic2_unnormalized_ornstein_multinoise(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4cssm_41ddm_flexbound_mic2_unnormalized_ornstein_multinoise(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_4cssm_35ddm_flexbound_mic2_unnormalized_ornstein_multinoise = {"ddm_flexbound_mic2_unnormalized_ornstein_multinoise", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_35ddm_flexbound_mic2_unnormalized_ornstein_multinoise, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4cssm_35ddm_flexbound_mic2_unnormalized_ornstein_multinoise(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4cssm_41ddm_flexbound_mic2_unnormalized_ornstein_multinoise = {"ddm_flexbound_mic2_unnormalized_ornstein_multinoise", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_41ddm_flexbound_mic2_unnormalized_ornstein_multinoise, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cssm_41ddm_flexbound_mic2_unnormalized_ornstein_multinoise(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyArrayObject *__pyx_v_vh = 0;
@@ -63683,26 +67857,26 @@
   __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
   __Pyx_GOTREF(__pyx_v_kwargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vh,&__pyx_n_s_vl1,&__pyx_n_s_vl2,&__pyx_n_s_a,&__pyx_n_s_zh,&__pyx_n_s_zl1,&__pyx_n_s_zl2,&__pyx_n_s_d,&__pyx_n_s_g,&__pyx_n_s_t,&__pyx_n_s_deadline,&__pyx_n_s_s,&__pyx_n_s_delta_t,&__pyx_n_s_max_t,&__pyx_n_s_n_samples,&__pyx_n_s_n_trials,&__pyx_n_s_print_info,&__pyx_n_s_boundary_fun,&__pyx_n_s_boundary_multiplicative,&__pyx_n_s_boundary_params,&__pyx_n_s_random_state,&__pyx_n_s_return_option,&__pyx_n_s_smooth,0};
     __pyx_defaults13 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_self);
     values[16] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
 
-    /* "cssm.pyx":3345
+    /* "cssm.pyx":3560
  *                                                         int n_trials = 1,
  *                                                         print_info = True,
  *                                                         boundary_fun = None, # function of t (and potentially other parameters) that takes in (t, *args)             # <<<<<<<<<<<<<<
  *                                                         boundary_multiplicative = True,
  *                                                         boundary_params = {},
  */
     values[17] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     values[18] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
     values[19] = __Pyx_Arg_NewRef_FASTCALL(__pyx_dynamic_args->__pyx_arg_boundary_params);
 
-    /* "cssm.pyx":3348
+    /* "cssm.pyx":3563
  *                                                         boundary_multiplicative = True,
  *                                                         boundary_params = {},
  *                                                         random_state = None,             # <<<<<<<<<<<<<<
  *                                                         return_option = 'full',
  *                                                         smooth = False,
  */
     values[20] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
@@ -63763,204 +67937,204 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vl1)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 1); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 1); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vl2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 2); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 2); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_a)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 3); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 3); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_zh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 4); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 4); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_zl1)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 5); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 5); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_zl2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[6]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 6); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 6); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_d)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[7]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 7); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 7); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_g)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[8]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 8); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 8); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_t)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[9]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 9); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 9); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (likely((values[10] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_deadline)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[10]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 10); __PYX_ERR(0, 3328, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, 10); __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s);
           if (value) { values[11] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 12:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_delta_t);
           if (value) { values[12] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 13:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_t);
           if (value) { values[13] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 14:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_samples);
           if (value) { values[14] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 15:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_trials);
           if (value) { values[15] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 16:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_print_info);
           if (value) { values[16] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 17:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boundary_fun);
           if (value) { values[17] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 18:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boundary_multiplicative);
           if (value) { values[18] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 19:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boundary_params);
           if (value) { values[19] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 20:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_random_state);
           if (value) { values[20] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 21:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_return_option);
           if (value) { values[21] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 22:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_smooth);
           if (value) { values[22] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3328, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3543, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "ddm_flexbound_mic2_unnormalized_ornstein_multinoise") < 0)) __PYX_ERR(0, 3328, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "ddm_flexbound_mic2_unnormalized_ornstein_multinoise") < 0)) __PYX_ERR(0, 3543, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case 23: values[22] = __Pyx_Arg_FASTCALL(__pyx_args, 22);
         CYTHON_FALLTHROUGH;
         case 22: values[21] = __Pyx_Arg_FASTCALL(__pyx_args, 21);
         CYTHON_FALLTHROUGH;
@@ -64007,77 +68181,77 @@
     __pyx_v_zl1 = ((PyArrayObject *)values[5]);
     __pyx_v_zl2 = ((PyArrayObject *)values[6]);
     __pyx_v_d = ((PyArrayObject *)values[7]);
     __pyx_v_g = ((PyArrayObject *)values[8]);
     __pyx_v_t = ((PyArrayObject *)values[9]);
     __pyx_v_deadline = ((PyArrayObject *)values[10]);
     if (values[11]) {
-      __pyx_v_s = __pyx_PyFloat_AsFloat(values[11]); if (unlikely((__pyx_v_s == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3339, __pyx_L3_error)
+      __pyx_v_s = __pyx_PyFloat_AsFloat(values[11]); if (unlikely((__pyx_v_s == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3554, __pyx_L3_error)
     } else {
       __pyx_v_s = ((float)((double)1.0));
     }
     if (values[12]) {
-      __pyx_v_delta_t = __pyx_PyFloat_AsFloat(values[12]); if (unlikely((__pyx_v_delta_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3340, __pyx_L3_error)
+      __pyx_v_delta_t = __pyx_PyFloat_AsFloat(values[12]); if (unlikely((__pyx_v_delta_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3555, __pyx_L3_error)
     } else {
       __pyx_v_delta_t = ((float)((double)0.001));
     }
     if (values[13]) {
-      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[13]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3341, __pyx_L3_error)
+      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[13]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3556, __pyx_L3_error)
     } else {
       __pyx_v_max_t = ((float)((float)20.0));
     }
     if (values[14]) {
-      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[14]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3342, __pyx_L3_error)
+      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[14]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3557, __pyx_L3_error)
     } else {
       __pyx_v_n_samples = ((int)((int)0x4E20));
     }
     if (values[15]) {
-      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[15]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3343, __pyx_L3_error)
+      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[15]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3558, __pyx_L3_error)
     } else {
       __pyx_v_n_trials = ((int)((int)1));
     }
     __pyx_v_print_info = values[16];
     __pyx_v_boundary_fun = values[17];
     __pyx_v_boundary_multiplicative = values[18];
     __pyx_v_boundary_params = values[19];
     __pyx_v_random_state = values[20];
     __pyx_v_return_option = values[21];
     __pyx_v_smooth = values[22];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, __pyx_nargs); __PYX_ERR(0, 3328, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("ddm_flexbound_mic2_unnormalized_ornstein_multinoise", 0, 11, 23, __pyx_nargs); __PYX_ERR(0, 3543, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cssm.ddm_flexbound_mic2_unnormalized_ornstein_multinoise", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vh), __pyx_ptype_5numpy_ndarray, 1, "vh", 0))) __PYX_ERR(0, 3328, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl1), __pyx_ptype_5numpy_ndarray, 1, "vl1", 0))) __PYX_ERR(0, 3329, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl2), __pyx_ptype_5numpy_ndarray, 1, "vl2", 0))) __PYX_ERR(0, 3330, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 3331, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zh), __pyx_ptype_5numpy_ndarray, 1, "zh", 0))) __PYX_ERR(0, 3332, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl1), __pyx_ptype_5numpy_ndarray, 1, "zl1", 0))) __PYX_ERR(0, 3333, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl2), __pyx_ptype_5numpy_ndarray, 1, "zl2", 0))) __PYX_ERR(0, 3334, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_d), __pyx_ptype_5numpy_ndarray, 1, "d", 0))) __PYX_ERR(0, 3335, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_5numpy_ndarray, 1, "g", 0))) __PYX_ERR(0, 3336, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_t), __pyx_ptype_5numpy_ndarray, 1, "t", 0))) __PYX_ERR(0, 3337, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 3338, __pyx_L1_error)
-  __pyx_r = __pyx_pf_4cssm_34ddm_flexbound_mic2_unnormalized_ornstein_multinoise(__pyx_self, __pyx_v_vh, __pyx_v_vl1, __pyx_v_vl2, __pyx_v_a, __pyx_v_zh, __pyx_v_zl1, __pyx_v_zl2, __pyx_v_d, __pyx_v_g, __pyx_v_t, __pyx_v_deadline, __pyx_v_s, __pyx_v_delta_t, __pyx_v_max_t, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_print_info, __pyx_v_boundary_fun, __pyx_v_boundary_multiplicative, __pyx_v_boundary_params, __pyx_v_random_state, __pyx_v_return_option, __pyx_v_smooth, __pyx_v_kwargs);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vh), __pyx_ptype_5numpy_ndarray, 1, "vh", 0))) __PYX_ERR(0, 3543, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl1), __pyx_ptype_5numpy_ndarray, 1, "vl1", 0))) __PYX_ERR(0, 3544, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl2), __pyx_ptype_5numpy_ndarray, 1, "vl2", 0))) __PYX_ERR(0, 3545, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 3546, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zh), __pyx_ptype_5numpy_ndarray, 1, "zh", 0))) __PYX_ERR(0, 3547, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl1), __pyx_ptype_5numpy_ndarray, 1, "zl1", 0))) __PYX_ERR(0, 3548, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl2), __pyx_ptype_5numpy_ndarray, 1, "zl2", 0))) __PYX_ERR(0, 3549, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_d), __pyx_ptype_5numpy_ndarray, 1, "d", 0))) __PYX_ERR(0, 3550, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_g), __pyx_ptype_5numpy_ndarray, 1, "g", 0))) __PYX_ERR(0, 3551, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_t), __pyx_ptype_5numpy_ndarray, 1, "t", 0))) __PYX_ERR(0, 3552, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 3553, __pyx_L1_error)
+  __pyx_r = __pyx_pf_4cssm_40ddm_flexbound_mic2_unnormalized_ornstein_multinoise(__pyx_self, __pyx_v_vh, __pyx_v_vl1, __pyx_v_vl2, __pyx_v_a, __pyx_v_zh, __pyx_v_zl1, __pyx_v_zl2, __pyx_v_d, __pyx_v_g, __pyx_v_t, __pyx_v_deadline, __pyx_v_s, __pyx_v_delta_t, __pyx_v_max_t, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_print_info, __pyx_v_boundary_fun, __pyx_v_boundary_multiplicative, __pyx_v_boundary_params, __pyx_v_random_state, __pyx_v_return_option, __pyx_v_smooth, __pyx_v_kwargs);
 
-  /* "cssm.pyx":3328
+  /* "cssm.pyx":3543
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                                         np.ndarray[float, ndim = 1] vl1,
  *                                                         np.ndarray[float, ndim = 1] vl2,
  */
 
@@ -64093,15 +68267,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4cssm_34ddm_flexbound_mic2_unnormalized_ornstein_multinoise(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
+static PyObject *__pyx_pf_4cssm_40ddm_flexbound_mic2_unnormalized_ornstein_multinoise(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_g, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
   __Pyx_memviewslice __pyx_v_vh_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_vl1_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_vl2_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_a_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_zh_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_zl1_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_zl2_view = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -64248,553 +68422,553 @@
   __pyx_pybuffernd_t.rcbuffer = &__pyx_pybuffer_t;
   __pyx_pybuffer_deadline.pybuffer.buf = NULL;
   __pyx_pybuffer_deadline.refcount = 0;
   __pyx_pybuffernd_deadline.data = NULL;
   __pyx_pybuffernd_deadline.rcbuffer = &__pyx_pybuffer_deadline;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vh.rcbuffer->pybuffer, (PyObject*)__pyx_v_vh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vh.rcbuffer->pybuffer, (PyObject*)__pyx_v_vh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_vh.diminfo[0].strides = __pyx_pybuffernd_vh.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vh.diminfo[0].shape = __pyx_pybuffernd_vh.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_vl1.diminfo[0].strides = __pyx_pybuffernd_vl1.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vl1.diminfo[0].shape = __pyx_pybuffernd_vl1.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_vl2.diminfo[0].strides = __pyx_pybuffernd_vl2.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vl2.diminfo[0].shape = __pyx_pybuffernd_vl2.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zh.rcbuffer->pybuffer, (PyObject*)__pyx_v_zh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zh.rcbuffer->pybuffer, (PyObject*)__pyx_v_zh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_zh.diminfo[0].strides = __pyx_pybuffernd_zh.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zh.diminfo[0].shape = __pyx_pybuffernd_zh.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_zl1.diminfo[0].strides = __pyx_pybuffernd_zl1.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zl1.diminfo[0].shape = __pyx_pybuffernd_zl1.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_zl2.diminfo[0].strides = __pyx_pybuffernd_zl2.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zl2.diminfo[0].shape = __pyx_pybuffernd_zl2.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_d.rcbuffer->pybuffer, (PyObject*)__pyx_v_d, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_d.rcbuffer->pybuffer, (PyObject*)__pyx_v_d, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_d.diminfo[0].strides = __pyx_pybuffernd_d.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_d.diminfo[0].shape = __pyx_pybuffernd_d.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_g.rcbuffer->pybuffer, (PyObject*)__pyx_v_g, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_g.rcbuffer->pybuffer, (PyObject*)__pyx_v_g, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_g.diminfo[0].strides = __pyx_pybuffernd_g.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_g.diminfo[0].shape = __pyx_pybuffernd_g.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_t.rcbuffer->pybuffer, (PyObject*)__pyx_v_t, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_t.rcbuffer->pybuffer, (PyObject*)__pyx_v_t, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_t.diminfo[0].strides = __pyx_pybuffernd_t.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_t.diminfo[0].shape = __pyx_pybuffernd_t.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3543, __pyx_L1_error)
   }
   __pyx_pybuffernd_deadline.diminfo[0].strides = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_deadline.diminfo[0].shape = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.shape[0];
 
-  /* "cssm.pyx":3353
+  /* "cssm.pyx":3568
  *                                                         **kwargs):
  * 
  *     set_seed(random_state)             # <<<<<<<<<<<<<<
  *     # Param views
  *     cdef float[:] vh_view = vh
  */
-  __pyx_t_1 = __pyx_f_4cssm_set_seed(__pyx_v_random_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3353, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4cssm_set_seed(__pyx_v_random_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cssm.pyx":3355
+  /* "cssm.pyx":3570
  *     set_seed(random_state)
  *     # Param views
  *     cdef float[:] vh_view = vh             # <<<<<<<<<<<<<<
  *     cdef float[:] vl1_view = vl1
  *     cdef float[:] vl2_view = vl2
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3355, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3570, __pyx_L1_error)
   __pyx_v_vh_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3356
+  /* "cssm.pyx":3571
  *     # Param views
  *     cdef float[:] vh_view = vh
  *     cdef float[:] vl1_view = vl1             # <<<<<<<<<<<<<<
  *     cdef float[:] vl2_view = vl2
  *     cdef float[:] a_view = a
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3356, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3571, __pyx_L1_error)
   __pyx_v_vl1_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3357
+  /* "cssm.pyx":3572
  *     cdef float[:] vh_view = vh
  *     cdef float[:] vl1_view = vl1
  *     cdef float[:] vl2_view = vl2             # <<<<<<<<<<<<<<
  *     cdef float[:] a_view = a
  *     cdef float[:] zh_view = zh
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3357, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3572, __pyx_L1_error)
   __pyx_v_vl2_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3358
+  /* "cssm.pyx":3573
  *     cdef float[:] vl1_view = vl1
  *     cdef float[:] vl2_view = vl2
  *     cdef float[:] a_view = a             # <<<<<<<<<<<<<<
  *     cdef float[:] zh_view = zh
  *     cdef float[:] zl1_view = zl1
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3358, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3573, __pyx_L1_error)
   __pyx_v_a_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3359
+  /* "cssm.pyx":3574
  *     cdef float[:] vl2_view = vl2
  *     cdef float[:] a_view = a
  *     cdef float[:] zh_view = zh             # <<<<<<<<<<<<<<
  *     cdef float[:] zl1_view = zl1
  *     cdef float[:] zl2_view = zl2
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3359, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3574, __pyx_L1_error)
   __pyx_v_zh_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3360
+  /* "cssm.pyx":3575
  *     cdef float[:] a_view = a
  *     cdef float[:] zh_view = zh
  *     cdef float[:] zl1_view = zl1             # <<<<<<<<<<<<<<
  *     cdef float[:] zl2_view = zl2
  *     cdef float[:] d_view = d
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3360, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3575, __pyx_L1_error)
   __pyx_v_zl1_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3361
+  /* "cssm.pyx":3576
  *     cdef float[:] zh_view = zh
  *     cdef float[:] zl1_view = zl1
  *     cdef float[:] zl2_view = zl2             # <<<<<<<<<<<<<<
  *     cdef float[:] d_view = d
  *     cdef float[:] g_view = g
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3361, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3576, __pyx_L1_error)
   __pyx_v_zl2_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3362
+  /* "cssm.pyx":3577
  *     cdef float[:] zl1_view = zl1
  *     cdef float[:] zl2_view = zl2
  *     cdef float[:] d_view = d             # <<<<<<<<<<<<<<
  *     cdef float[:] g_view = g
  *     cdef float[:] t_view = t
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_d), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3362, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_d), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3577, __pyx_L1_error)
   __pyx_v_d_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3363
+  /* "cssm.pyx":3578
  *     cdef float[:] zl2_view = zl2
  *     cdef float[:] d_view = d
  *     cdef float[:] g_view = g             # <<<<<<<<<<<<<<
  *     cdef float[:] t_view = t
  *     cdef float[:] deadline_view = deadline
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_g), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3363, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_g), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3578, __pyx_L1_error)
   __pyx_v_g_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3364
+  /* "cssm.pyx":3579
  *     cdef float[:] d_view = d
  *     cdef float[:] g_view = g
  *     cdef float[:] t_view = t             # <<<<<<<<<<<<<<
  *     cdef float[:] deadline_view = deadline
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_t), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3364, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_t), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3579, __pyx_L1_error)
   __pyx_v_t_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3365
+  /* "cssm.pyx":3580
  *     cdef float[:] g_view = g
  *     cdef float[:] t_view = t
  *     cdef float[:] deadline_view = deadline             # <<<<<<<<<<<<<<
  * 
  *     # TD: Add trajectory --> same issue as with par2 model above... might need to make a separate simulator for trajectories
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3365, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3580, __pyx_L1_error)
   __pyx_v_deadline_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3368
+  /* "cssm.pyx":3583
  * 
  *     # TD: Add trajectory --> same issue as with par2 model above... might need to make a separate simulator for trajectories
  *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
  *     rts_low = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 3368, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 3583, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 3368, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 3583, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_int_1)) __PYX_ERR(0, 3368, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_int_1)) __PYX_ERR(0, 3583, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 3368, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 3583, __pyx_L1_error);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 3368, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3368, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_rts = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cssm.pyx":3369
+  /* "cssm.pyx":3584
  *     # TD: Add trajectory --> same issue as with par2 model above... might need to make a separate simulator for trajectories
  *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)             # <<<<<<<<<<<<<<
  *     rts_low = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  *     rts_high = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 3369, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 3584, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 3369, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 3584, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_int_1)) __PYX_ERR(0, 3369, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_int_1)) __PYX_ERR(0, 3584, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3369, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3584, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_intc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_intc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3369, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3369, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3584, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_choices = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "cssm.pyx":3370
+  /* "cssm.pyx":3585
  *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
  *     rts_low = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     rts_high = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3370, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3585, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 3370, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 3585, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_int_1)) __PYX_ERR(0, 3370, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_int_1)) __PYX_ERR(0, 3585, __pyx_L1_error);
   __pyx_t_6 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 3370, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 3585, __pyx_L1_error);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3370, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_rts_low = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "cssm.pyx":3371
+  /* "cssm.pyx":3586
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
  *     rts_low = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  *     rts_high = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
  * 
  *     cdef float[:, :, :] rts_view = rts
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 3371, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 3586, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 3371, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 3586, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_int_1)) __PYX_ERR(0, 3371, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_int_1)) __PYX_ERR(0, 3586, __pyx_L1_error);
   __pyx_t_6 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3371, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3586, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3371, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3371, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_rts_high = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "cssm.pyx":3373
+  /* "cssm.pyx":3588
  *     rts_high = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  * 
  *     cdef float[:, :, :] rts_view = rts             # <<<<<<<<<<<<<<
  *     cdef float[:, :, :] rts_high_view = rts_high
  *     cdef float[:, :, :] rts_low_view = rts_low
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3373, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3588, __pyx_L1_error)
   __pyx_v_rts_view = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "cssm.pyx":3374
+  /* "cssm.pyx":3589
  * 
  *     cdef float[:, :, :] rts_view = rts
  *     cdef float[:, :, :] rts_high_view = rts_high             # <<<<<<<<<<<<<<
  *     cdef float[:, :, :] rts_low_view = rts_low
  *     cdef int[:, :, :] choices_view = choices
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts_high, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3374, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts_high, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3589, __pyx_L1_error)
   __pyx_v_rts_high_view = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "cssm.pyx":3375
+  /* "cssm.pyx":3590
  *     cdef float[:, :, :] rts_view = rts
  *     cdef float[:, :, :] rts_high_view = rts_high
  *     cdef float[:, :, :] rts_low_view = rts_low             # <<<<<<<<<<<<<<
  *     cdef int[:, :, :] choices_view = choices
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts_low, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3375, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts_low, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3590, __pyx_L1_error)
   __pyx_v_rts_low_view = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "cssm.pyx":3376
+  /* "cssm.pyx":3591
  *     cdef float[:, :, :] rts_high_view = rts_high
  *     cdef float[:, :, :] rts_low_view = rts_low
  *     cdef int[:, :, :] choices_view = choices             # <<<<<<<<<<<<<<
  * 
  *     traj = np.zeros((int(max_t / delta_t) + 1, 3), dtype = DTYPE)
  */
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 3376, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 3591, __pyx_L1_error)
   __pyx_v_choices_view = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "cssm.pyx":3378
+  /* "cssm.pyx":3593
  *     cdef int[:, :, :] choices_view = choices
  * 
  *     traj = np.zeros((int(max_t / delta_t) + 1, 3), dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     traj[:, :] = -999
  *     cdef float[:, :] traj_view = traj
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyInt_FromDouble((__pyx_v_max_t / __pyx_v_delta_t)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_FromDouble((__pyx_v_max_t / __pyx_v_delta_t)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_6, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_AddObjC(__pyx_t_6, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4)) __PYX_ERR(0, 3378, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_4)) __PYX_ERR(0, 3593, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_3);
   __Pyx_GIVEREF(__pyx_int_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_int_3)) __PYX_ERR(0, 3378, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_int_3)) __PYX_ERR(0, 3593, __pyx_L1_error);
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6)) __PYX_ERR(0, 3378, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_6)) __PYX_ERR(0, 3593, __pyx_L1_error);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 3378, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3378, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3593, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_traj = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cssm.pyx":3379
+  /* "cssm.pyx":3594
  * 
  *     traj = np.zeros((int(max_t / delta_t) + 1, 3), dtype = DTYPE)
  *     traj[:, :] = -999             # <<<<<<<<<<<<<<
  *     cdef float[:, :] traj_view = traj
  * 
  */
-  if (unlikely((PyObject_SetItem(__pyx_v_traj, __pyx_tuple__12, __pyx_int_neg_999) < 0))) __PYX_ERR(0, 3379, __pyx_L1_error)
+  if (unlikely((PyObject_SetItem(__pyx_v_traj, __pyx_tuple__12, __pyx_int_neg_999) < 0))) __PYX_ERR(0, 3594, __pyx_L1_error)
 
-  /* "cssm.pyx":3380
+  /* "cssm.pyx":3595
  *     traj = np.zeros((int(max_t / delta_t) + 1, 3), dtype = DTYPE)
  *     traj[:, :] = -999
  *     cdef float[:, :] traj_view = traj             # <<<<<<<<<<<<<<
  * 
  *     cdef float delta_t_sqrt = sqrt(delta_t) # correct scalar so we can use standard normal samples for the brownian motion
  */
-  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(__pyx_v_traj, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 3380, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_to_MemoryviewSlice_dsds_float(__pyx_v_traj, PyBUF_WRITABLE); if (unlikely(!__pyx_t_9.memview)) __PYX_ERR(0, 3595, __pyx_L1_error)
   __pyx_v_traj_view = __pyx_t_9;
   __pyx_t_9.memview = NULL;
   __pyx_t_9.data = NULL;
 
-  /* "cssm.pyx":3382
+  /* "cssm.pyx":3597
  *     cdef float[:, :] traj_view = traj
  * 
  *     cdef float delta_t_sqrt = sqrt(delta_t) # correct scalar so we can use standard normal samples for the brownian motion             # <<<<<<<<<<<<<<
  *     cdef float sqrt_st = delta_t_sqrt * s # scalar to ensure the correct variance for the gaussian step
  * 
  */
   __pyx_v_delta_t_sqrt = sqrt(__pyx_v_delta_t);
 
-  /* "cssm.pyx":3383
+  /* "cssm.pyx":3598
  * 
  *     cdef float delta_t_sqrt = sqrt(delta_t) # correct scalar so we can use standard normal samples for the brownian motion
  *     cdef float sqrt_st = delta_t_sqrt * s # scalar to ensure the correct variance for the gaussian step             # <<<<<<<<<<<<<<
  * 
  *     # Boundary storage for the upper bound
  */
   __pyx_v_sqrt_st = (__pyx_v_delta_t_sqrt * __pyx_v_s);
 
-  /* "cssm.pyx":3386
+  /* "cssm.pyx":3601
  * 
  *     # Boundary storage for the upper bound
  *     cdef int num_draws = int((max_t / delta_t) + 1)             # <<<<<<<<<<<<<<
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)
  */
   __pyx_v_num_draws = ((int)((__pyx_v_max_t / __pyx_v_delta_t) + 1.0));
 
-  /* "cssm.pyx":3387
+  /* "cssm.pyx":3602
  *     # Boundary storage for the upper bound
  *     cdef int num_draws = int((max_t / delta_t) + 1)
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)             # <<<<<<<<<<<<<<
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)
  *     cdef float[:] boundary_view = boundary
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_arange); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_max_t + __pyx_v_delta_t)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_max_t + __pyx_v_delta_t)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_10 = NULL;
   __pyx_t_11 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_10)) {
@@ -64808,22 +68982,22 @@
   #endif
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_10, __pyx_int_0, __pyx_t_4, __pyx_t_1};
     __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_11, 3+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3387, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3387, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3602, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_1 = NULL;
   __pyx_t_11 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_1)) {
@@ -64836,267 +69010,267 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_6};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_11, 1+__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3387, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3602, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_t_s = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cssm.pyx":3388
+  /* "cssm.pyx":3603
  *     cdef int num_draws = int((max_t / delta_t) + 1)
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     cdef float[:] boundary_view = boundary
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_np); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_t_s, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_t_s, __pyx_n_s_shape); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 3388, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_5)) __PYX_ERR(0, 3603, __pyx_L1_error);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 3388, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3388, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_6, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3603, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_boundary = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cssm.pyx":3389
+  /* "cssm.pyx":3604
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)
  *     cdef float[:] boundary_view = boundary             # <<<<<<<<<<<<<<
  * 
  *     # Y particle trace
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_boundary, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3389, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_boundary, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3604, __pyx_L1_error)
   __pyx_v_boundary_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3392
+  /* "cssm.pyx":3607
  * 
  *     # Y particle trace
  *     bias_trace_l1 = np.zeros(num_draws, dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     bias_trace_l2 = np.zeros(num_draws, dtype = DTYPE)
  *     cdef float[:] bias_trace_l1_view = bias_trace_l1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_draws); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_draws); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 3392, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 3607, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 3392, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_3) < 0) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3392, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_6, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3607, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_bias_trace_l1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "cssm.pyx":3393
+  /* "cssm.pyx":3608
  *     # Y particle trace
  *     bias_trace_l1 = np.zeros(num_draws, dtype = DTYPE)
  *     bias_trace_l2 = np.zeros(num_draws, dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     cdef float[:] bias_trace_l1_view = bias_trace_l1
  *     cdef float[:] bias_trace_l2_view = bias_trace_l2
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_zeros); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_num_draws); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_num_draws); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 3393, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_3)) __PYX_ERR(0, 3608, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 3393, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3393, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3608, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_bias_trace_l2 = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cssm.pyx":3394
+  /* "cssm.pyx":3609
  *     bias_trace_l1 = np.zeros(num_draws, dtype = DTYPE)
  *     bias_trace_l2 = np.zeros(num_draws, dtype = DTYPE)
  *     cdef float[:] bias_trace_l1_view = bias_trace_l1             # <<<<<<<<<<<<<<
  *     cdef float[:] bias_trace_l2_view = bias_trace_l2
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_bias_trace_l1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_bias_trace_l1, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3609, __pyx_L1_error)
   __pyx_v_bias_trace_l1_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3395
+  /* "cssm.pyx":3610
  *     bias_trace_l2 = np.zeros(num_draws, dtype = DTYPE)
  *     cdef float[:] bias_trace_l1_view = bias_trace_l1
  *     cdef float[:] bias_trace_l2_view = bias_trace_l2             # <<<<<<<<<<<<<<
  * 
  *     cdef float y_h, y_l, y_l1, y_l2
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_bias_trace_l2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3395, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_bias_trace_l2, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3610, __pyx_L1_error)
   __pyx_v_bias_trace_l2_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3401
+  /* "cssm.pyx":3616
  *     cdef float t_h, t_l, t_l1, t_l2, smooth_u, deadline_tmp
  *     cdef Py_ssize_t n, ix, ix1, ix2, ix_l, ix_tmp, ix1_tmp, ix2_tmp, k
  *     cdef Py_ssize_t m = 0             # <<<<<<<<<<<<<<
  *     cdef float[:] gaussian_values = draw_gaussian(num_draws)
  * 
  */
   __pyx_v_m = 0;
 
-  /* "cssm.pyx":3402
+  /* "cssm.pyx":3617
  *     cdef Py_ssize_t n, ix, ix1, ix2, ix_l, ix_tmp, ix1_tmp, ix2_tmp, k
  *     cdef Py_ssize_t m = 0
  *     cdef float[:] gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  * 
  *     for k in range(n_trials):
  */
-  __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3402, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3617, __pyx_L1_error)
   __pyx_v_gaussian_values = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3404
+  /* "cssm.pyx":3619
  *     cdef float[:] gaussian_values = draw_gaussian(num_draws)
  * 
  *     for k in range(n_trials):             # <<<<<<<<<<<<<<
  *         # Precompute boundary evaluations
  *         boundary_params_tmp = {key: boundary_params[key][k] for key in boundary_params.keys()}
  */
   __pyx_t_11 = __pyx_v_n_trials;
   __pyx_t_12 = __pyx_t_11;
   for (__pyx_t_13 = 0; __pyx_t_13 < __pyx_t_12; __pyx_t_13+=1) {
     __pyx_v_k = __pyx_t_13;
 
-    /* "cssm.pyx":3406
+    /* "cssm.pyx":3621
  *     for k in range(n_trials):
  *         # Precompute boundary evaluations
  *         boundary_params_tmp = {key: boundary_params[key][k] for key in boundary_params.keys()}             # <<<<<<<<<<<<<<
  * 
  *         # Precompute boundary evaluations
  */
     { /* enter inner scope */
-      __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3406, __pyx_L7_error)
+      __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3621, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_14 = 0;
       if (unlikely(__pyx_v_boundary_params == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-        __PYX_ERR(0, 3406, __pyx_L7_error)
+        __PYX_ERR(0, 3621, __pyx_L7_error)
       }
-      __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_boundary_params, 0, __pyx_n_s_keys, (&__pyx_t_15), (&__pyx_t_16)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3406, __pyx_L7_error)
+      __pyx_t_6 = __Pyx_dict_iterator(__pyx_v_boundary_params, 0, __pyx_n_s_keys, (&__pyx_t_15), (&__pyx_t_16)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3621, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_3);
       __pyx_t_3 = __pyx_t_6;
       __pyx_t_6 = 0;
       while (1) {
         __pyx_t_17 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_15, &__pyx_t_14, &__pyx_t_6, NULL, NULL, __pyx_t_16);
         if (unlikely(__pyx_t_17 == 0)) break;
-        if (unlikely(__pyx_t_17 == -1)) __PYX_ERR(0, 3406, __pyx_L7_error)
+        if (unlikely(__pyx_t_17 == -1)) __PYX_ERR(0, 3621, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_XDECREF_SET(__pyx_9genexpr14__pyx_v_key, __pyx_t_6);
         __pyx_t_6 = 0;
-        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_boundary_params, __pyx_9genexpr14__pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3406, __pyx_L7_error)
+        __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_v_boundary_params, __pyx_9genexpr14__pyx_v_key); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3621, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_k, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3406, __pyx_L7_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_t_6, __pyx_v_k, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3621, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_9genexpr14__pyx_v_key, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 3406, __pyx_L7_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_9genexpr14__pyx_v_key, (PyObject*)__pyx_t_1))) __PYX_ERR(0, 3621, __pyx_L7_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_XDECREF(__pyx_9genexpr14__pyx_v_key); __pyx_9genexpr14__pyx_v_key = 0;
       goto __pyx_L10_exit_scope;
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_9genexpr14__pyx_v_key); __pyx_9genexpr14__pyx_v_key = 0;
       goto __pyx_L1_error;
       __pyx_L10_exit_scope:;
     } /* exit inner scope */
     __Pyx_XDECREF_SET(__pyx_v_boundary_params_tmp, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "cssm.pyx":3409
+    /* "cssm.pyx":3624
  * 
  *         # Precompute boundary evaluations
  *         if boundary_multiplicative:             # <<<<<<<<<<<<<<
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  *         else:
  */
-    __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_boundary_multiplicative); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3409, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_boundary_multiplicative); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3624, __pyx_L1_error)
     if (__pyx_t_18) {
 
-      /* "cssm.pyx":3410
+      /* "cssm.pyx":3625
  *         # Precompute boundary evaluations
  *         if boundary_multiplicative:
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)             # <<<<<<<<<<<<<<
  *         else:
  *             boundary[:] = np.add(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_multiply); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_multiply); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_19 = __pyx_v_k;
-      __pyx_t_1 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_19 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      __pyx_t_1 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_19 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
-      if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 3410, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_10, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 3625, __pyx_L1_error)
       __pyx_t_4 = __pyx_t_10;
       __pyx_t_10 = 0;
-      if (__Pyx_MergeKeywords(__pyx_t_4, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 3410, __pyx_L1_error)
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      if (__Pyx_MergeKeywords(__pyx_t_4, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 3625, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       __pyx_t_16 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_6);
@@ -65111,22 +69285,22 @@
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_1, __pyx_t_10};
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_16, 2+__pyx_t_16);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3410, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3625, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3410, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_10 = NULL;
       __pyx_t_16 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_10)) {
@@ -65139,54 +69313,54 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_3};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3410, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3625, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
-      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 3410, __pyx_L1_error)
+      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 3625, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "cssm.pyx":3409
+      /* "cssm.pyx":3624
  * 
  *         # Precompute boundary evaluations
  *         if boundary_multiplicative:             # <<<<<<<<<<<<<<
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  *         else:
  */
       goto __pyx_L11;
     }
 
-    /* "cssm.pyx":3412
+    /* "cssm.pyx":3627
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  *         else:
  *             boundary[:] = np.add(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)             # <<<<<<<<<<<<<<
  * 
  *         deadline_tmp = min(max_t, deadline_view[k] - t_view[k])
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_np); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_add); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_add); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_19 = __pyx_v_k;
-      __pyx_t_3 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_19 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      __pyx_t_3 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_19 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 3412, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 3627, __pyx_L1_error)
       __pyx_t_1 = __pyx_t_4;
       __pyx_t_4 = 0;
-      if (__Pyx_MergeKeywords(__pyx_t_1, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 3412, __pyx_L1_error)
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      if (__Pyx_MergeKeywords(__pyx_t_1, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 3627, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = NULL;
       __pyx_t_16 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_10);
@@ -65201,22 +69375,22 @@
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_1, __pyx_t_3, __pyx_t_4};
         __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_16, 2+__pyx_t_16);
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3412, __pyx_L1_error)
+        if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3627, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
-      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_astype); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_astype); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3412, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_4 = NULL;
       __pyx_t_16 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_10))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_10);
         if (likely(__pyx_t_4)) {
@@ -65229,24 +69403,24 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_6};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_10, __pyx_callargs+1-__pyx_t_16, 1+__pyx_t_16);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3412, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3627, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
-      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 3412, __pyx_L1_error)
+      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 3627, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_L11:;
 
-    /* "cssm.pyx":3414
+    /* "cssm.pyx":3629
  *             boundary[:] = np.add(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  * 
  *         deadline_tmp = min(max_t, deadline_view[k] - t_view[k])             # <<<<<<<<<<<<<<
  *         # Loop over samples
  *         for n in range(n_samples):
  */
     __pyx_t_19 = __pyx_v_k;
@@ -65257,186 +69431,186 @@
     if (__pyx_t_18) {
       __pyx_t_23 = __pyx_t_21;
     } else {
       __pyx_t_23 = __pyx_t_22;
     }
     __pyx_v_deadline_tmp = __pyx_t_23;
 
-    /* "cssm.pyx":3416
+    /* "cssm.pyx":3631
  *         deadline_tmp = min(max_t, deadline_view[k] - t_view[k])
  *         # Loop over samples
  *         for n in range(n_samples):             # <<<<<<<<<<<<<<
  *             choices_view[n, k, 0] = 0 # reset choice
  *             t_h = 0 # reset time high dimension
  */
     __pyx_t_16 = __pyx_v_n_samples;
     __pyx_t_17 = __pyx_t_16;
     for (__pyx_t_15 = 0; __pyx_t_15 < __pyx_t_17; __pyx_t_15+=1) {
       __pyx_v_n = __pyx_t_15;
 
-      /* "cssm.pyx":3417
+      /* "cssm.pyx":3632
  *         # Loop over samples
  *         for n in range(n_samples):
  *             choices_view[n, k, 0] = 0 # reset choice             # <<<<<<<<<<<<<<
  *             t_h = 0 # reset time high dimension
  *             t_l = 0 # reset time low dimension
  */
       __pyx_t_20 = __pyx_v_n;
       __pyx_t_19 = __pyx_v_k;
       __pyx_t_24 = 0;
       *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_20 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[2]) )) = 0;
 
-      /* "cssm.pyx":3418
+      /* "cssm.pyx":3633
  *         for n in range(n_samples):
  *             choices_view[n, k, 0] = 0 # reset choice
  *             t_h = 0 # reset time high dimension             # <<<<<<<<<<<<<<
  *             t_l = 0 # reset time low dimension
  *             t_l1 = 0 # reset time low dimension (1)
  */
       __pyx_v_t_h = 0.0;
 
-      /* "cssm.pyx":3419
+      /* "cssm.pyx":3634
  *             choices_view[n, k, 0] = 0 # reset choice
  *             t_h = 0 # reset time high dimension
  *             t_l = 0 # reset time low dimension             # <<<<<<<<<<<<<<
  *             t_l1 = 0 # reset time low dimension (1)
  *             t_l2 = 0 # reset time low dimension (2)
  */
       __pyx_v_t_l = 0.0;
 
-      /* "cssm.pyx":3420
+      /* "cssm.pyx":3635
  *             t_h = 0 # reset time high dimension
  *             t_l = 0 # reset time low dimension
  *             t_l1 = 0 # reset time low dimension (1)             # <<<<<<<<<<<<<<
  *             t_l2 = 0 # reset time low dimension (2)
  *             ix = 0 # reset boundary index
  */
       __pyx_v_t_l1 = 0.0;
 
-      /* "cssm.pyx":3421
+      /* "cssm.pyx":3636
  *             t_l = 0 # reset time low dimension
  *             t_l1 = 0 # reset time low dimension (1)
  *             t_l2 = 0 # reset time low dimension (2)             # <<<<<<<<<<<<<<
  *             ix = 0 # reset boundary index
  *             ix1 = 0 # reset boundary index (1)
  */
       __pyx_v_t_l2 = 0.0;
 
-      /* "cssm.pyx":3422
+      /* "cssm.pyx":3637
  *             t_l1 = 0 # reset time low dimension (1)
  *             t_l2 = 0 # reset time low dimension (2)
  *             ix = 0 # reset boundary index             # <<<<<<<<<<<<<<
  *             ix1 = 0 # reset boundary index (1)
  *             ix2 = 0 # reset boundary index (2)
  */
       __pyx_v_ix = 0;
 
-      /* "cssm.pyx":3423
+      /* "cssm.pyx":3638
  *             t_l2 = 0 # reset time low dimension (2)
  *             ix = 0 # reset boundary index
  *             ix1 = 0 # reset boundary index (1)             # <<<<<<<<<<<<<<
  *             ix2 = 0 # reset boundary index (2)
  * 
  */
       __pyx_v_ix1 = 0;
 
-      /* "cssm.pyx":3424
+      /* "cssm.pyx":3639
  *             ix = 0 # reset boundary index
  *             ix1 = 0 # reset boundary index (1)
  *             ix2 = 0 # reset boundary index (2)             # <<<<<<<<<<<<<<
  * 
  *             # Initialize walkers
  */
       __pyx_v_ix2 = 0;
 
-      /* "cssm.pyx":3428
+      /* "cssm.pyx":3643
  *             # Initialize walkers
  *             # Particle
  *             y_h = (-1) * boundary_view[0] + (zh_view[k] * 2 * (boundary_view[0]))             # <<<<<<<<<<<<<<
  *             # Relative particle position (used as resource allocator for low dim choice)
  *             bias_trace_l2_view[0] = ((y_h + boundary_view[0]) / (2))
  */
       __pyx_t_24 = 0;
       __pyx_t_19 = __pyx_v_k;
       __pyx_t_20 = 0;
       __pyx_v_y_h = ((-1.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_24 * __pyx_v_boundary_view.strides[0]) )))) + (((*((float *) ( /* dim=0 */ (__pyx_v_zh_view.data + __pyx_t_19 * __pyx_v_zh_view.strides[0]) ))) * 2.0) * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) )))));
 
-      /* "cssm.pyx":3430
+      /* "cssm.pyx":3645
  *             y_h = (-1) * boundary_view[0] + (zh_view[k] * 2 * (boundary_view[0]))
  *             # Relative particle position (used as resource allocator for low dim choice)
  *             bias_trace_l2_view[0] = ((y_h + boundary_view[0]) / (2))             # <<<<<<<<<<<<<<
  *             bias_trace_l1_view[0] = boundary_view[0] - bias_trace_l2_view[0]
  * 
  */
       __pyx_t_20 = 0;
       __pyx_t_19 = 0;
       *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_19 * __pyx_v_bias_trace_l2_view.strides[0]) )) = ((__pyx_v_y_h + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) )))) / 2.0);
 
-      /* "cssm.pyx":3431
+      /* "cssm.pyx":3646
  *             # Relative particle position (used as resource allocator for low dim choice)
  *             bias_trace_l2_view[0] = ((y_h + boundary_view[0]) / (2))
  *             bias_trace_l1_view[0] = boundary_view[0] - bias_trace_l2_view[0]             # <<<<<<<<<<<<<<
  * 
  *             if n == 0:
  */
       __pyx_t_20 = 0;
       __pyx_t_19 = 0;
       __pyx_t_24 = 0;
       *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_24 * __pyx_v_bias_trace_l1_view.strides[0]) )) = ((*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) ))) - (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_19 * __pyx_v_bias_trace_l2_view.strides[0]) ))));
 
-      /* "cssm.pyx":3433
+      /* "cssm.pyx":3648
  *             bias_trace_l1_view[0] = boundary_view[0] - bias_trace_l2_view[0]
  * 
  *             if n == 0:             # <<<<<<<<<<<<<<
  *                 if k == 0:
  *                     traj_view[0, 0] = y_h
  */
       __pyx_t_18 = (__pyx_v_n == 0);
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3434
+        /* "cssm.pyx":3649
  * 
  *             if n == 0:
  *                 if k == 0:             # <<<<<<<<<<<<<<
  *                     traj_view[0, 0] = y_h
  * 
  */
         __pyx_t_18 = (__pyx_v_k == 0);
         if (__pyx_t_18) {
 
-          /* "cssm.pyx":3435
+          /* "cssm.pyx":3650
  *             if n == 0:
  *                 if k == 0:
  *                     traj_view[0, 0] = y_h             # <<<<<<<<<<<<<<
  * 
  *             # Random walks until y_h hits bound
  */
           __pyx_t_19 = 0;
           __pyx_t_20 = 0;
           *((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_traj_view.data + __pyx_t_19 * __pyx_v_traj_view.strides[0]) ) + __pyx_t_20 * __pyx_v_traj_view.strides[1]) )) = __pyx_v_y_h;
 
-          /* "cssm.pyx":3434
+          /* "cssm.pyx":3649
  * 
  *             if n == 0:
  *                 if k == 0:             # <<<<<<<<<<<<<<
  *                     traj_view[0, 0] = y_h
  * 
  */
         }
 
-        /* "cssm.pyx":3433
+        /* "cssm.pyx":3648
  *             bias_trace_l1_view[0] = boundary_view[0] - bias_trace_l2_view[0]
  * 
  *             if n == 0:             # <<<<<<<<<<<<<<
  *                 if k == 0:
  *                     traj_view[0, 0] = y_h
  */
       }
 
-      /* "cssm.pyx":3438
+      /* "cssm.pyx":3653
  * 
  *             # Random walks until y_h hits bound
  *             while (y_h >= ((-1) * boundary_view[ix])) and ((y_h <= boundary_view[ix])) and (t_h <= deadline_tmp):             # <<<<<<<<<<<<<<
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])
  *                 bias_trace_l2_view[ix] = ((y_h + boundary_view[ix]) / (2))
  */
       while (1) {
@@ -65455,369 +69629,369 @@
           goto __pyx_L18_bool_binop_done;
         }
         __pyx_t_25 = (__pyx_v_t_h <= __pyx_v_deadline_tmp);
         __pyx_t_18 = __pyx_t_25;
         __pyx_L18_bool_binop_done:;
         if (!__pyx_t_18) break;
 
-        /* "cssm.pyx":3439
+        /* "cssm.pyx":3654
  *             # Random walks until y_h hits bound
  *             while (y_h >= ((-1) * boundary_view[ix])) and ((y_h <= boundary_view[ix])) and (t_h <= deadline_tmp):
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])             # <<<<<<<<<<<<<<
  *                 bias_trace_l2_view[ix] = ((y_h + boundary_view[ix]) / (2))
  *                 bias_trace_l1_view[ix] = boundary_view[ix] - bias_trace_l2_view[ix]
  */
         __pyx_t_20 = __pyx_v_k;
         __pyx_t_19 = __pyx_v_m;
         __pyx_v_y_h = (__pyx_v_y_h + (((*((float *) ( /* dim=0 */ (__pyx_v_vh_view.data + __pyx_t_20 * __pyx_v_vh_view.strides[0]) ))) * __pyx_v_delta_t) + (__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_19 * __pyx_v_gaussian_values.strides[0]) ))))));
 
-        /* "cssm.pyx":3440
+        /* "cssm.pyx":3655
  *             while (y_h >= ((-1) * boundary_view[ix])) and ((y_h <= boundary_view[ix])) and (t_h <= deadline_tmp):
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])
  *                 bias_trace_l2_view[ix] = ((y_h + boundary_view[ix]) / (2))             # <<<<<<<<<<<<<<
  *                 bias_trace_l1_view[ix] = boundary_view[ix] - bias_trace_l2_view[ix]
  *                 t_h += delta_t
  */
         __pyx_t_19 = __pyx_v_ix;
         __pyx_t_20 = __pyx_v_ix;
         *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_20 * __pyx_v_bias_trace_l2_view.strides[0]) )) = ((__pyx_v_y_h + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) / 2.0);
 
-        /* "cssm.pyx":3441
+        /* "cssm.pyx":3656
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])
  *                 bias_trace_l2_view[ix] = ((y_h + boundary_view[ix]) / (2))
  *                 bias_trace_l1_view[ix] = boundary_view[ix] - bias_trace_l2_view[ix]             # <<<<<<<<<<<<<<
  *                 t_h += delta_t
  *                 ix += 1
  */
         __pyx_t_19 = __pyx_v_ix;
         __pyx_t_20 = __pyx_v_ix;
         __pyx_t_24 = __pyx_v_ix;
         *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_24 * __pyx_v_bias_trace_l1_view.strides[0]) )) = ((*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) ))) - (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_20 * __pyx_v_bias_trace_l2_view.strides[0]) ))));
 
-        /* "cssm.pyx":3442
+        /* "cssm.pyx":3657
  *                 bias_trace_l2_view[ix] = ((y_h + boundary_view[ix]) / (2))
  *                 bias_trace_l1_view[ix] = boundary_view[ix] - bias_trace_l2_view[ix]
  *                 t_h += delta_t             # <<<<<<<<<<<<<<
  *                 ix += 1
  *                 m += 1
  */
         __pyx_v_t_h = (__pyx_v_t_h + __pyx_v_delta_t);
 
-        /* "cssm.pyx":3443
+        /* "cssm.pyx":3658
  *                 bias_trace_l1_view[ix] = boundary_view[ix] - bias_trace_l2_view[ix]
  *                 t_h += delta_t
  *                 ix += 1             # <<<<<<<<<<<<<<
  *                 m += 1
  *                 if m == num_draws:
  */
         __pyx_v_ix = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3444
+        /* "cssm.pyx":3659
  *                 t_h += delta_t
  *                 ix += 1
  *                 m += 1             # <<<<<<<<<<<<<<
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)
  */
         __pyx_v_m = (__pyx_v_m + 1);
 
-        /* "cssm.pyx":3445
+        /* "cssm.pyx":3660
  *                 ix += 1
  *                 m += 1
  *                 if m == num_draws:             # <<<<<<<<<<<<<<
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0
  */
         __pyx_t_18 = (__pyx_v_m == __pyx_v_num_draws);
         if (__pyx_t_18) {
 
-          /* "cssm.pyx":3446
+          /* "cssm.pyx":3661
  *                 m += 1
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  *                     m = 0
  * 
  */
-          __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3446, __pyx_L1_error)
+          __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3661, __pyx_L1_error)
           __PYX_XCLEAR_MEMVIEW(&__pyx_v_gaussian_values, 1);
           __pyx_v_gaussian_values = __pyx_t_2;
           __pyx_t_2.memview = NULL;
           __pyx_t_2.data = NULL;
 
-          /* "cssm.pyx":3447
+          /* "cssm.pyx":3662
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0             # <<<<<<<<<<<<<<
  * 
  *             # The probability of making a 'mistake' 1 - (relative y position)
  */
           __pyx_v_m = 0;
 
-          /* "cssm.pyx":3445
+          /* "cssm.pyx":3660
  *                 ix += 1
  *                 m += 1
  *                 if m == num_draws:             # <<<<<<<<<<<<<<
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0
  */
         }
       }
 
-      /* "cssm.pyx":3454
+      /* "cssm.pyx":3669
  * 
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
  *                 if random_uniform() <= 0.5:
  *                     choices_view[n, k, 0] += 2
  */
       __pyx_t_20 = __pyx_v_ix;
       __pyx_t_18 = ((*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) ))) <= 0.0);
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3455
+        /* "cssm.pyx":3670
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:
  *                 if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
  *                     choices_view[n, k, 0] += 2
  *             # Otherwise, apply rule from above
  */
-        __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3455, __pyx_L1_error)
+        __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3670, __pyx_L1_error)
         __pyx_t_18 = (__pyx_t_23 <= 0.5);
         if (__pyx_t_18) {
 
-          /* "cssm.pyx":3456
+          /* "cssm.pyx":3671
  *             if boundary_view[ix] <= 0:
  *                 if random_uniform() <= 0.5:
  *                     choices_view[n, k, 0] += 2             # <<<<<<<<<<<<<<
  *             # Otherwise, apply rule from above
  *             elif random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):
  */
           __pyx_t_20 = __pyx_v_n;
           __pyx_t_19 = __pyx_v_k;
           __pyx_t_24 = 0;
           *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_20 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[2]) )) += 2;
 
-          /* "cssm.pyx":3455
+          /* "cssm.pyx":3670
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:
  *                 if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
  *                     choices_view[n, k, 0] += 2
  *             # Otherwise, apply rule from above
  */
         }
 
-        /* "cssm.pyx":3454
+        /* "cssm.pyx":3669
  * 
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
  *                 if random_uniform() <= 0.5:
  *                     choices_view[n, k, 0] += 2
  */
         goto __pyx_L22;
       }
 
-      /* "cssm.pyx":3458
+      /* "cssm.pyx":3673
  *                     choices_view[n, k, 0] += 2
  *             # Otherwise, apply rule from above
  *             elif random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 2
  * 
  */
-      __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3458, __pyx_L1_error)
+      __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3673, __pyx_L1_error)
       __pyx_t_24 = __pyx_v_ix;
       __pyx_t_19 = __pyx_v_ix;
       __pyx_t_18 = (__pyx_t_23 <= ((__pyx_v_y_h + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_24 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) ))))));
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3459
+        /* "cssm.pyx":3674
  *             # Otherwise, apply rule from above
  *             elif random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):
  *                 choices_view[n, k, 0] += 2             # <<<<<<<<<<<<<<
  * 
  *             y_l2 = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))
  */
         __pyx_t_19 = __pyx_v_n;
         __pyx_t_24 = __pyx_v_k;
         __pyx_t_20 = 0;
         *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_19 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_20 * __pyx_v_choices_view.strides[2]) )) += 2;
 
-        /* "cssm.pyx":3458
+        /* "cssm.pyx":3673
  *                     choices_view[n, k, 0] += 2
  *             # Otherwise, apply rule from above
  *             elif random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 2
  * 
  */
       }
       __pyx_L22:;
 
-      /* "cssm.pyx":3461
+      /* "cssm.pyx":3676
  *                 choices_view[n, k, 0] += 2
  * 
  *             y_l2 = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))             # <<<<<<<<<<<<<<
  *             y_l1 = (- 1) * boundary_view[0] + (zl1_view[k] * 2 * (boundary_view[0]))
  * 
  */
       __pyx_t_20 = 0;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_19 = 0;
       __pyx_v_y_l2 = ((-1.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) )))) + (((*((float *) ( /* dim=0 */ (__pyx_v_zl2_view.data + __pyx_t_24 * __pyx_v_zl2_view.strides[0]) ))) * 2.0) * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))));
 
-      /* "cssm.pyx":3462
+      /* "cssm.pyx":3677
  * 
  *             y_l2 = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))
  *             y_l1 = (- 1) * boundary_view[0] + (zl1_view[k] * 2 * (boundary_view[0]))             # <<<<<<<<<<<<<<
  * 
  *             if choices_view[n, k, 0] == 0:
  */
       __pyx_t_19 = 0;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_20 = 0;
       __pyx_v_y_l1 = ((-1.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) + (((*((float *) ( /* dim=0 */ (__pyx_v_zl1_view.data + __pyx_t_24 * __pyx_v_zl1_view.strides[0]) ))) * 2.0) * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) )))));
 
-      /* "cssm.pyx":3464
+      /* "cssm.pyx":3679
  *             y_l1 = (- 1) * boundary_view[0] + (zl1_view[k] * 2 * (boundary_view[0]))
  * 
  *             if choices_view[n, k, 0] == 0:             # <<<<<<<<<<<<<<
  *                  # Fill bias trace a until max_rt reached
  *                 ix1_tmp = ix + 1
  */
       __pyx_t_20 = __pyx_v_n;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_19 = 0;
       __pyx_t_18 = ((*((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_20 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[2]) ))) == 0);
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3466
+        /* "cssm.pyx":3681
  *             if choices_view[n, k, 0] == 0:
  *                  # Fill bias trace a until max_rt reached
  *                 ix1_tmp = ix + 1             # <<<<<<<<<<<<<<
  *                 while ix1_tmp < num_draws:
  *                     bias_trace_l2_view[ix1_tmp] = 0.0
  */
         __pyx_v_ix1_tmp = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3467
+        /* "cssm.pyx":3682
  *                  # Fill bias trace a until max_rt reached
  *                 ix1_tmp = ix + 1
  *                 while ix1_tmp < num_draws:             # <<<<<<<<<<<<<<
  *                     bias_trace_l2_view[ix1_tmp] = 0.0
  *                     bias_trace_l1_view[ix1_tmp] = 1.0
  */
         while (1) {
           __pyx_t_18 = (__pyx_v_ix1_tmp < __pyx_v_num_draws);
           if (!__pyx_t_18) break;
 
-          /* "cssm.pyx":3468
+          /* "cssm.pyx":3683
  *                 ix1_tmp = ix + 1
  *                 while ix1_tmp < num_draws:
  *                     bias_trace_l2_view[ix1_tmp] = 0.0             # <<<<<<<<<<<<<<
  *                     bias_trace_l1_view[ix1_tmp] = 1.0
  *                     ix1_tmp += 1
  */
           __pyx_t_19 = __pyx_v_ix1_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_19 * __pyx_v_bias_trace_l2_view.strides[0]) )) = 0.0;
 
-          /* "cssm.pyx":3469
+          /* "cssm.pyx":3684
  *                 while ix1_tmp < num_draws:
  *                     bias_trace_l2_view[ix1_tmp] = 0.0
  *                     bias_trace_l1_view[ix1_tmp] = 1.0             # <<<<<<<<<<<<<<
  *                     ix1_tmp += 1
  * 
  */
           __pyx_t_19 = __pyx_v_ix1_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_19 * __pyx_v_bias_trace_l1_view.strides[0]) )) = 1.0;
 
-          /* "cssm.pyx":3470
+          /* "cssm.pyx":3685
  *                     bias_trace_l2_view[ix1_tmp] = 0.0
  *                     bias_trace_l1_view[ix1_tmp] = 1.0
  *                     ix1_tmp += 1             # <<<<<<<<<<<<<<
  * 
  *             else: # Store intermediate choice
  */
           __pyx_v_ix1_tmp = (__pyx_v_ix1_tmp + 1);
         }
 
-        /* "cssm.pyx":3464
+        /* "cssm.pyx":3679
  *             y_l1 = (- 1) * boundary_view[0] + (zl1_view[k] * 2 * (boundary_view[0]))
  * 
  *             if choices_view[n, k, 0] == 0:             # <<<<<<<<<<<<<<
  *                  # Fill bias trace a until max_rt reached
  *                 ix1_tmp = ix + 1
  */
         goto __pyx_L24;
       }
 
-      /* "cssm.pyx":3474
+      /* "cssm.pyx":3689
  *             else: # Store intermediate choice
  *                 # Fill bias tracea until max_rt reached
  *                 ix2_tmp = ix + 1             # <<<<<<<<<<<<<<
  *                 while ix2_tmp < num_draws:
  *                     bias_trace_l2_view[ix2_tmp] = 1.0
  */
       /*else*/ {
         __pyx_v_ix2_tmp = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3475
+        /* "cssm.pyx":3690
  *                 # Fill bias tracea until max_rt reached
  *                 ix2_tmp = ix + 1
  *                 while ix2_tmp < num_draws:             # <<<<<<<<<<<<<<
  *                     bias_trace_l2_view[ix2_tmp] = 1.0
  *                     bias_trace_l1_view[ix2_tmp] = 0.0
  */
         while (1) {
           __pyx_t_18 = (__pyx_v_ix2_tmp < __pyx_v_num_draws);
           if (!__pyx_t_18) break;
 
-          /* "cssm.pyx":3476
+          /* "cssm.pyx":3691
  *                 ix2_tmp = ix + 1
  *                 while ix2_tmp < num_draws:
  *                     bias_trace_l2_view[ix2_tmp] = 1.0             # <<<<<<<<<<<<<<
  *                     bias_trace_l1_view[ix2_tmp] = 0.0
  *                     ix2_tmp += 1
  */
           __pyx_t_19 = __pyx_v_ix2_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_19 * __pyx_v_bias_trace_l2_view.strides[0]) )) = 1.0;
 
-          /* "cssm.pyx":3477
+          /* "cssm.pyx":3692
  *                 while ix2_tmp < num_draws:
  *                     bias_trace_l2_view[ix2_tmp] = 1.0
  *                     bias_trace_l1_view[ix2_tmp] = 0.0             # <<<<<<<<<<<<<<
  *                     ix2_tmp += 1
  * 
  */
           __pyx_t_19 = __pyx_v_ix2_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_19 * __pyx_v_bias_trace_l1_view.strides[0]) )) = 0.0;
 
-          /* "cssm.pyx":3478
+          /* "cssm.pyx":3693
  *                     bias_trace_l2_view[ix2_tmp] = 1.0
  *                     bias_trace_l1_view[ix2_tmp] = 0.0
  *                     ix2_tmp += 1             # <<<<<<<<<<<<<<
  * 
  *             # lower level random walker (1)
  */
           __pyx_v_ix2_tmp = (__pyx_v_ix2_tmp + 1);
         }
       }
       __pyx_L24:;
 
-      /* "cssm.pyx":3481
+      /* "cssm.pyx":3696
  * 
  *             # lower level random walker (1)
  *             if (choices_view[n, k, 0] == 0) | ((n == 0) & (k == 0)):             # <<<<<<<<<<<<<<
  *                 while (y_l1 >= ((-1) * boundary_view[ix1])) and (y_l1 <= boundary_view[ix1]) and (t_l1 <= deadline_tmp):
  *                     if (bias_trace_l1_view[ix1] < boundary_view[ix1]) and (bias_trace_l1_view[ix1] > 0):
  */
       __pyx_t_19 = __pyx_v_n;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_20 = 0;
       __pyx_t_18 = (((*((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_19 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_20 * __pyx_v_choices_view.strides[2]) ))) == 0) | ((__pyx_v_n == 0) & (__pyx_v_k == 0)));
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3482
+        /* "cssm.pyx":3697
  *             # lower level random walker (1)
  *             if (choices_view[n, k, 0] == 0) | ((n == 0) & (k == 0)):
  *                 while (y_l1 >= ((-1) * boundary_view[ix1])) and (y_l1 <= boundary_view[ix1]) and (t_l1 <= deadline_tmp):             # <<<<<<<<<<<<<<
  *                     if (bias_trace_l1_view[ix1] < boundary_view[ix1]) and (bias_trace_l1_view[ix1] > 0):
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  */
         while (1) {
@@ -65836,15 +70010,15 @@
             goto __pyx_L32_bool_binop_done;
           }
           __pyx_t_25 = (__pyx_v_t_l1 <= __pyx_v_deadline_tmp);
           __pyx_t_18 = __pyx_t_25;
           __pyx_L32_bool_binop_done:;
           if (!__pyx_t_18) break;
 
-          /* "cssm.pyx":3483
+          /* "cssm.pyx":3698
  *             if (choices_view[n, k, 0] == 0) | ((n == 0) & (k == 0)):
  *                 while (y_l1 >= ((-1) * boundary_view[ix1])) and (y_l1 <= boundary_view[ix1]) and (t_l1 <= deadline_tmp):
  *                     if (bias_trace_l1_view[ix1] < boundary_view[ix1]) and (bias_trace_l1_view[ix1] > 0):             # <<<<<<<<<<<<<<
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  *                         y_l1 += (((vl1_view[k] * bias_trace_l1_view[ix1] * (1 - d_view[k])) - (g_view[k] * y_l1)) * delta_t)
  */
           __pyx_t_20 = __pyx_v_ix1;
@@ -65857,212 +70031,212 @@
           }
           __pyx_t_24 = __pyx_v_ix1;
           __pyx_t_25 = ((*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_24 * __pyx_v_bias_trace_l1_view.strides[0]) ))) > 0.0);
           __pyx_t_18 = __pyx_t_25;
           __pyx_L36_bool_binop_done:;
           if (__pyx_t_18) {
 
-            /* "cssm.pyx":3485
+            /* "cssm.pyx":3700
  *                     if (bias_trace_l1_view[ix1] < boundary_view[ix1]) and (bias_trace_l1_view[ix1] > 0):
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  *                         y_l1 += (((vl1_view[k] * bias_trace_l1_view[ix1] * (1 - d_view[k])) - (g_view[k] * y_l1)) * delta_t)             # <<<<<<<<<<<<<<
  *                         # add gaussian displacement
  *                         y_l1 += (sqrt_st * gaussian_values[m]) * bias_trace_l1_view[ix1]
  */
             __pyx_t_24 = __pyx_v_k;
             __pyx_t_20 = __pyx_v_ix1;
             __pyx_t_19 = __pyx_v_k;
             __pyx_t_26 = __pyx_v_k;
             __pyx_v_y_l1 = (__pyx_v_y_l1 + (((((*((float *) ( /* dim=0 */ (__pyx_v_vl1_view.data + __pyx_t_24 * __pyx_v_vl1_view.strides[0]) ))) * (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_20 * __pyx_v_bias_trace_l1_view.strides[0]) )))) * (1.0 - (*((float *) ( /* dim=0 */ (__pyx_v_d_view.data + __pyx_t_19 * __pyx_v_d_view.strides[0]) ))))) - ((*((float *) ( /* dim=0 */ (__pyx_v_g_view.data + __pyx_t_26 * __pyx_v_g_view.strides[0]) ))) * __pyx_v_y_l1)) * __pyx_v_delta_t));
 
-            /* "cssm.pyx":3487
+            /* "cssm.pyx":3702
  *                         y_l1 += (((vl1_view[k] * bias_trace_l1_view[ix1] * (1 - d_view[k])) - (g_view[k] * y_l1)) * delta_t)
  *                         # add gaussian displacement
  *                         y_l1 += (sqrt_st * gaussian_values[m]) * bias_trace_l1_view[ix1]             # <<<<<<<<<<<<<<
  *                     else:
  *                         # main propagation if bias_trace is not between 0 and 1 (high level choice is already made)
  */
             __pyx_t_26 = __pyx_v_m;
             __pyx_t_19 = __pyx_v_ix1;
             __pyx_v_y_l1 = (__pyx_v_y_l1 + ((__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_26 * __pyx_v_gaussian_values.strides[0]) )))) * (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l1_view.data + __pyx_t_19 * __pyx_v_bias_trace_l1_view.strides[0]) )))));
 
-            /* "cssm.pyx":3483
+            /* "cssm.pyx":3698
  *             if (choices_view[n, k, 0] == 0) | ((n == 0) & (k == 0)):
  *                 while (y_l1 >= ((-1) * boundary_view[ix1])) and (y_l1 <= boundary_view[ix1]) and (t_l1 <= deadline_tmp):
  *                     if (bias_trace_l1_view[ix1] < boundary_view[ix1]) and (bias_trace_l1_view[ix1] > 0):             # <<<<<<<<<<<<<<
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  *                         y_l1 += (((vl1_view[k] * bias_trace_l1_view[ix1] * (1 - d_view[k])) - (g_view[k] * y_l1)) * delta_t)
  */
             goto __pyx_L35;
           }
 
-          /* "cssm.pyx":3490
+          /* "cssm.pyx":3705
  *                     else:
  *                         # main propagation if bias_trace is not between 0 and 1 (high level choice is already made)
  *                         y_l1 += (vl1_view[k] * delta_t)             # <<<<<<<<<<<<<<
  *                         # add gaussian displacement
  *                         y_l1 += (sqrt_st * gaussian_values[m])
  */
           /*else*/ {
             __pyx_t_19 = __pyx_v_k;
             __pyx_v_y_l1 = (__pyx_v_y_l1 + ((*((float *) ( /* dim=0 */ (__pyx_v_vl1_view.data + __pyx_t_19 * __pyx_v_vl1_view.strides[0]) ))) * __pyx_v_delta_t));
 
-            /* "cssm.pyx":3492
+            /* "cssm.pyx":3707
  *                         y_l1 += (vl1_view[k] * delta_t)
  *                         # add gaussian displacement
  *                         y_l1 += (sqrt_st * gaussian_values[m])             # <<<<<<<<<<<<<<
  * 
  *                     # propagate time and indices
  */
             __pyx_t_19 = __pyx_v_m;
             __pyx_v_y_l1 = (__pyx_v_y_l1 + (__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_19 * __pyx_v_gaussian_values.strides[0]) )))));
           }
           __pyx_L35:;
 
-          /* "cssm.pyx":3495
+          /* "cssm.pyx":3710
  * 
  *                     # propagate time and indices
  *                     t_l1 += delta_t             # <<<<<<<<<<<<<<
  *                     ix1 += 1
  *                     m += 1
  */
           __pyx_v_t_l1 = (__pyx_v_t_l1 + __pyx_v_delta_t);
 
-          /* "cssm.pyx":3496
+          /* "cssm.pyx":3711
  *                     # propagate time and indices
  *                     t_l1 += delta_t
  *                     ix1 += 1             # <<<<<<<<<<<<<<
  *                     m += 1
  *                     if m == num_draws:
  */
           __pyx_v_ix1 = (__pyx_v_ix1 + 1);
 
-          /* "cssm.pyx":3497
+          /* "cssm.pyx":3712
  *                     t_l1 += delta_t
  *                     ix1 += 1
  *                     m += 1             # <<<<<<<<<<<<<<
  *                     if m == num_draws:
  *                         gaussian_values = draw_gaussian(num_draws)
  */
           __pyx_v_m = (__pyx_v_m + 1);
 
-          /* "cssm.pyx":3498
+          /* "cssm.pyx":3713
  *                     ix1 += 1
  *                     m += 1
  *                     if m == num_draws:             # <<<<<<<<<<<<<<
  *                         gaussian_values = draw_gaussian(num_draws)
  *                         m = 0
  */
           __pyx_t_18 = (__pyx_v_m == __pyx_v_num_draws);
           if (__pyx_t_18) {
 
-            /* "cssm.pyx":3499
+            /* "cssm.pyx":3714
  *                     m += 1
  *                     if m == num_draws:
  *                         gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  *                         m = 0
  * 
  */
-            __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3499, __pyx_L1_error)
+            __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3714, __pyx_L1_error)
             __PYX_XCLEAR_MEMVIEW(&__pyx_v_gaussian_values, 1);
             __pyx_v_gaussian_values = __pyx_t_2;
             __pyx_t_2.memview = NULL;
             __pyx_t_2.data = NULL;
 
-            /* "cssm.pyx":3500
+            /* "cssm.pyx":3715
  *                     if m == num_draws:
  *                         gaussian_values = draw_gaussian(num_draws)
  *                         m = 0             # <<<<<<<<<<<<<<
  * 
  *                     if n == 0:
  */
             __pyx_v_m = 0;
 
-            /* "cssm.pyx":3498
+            /* "cssm.pyx":3713
  *                     ix1 += 1
  *                     m += 1
  *                     if m == num_draws:             # <<<<<<<<<<<<<<
  *                         gaussian_values = draw_gaussian(num_draws)
  *                         m = 0
  */
           }
 
-          /* "cssm.pyx":3502
+          /* "cssm.pyx":3717
  *                         m = 0
  * 
  *                     if n == 0:             # <<<<<<<<<<<<<<
  *                         if k == 0:
  *                             traj_view[ix1, 1] = y_l1
  */
           __pyx_t_18 = (__pyx_v_n == 0);
           if (__pyx_t_18) {
 
-            /* "cssm.pyx":3503
+            /* "cssm.pyx":3718
  * 
  *                     if n == 0:
  *                         if k == 0:             # <<<<<<<<<<<<<<
  *                             traj_view[ix1, 1] = y_l1
  * 
  */
             __pyx_t_18 = (__pyx_v_k == 0);
             if (__pyx_t_18) {
 
-              /* "cssm.pyx":3504
+              /* "cssm.pyx":3719
  *                     if n == 0:
  *                         if k == 0:
  *                             traj_view[ix1, 1] = y_l1             # <<<<<<<<<<<<<<
  * 
  *             # lower level random walker (2)
  */
               __pyx_t_19 = __pyx_v_ix1;
               __pyx_t_26 = 1;
               *((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_traj_view.data + __pyx_t_19 * __pyx_v_traj_view.strides[0]) ) + __pyx_t_26 * __pyx_v_traj_view.strides[1]) )) = __pyx_v_y_l1;
 
-              /* "cssm.pyx":3503
+              /* "cssm.pyx":3718
  * 
  *                     if n == 0:
  *                         if k == 0:             # <<<<<<<<<<<<<<
  *                             traj_view[ix1, 1] = y_l1
  * 
  */
             }
 
-            /* "cssm.pyx":3502
+            /* "cssm.pyx":3717
  *                         m = 0
  * 
  *                     if n == 0:             # <<<<<<<<<<<<<<
  *                         if k == 0:
  *                             traj_view[ix1, 1] = y_l1
  */
           }
         }
 
-        /* "cssm.pyx":3481
+        /* "cssm.pyx":3696
  * 
  *             # lower level random walker (1)
  *             if (choices_view[n, k, 0] == 0) | ((n == 0) & (k == 0)):             # <<<<<<<<<<<<<<
  *                 while (y_l1 >= ((-1) * boundary_view[ix1])) and (y_l1 <= boundary_view[ix1]) and (t_l1 <= deadline_tmp):
  *                     if (bias_trace_l1_view[ix1] < boundary_view[ix1]) and (bias_trace_l1_view[ix1] > 0):
  */
       }
 
-      /* "cssm.pyx":3507
+      /* "cssm.pyx":3722
  * 
  *             # lower level random walker (2)
  *             if (choices_view[n, k, 0] == 2) | ((n == 0) & (k == 0)):             # <<<<<<<<<<<<<<
  *                 while (y_l2 >= ((-1) * boundary_view[ix2])) and (y_l2 <= boundary_view[ix2]) and (t_l2 <= deadline_tmp):
  *                     if (bias_trace_l2_view[ix2] < boundary_view[ix2]) and (bias_trace_l2_view[ix2] > 0):
  */
       __pyx_t_26 = __pyx_v_n;
       __pyx_t_19 = __pyx_v_k;
       __pyx_t_20 = 0;
       __pyx_t_18 = (((*((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_26 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_20 * __pyx_v_choices_view.strides[2]) ))) == 2) | ((__pyx_v_n == 0) & (__pyx_v_k == 0)));
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3508
+        /* "cssm.pyx":3723
  *             # lower level random walker (2)
  *             if (choices_view[n, k, 0] == 2) | ((n == 0) & (k == 0)):
  *                 while (y_l2 >= ((-1) * boundary_view[ix2])) and (y_l2 <= boundary_view[ix2]) and (t_l2 <= deadline_tmp):             # <<<<<<<<<<<<<<
  *                     if (bias_trace_l2_view[ix2] < boundary_view[ix2]) and (bias_trace_l2_view[ix2] > 0):
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  */
         while (1) {
@@ -66081,15 +70255,15 @@
             goto __pyx_L44_bool_binop_done;
           }
           __pyx_t_25 = (__pyx_v_t_l2 <= __pyx_v_deadline_tmp);
           __pyx_t_18 = __pyx_t_25;
           __pyx_L44_bool_binop_done:;
           if (!__pyx_t_18) break;
 
-          /* "cssm.pyx":3509
+          /* "cssm.pyx":3724
  *             if (choices_view[n, k, 0] == 2) | ((n == 0) & (k == 0)):
  *                 while (y_l2 >= ((-1) * boundary_view[ix2])) and (y_l2 <= boundary_view[ix2]) and (t_l2 <= deadline_tmp):
  *                     if (bias_trace_l2_view[ix2] < boundary_view[ix2]) and (bias_trace_l2_view[ix2] > 0):             # <<<<<<<<<<<<<<
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  *                         y_l2 += (((vl2_view[k] * bias_trace_l2_view[ix2] * (1 - d_view[k])) - (g_view[k] * y_l2)) * delta_t)
  */
           __pyx_t_20 = __pyx_v_ix2;
@@ -66102,937 +70276,937 @@
           }
           __pyx_t_19 = __pyx_v_ix2;
           __pyx_t_25 = ((*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_19 * __pyx_v_bias_trace_l2_view.strides[0]) ))) > 0.0);
           __pyx_t_18 = __pyx_t_25;
           __pyx_L48_bool_binop_done:;
           if (__pyx_t_18) {
 
-            /* "cssm.pyx":3511
+            /* "cssm.pyx":3726
  *                     if (bias_trace_l2_view[ix2] < boundary_view[ix2]) and (bias_trace_l2_view[ix2] > 0):
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  *                         y_l2 += (((vl2_view[k] * bias_trace_l2_view[ix2] * (1 - d_view[k])) - (g_view[k] * y_l2)) * delta_t)             # <<<<<<<<<<<<<<
  *                         # add gaussian displacement
  *                         y_l2 += (sqrt_st * gaussian_values[m]) * bias_trace_l2_view[ix2]
  */
             __pyx_t_19 = __pyx_v_k;
             __pyx_t_20 = __pyx_v_ix2;
             __pyx_t_26 = __pyx_v_k;
             __pyx_t_24 = __pyx_v_k;
             __pyx_v_y_l2 = (__pyx_v_y_l2 + (((((*((float *) ( /* dim=0 */ (__pyx_v_vl2_view.data + __pyx_t_19 * __pyx_v_vl2_view.strides[0]) ))) * (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_20 * __pyx_v_bias_trace_l2_view.strides[0]) )))) * (1.0 - (*((float *) ( /* dim=0 */ (__pyx_v_d_view.data + __pyx_t_26 * __pyx_v_d_view.strides[0]) ))))) - ((*((float *) ( /* dim=0 */ (__pyx_v_g_view.data + __pyx_t_24 * __pyx_v_g_view.strides[0]) ))) * __pyx_v_y_l2)) * __pyx_v_delta_t));
 
-            /* "cssm.pyx":3513
+            /* "cssm.pyx":3728
  *                         y_l2 += (((vl2_view[k] * bias_trace_l2_view[ix2] * (1 - d_view[k])) - (g_view[k] * y_l2)) * delta_t)
  *                         # add gaussian displacement
  *                         y_l2 += (sqrt_st * gaussian_values[m]) * bias_trace_l2_view[ix2]             # <<<<<<<<<<<<<<
  *                     else:
  *                         # main propagation if bias_trace is not between 0 and 1 (high level choice is already made)
  */
             __pyx_t_24 = __pyx_v_m;
             __pyx_t_26 = __pyx_v_ix2;
             __pyx_v_y_l2 = (__pyx_v_y_l2 + ((__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_24 * __pyx_v_gaussian_values.strides[0]) )))) * (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_l2_view.data + __pyx_t_26 * __pyx_v_bias_trace_l2_view.strides[0]) )))));
 
-            /* "cssm.pyx":3509
+            /* "cssm.pyx":3724
  *             if (choices_view[n, k, 0] == 2) | ((n == 0) & (k == 0)):
  *                 while (y_l2 >= ((-1) * boundary_view[ix2])) and (y_l2 <= boundary_view[ix2]) and (t_l2 <= deadline_tmp):
  *                     if (bias_trace_l2_view[ix2] < boundary_view[ix2]) and (bias_trace_l2_view[ix2] > 0):             # <<<<<<<<<<<<<<
  *                         # main propagation if bias_trace is between 0 and 1 (high level choice is not yet made)
  *                         y_l2 += (((vl2_view[k] * bias_trace_l2_view[ix2] * (1 - d_view[k])) - (g_view[k] * y_l2)) * delta_t)
  */
             goto __pyx_L47;
           }
 
-          /* "cssm.pyx":3516
+          /* "cssm.pyx":3731
  *                     else:
  *                         # main propagation if bias_trace is not between 0 and 1 (high level choice is already made)
  *                         y_l2 += (vl2_view[k] * delta_t)             # <<<<<<<<<<<<<<
  *                         # add gaussian displacement
  *                         y_l2 += (sqrt_st * gaussian_values[m])
  */
           /*else*/ {
             __pyx_t_26 = __pyx_v_k;
             __pyx_v_y_l2 = (__pyx_v_y_l2 + ((*((float *) ( /* dim=0 */ (__pyx_v_vl2_view.data + __pyx_t_26 * __pyx_v_vl2_view.strides[0]) ))) * __pyx_v_delta_t));
 
-            /* "cssm.pyx":3518
+            /* "cssm.pyx":3733
  *                         y_l2 += (vl2_view[k] * delta_t)
  *                         # add gaussian displacement
  *                         y_l2 += (sqrt_st * gaussian_values[m])             # <<<<<<<<<<<<<<
  * 
  *                     # propagate time and indices
  */
             __pyx_t_26 = __pyx_v_m;
             __pyx_v_y_l2 = (__pyx_v_y_l2 + (__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_26 * __pyx_v_gaussian_values.strides[0]) )))));
           }
           __pyx_L47:;
 
-          /* "cssm.pyx":3521
+          /* "cssm.pyx":3736
  * 
  *                     # propagate time and indices
  *                     t_l2 += delta_t             # <<<<<<<<<<<<<<
  *                     ix2 += 1
  *                     m += 1
  */
           __pyx_v_t_l2 = (__pyx_v_t_l2 + __pyx_v_delta_t);
 
-          /* "cssm.pyx":3522
+          /* "cssm.pyx":3737
  *                     # propagate time and indices
  *                     t_l2 += delta_t
  *                     ix2 += 1             # <<<<<<<<<<<<<<
  *                     m += 1
  *                     if m == num_draws:
  */
           __pyx_v_ix2 = (__pyx_v_ix2 + 1);
 
-          /* "cssm.pyx":3523
+          /* "cssm.pyx":3738
  *                     t_l2 += delta_t
  *                     ix2 += 1
  *                     m += 1             # <<<<<<<<<<<<<<
  *                     if m == num_draws:
  *                         gaussian_values = draw_gaussian(num_draws)
  */
           __pyx_v_m = (__pyx_v_m + 1);
 
-          /* "cssm.pyx":3524
+          /* "cssm.pyx":3739
  *                     ix2 += 1
  *                     m += 1
  *                     if m == num_draws:             # <<<<<<<<<<<<<<
  *                         gaussian_values = draw_gaussian(num_draws)
  *                         m = 0
  */
           __pyx_t_18 = (__pyx_v_m == __pyx_v_num_draws);
           if (__pyx_t_18) {
 
-            /* "cssm.pyx":3525
+            /* "cssm.pyx":3740
  *                     m += 1
  *                     if m == num_draws:
  *                         gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  *                         m = 0
  * 
  */
-            __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3525, __pyx_L1_error)
+            __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3740, __pyx_L1_error)
             __PYX_XCLEAR_MEMVIEW(&__pyx_v_gaussian_values, 1);
             __pyx_v_gaussian_values = __pyx_t_2;
             __pyx_t_2.memview = NULL;
             __pyx_t_2.data = NULL;
 
-            /* "cssm.pyx":3526
+            /* "cssm.pyx":3741
  *                     if m == num_draws:
  *                         gaussian_values = draw_gaussian(num_draws)
  *                         m = 0             # <<<<<<<<<<<<<<
  * 
  *                     if n == 0:
  */
             __pyx_v_m = 0;
 
-            /* "cssm.pyx":3524
+            /* "cssm.pyx":3739
  *                     ix2 += 1
  *                     m += 1
  *                     if m == num_draws:             # <<<<<<<<<<<<<<
  *                         gaussian_values = draw_gaussian(num_draws)
  *                         m = 0
  */
           }
 
-          /* "cssm.pyx":3528
+          /* "cssm.pyx":3743
  *                         m = 0
  * 
  *                     if n == 0:             # <<<<<<<<<<<<<<
  *                         if k == 0:
  *                             traj_view[ix2, 2] = y_l2
  */
           __pyx_t_18 = (__pyx_v_n == 0);
           if (__pyx_t_18) {
 
-            /* "cssm.pyx":3529
+            /* "cssm.pyx":3744
  * 
  *                     if n == 0:
  *                         if k == 0:             # <<<<<<<<<<<<<<
  *                             traj_view[ix2, 2] = y_l2
  * 
  */
             __pyx_t_18 = (__pyx_v_k == 0);
             if (__pyx_t_18) {
 
-              /* "cssm.pyx":3530
+              /* "cssm.pyx":3745
  *                     if n == 0:
  *                         if k == 0:
  *                             traj_view[ix2, 2] = y_l2             # <<<<<<<<<<<<<<
  * 
  *             # Get back to single y_l and t_l
  */
               __pyx_t_26 = __pyx_v_ix2;
               __pyx_t_24 = 2;
               *((float *) ( /* dim=1 */ (( /* dim=0 */ (__pyx_v_traj_view.data + __pyx_t_26 * __pyx_v_traj_view.strides[0]) ) + __pyx_t_24 * __pyx_v_traj_view.strides[1]) )) = __pyx_v_y_l2;
 
-              /* "cssm.pyx":3529
+              /* "cssm.pyx":3744
  * 
  *                     if n == 0:
  *                         if k == 0:             # <<<<<<<<<<<<<<
  *                             traj_view[ix2, 2] = y_l2
  * 
  */
             }
 
-            /* "cssm.pyx":3528
+            /* "cssm.pyx":3743
  *                         m = 0
  * 
  *                     if n == 0:             # <<<<<<<<<<<<<<
  *                         if k == 0:
  *                             traj_view[ix2, 2] = y_l2
  */
           }
         }
 
-        /* "cssm.pyx":3507
+        /* "cssm.pyx":3722
  * 
  *             # lower level random walker (2)
  *             if (choices_view[n, k, 0] == 2) | ((n == 0) & (k == 0)):             # <<<<<<<<<<<<<<
  *                 while (y_l2 >= ((-1) * boundary_view[ix2])) and (y_l2 <= boundary_view[ix2]) and (t_l2 <= deadline_tmp):
  *                     if (bias_trace_l2_view[ix2] < boundary_view[ix2]) and (bias_trace_l2_view[ix2] > 0):
  */
       }
 
-      /* "cssm.pyx":3533
+      /* "cssm.pyx":3748
  * 
  *             # Get back to single y_l and t_l
  *             if (choices_view[n, k, 0] == 0):             # <<<<<<<<<<<<<<
  *                 t_l = t_l1
  *                 y_l = y_l1
  */
       __pyx_t_24 = __pyx_v_n;
       __pyx_t_26 = __pyx_v_k;
       __pyx_t_20 = 0;
       __pyx_t_18 = ((*((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_24 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_26 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_20 * __pyx_v_choices_view.strides[2]) ))) == 0);
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3534
+        /* "cssm.pyx":3749
  *             # Get back to single y_l and t_l
  *             if (choices_view[n, k, 0] == 0):
  *                 t_l = t_l1             # <<<<<<<<<<<<<<
  *                 y_l = y_l1
  *                 ix_l = ix1
  */
         __pyx_v_t_l = __pyx_v_t_l1;
 
-        /* "cssm.pyx":3535
+        /* "cssm.pyx":3750
  *             if (choices_view[n, k, 0] == 0):
  *                 t_l = t_l1
  *                 y_l = y_l1             # <<<<<<<<<<<<<<
  *                 ix_l = ix1
  *             else:
  */
         __pyx_v_y_l = __pyx_v_y_l1;
 
-        /* "cssm.pyx":3536
+        /* "cssm.pyx":3751
  *                 t_l = t_l1
  *                 y_l = y_l1
  *                 ix_l = ix1             # <<<<<<<<<<<<<<
  *             else:
  *                 t_l = t_l2
  */
         __pyx_v_ix_l = __pyx_v_ix1;
 
-        /* "cssm.pyx":3533
+        /* "cssm.pyx":3748
  * 
  *             # Get back to single y_l and t_l
  *             if (choices_view[n, k, 0] == 0):             # <<<<<<<<<<<<<<
  *                 t_l = t_l1
  *                 y_l = y_l1
  */
         goto __pyx_L53;
       }
 
-      /* "cssm.pyx":3538
+      /* "cssm.pyx":3753
  *                 ix_l = ix1
  *             else:
  *                 t_l = t_l2             # <<<<<<<<<<<<<<
  *                 y_l = y_l2
  *                 ix_l = ix2
  */
       /*else*/ {
         __pyx_v_t_l = __pyx_v_t_l2;
 
-        /* "cssm.pyx":3539
+        /* "cssm.pyx":3754
  *             else:
  *                 t_l = t_l2
  *                 y_l = y_l2             # <<<<<<<<<<<<<<
  *                 ix_l = ix2
  * 
  */
         __pyx_v_y_l = __pyx_v_y_l2;
 
-        /* "cssm.pyx":3540
+        /* "cssm.pyx":3755
  *                 t_l = t_l2
  *                 y_l = y_l2
  *                 ix_l = ix2             # <<<<<<<<<<<<<<
  * 
  *             if smooth:
  */
         __pyx_v_ix_l = __pyx_v_ix2;
       }
       __pyx_L53:;
 
-      /* "cssm.pyx":3542
+      /* "cssm.pyx":3757
  *                 ix_l = ix2
  * 
  *             if smooth:             # <<<<<<<<<<<<<<
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  */
-      __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_smooth); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3542, __pyx_L1_error)
+      __pyx_t_18 = __Pyx_PyObject_IsTrue(__pyx_v_smooth); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3757, __pyx_L1_error)
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3543
+        /* "cssm.pyx":3758
  * 
  *             if smooth:
  *                 if t_h == 0.0:             # <<<<<<<<<<<<<<
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  */
         __pyx_t_18 = (__pyx_v_t_h == 0.0);
         if (__pyx_t_18) {
 
-          /* "cssm.pyx":3544
+          /* "cssm.pyx":3759
  *             if smooth:
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t             # <<<<<<<<<<<<<<
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  */
-          __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3544, __pyx_L1_error)
+          __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3759, __pyx_L1_error)
           __pyx_v_smooth_u = ((__pyx_t_23 * 0.5) * __pyx_v_delta_t);
 
-          /* "cssm.pyx":3543
+          /* "cssm.pyx":3758
  * 
  *             if smooth:
  *                 if t_h == 0.0:             # <<<<<<<<<<<<<<
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  */
           goto __pyx_L55;
         }
 
-        /* "cssm.pyx":3545
+        /* "cssm.pyx":3760
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:             # <<<<<<<<<<<<<<
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  *                 else:
  */
         __pyx_t_18 = (fmax(__pyx_v_t_h, __pyx_v_t_l) < __pyx_v_deadline_tmp);
         if (__pyx_t_18) {
 
-          /* "cssm.pyx":3546
+          /* "cssm.pyx":3761
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  *                     smooth_u = (0.5 - random_uniform()) * delta_t             # <<<<<<<<<<<<<<
  *                 else:
  *                     smooth_u = 0.0
  */
-          __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3546, __pyx_L1_error)
+          __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3761, __pyx_L1_error)
           __pyx_v_smooth_u = ((0.5 - __pyx_t_23) * __pyx_v_delta_t);
 
-          /* "cssm.pyx":3545
+          /* "cssm.pyx":3760
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:             # <<<<<<<<<<<<<<
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  *                 else:
  */
           goto __pyx_L55;
         }
 
-        /* "cssm.pyx":3548
+        /* "cssm.pyx":3763
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  *                 else:
  *                     smooth_u = 0.0             # <<<<<<<<<<<<<<
  *             else:
  *                 smooth_u = 0.0
  */
         /*else*/ {
           __pyx_v_smooth_u = 0.0;
         }
         __pyx_L55:;
 
-        /* "cssm.pyx":3542
+        /* "cssm.pyx":3757
  *                 ix_l = ix2
  * 
  *             if smooth:             # <<<<<<<<<<<<<<
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  */
         goto __pyx_L54;
       }
 
-      /* "cssm.pyx":3550
+      /* "cssm.pyx":3765
  *                     smooth_u = 0.0
  *             else:
  *                 smooth_u = 0.0             # <<<<<<<<<<<<<<
  * 
  *             rts_view[n, k, 0] = fmax(t_h, t_l) + t_view[k]
  */
       /*else*/ {
         __pyx_v_smooth_u = 0.0;
       }
       __pyx_L54:;
 
-      /* "cssm.pyx":3552
+      /* "cssm.pyx":3767
  *                 smooth_u = 0.0
  * 
  *             rts_view[n, k, 0] = fmax(t_h, t_l) + t_view[k]             # <<<<<<<<<<<<<<
  *             rts_high_view[n, k, 0] = t_h + t_view[k]
  *             rts_low_view[n, k, 0] = t_l + t_view[k]
  */
       __pyx_t_20 = __pyx_v_k;
       __pyx_t_26 = __pyx_v_n;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_19 = 0;
       *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_26 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_24 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[2]) )) = (fmax(__pyx_v_t_h, __pyx_v_t_l) + (*((float *) ( /* dim=0 */ (__pyx_v_t_view.data + __pyx_t_20 * __pyx_v_t_view.strides[0]) ))));
 
-      /* "cssm.pyx":3553
+      /* "cssm.pyx":3768
  * 
  *             rts_view[n, k, 0] = fmax(t_h, t_l) + t_view[k]
  *             rts_high_view[n, k, 0] = t_h + t_view[k]             # <<<<<<<<<<<<<<
  *             rts_low_view[n, k, 0] = t_l + t_view[k]
  * 
  */
       __pyx_t_20 = __pyx_v_k;
       __pyx_t_19 = __pyx_v_n;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_26 = 0;
       *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_high_view.data + __pyx_t_19 * __pyx_v_rts_high_view.strides[0]) ) + __pyx_t_24 * __pyx_v_rts_high_view.strides[1]) ) + __pyx_t_26 * __pyx_v_rts_high_view.strides[2]) )) = (__pyx_v_t_h + (*((float *) ( /* dim=0 */ (__pyx_v_t_view.data + __pyx_t_20 * __pyx_v_t_view.strides[0]) ))));
 
-      /* "cssm.pyx":3554
+      /* "cssm.pyx":3769
  *             rts_view[n, k, 0] = fmax(t_h, t_l) + t_view[k]
  *             rts_high_view[n, k, 0] = t_h + t_view[k]
  *             rts_low_view[n, k, 0] = t_l + t_view[k]             # <<<<<<<<<<<<<<
  * 
  *             # The probability of making a 'mistake' 1 - (relative y position)
  */
       __pyx_t_20 = __pyx_v_k;
       __pyx_t_26 = __pyx_v_n;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_19 = 0;
       *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_low_view.data + __pyx_t_26 * __pyx_v_rts_low_view.strides[0]) ) + __pyx_t_24 * __pyx_v_rts_low_view.strides[1]) ) + __pyx_t_19 * __pyx_v_rts_low_view.strides[2]) )) = (__pyx_v_t_l + (*((float *) ( /* dim=0 */ (__pyx_v_t_view.data + __pyx_t_20 * __pyx_v_t_view.strides[0]) ))));
 
-      /* "cssm.pyx":3561
+      /* "cssm.pyx":3776
  * 
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
  *                 if random_uniform() <= 0.5:
  *                     choices_view[n, k, 0] += 1
  */
       __pyx_t_20 = __pyx_v_ix;
       __pyx_t_18 = ((*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_20 * __pyx_v_boundary_view.strides[0]) ))) <= 0.0);
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3562
+        /* "cssm.pyx":3777
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:
  *                 if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
  *                     choices_view[n, k, 0] += 1
  *             # Otherwise apply rule from above
  */
-        __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3562, __pyx_L1_error)
+        __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3777, __pyx_L1_error)
         __pyx_t_18 = (__pyx_t_23 <= 0.5);
         if (__pyx_t_18) {
 
-          /* "cssm.pyx":3563
+          /* "cssm.pyx":3778
  *             if boundary_view[ix] <= 0:
  *                 if random_uniform() <= 0.5:
  *                     choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
  *             # Otherwise apply rule from above
  *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
  */
           __pyx_t_20 = __pyx_v_n;
           __pyx_t_19 = __pyx_v_k;
           __pyx_t_24 = 0;
           *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_20 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[2]) )) += 1;
 
-          /* "cssm.pyx":3562
+          /* "cssm.pyx":3777
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:
  *                 if random_uniform() <= 0.5:             # <<<<<<<<<<<<<<
  *                     choices_view[n, k, 0] += 1
  *             # Otherwise apply rule from above
  */
         }
 
-        /* "cssm.pyx":3561
+        /* "cssm.pyx":3776
  * 
  *             # If boundary is negative (or 0) already, we flip a coin
  *             if boundary_view[ix] <= 0:             # <<<<<<<<<<<<<<
  *                 if random_uniform() <= 0.5:
  *                     choices_view[n, k, 0] += 1
  */
         goto __pyx_L56;
       }
 
-      /* "cssm.pyx":3565
+      /* "cssm.pyx":3780
  *                     choices_view[n, k, 0] += 1
  *             # Otherwise apply rule from above
  *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 1
  * 
  */
-      __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3565, __pyx_L1_error)
+      __pyx_t_23 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_23 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3780, __pyx_L1_error)
       __pyx_t_24 = __pyx_v_ix;
       __pyx_t_19 = __pyx_v_ix;
       __pyx_t_18 = (__pyx_t_23 <= ((__pyx_v_y_l + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_24 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) ))))));
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3566
+        /* "cssm.pyx":3781
  *             # Otherwise apply rule from above
  *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
  *                 choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):
  */
         __pyx_t_19 = __pyx_v_n;
         __pyx_t_24 = __pyx_v_k;
         __pyx_t_20 = 0;
         *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_19 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_24 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_20 * __pyx_v_choices_view.strides[2]) )) += 1;
 
-        /* "cssm.pyx":3565
+        /* "cssm.pyx":3780
  *                     choices_view[n, k, 0] += 1
  *             # Otherwise apply rule from above
  *             elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 1
  * 
  */
       }
       __pyx_L56:;
 
-      /* "cssm.pyx":3568
+      /* "cssm.pyx":3783
  *                 choices_view[n, k, 0] += 1
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):             # <<<<<<<<<<<<<<
  *                 rts_view[n, k, 0] = -999
  * 
  */
       __pyx_t_20 = __pyx_v_n;
       __pyx_t_24 = __pyx_v_k;
       __pyx_t_19 = 0;
       __pyx_t_26 = __pyx_v_k;
       __pyx_t_27 = __pyx_v_k;
       __pyx_t_18 = (((*((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_20 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_24 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[2]) ))) >= (*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_26 * __pyx_v_deadline_view.strides[0]) )))) | ((*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_27 * __pyx_v_deadline_view.strides[0]) ))) <= 0.0));
       if (__pyx_t_18) {
 
-        /* "cssm.pyx":3569
+        /* "cssm.pyx":3784
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):
  *                 rts_view[n, k, 0] = -999             # <<<<<<<<<<<<<<
  * 
  *     if return_option == 'full':
  */
         __pyx_t_27 = __pyx_v_n;
         __pyx_t_26 = __pyx_v_k;
         __pyx_t_19 = 0;
         *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_27 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_26 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[2]) )) = -999.0;
 
-        /* "cssm.pyx":3568
+        /* "cssm.pyx":3783
  *                 choices_view[n, k, 0] += 1
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):             # <<<<<<<<<<<<<<
  *                 rts_view[n, k, 0] = -999
  * 
  */
       }
     }
   }
 
-  /* "cssm.pyx":3571
+  /* "cssm.pyx":3786
  *                 rts_view[n, k, 0] = -999
  * 
  *     if return_option == 'full':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'vh': vh,
  */
-  __pyx_t_18 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_full, Py_EQ)); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3571, __pyx_L1_error)
+  __pyx_t_18 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_full, Py_EQ)); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3786, __pyx_L1_error)
   if (__pyx_t_18) {
 
-    /* "cssm.pyx":3572
+    /* "cssm.pyx":3787
  * 
  *     if return_option == 'full':
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,             # <<<<<<<<<<<<<<
  *                 'metadata': {'vh': vh,
  *                             'vl1': vl1,
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3572, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3787, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3572, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3572, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_high, __pyx_v_rts_high) < 0) __PYX_ERR(0, 3572, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_low, __pyx_v_rts_low) < 0) __PYX_ERR(0, 3572, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3787, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3787, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_high, __pyx_v_rts_high) < 0) __PYX_ERR(0, 3787, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_low, __pyx_v_rts_low) < 0) __PYX_ERR(0, 3787, __pyx_L1_error)
 
-    /* "cssm.pyx":3573
+    /* "cssm.pyx":3788
  *     if return_option == 'full':
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'vh': vh,             # <<<<<<<<<<<<<<
  *                             'vl1': vl1,
  *                             'vl2': vl2,
  */
-    __pyx_t_6 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3573, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3788, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_vh, ((PyObject *)__pyx_v_vh)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_vh, ((PyObject *)__pyx_v_vh)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3574
+    /* "cssm.pyx":3789
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'vh': vh,
  *                             'vl1': vl1,             # <<<<<<<<<<<<<<
  *                             'vl2': vl2,
  *                             'a': a,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_vl1, ((PyObject *)__pyx_v_vl1)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_vl1, ((PyObject *)__pyx_v_vl1)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3575
+    /* "cssm.pyx":3790
  *                 'metadata': {'vh': vh,
  *                             'vl1': vl1,
  *                             'vl2': vl2,             # <<<<<<<<<<<<<<
  *                             'a': a,
  *                             'zh': zh,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_vl2, ((PyObject *)__pyx_v_vl2)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_vl2, ((PyObject *)__pyx_v_vl2)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3576
+    /* "cssm.pyx":3791
  *                             'vl1': vl1,
  *                             'vl2': vl2,
  *                             'a': a,             # <<<<<<<<<<<<<<
  *                             'zh': zh,
  *                             'zl1': zl1,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3577
+    /* "cssm.pyx":3792
  *                             'vl2': vl2,
  *                             'a': a,
  *                             'zh': zh,             # <<<<<<<<<<<<<<
  *                             'zl1': zl1,
  *                             'zl2': zl2,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_zh, ((PyObject *)__pyx_v_zh)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_zh, ((PyObject *)__pyx_v_zh)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3578
+    /* "cssm.pyx":3793
  *                             'a': a,
  *                             'zh': zh,
  *                             'zl1': zl1,             # <<<<<<<<<<<<<<
  *                             'zl2': zl2,
  *                             'd': d,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_zl1, ((PyObject *)__pyx_v_zl1)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_zl1, ((PyObject *)__pyx_v_zl1)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3579
+    /* "cssm.pyx":3794
  *                             'zh': zh,
  *                             'zl1': zl1,
  *                             'zl2': zl2,             # <<<<<<<<<<<<<<
  *                             'd': d,
  *                             't': t,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_zl2, ((PyObject *)__pyx_v_zl2)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_zl2, ((PyObject *)__pyx_v_zl2)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3580
+    /* "cssm.pyx":3795
  *                             'zl1': zl1,
  *                             'zl2': zl2,
  *                             'd': d,             # <<<<<<<<<<<<<<
  *                             't': t,
  *                             'deadline': deadline,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_d, ((PyObject *)__pyx_v_d)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_d, ((PyObject *)__pyx_v_d)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3581
+    /* "cssm.pyx":3796
  *                             'zl2': zl2,
  *                             'd': d,
  *                             't': t,             # <<<<<<<<<<<<<<
  *                             'deadline': deadline,
  *                             's': s,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_t, ((PyObject *)__pyx_v_t)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_t, ((PyObject *)__pyx_v_t)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3582
+    /* "cssm.pyx":3797
  *                             'd': d,
  *                             't': t,
  *                             'deadline': deadline,             # <<<<<<<<<<<<<<
  *                             's': s,
  *                             **boundary_params,
  */
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
 
-    /* "cssm.pyx":3583
+    /* "cssm.pyx":3798
  *                             't': t,
  *                             'deadline': deadline,
  *                             's': s,             # <<<<<<<<<<<<<<
  *                             **boundary_params,
  *                             'delta_t': delta_t,
  */
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_s); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3583, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_s); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3798, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_s, __pyx_t_4) < 0) __PYX_ERR(0, 3573, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_u_s, __pyx_t_4) < 0) __PYX_ERR(0, 3788, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_10 = __pyx_t_6;
     __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3584
+    /* "cssm.pyx":3799
  *                             'deadline': deadline,
  *                             's': s,
  *                             **boundary_params,             # <<<<<<<<<<<<<<
  *                             'delta_t': delta_t,
  *                             'max_t': max_t,
  */
     if (unlikely(__pyx_v_boundary_params == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 3584, __pyx_L1_error)
+      __PYX_ERR(0, 3799, __pyx_L1_error)
     }
     if (unlikely(PyDict_Update(__pyx_t_10, __pyx_v_boundary_params) < 0)) {
       if (PyErr_ExceptionMatches(PyExc_AttributeError)) __Pyx_RaiseMappingExpectedError(__pyx_v_boundary_params);
-      __PYX_ERR(0, 3584, __pyx_L1_error)
+      __PYX_ERR(0, 3799, __pyx_L1_error)
     }
 
-    /* "cssm.pyx":3585
+    /* "cssm.pyx":3800
  *                             's': s,
  *                             **boundary_params,
  *                             'delta_t': delta_t,             # <<<<<<<<<<<<<<
  *                             'max_t': max_t,
  *                             'n_samples': n_samples,
  */
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3585, __pyx_L1_error)
+    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3800, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_delta_t, __pyx_t_6) < 0) __PYX_ERR(0, 3585, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_delta_t, __pyx_t_6) < 0) __PYX_ERR(0, 3800, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3586
+    /* "cssm.pyx":3801
  *                             **boundary_params,
  *                             'delta_t': delta_t,
  *                             'max_t': max_t,             # <<<<<<<<<<<<<<
  *                             'n_samples': n_samples,
  *                             'n_trials': n_trials,
  */
-    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3586, __pyx_L1_error)
+    __pyx_t_6 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3801, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max_t, __pyx_t_6) < 0) __PYX_ERR(0, 3586, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_max_t, __pyx_t_6) < 0) __PYX_ERR(0, 3801, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3587
+    /* "cssm.pyx":3802
  *                             'delta_t': delta_t,
  *                             'max_t': max_t,
  *                             'n_samples': n_samples,             # <<<<<<<<<<<<<<
  *                             'n_trials': n_trials,
  *                             'simulator': 'ddm_flexbound_mic2_adj',
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3587, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3802, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_samples, __pyx_t_6) < 0) __PYX_ERR(0, 3587, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_samples, __pyx_t_6) < 0) __PYX_ERR(0, 3802, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3588
+    /* "cssm.pyx":3803
  *                             'max_t': max_t,
  *                             'n_samples': n_samples,
  *                             'n_trials': n_trials,             # <<<<<<<<<<<<<<
  *                             'simulator': 'ddm_flexbound_mic2_adj',
  *                             'boundary_fun_type': boundary_fun.__name__,
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3588, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3803, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_trials, __pyx_t_6) < 0) __PYX_ERR(0, 3588, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_trials, __pyx_t_6) < 0) __PYX_ERR(0, 3803, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 3589, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 3804, __pyx_L1_error)
 
-    /* "cssm.pyx":3590
+    /* "cssm.pyx":3805
  *                             'n_trials': n_trials,
  *                             'simulator': 'ddm_flexbound_mic2_adj',
  *                             'boundary_fun_type': boundary_fun.__name__,             # <<<<<<<<<<<<<<
  *                             'possible_choices': [0, 1, 2, 3],
  *                             'trajectory': traj,
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3590, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3805, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_boundary_fun_type, __pyx_t_6) < 0) __PYX_ERR(0, 3590, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_boundary_fun_type, __pyx_t_6) < 0) __PYX_ERR(0, 3805, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3591
+    /* "cssm.pyx":3806
  *                             'simulator': 'ddm_flexbound_mic2_adj',
  *                             'boundary_fun_type': boundary_fun.__name__,
  *                             'possible_choices': [0, 1, 2, 3],             # <<<<<<<<<<<<<<
  *                             'trajectory': traj,
  *                             'boundary': boundary}}
  */
-    __pyx_t_6 = PyList_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3591, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3806, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_int_0)) __PYX_ERR(0, 3591, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_int_0)) __PYX_ERR(0, 3806, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 1, __pyx_int_1)) __PYX_ERR(0, 3591, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 1, __pyx_int_1)) __PYX_ERR(0, 3806, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 2, __pyx_int_2)) __PYX_ERR(0, 3591, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 2, __pyx_int_2)) __PYX_ERR(0, 3806, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 3, __pyx_int_3)) __PYX_ERR(0, 3591, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_possible_choices, __pyx_t_6) < 0) __PYX_ERR(0, 3591, __pyx_L1_error)
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 3, __pyx_int_3)) __PYX_ERR(0, 3806, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_possible_choices, __pyx_t_6) < 0) __PYX_ERR(0, 3806, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3592
+    /* "cssm.pyx":3807
  *                             'boundary_fun_type': boundary_fun.__name__,
  *                             'possible_choices': [0, 1, 2, 3],
  *                             'trajectory': traj,             # <<<<<<<<<<<<<<
  *                             'boundary': boundary}}
  *     elif return_option == 'minimal':
  */
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_trajectory, __pyx_v_traj) < 0) __PYX_ERR(0, 3592, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_trajectory, __pyx_v_traj) < 0) __PYX_ERR(0, 3807, __pyx_L1_error)
 
-    /* "cssm.pyx":3593
+    /* "cssm.pyx":3808
  *                             'possible_choices': [0, 1, 2, 3],
  *                             'trajectory': traj,
  *                             'boundary': boundary}}             # <<<<<<<<<<<<<<
  *     elif return_option == 'minimal':
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  */
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_boundary, __pyx_v_boundary) < 0) __PYX_ERR(0, 3593, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_10) < 0) __PYX_ERR(0, 3572, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_boundary, __pyx_v_boundary) < 0) __PYX_ERR(0, 3808, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_10) < 0) __PYX_ERR(0, 3787, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "cssm.pyx":3571
+    /* "cssm.pyx":3786
  *                 rts_view[n, k, 0] = -999
  * 
  *     if return_option == 'full':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'vh': vh,
  */
   }
 
-  /* "cssm.pyx":3594
+  /* "cssm.pyx":3809
  *                             'trajectory': traj,
  *                             'boundary': boundary}}
  *     elif return_option == 'minimal':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  */
-  __pyx_t_18 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_minimal, Py_EQ)); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3594, __pyx_L1_error)
+  __pyx_t_18 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_minimal, Py_EQ)); if (unlikely((__pyx_t_18 < 0))) __PYX_ERR(0, 3809, __pyx_L1_error)
   if (likely(__pyx_t_18)) {
 
-    /* "cssm.pyx":3595
+    /* "cssm.pyx":3810
  *                             'boundary': boundary}}
  *     elif return_option == 'minimal':
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,             # <<<<<<<<<<<<<<
  *                 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                              'possible_choices': [0, 1, 2, 3],
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3595, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3810, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3595, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3595, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_high, __pyx_v_rts_high) < 0) __PYX_ERR(0, 3595, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_low, __pyx_v_rts_low) < 0) __PYX_ERR(0, 3595, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 3810, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 3810, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_high, __pyx_v_rts_high) < 0) __PYX_ERR(0, 3810, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts_low, __pyx_v_rts_low) < 0) __PYX_ERR(0, 3810, __pyx_L1_error)
 
-    /* "cssm.pyx":3596
+    /* "cssm.pyx":3811
  *     elif return_option == 'minimal':
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',             # <<<<<<<<<<<<<<
  *                              'possible_choices': [0, 1, 2, 3],
  *                              'boundary_fun_type': boundary_fun.__name__,
  */
-    __pyx_t_10 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3596, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3811, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 3596, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 3811, __pyx_L1_error)
 
-    /* "cssm.pyx":3597
+    /* "cssm.pyx":3812
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                              'possible_choices': [0, 1, 2, 3],             # <<<<<<<<<<<<<<
  *                              'boundary_fun_type': boundary_fun.__name__,
  *                              'n_samples': n_samples,
  */
-    __pyx_t_6 = PyList_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3597, __pyx_L1_error)
+    __pyx_t_6 = PyList_New(4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3812, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_int_0)) __PYX_ERR(0, 3597, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 0, __pyx_int_0)) __PYX_ERR(0, 3812, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 1, __pyx_int_1)) __PYX_ERR(0, 3597, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 1, __pyx_int_1)) __PYX_ERR(0, 3812, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 2, __pyx_int_2)) __PYX_ERR(0, 3597, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 2, __pyx_int_2)) __PYX_ERR(0, 3812, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 3, __pyx_int_3)) __PYX_ERR(0, 3597, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_possible_choices, __pyx_t_6) < 0) __PYX_ERR(0, 3596, __pyx_L1_error)
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_6, 3, __pyx_int_3)) __PYX_ERR(0, 3812, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_possible_choices, __pyx_t_6) < 0) __PYX_ERR(0, 3811, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3598
+    /* "cssm.pyx":3813
  *                 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                              'possible_choices': [0, 1, 2, 3],
  *                              'boundary_fun_type': boundary_fun.__name__,             # <<<<<<<<<<<<<<
  *                              'n_samples': n_samples,
  *                              'n_trials': n_trials,
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3598, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3813, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_boundary_fun_type, __pyx_t_6) < 0) __PYX_ERR(0, 3596, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_boundary_fun_type, __pyx_t_6) < 0) __PYX_ERR(0, 3811, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3599
+    /* "cssm.pyx":3814
  *                              'possible_choices': [0, 1, 2, 3],
  *                              'boundary_fun_type': boundary_fun.__name__,
  *                              'n_samples': n_samples,             # <<<<<<<<<<<<<<
  *                              'n_trials': n_trials,
  *                              }}
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3599, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3814, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_samples, __pyx_t_6) < 0) __PYX_ERR(0, 3596, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_samples, __pyx_t_6) < 0) __PYX_ERR(0, 3811, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "cssm.pyx":3600
+    /* "cssm.pyx":3815
  *                              'boundary_fun_type': boundary_fun.__name__,
  *                              'n_samples': n_samples,
  *                              'n_trials': n_trials,             # <<<<<<<<<<<<<<
  *                              }}
  *     else:
  */
-    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3600, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3815, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_trials, __pyx_t_6) < 0) __PYX_ERR(0, 3596, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_10, __pyx_n_u_n_trials, __pyx_t_6) < 0) __PYX_ERR(0, 3811, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_10) < 0) __PYX_ERR(0, 3595, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_10) < 0) __PYX_ERR(0, 3810, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "cssm.pyx":3594
+    /* "cssm.pyx":3809
  *                             'trajectory': traj,
  *                             'boundary': boundary}}
  *     elif return_option == 'minimal':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'rts_high': rts_high, 'rts_low': rts_low,
  *                 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  */
   }
 
-  /* "cssm.pyx":3603
+  /* "cssm.pyx":3818
  *                              }}
  *     else:
  *         raise ValueError('return_option must be either "full" or "minimal"')             # <<<<<<<<<<<<<<
  * # ----------------------------------------------------------------------------------------------------
  * 
  */
   /*else*/ {
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3603, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3818, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 3603, __pyx_L1_error)
+    __PYX_ERR(0, 3818, __pyx_L1_error)
   }
 
-  /* "cssm.pyx":3328
+  /* "cssm.pyx":3543
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                                         np.ndarray[float, ndim = 1] vl1,
  *                                                         np.ndarray[float, ndim = 1] vl2,
  */
 
@@ -67112,139 +71286,139 @@
   __Pyx_XDECREF(__pyx_v_boundary_params_tmp);
   __Pyx_XDECREF(__pyx_9genexpr14__pyx_v_key);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "cssm.pyx":3839
+/* "cssm.pyx":4054
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_tradeoff(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                            np.ndarray[float, ndim = 1] vl1,
  *                            np.ndarray[float, ndim = 1] vl2,
  */
 
-static PyObject *__pyx_pf_4cssm_66__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_4cssm_72__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__defaults__", 1);
   __Pyx_XDECREF(__pyx_r);
 
-  /* "cssm.pyx":3849
+  /* "cssm.pyx":4064
  *                            np.ndarray[float, ndim = 1] t,
  *                            np.ndarray[float, ndim = 1] deadline,
  *                            float s = 1,             # <<<<<<<<<<<<<<
  *                            float delta_t = 0.001,
  *                            float max_t = 20,
  */
-  __pyx_t_1 = PyFloat_FromDouble(((float)1.0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3849, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(((float)1.0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4064, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "cssm.pyx":3850
+  /* "cssm.pyx":4065
  *                            np.ndarray[float, ndim = 1] deadline,
  *                            float s = 1,
  *                            float delta_t = 0.001,             # <<<<<<<<<<<<<<
  *                            float max_t = 20,
  *                            int n_samples = 20000,
  */
-  __pyx_t_2 = PyFloat_FromDouble(((double)0.001)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 3850, __pyx_L1_error)
+  __pyx_t_2 = PyFloat_FromDouble(((double)0.001)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 4065, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "cssm.pyx":3851
+  /* "cssm.pyx":4066
  *                            float s = 1,
  *                            float delta_t = 0.001,
  *                            float max_t = 20,             # <<<<<<<<<<<<<<
  *                            int n_samples = 20000,
  *                            int n_trials = 1,
  */
-  __pyx_t_3 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3851, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4066, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "cssm.pyx":3852
+  /* "cssm.pyx":4067
  *                            float delta_t = 0.001,
  *                            float max_t = 20,
  *                            int n_samples = 20000,             # <<<<<<<<<<<<<<
  *                            int n_trials = 1,
  *                            print_info = True,
  */
-  __pyx_t_4 = __Pyx_PyInt_From_int(((int)0x4E20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3852, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(((int)0x4E20)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4067, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
 
-  /* "cssm.pyx":3853
+  /* "cssm.pyx":4068
  *                            float max_t = 20,
  *                            int n_samples = 20000,
  *                            int n_trials = 1,             # <<<<<<<<<<<<<<
  *                            print_info = True,
  *                            boundary_fun = None, # function of t (and potentially other parameters) that takes in (t, *args)
  */
-  __pyx_t_5 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3853, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4068, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "cssm.pyx":3839
+  /* "cssm.pyx":4054
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_tradeoff(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                            np.ndarray[float, ndim = 1] vl1,
  *                            np.ndarray[float, ndim = 1] vl2,
  */
-  __pyx_t_6 = PyTuple_New(12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3839, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(12); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_t_1)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_2)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_3)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_t_3)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_4)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 3, __pyx_t_4)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_t_5)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 4, __pyx_t_5)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_True));
   __Pyx_GIVEREF(((PyObject *)Py_True));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, ((PyObject *)Py_True))) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 5, ((PyObject *)Py_True))) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 6, Py_None)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 6, Py_None)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_True));
   __Pyx_GIVEREF(((PyObject *)Py_True));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 7, ((PyObject *)Py_True))) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 7, ((PyObject *)Py_True))) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(__Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_self)->__pyx_arg_boundary_params);
   __Pyx_GIVEREF(__Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_self)->__pyx_arg_boundary_params);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 8, __Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_self)->__pyx_arg_boundary_params)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 8, __Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_self)->__pyx_arg_boundary_params)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 9, Py_None)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 9, Py_None)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(((PyObject*)__pyx_n_u_full));
   __Pyx_GIVEREF(((PyObject*)__pyx_n_u_full));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 10, ((PyObject*)__pyx_n_u_full))) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 10, ((PyObject*)__pyx_n_u_full))) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(((PyObject *)Py_False));
   __Pyx_GIVEREF(((PyObject *)Py_False));
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 11, ((PyObject *)Py_False))) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_6, 11, ((PyObject *)Py_False))) __PYX_ERR(0, 4054, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
-  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3839, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4054, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, Py_None)) __PYX_ERR(0, 3839, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, Py_None)) __PYX_ERR(0, 4054, __pyx_L1_error);
   __pyx_t_6 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -67259,23 +71433,23 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4cssm_37ddm_flexbound_tradeoff(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4cssm_43ddm_flexbound_tradeoff(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_4cssm_37ddm_flexbound_tradeoff = {"ddm_flexbound_tradeoff", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_37ddm_flexbound_tradeoff, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4cssm_37ddm_flexbound_tradeoff(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4cssm_43ddm_flexbound_tradeoff = {"ddm_flexbound_tradeoff", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4cssm_43ddm_flexbound_tradeoff, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cssm_43ddm_flexbound_tradeoff(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyArrayObject *__pyx_v_vh = 0;
@@ -67323,26 +71497,26 @@
   __pyx_v_kwargs = PyDict_New(); if (unlikely(!__pyx_v_kwargs)) return NULL;
   __Pyx_GOTREF(__pyx_v_kwargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_vh,&__pyx_n_s_vl1,&__pyx_n_s_vl2,&__pyx_n_s_a,&__pyx_n_s_zh,&__pyx_n_s_zl1,&__pyx_n_s_zl2,&__pyx_n_s_d,&__pyx_n_s_t,&__pyx_n_s_deadline,&__pyx_n_s_s,&__pyx_n_s_delta_t,&__pyx_n_s_max_t,&__pyx_n_s_n_samples,&__pyx_n_s_n_trials,&__pyx_n_s_print_info,&__pyx_n_s_boundary_fun,&__pyx_n_s_boundary_multiplicative,&__pyx_n_s_boundary_params,&__pyx_n_s_random_state,&__pyx_n_s_return_option,&__pyx_n_s_smooth,0};
     __pyx_defaults14 *__pyx_dynamic_args = __Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_self);
     values[15] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
 
-    /* "cssm.pyx":3855
+    /* "cssm.pyx":4070
  *                            int n_trials = 1,
  *                            print_info = True,
  *                            boundary_fun = None, # function of t (and potentially other parameters) that takes in (t, *args)             # <<<<<<<<<<<<<<
  *                            boundary_multiplicative = True,
  *                            boundary_params = {},
  */
     values[16] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
     values[17] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)((PyObject *)Py_True)));
     values[18] = __Pyx_Arg_NewRef_FASTCALL(__pyx_dynamic_args->__pyx_arg_boundary_params);
 
-    /* "cssm.pyx":3858
+    /* "cssm.pyx":4073
  *                            boundary_multiplicative = True,
  *                            boundary_params = {},
  *                            random_state = None,             # <<<<<<<<<<<<<<
  *                            return_option = 'full',
  *                            smooth = False,
  */
     values[19] = __Pyx_Arg_NewRef_FASTCALL(((PyObject *)Py_None));
@@ -67401,194 +71575,194 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vl1)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 1); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 1); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_vl2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 2); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 2); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_a)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 3); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 3); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_zh)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 4); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 4); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_zl1)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 5); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 5); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_zl2)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[6]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 6); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 6); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_d)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[7]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 7); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 7); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_t)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[8]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 8); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 8); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_deadline)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[9]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 9); __PYX_ERR(0, 3839, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, 9); __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s);
           if (value) { values[10] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 11:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_delta_t);
           if (value) { values[11] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 12:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_max_t);
           if (value) { values[12] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 13:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_samples);
           if (value) { values[13] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 14:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_trials);
           if (value) { values[14] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 15:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_print_info);
           if (value) { values[15] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 16:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boundary_fun);
           if (value) { values[16] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 17:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boundary_multiplicative);
           if (value) { values[17] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 18:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_boundary_params);
           if (value) { values[18] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 19:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_random_state);
           if (value) { values[19] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 20:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_return_option);
           if (value) { values[20] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 21:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_smooth);
           if (value) { values[21] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 3839, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 4054, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "ddm_flexbound_tradeoff") < 0)) __PYX_ERR(0, 3839, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwargs, values + 0, kwd_pos_args, "ddm_flexbound_tradeoff") < 0)) __PYX_ERR(0, 4054, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case 22: values[21] = __Pyx_Arg_FASTCALL(__pyx_args, 21);
         CYTHON_FALLTHROUGH;
         case 21: values[20] = __Pyx_Arg_FASTCALL(__pyx_args, 20);
         CYTHON_FALLTHROUGH;
@@ -67633,76 +71807,76 @@
     __pyx_v_zh = ((PyArrayObject *)values[4]);
     __pyx_v_zl1 = ((PyArrayObject *)values[5]);
     __pyx_v_zl2 = ((PyArrayObject *)values[6]);
     __pyx_v_d = ((PyArrayObject *)values[7]);
     __pyx_v_t = ((PyArrayObject *)values[8]);
     __pyx_v_deadline = ((PyArrayObject *)values[9]);
     if (values[10]) {
-      __pyx_v_s = __pyx_PyFloat_AsFloat(values[10]); if (unlikely((__pyx_v_s == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3849, __pyx_L3_error)
+      __pyx_v_s = __pyx_PyFloat_AsFloat(values[10]); if (unlikely((__pyx_v_s == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4064, __pyx_L3_error)
     } else {
       __pyx_v_s = ((float)((float)1.0));
     }
     if (values[11]) {
-      __pyx_v_delta_t = __pyx_PyFloat_AsFloat(values[11]); if (unlikely((__pyx_v_delta_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3850, __pyx_L3_error)
+      __pyx_v_delta_t = __pyx_PyFloat_AsFloat(values[11]); if (unlikely((__pyx_v_delta_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4065, __pyx_L3_error)
     } else {
       __pyx_v_delta_t = ((float)((double)0.001));
     }
     if (values[12]) {
-      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[12]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3851, __pyx_L3_error)
+      __pyx_v_max_t = __pyx_PyFloat_AsFloat(values[12]); if (unlikely((__pyx_v_max_t == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4066, __pyx_L3_error)
     } else {
       __pyx_v_max_t = ((float)((float)20.0));
     }
     if (values[13]) {
-      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[13]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3852, __pyx_L3_error)
+      __pyx_v_n_samples = __Pyx_PyInt_As_int(values[13]); if (unlikely((__pyx_v_n_samples == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 4067, __pyx_L3_error)
     } else {
       __pyx_v_n_samples = ((int)((int)0x4E20));
     }
     if (values[14]) {
-      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[14]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 3853, __pyx_L3_error)
+      __pyx_v_n_trials = __Pyx_PyInt_As_int(values[14]); if (unlikely((__pyx_v_n_trials == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 4068, __pyx_L3_error)
     } else {
       __pyx_v_n_trials = ((int)((int)1));
     }
     __pyx_v_print_info = values[15];
     __pyx_v_boundary_fun = values[16];
     __pyx_v_boundary_multiplicative = values[17];
     __pyx_v_boundary_params = values[18];
     __pyx_v_random_state = values[19];
     __pyx_v_return_option = values[20];
     __pyx_v_smooth = values[21];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, __pyx_nargs); __PYX_ERR(0, 3839, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("ddm_flexbound_tradeoff", 0, 10, 22, __pyx_nargs); __PYX_ERR(0, 4054, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("cssm.ddm_flexbound_tradeoff", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vh), __pyx_ptype_5numpy_ndarray, 1, "vh", 0))) __PYX_ERR(0, 3839, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl1), __pyx_ptype_5numpy_ndarray, 1, "vl1", 0))) __PYX_ERR(0, 3840, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl2), __pyx_ptype_5numpy_ndarray, 1, "vl2", 0))) __PYX_ERR(0, 3841, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 3842, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zh), __pyx_ptype_5numpy_ndarray, 1, "zh", 0))) __PYX_ERR(0, 3843, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl1), __pyx_ptype_5numpy_ndarray, 1, "zl1", 0))) __PYX_ERR(0, 3844, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl2), __pyx_ptype_5numpy_ndarray, 1, "zl2", 0))) __PYX_ERR(0, 3845, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_d), __pyx_ptype_5numpy_ndarray, 1, "d", 0))) __PYX_ERR(0, 3846, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_t), __pyx_ptype_5numpy_ndarray, 1, "t", 0))) __PYX_ERR(0, 3847, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 3848, __pyx_L1_error)
-  __pyx_r = __pyx_pf_4cssm_36ddm_flexbound_tradeoff(__pyx_self, __pyx_v_vh, __pyx_v_vl1, __pyx_v_vl2, __pyx_v_a, __pyx_v_zh, __pyx_v_zl1, __pyx_v_zl2, __pyx_v_d, __pyx_v_t, __pyx_v_deadline, __pyx_v_s, __pyx_v_delta_t, __pyx_v_max_t, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_print_info, __pyx_v_boundary_fun, __pyx_v_boundary_multiplicative, __pyx_v_boundary_params, __pyx_v_random_state, __pyx_v_return_option, __pyx_v_smooth, __pyx_v_kwargs);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vh), __pyx_ptype_5numpy_ndarray, 1, "vh", 0))) __PYX_ERR(0, 4054, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl1), __pyx_ptype_5numpy_ndarray, 1, "vl1", 0))) __PYX_ERR(0, 4055, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_vl2), __pyx_ptype_5numpy_ndarray, 1, "vl2", 0))) __PYX_ERR(0, 4056, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_a), __pyx_ptype_5numpy_ndarray, 1, "a", 0))) __PYX_ERR(0, 4057, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zh), __pyx_ptype_5numpy_ndarray, 1, "zh", 0))) __PYX_ERR(0, 4058, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl1), __pyx_ptype_5numpy_ndarray, 1, "zl1", 0))) __PYX_ERR(0, 4059, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_zl2), __pyx_ptype_5numpy_ndarray, 1, "zl2", 0))) __PYX_ERR(0, 4060, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_d), __pyx_ptype_5numpy_ndarray, 1, "d", 0))) __PYX_ERR(0, 4061, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_t), __pyx_ptype_5numpy_ndarray, 1, "t", 0))) __PYX_ERR(0, 4062, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_deadline), __pyx_ptype_5numpy_ndarray, 1, "deadline", 0))) __PYX_ERR(0, 4063, __pyx_L1_error)
+  __pyx_r = __pyx_pf_4cssm_42ddm_flexbound_tradeoff(__pyx_self, __pyx_v_vh, __pyx_v_vl1, __pyx_v_vl2, __pyx_v_a, __pyx_v_zh, __pyx_v_zl1, __pyx_v_zl2, __pyx_v_d, __pyx_v_t, __pyx_v_deadline, __pyx_v_s, __pyx_v_delta_t, __pyx_v_max_t, __pyx_v_n_samples, __pyx_v_n_trials, __pyx_v_print_info, __pyx_v_boundary_fun, __pyx_v_boundary_multiplicative, __pyx_v_boundary_params, __pyx_v_random_state, __pyx_v_return_option, __pyx_v_smooth, __pyx_v_kwargs);
 
-  /* "cssm.pyx":3839
+  /* "cssm.pyx":4054
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_tradeoff(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                            np.ndarray[float, ndim = 1] vl1,
  *                            np.ndarray[float, ndim = 1] vl2,
  */
 
@@ -67718,15 +71892,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4cssm_36ddm_flexbound_tradeoff(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
+static PyObject *__pyx_pf_4cssm_42ddm_flexbound_tradeoff(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_vh, PyArrayObject *__pyx_v_vl1, PyArrayObject *__pyx_v_vl2, PyArrayObject *__pyx_v_a, PyArrayObject *__pyx_v_zh, PyArrayObject *__pyx_v_zl1, PyArrayObject *__pyx_v_zl2, PyArrayObject *__pyx_v_d, PyArrayObject *__pyx_v_t, PyArrayObject *__pyx_v_deadline, float __pyx_v_s, float __pyx_v_delta_t, float __pyx_v_max_t, int __pyx_v_n_samples, int __pyx_v_n_trials, CYTHON_UNUSED PyObject *__pyx_v_print_info, PyObject *__pyx_v_boundary_fun, PyObject *__pyx_v_boundary_multiplicative, PyObject *__pyx_v_boundary_params, PyObject *__pyx_v_random_state, PyObject *__pyx_v_return_option, PyObject *__pyx_v_smooth, CYTHON_UNUSED PyObject *__pyx_v_kwargs) {
   __Pyx_memviewslice __pyx_v_vh_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_vl1_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_vl2_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_a_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_zh_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_zl1_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_zl2_view = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -67851,355 +72025,355 @@
   __pyx_pybuffernd_t.rcbuffer = &__pyx_pybuffer_t;
   __pyx_pybuffer_deadline.pybuffer.buf = NULL;
   __pyx_pybuffer_deadline.refcount = 0;
   __pyx_pybuffernd_deadline.data = NULL;
   __pyx_pybuffernd_deadline.rcbuffer = &__pyx_pybuffer_deadline;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vh.rcbuffer->pybuffer, (PyObject*)__pyx_v_vh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vh.rcbuffer->pybuffer, (PyObject*)__pyx_v_vh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_vh.diminfo[0].strides = __pyx_pybuffernd_vh.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vh.diminfo[0].shape = __pyx_pybuffernd_vh.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_vl1.diminfo[0].strides = __pyx_pybuffernd_vl1.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vl1.diminfo[0].shape = __pyx_pybuffernd_vl1.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_vl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_vl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_vl2.diminfo[0].strides = __pyx_pybuffernd_vl2.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_vl2.diminfo[0].shape = __pyx_pybuffernd_vl2.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_a.rcbuffer->pybuffer, (PyObject*)__pyx_v_a, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_a.diminfo[0].strides = __pyx_pybuffernd_a.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_a.diminfo[0].shape = __pyx_pybuffernd_a.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zh.rcbuffer->pybuffer, (PyObject*)__pyx_v_zh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zh.rcbuffer->pybuffer, (PyObject*)__pyx_v_zh, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_zh.diminfo[0].strides = __pyx_pybuffernd_zh.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zh.diminfo[0].shape = __pyx_pybuffernd_zh.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl1.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl1, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_zl1.diminfo[0].strides = __pyx_pybuffernd_zl1.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zl1.diminfo[0].shape = __pyx_pybuffernd_zl1.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_zl2.rcbuffer->pybuffer, (PyObject*)__pyx_v_zl2, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_zl2.diminfo[0].strides = __pyx_pybuffernd_zl2.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_zl2.diminfo[0].shape = __pyx_pybuffernd_zl2.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_d.rcbuffer->pybuffer, (PyObject*)__pyx_v_d, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_d.rcbuffer->pybuffer, (PyObject*)__pyx_v_d, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_d.diminfo[0].strides = __pyx_pybuffernd_d.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_d.diminfo[0].shape = __pyx_pybuffernd_d.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_t.rcbuffer->pybuffer, (PyObject*)__pyx_v_t, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_t.rcbuffer->pybuffer, (PyObject*)__pyx_v_t, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_t.diminfo[0].strides = __pyx_pybuffernd_t.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_t.diminfo[0].shape = __pyx_pybuffernd_t.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_deadline.rcbuffer->pybuffer, (PyObject*)__pyx_v_deadline, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 4054, __pyx_L1_error)
   }
   __pyx_pybuffernd_deadline.diminfo[0].strides = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_deadline.diminfo[0].shape = __pyx_pybuffernd_deadline.rcbuffer->pybuffer.shape[0];
 
-  /* "cssm.pyx":3863
+  /* "cssm.pyx":4078
  *                            **kwargs):
  * 
  *     set_seed(random_state)             # <<<<<<<<<<<<<<
  *     # Param views
  *     cdef float[:] vh_view = vh
  */
-  __pyx_t_1 = __pyx_f_4cssm_set_seed(__pyx_v_random_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3863, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_4cssm_set_seed(__pyx_v_random_state); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4078, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cssm.pyx":3865
+  /* "cssm.pyx":4080
  *     set_seed(random_state)
  *     # Param views
  *     cdef float[:] vh_view = vh             # <<<<<<<<<<<<<<
  *     cdef float[:] vl1_view = vl1
  *     cdef float[:] vl2_view = vl2
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3865, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4080, __pyx_L1_error)
   __pyx_v_vh_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3866
+  /* "cssm.pyx":4081
  *     # Param views
  *     cdef float[:] vh_view = vh
  *     cdef float[:] vl1_view = vl1             # <<<<<<<<<<<<<<
  *     cdef float[:] vl2_view = vl2
  *     cdef float[:] a_view = a
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3866, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4081, __pyx_L1_error)
   __pyx_v_vl1_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3867
+  /* "cssm.pyx":4082
  *     cdef float[:] vh_view = vh
  *     cdef float[:] vl1_view = vl1
  *     cdef float[:] vl2_view = vl2             # <<<<<<<<<<<<<<
  *     cdef float[:] a_view = a
  *     cdef float[:] zh_view = zh
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3867, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_vl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4082, __pyx_L1_error)
   __pyx_v_vl2_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3868
+  /* "cssm.pyx":4083
  *     cdef float[:] vl1_view = vl1
  *     cdef float[:] vl2_view = vl2
  *     cdef float[:] a_view = a             # <<<<<<<<<<<<<<
  *     cdef float[:] zh_view = zh
  *     cdef float[:] zl1_view = zl1
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3868, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_a), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4083, __pyx_L1_error)
   __pyx_v_a_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3869
+  /* "cssm.pyx":4084
  *     cdef float[:] vl2_view = vl2
  *     cdef float[:] a_view = a
  *     cdef float[:] zh_view = zh             # <<<<<<<<<<<<<<
  *     cdef float[:] zl1_view = zl1
  *     cdef float[:] zl2_view = zl2
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3869, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zh), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4084, __pyx_L1_error)
   __pyx_v_zh_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3870
+  /* "cssm.pyx":4085
  *     cdef float[:] a_view = a
  *     cdef float[:] zh_view = zh
  *     cdef float[:] zl1_view = zl1             # <<<<<<<<<<<<<<
  *     cdef float[:] zl2_view = zl2
  *     cdef float[:] d_view = d
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3870, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl1), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4085, __pyx_L1_error)
   __pyx_v_zl1_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3871
+  /* "cssm.pyx":4086
  *     cdef float[:] zh_view = zh
  *     cdef float[:] zl1_view = zl1
  *     cdef float[:] zl2_view = zl2             # <<<<<<<<<<<<<<
  *     cdef float[:] d_view = d
  *     cdef float[:] t_view = t
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3871, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_zl2), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4086, __pyx_L1_error)
   __pyx_v_zl2_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3872
+  /* "cssm.pyx":4087
  *     cdef float[:] zl1_view = zl1
  *     cdef float[:] zl2_view = zl2
  *     cdef float[:] d_view = d             # <<<<<<<<<<<<<<
  *     cdef float[:] t_view = t
  *     cdef float[:] deadline_view = deadline
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_d), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3872, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_d), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4087, __pyx_L1_error)
   __pyx_v_d_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3873
+  /* "cssm.pyx":4088
  *     cdef float[:] zl2_view = zl2
  *     cdef float[:] d_view = d
  *     cdef float[:] t_view = t             # <<<<<<<<<<<<<<
  *     cdef float[:] deadline_view = deadline
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_t), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3873, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_t), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4088, __pyx_L1_error)
   __pyx_v_t_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3874
+  /* "cssm.pyx":4089
  *     cdef float[:] d_view = d
  *     cdef float[:] t_view = t
  *     cdef float[:] deadline_view = deadline             # <<<<<<<<<<<<<<
  * 
  *     # TD: Add trajectory --> same issue as with par2 model above... might need to make a separate simulator for trajectories
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3874, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(((PyObject *)__pyx_v_deadline), PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4089, __pyx_L1_error)
   __pyx_v_deadline_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3878
+  /* "cssm.pyx":4093
  *     # TD: Add trajectory --> same issue as with par2 model above... might need to make a separate simulator for trajectories
  * 
  *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 3878, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1)) __PYX_ERR(0, 4093, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 3878, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_4)) __PYX_ERR(0, 4093, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_int_1)) __PYX_ERR(0, 3878, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_int_1)) __PYX_ERR(0, 4093, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 3878, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_5)) __PYX_ERR(0, 4093, __pyx_L1_error);
   __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 3878, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3878, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4093, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_rts = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cssm.pyx":3879
+  /* "cssm.pyx":4094
  * 
  *     rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)             # <<<<<<<<<<<<<<
  * 
  *     cdef float[:, :, :] rts_view = rts
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 3879, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 4094, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 3879, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 4094, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_int_1)) __PYX_ERR(0, 3879, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_int_1)) __PYX_ERR(0, 4094, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 3879, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 4094, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_intc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_intc); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 3879, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3879, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4094, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_choices = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "cssm.pyx":3881
+  /* "cssm.pyx":4096
  *     choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
  * 
  *     cdef float[:, :, :] rts_view = rts             # <<<<<<<<<<<<<<
  *     cdef int[:, :, :] choices_view = choices
  * 
  */
-  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 3881, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_float(__pyx_v_rts, PyBUF_WRITABLE); if (unlikely(!__pyx_t_7.memview)) __PYX_ERR(0, 4096, __pyx_L1_error)
   __pyx_v_rts_view = __pyx_t_7;
   __pyx_t_7.memview = NULL;
   __pyx_t_7.data = NULL;
 
-  /* "cssm.pyx":3882
+  /* "cssm.pyx":4097
  * 
  *     cdef float[:, :, :] rts_view = rts
  *     cdef int[:, :, :] choices_view = choices             # <<<<<<<<<<<<<<
  * 
  *     cdef float delta_t_sqrt = sqrt(delta_t) # correct scalar so we can use standard normal samples for the brownian motion
  */
-  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 3882, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_to_MemoryviewSlice_dsdsds_int(__pyx_v_choices, PyBUF_WRITABLE); if (unlikely(!__pyx_t_8.memview)) __PYX_ERR(0, 4097, __pyx_L1_error)
   __pyx_v_choices_view = __pyx_t_8;
   __pyx_t_8.memview = NULL;
   __pyx_t_8.data = NULL;
 
-  /* "cssm.pyx":3884
+  /* "cssm.pyx":4099
  *     cdef int[:, :, :] choices_view = choices
  * 
  *     cdef float delta_t_sqrt = sqrt(delta_t) # correct scalar so we can use standard normal samples for the brownian motion             # <<<<<<<<<<<<<<
  *     cdef float sqrt_st = delta_t_sqrt * s # scalar to ensure the correct variance for the gaussian step
  * 
  */
   __pyx_v_delta_t_sqrt = sqrt(__pyx_v_delta_t);
 
-  /* "cssm.pyx":3885
+  /* "cssm.pyx":4100
  * 
  *     cdef float delta_t_sqrt = sqrt(delta_t) # correct scalar so we can use standard normal samples for the brownian motion
  *     cdef float sqrt_st = delta_t_sqrt * s # scalar to ensure the correct variance for the gaussian step             # <<<<<<<<<<<<<<
  * 
  *     # Boundary storage for the upper bound
  */
   __pyx_v_sqrt_st = (__pyx_v_delta_t_sqrt * __pyx_v_s);
 
-  /* "cssm.pyx":3888
+  /* "cssm.pyx":4103
  * 
  *     # Boundary storage for the upper bound
  *     cdef int num_draws = int((max_t / delta_t) + 1)             # <<<<<<<<<<<<<<
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)
  */
   __pyx_v_num_draws = ((int)((__pyx_v_max_t / __pyx_v_delta_t) + 1.0));
 
-  /* "cssm.pyx":3889
+  /* "cssm.pyx":4104
  *     # Boundary storage for the upper bound
  *     cdef int num_draws = int((max_t / delta_t) + 1)
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)             # <<<<<<<<<<<<<<
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)
  *     cdef float[:] boundary_view = boundary
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3889, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_arange); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3889, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_arange); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_max_t + __pyx_v_delta_t)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3889, __pyx_L1_error)
+  __pyx_t_4 = PyFloat_FromDouble((__pyx_v_max_t + __pyx_v_delta_t)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3889, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_9 = NULL;
   __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_9)) {
@@ -68213,22 +72387,22 @@
   #endif
   {
     PyObject *__pyx_callargs[4] = {__pyx_t_9, __pyx_int_0, __pyx_t_4, __pyx_t_1};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_10, 3+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3889, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3889, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3889, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4104, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_1 = NULL;
   __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
   if (likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_1)) {
@@ -68241,222 +72415,222 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_3};
     __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3889, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4104, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_v_t_s = __pyx_t_6;
   __pyx_t_6 = 0;
 
-  /* "cssm.pyx":3890
+  /* "cssm.pyx":4105
  *     cdef int num_draws = int((max_t / delta_t) + 1)
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     cdef float[:] boundary_view = boundary
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_zeros); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_t_s, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_t_s, __pyx_n_s_shape); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 3890, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_6)) __PYX_ERR(0, 4105, __pyx_L1_error);
   __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 3890, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3890, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_v_boundary = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "cssm.pyx":3891
+  /* "cssm.pyx":4106
  *     t_s = np.arange(0, max_t + delta_t, delta_t).astype(DTYPE)
  *     boundary = np.zeros(t_s.shape, dtype = DTYPE)
  *     cdef float[:] boundary_view = boundary             # <<<<<<<<<<<<<<
  * 
  *     # Y particle trace
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_boundary, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3891, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_boundary, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4106, __pyx_L1_error)
   __pyx_v_boundary_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3894
+  /* "cssm.pyx":4109
  * 
  *     # Y particle trace
  *     bias_trace = np.zeros(num_draws, dtype = DTYPE)             # <<<<<<<<<<<<<<
  *     cdef float[:] bias_trace_view = bias_trace
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_draws); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_num_draws); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 3894, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 4109, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 3894, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3894, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_bias_trace = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "cssm.pyx":3895
+  /* "cssm.pyx":4110
  *     # Y particle trace
  *     bias_trace = np.zeros(num_draws, dtype = DTYPE)
  *     cdef float[:] bias_trace_view = bias_trace             # <<<<<<<<<<<<<<
  * 
  *     cdef float y_h, y_l, v_l, t_h, t_l, tmp_pos_dep, smooth_u, deadline_tmp
  */
-  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_bias_trace, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3895, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_to_MemoryviewSlice_ds_float(__pyx_v_bias_trace, PyBUF_WRITABLE); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4110, __pyx_L1_error)
   __pyx_v_bias_trace_view = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3899
+  /* "cssm.pyx":4114
  *     cdef float y_h, y_l, v_l, t_h, t_l, tmp_pos_dep, smooth_u, deadline_tmp
  *     cdef Py_ssize_t n, ix, ix_tmp, k
  *     cdef Py_ssize_t m = 0             # <<<<<<<<<<<<<<
  *     cdef float[:] gaussian_values = draw_gaussian(num_draws)
  * 
  */
   __pyx_v_m = 0;
 
-  /* "cssm.pyx":3900
+  /* "cssm.pyx":4115
  *     cdef Py_ssize_t n, ix, ix_tmp, k
  *     cdef Py_ssize_t m = 0
  *     cdef float[:] gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  * 
  *     for k in range(n_trials):
  */
-  __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3900, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4115, __pyx_L1_error)
   __pyx_v_gaussian_values = __pyx_t_2;
   __pyx_t_2.memview = NULL;
   __pyx_t_2.data = NULL;
 
-  /* "cssm.pyx":3902
+  /* "cssm.pyx":4117
  *     cdef float[:] gaussian_values = draw_gaussian(num_draws)
  * 
  *     for k in range(n_trials):             # <<<<<<<<<<<<<<
  *         # Precompute boundary evaluations
  *         boundary_params_tmp = {key: boundary_params[key][k] for key in boundary_params.keys()}
  */
   __pyx_t_10 = __pyx_v_n_trials;
   __pyx_t_11 = __pyx_t_10;
   for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
     __pyx_v_k = __pyx_t_12;
 
-    /* "cssm.pyx":3904
+    /* "cssm.pyx":4119
  *     for k in range(n_trials):
  *         # Precompute boundary evaluations
  *         boundary_params_tmp = {key: boundary_params[key][k] for key in boundary_params.keys()}             # <<<<<<<<<<<<<<
  * 
  *         # Precompute boundary evaluations
  */
     { /* enter inner scope */
-      __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3904, __pyx_L7_error)
+      __pyx_t_5 = PyDict_New(); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4119, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_13 = 0;
       if (unlikely(__pyx_v_boundary_params == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "keys");
-        __PYX_ERR(0, 3904, __pyx_L7_error)
+        __PYX_ERR(0, 4119, __pyx_L7_error)
       }
-      __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_boundary_params, 0, __pyx_n_s_keys, (&__pyx_t_14), (&__pyx_t_15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3904, __pyx_L7_error)
+      __pyx_t_3 = __Pyx_dict_iterator(__pyx_v_boundary_params, 0, __pyx_n_s_keys, (&__pyx_t_14), (&__pyx_t_15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4119, __pyx_L7_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_XDECREF(__pyx_t_1);
       __pyx_t_1 = __pyx_t_3;
       __pyx_t_3 = 0;
       while (1) {
         __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_14, &__pyx_t_13, &__pyx_t_3, NULL, NULL, __pyx_t_15);
         if (unlikely(__pyx_t_16 == 0)) break;
-        if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 3904, __pyx_L7_error)
+        if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 4119, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_XDECREF_SET(__pyx_9genexpr15__pyx_v_key, __pyx_t_3);
         __pyx_t_3 = 0;
-        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_boundary_params, __pyx_9genexpr15__pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3904, __pyx_L7_error)
+        __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_boundary_params, __pyx_9genexpr15__pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4119, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_3, __pyx_v_k, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3904, __pyx_L7_error)
+        __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_3, __pyx_v_k, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4119, __pyx_L7_error)
         __Pyx_GOTREF(__pyx_t_6);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_9genexpr15__pyx_v_key, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 3904, __pyx_L7_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_5, (PyObject*)__pyx_9genexpr15__pyx_v_key, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 4119, __pyx_L7_error)
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_9genexpr15__pyx_v_key); __pyx_9genexpr15__pyx_v_key = 0;
       goto __pyx_L10_exit_scope;
       __pyx_L7_error:;
       __Pyx_XDECREF(__pyx_9genexpr15__pyx_v_key); __pyx_9genexpr15__pyx_v_key = 0;
       goto __pyx_L1_error;
       __pyx_L10_exit_scope:;
     } /* exit inner scope */
     __Pyx_XDECREF_SET(__pyx_v_boundary_params_tmp, ((PyObject*)__pyx_t_5));
     __pyx_t_5 = 0;
 
-    /* "cssm.pyx":3907
+    /* "cssm.pyx":4122
  * 
  *         # Precompute boundary evaluations
  *         if boundary_multiplicative:             # <<<<<<<<<<<<<<
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  *         else:
  */
-    __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_v_boundary_multiplicative); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3907, __pyx_L1_error)
+    __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_v_boundary_multiplicative); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 4122, __pyx_L1_error)
     if (__pyx_t_17) {
 
-      /* "cssm.pyx":3908
+      /* "cssm.pyx":4123
  *         # Precompute boundary evaluations
  *         if boundary_multiplicative:
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)             # <<<<<<<<<<<<<<
  *         else:
  *             boundary[:] = np.add(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_multiply); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_multiply); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_18 = __pyx_v_k;
-      __pyx_t_6 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_18 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      __pyx_t_6 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_18 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 3908, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_9, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 4123, __pyx_L1_error)
       __pyx_t_4 = __pyx_t_9;
       __pyx_t_9 = 0;
-      if (__Pyx_MergeKeywords(__pyx_t_4, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 3908, __pyx_L1_error)
-      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      if (__Pyx_MergeKeywords(__pyx_t_4, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 4123, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       __pyx_t_15 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -68471,22 +72645,22 @@
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_6, __pyx_t_9};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_15, 2+__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3908, __pyx_L1_error)
+        if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4123, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_astype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3908, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_9 = NULL;
       __pyx_t_15 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_3))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_3);
         if (likely(__pyx_t_9)) {
@@ -68499,54 +72673,54 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_1};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_15, 1+__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3908, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4123, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       }
-      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 3908, __pyx_L1_error)
+      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 4123, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-      /* "cssm.pyx":3907
+      /* "cssm.pyx":4122
  * 
  *         # Precompute boundary evaluations
  *         if boundary_multiplicative:             # <<<<<<<<<<<<<<
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  *         else:
  */
       goto __pyx_L11;
     }
 
-    /* "cssm.pyx":3910
+    /* "cssm.pyx":4125
  *             boundary[:] = np.multiply(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  *         else:
  *             boundary[:] = np.add(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)             # <<<<<<<<<<<<<<
  * 
  *         deadline_tmp = min(max_t, deadline_view[k] - t_view[k])
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_add); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_add); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_18 = __pyx_v_k;
-      __pyx_t_1 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_18 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      __pyx_t_1 = PyFloat_FromDouble((*((float *) ( /* dim=0 */ (__pyx_v_a_view.data + __pyx_t_18 * __pyx_v_a_view.strides[0]) )))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 3910, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_t, __pyx_v_t_s) < 0) __PYX_ERR(0, 4125, __pyx_L1_error)
       __pyx_t_6 = __pyx_t_4;
       __pyx_t_4 = 0;
-      if (__Pyx_MergeKeywords(__pyx_t_6, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 3910, __pyx_L1_error)
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      if (__Pyx_MergeKeywords(__pyx_t_6, __pyx_v_boundary_params_tmp) < 0) __PYX_ERR(0, 4125, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_v_boundary_fun, __pyx_empty_tuple, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       __pyx_t_15 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_9);
@@ -68561,22 +72735,22 @@
       #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_6, __pyx_t_1, __pyx_t_4};
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_15, 2+__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3910, __pyx_L1_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4125, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_astype); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3910, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_DTYPE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = NULL;
       __pyx_t_15 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_9);
         if (likely(__pyx_t_4)) {
@@ -68589,24 +72763,24 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_15, 1+__pyx_t_15);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3910, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4125, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
-      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 3910, __pyx_L1_error)
+      if (__Pyx_PyObject_SetSlice(__pyx_v_boundary, __pyx_t_5, 0, 0, NULL, NULL, &__pyx_slice__5, 0, 0, 0) < 0) __PYX_ERR(0, 4125, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __pyx_L11:;
 
-    /* "cssm.pyx":3912
+    /* "cssm.pyx":4127
  *             boundary[:] = np.add(a_view[k], boundary_fun(t = t_s, **boundary_params_tmp)).astype(DTYPE)
  * 
  *         deadline_tmp = min(max_t, deadline_view[k] - t_view[k])             # <<<<<<<<<<<<<<
  *         # Loop over samples
  *         for n in range(n_samples):
  */
     __pyx_t_18 = __pyx_v_k;
@@ -68617,90 +72791,90 @@
     if (__pyx_t_17) {
       __pyx_t_22 = __pyx_t_20;
     } else {
       __pyx_t_22 = __pyx_t_21;
     }
     __pyx_v_deadline_tmp = __pyx_t_22;
 
-    /* "cssm.pyx":3914
+    /* "cssm.pyx":4129
  *         deadline_tmp = min(max_t, deadline_view[k] - t_view[k])
  *         # Loop over samples
  *         for n in range(n_samples):             # <<<<<<<<<<<<<<
  *             choices_view[n, k, 0] = 0 # reset choice
  *             t_h = 0 # reset time high dimension
  */
     __pyx_t_15 = __pyx_v_n_samples;
     __pyx_t_16 = __pyx_t_15;
     for (__pyx_t_14 = 0; __pyx_t_14 < __pyx_t_16; __pyx_t_14+=1) {
       __pyx_v_n = __pyx_t_14;
 
-      /* "cssm.pyx":3915
+      /* "cssm.pyx":4130
  *         # Loop over samples
  *         for n in range(n_samples):
  *             choices_view[n, k, 0] = 0 # reset choice             # <<<<<<<<<<<<<<
  *             t_h = 0 # reset time high dimension
  *             t_l = 0 # reset time low dimension
  */
       __pyx_t_19 = __pyx_v_n;
       __pyx_t_18 = __pyx_v_k;
       __pyx_t_23 = 0;
       *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_19 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_18 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_23 * __pyx_v_choices_view.strides[2]) )) = 0;
 
-      /* "cssm.pyx":3916
+      /* "cssm.pyx":4131
  *         for n in range(n_samples):
  *             choices_view[n, k, 0] = 0 # reset choice
  *             t_h = 0 # reset time high dimension             # <<<<<<<<<<<<<<
  *             t_l = 0 # reset time low dimension
  *             ix = 0 # reset boundary index
  */
       __pyx_v_t_h = 0.0;
 
-      /* "cssm.pyx":3917
+      /* "cssm.pyx":4132
  *             choices_view[n, k, 0] = 0 # reset choice
  *             t_h = 0 # reset time high dimension
  *             t_l = 0 # reset time low dimension             # <<<<<<<<<<<<<<
  *             ix = 0 # reset boundary index
  * 
  */
       __pyx_v_t_l = 0.0;
 
-      /* "cssm.pyx":3918
+      /* "cssm.pyx":4133
  *             t_h = 0 # reset time high dimension
  *             t_l = 0 # reset time low dimension
  *             ix = 0 # reset boundary index             # <<<<<<<<<<<<<<
  * 
  *             # Initialize walkers
  */
       __pyx_v_ix = 0;
 
-      /* "cssm.pyx":3921
+      /* "cssm.pyx":4136
  * 
  *             # Initialize walkers
  *             y_h = (-1) * boundary_view[0] + (zh_view[k] * 2 * (boundary_view[0]))             # <<<<<<<<<<<<<<
  *             bias_trace_view[0] = ((y_h + boundary_view[0]) / (2 * boundary_view[0]))
  * 
  */
       __pyx_t_23 = 0;
       __pyx_t_18 = __pyx_v_k;
       __pyx_t_19 = 0;
       __pyx_v_y_h = ((-1.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_23 * __pyx_v_boundary_view.strides[0]) )))) + (((*((float *) ( /* dim=0 */ (__pyx_v_zh_view.data + __pyx_t_18 * __pyx_v_zh_view.strides[0]) ))) * 2.0) * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))));
 
-      /* "cssm.pyx":3922
+      /* "cssm.pyx":4137
  *             # Initialize walkers
  *             y_h = (-1) * boundary_view[0] + (zh_view[k] * 2 * (boundary_view[0]))
  *             bias_trace_view[0] = ((y_h + boundary_view[0]) / (2 * boundary_view[0]))             # <<<<<<<<<<<<<<
  * 
  *             # Random walks until y_h hits bound
  */
       __pyx_t_19 = 0;
       __pyx_t_18 = 0;
       __pyx_t_23 = 0;
       *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_23 * __pyx_v_bias_trace_view.strides[0]) )) = ((__pyx_v_y_h + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_18 * __pyx_v_boundary_view.strides[0]) )))));
 
-      /* "cssm.pyx":3925
+      /* "cssm.pyx":4140
  * 
  *             # Random walks until y_h hits bound
  *             while (y_h >= ((-1) * boundary_view[ix])) and ((y_h <= boundary_view[ix])) and (t_h <= deadline_tmp):             # <<<<<<<<<<<<<<
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])
  *                 bias_trace_view[ix] = ((y_h + boundary_view[ix]) / (2 * boundary_view[ix]))
  */
       while (1) {
@@ -68719,341 +72893,341 @@
           goto __pyx_L16_bool_binop_done;
         }
         __pyx_t_24 = (__pyx_v_t_h <= __pyx_v_deadline_tmp);
         __pyx_t_17 = __pyx_t_24;
         __pyx_L16_bool_binop_done:;
         if (!__pyx_t_17) break;
 
-        /* "cssm.pyx":3926
+        /* "cssm.pyx":4141
  *             # Random walks until y_h hits bound
  *             while (y_h >= ((-1) * boundary_view[ix])) and ((y_h <= boundary_view[ix])) and (t_h <= deadline_tmp):
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])             # <<<<<<<<<<<<<<
  *                 bias_trace_view[ix] = ((y_h + boundary_view[ix]) / (2 * boundary_view[ix]))
  *                 t_h += delta_t
  */
         __pyx_t_18 = __pyx_v_k;
         __pyx_t_19 = __pyx_v_m;
         __pyx_v_y_h = (__pyx_v_y_h + (((*((float *) ( /* dim=0 */ (__pyx_v_vh_view.data + __pyx_t_18 * __pyx_v_vh_view.strides[0]) ))) * __pyx_v_delta_t) + (__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_19 * __pyx_v_gaussian_values.strides[0]) ))))));
 
-        /* "cssm.pyx":3927
+        /* "cssm.pyx":4142
  *             while (y_h >= ((-1) * boundary_view[ix])) and ((y_h <= boundary_view[ix])) and (t_h <= deadline_tmp):
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])
  *                 bias_trace_view[ix] = ((y_h + boundary_view[ix]) / (2 * boundary_view[ix]))             # <<<<<<<<<<<<<<
  *                 t_h += delta_t
  *                 ix += 1
  */
         __pyx_t_19 = __pyx_v_ix;
         __pyx_t_18 = __pyx_v_ix;
         __pyx_t_23 = __pyx_v_ix;
         *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_23 * __pyx_v_bias_trace_view.strides[0]) )) = ((__pyx_v_y_h + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_18 * __pyx_v_boundary_view.strides[0]) )))));
 
-        /* "cssm.pyx":3928
+        /* "cssm.pyx":4143
  *                 y_h += (vh_view[k] * delta_t) + (sqrt_st * gaussian_values[m])
  *                 bias_trace_view[ix] = ((y_h + boundary_view[ix]) / (2 * boundary_view[ix]))
  *                 t_h += delta_t             # <<<<<<<<<<<<<<
  *                 ix += 1
  *                 m += 1
  */
         __pyx_v_t_h = (__pyx_v_t_h + __pyx_v_delta_t);
 
-        /* "cssm.pyx":3929
+        /* "cssm.pyx":4144
  *                 bias_trace_view[ix] = ((y_h + boundary_view[ix]) / (2 * boundary_view[ix]))
  *                 t_h += delta_t
  *                 ix += 1             # <<<<<<<<<<<<<<
  *                 m += 1
  *                 if m == num_draws:
  */
         __pyx_v_ix = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3930
+        /* "cssm.pyx":4145
  *                 t_h += delta_t
  *                 ix += 1
  *                 m += 1             # <<<<<<<<<<<<<<
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)
  */
         __pyx_v_m = (__pyx_v_m + 1);
 
-        /* "cssm.pyx":3931
+        /* "cssm.pyx":4146
  *                 ix += 1
  *                 m += 1
  *                 if m == num_draws:             # <<<<<<<<<<<<<<
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0
  */
         __pyx_t_17 = (__pyx_v_m == __pyx_v_num_draws);
         if (__pyx_t_17) {
 
-          /* "cssm.pyx":3932
+          /* "cssm.pyx":4147
  *                 m += 1
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  *                     m = 0
  * 
  */
-          __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3932, __pyx_L1_error)
+          __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4147, __pyx_L1_error)
           __PYX_XCLEAR_MEMVIEW(&__pyx_v_gaussian_values, 1);
           __pyx_v_gaussian_values = __pyx_t_2;
           __pyx_t_2.memview = NULL;
           __pyx_t_2.data = NULL;
 
-          /* "cssm.pyx":3933
+          /* "cssm.pyx":4148
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0             # <<<<<<<<<<<<<<
  * 
  *             # The probability of making a 'mistake' 1 - (relative y position)
  */
           __pyx_v_m = 0;
 
-          /* "cssm.pyx":3931
+          /* "cssm.pyx":4146
  *                 ix += 1
  *                 m += 1
  *                 if m == num_draws:             # <<<<<<<<<<<<<<
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0
  */
         }
       }
 
-      /* "cssm.pyx":3938
+      /* "cssm.pyx":4153
  *             # y at upper bound --> choices_view[n, k, 0] add 2 deterministically
  *             # y at lower bound --> choice_view[n, k, 0] stay the same deterministically
  *             if random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 2
  * 
  */
-      __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3938, __pyx_L1_error)
+      __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4153, __pyx_L1_error)
       __pyx_t_18 = __pyx_v_ix;
       __pyx_t_19 = __pyx_v_ix;
       __pyx_t_17 = (__pyx_t_22 <= ((__pyx_v_y_h + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_18 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) ))))));
       if (__pyx_t_17) {
 
-        /* "cssm.pyx":3939
+        /* "cssm.pyx":4154
  *             # y at lower bound --> choice_view[n, k, 0] stay the same deterministically
  *             if random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):
  *                 choices_view[n, k, 0] += 2             # <<<<<<<<<<<<<<
  * 
  *             if choices_view[n, k, 0] == 2:
  */
         __pyx_t_19 = __pyx_v_n;
         __pyx_t_18 = __pyx_v_k;
         __pyx_t_23 = 0;
         *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_19 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_18 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_23 * __pyx_v_choices_view.strides[2]) )) += 2;
 
-        /* "cssm.pyx":3938
+        /* "cssm.pyx":4153
  *             # y at upper bound --> choices_view[n, k, 0] add 2 deterministically
  *             # y at lower bound --> choice_view[n, k, 0] stay the same deterministically
  *             if random_uniform() <= ((y_h + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 2
  * 
  */
       }
 
-      /* "cssm.pyx":3941
+      /* "cssm.pyx":4156
  *                 choices_view[n, k, 0] += 2
  * 
  *             if choices_view[n, k, 0] == 2:             # <<<<<<<<<<<<<<
  *                 y_l = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))
  *                 v_l = vl2_view[k]
  */
       __pyx_t_23 = __pyx_v_n;
       __pyx_t_18 = __pyx_v_k;
       __pyx_t_19 = 0;
       __pyx_t_17 = ((*((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_23 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_18 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[2]) ))) == 2);
       if (__pyx_t_17) {
 
-        /* "cssm.pyx":3942
+        /* "cssm.pyx":4157
  * 
  *             if choices_view[n, k, 0] == 2:
  *                 y_l = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))             # <<<<<<<<<<<<<<
  *                 v_l = vl2_view[k]
  * 
  */
         __pyx_t_19 = 0;
         __pyx_t_18 = __pyx_v_k;
         __pyx_t_23 = 0;
         __pyx_v_y_l = ((-1.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))) + (((*((float *) ( /* dim=0 */ (__pyx_v_zl2_view.data + __pyx_t_18 * __pyx_v_zl2_view.strides[0]) ))) * 2.0) * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_23 * __pyx_v_boundary_view.strides[0]) )))));
 
-        /* "cssm.pyx":3943
+        /* "cssm.pyx":4158
  *             if choices_view[n, k, 0] == 2:
  *                 y_l = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))
  *                 v_l = vl2_view[k]             # <<<<<<<<<<<<<<
  * 
  *                 # Fill bias trace until max_rt reached
  */
         __pyx_t_23 = __pyx_v_k;
         __pyx_v_v_l = (*((float *) ( /* dim=0 */ (__pyx_v_vl2_view.data + __pyx_t_23 * __pyx_v_vl2_view.strides[0]) )));
 
-        /* "cssm.pyx":3946
+        /* "cssm.pyx":4161
  * 
  *                 # Fill bias trace until max_rt reached
  *                 ix_tmp = ix + 1             # <<<<<<<<<<<<<<
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 1.0
  */
         __pyx_v_ix_tmp = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3947
+        /* "cssm.pyx":4162
  *                 # Fill bias trace until max_rt reached
  *                 ix_tmp = ix + 1
  *                 while ix_tmp < num_draws:             # <<<<<<<<<<<<<<
  *                     bias_trace_view[ix_tmp] = 1.0
  *                     ix_tmp += 1
  */
         while (1) {
           __pyx_t_17 = (__pyx_v_ix_tmp < __pyx_v_num_draws);
           if (!__pyx_t_17) break;
 
-          /* "cssm.pyx":3948
+          /* "cssm.pyx":4163
  *                 ix_tmp = ix + 1
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 1.0             # <<<<<<<<<<<<<<
  *                     ix_tmp += 1
  * 
  */
           __pyx_t_23 = __pyx_v_ix_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_23 * __pyx_v_bias_trace_view.strides[0]) )) = 1.0;
 
-          /* "cssm.pyx":3949
+          /* "cssm.pyx":4164
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 1.0
  *                     ix_tmp += 1             # <<<<<<<<<<<<<<
  * 
  *             else: # Store intermediate choice
  */
           __pyx_v_ix_tmp = (__pyx_v_ix_tmp + 1);
         }
 
-        /* "cssm.pyx":3941
+        /* "cssm.pyx":4156
  *                 choices_view[n, k, 0] += 2
  * 
  *             if choices_view[n, k, 0] == 2:             # <<<<<<<<<<<<<<
  *                 y_l = (- 1) * boundary_view[0] + (zl2_view[k] * 2 * (boundary_view[0]))
  *                 v_l = vl2_view[k]
  */
         goto __pyx_L21;
       }
 
-      /* "cssm.pyx":3952
+      /* "cssm.pyx":4167
  * 
  *             else: # Store intermediate choice
  *                 y_l = (- 1) * boundary_view[0] + (zl1_view[k] * 2 * (boundary_view[0]))             # <<<<<<<<<<<<<<
  *                 v_l = vl1_view[k]
  * 
  */
       /*else*/ {
         __pyx_t_23 = 0;
         __pyx_t_18 = __pyx_v_k;
         __pyx_t_19 = 0;
         __pyx_v_y_l = ((-1.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_23 * __pyx_v_boundary_view.strides[0]) )))) + (((*((float *) ( /* dim=0 */ (__pyx_v_zl1_view.data + __pyx_t_18 * __pyx_v_zl1_view.strides[0]) ))) * 2.0) * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_19 * __pyx_v_boundary_view.strides[0]) )))));
 
-        /* "cssm.pyx":3953
+        /* "cssm.pyx":4168
  *             else: # Store intermediate choice
  *                 y_l = (- 1) * boundary_view[0] + (zl1_view[k] * 2 * (boundary_view[0]))
  *                 v_l = vl1_view[k]             # <<<<<<<<<<<<<<
  * 
  *                 # Fill bias trace until max_rt reached
  */
         __pyx_t_19 = __pyx_v_k;
         __pyx_v_v_l = (*((float *) ( /* dim=0 */ (__pyx_v_vl1_view.data + __pyx_t_19 * __pyx_v_vl1_view.strides[0]) )));
 
-        /* "cssm.pyx":3956
+        /* "cssm.pyx":4171
  * 
  *                 # Fill bias trace until max_rt reached
  *                 ix_tmp = ix + 1             # <<<<<<<<<<<<<<
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 0.0
  */
         __pyx_v_ix_tmp = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3957
+        /* "cssm.pyx":4172
  *                 # Fill bias trace until max_rt reached
  *                 ix_tmp = ix + 1
  *                 while ix_tmp < num_draws:             # <<<<<<<<<<<<<<
  *                     bias_trace_view[ix_tmp] = 0.0
  *                     ix_tmp += 1
  */
         while (1) {
           __pyx_t_17 = (__pyx_v_ix_tmp < __pyx_v_num_draws);
           if (!__pyx_t_17) break;
 
-          /* "cssm.pyx":3958
+          /* "cssm.pyx":4173
  *                 ix_tmp = ix + 1
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 0.0             # <<<<<<<<<<<<<<
  *                     ix_tmp += 1
  * 
  */
           __pyx_t_19 = __pyx_v_ix_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_19 * __pyx_v_bias_trace_view.strides[0]) )) = 0.0;
 
-          /* "cssm.pyx":3959
+          /* "cssm.pyx":4174
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 0.0
  *                     ix_tmp += 1             # <<<<<<<<<<<<<<
  * 
  *                 #We need to reverse the bias_trace if we took the lower choice
  */
           __pyx_v_ix_tmp = (__pyx_v_ix_tmp + 1);
         }
 
-        /* "cssm.pyx":3962
+        /* "cssm.pyx":4177
  * 
  *                 #We need to reverse the bias_trace if we took the lower choice
  *                 ix_tmp = 0             # <<<<<<<<<<<<<<
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 1.0 - bias_trace_view[ix_tmp]
  */
         __pyx_v_ix_tmp = 0;
 
-        /* "cssm.pyx":3963
+        /* "cssm.pyx":4178
  *                 #We need to reverse the bias_trace if we took the lower choice
  *                 ix_tmp = 0
  *                 while ix_tmp < num_draws:             # <<<<<<<<<<<<<<
  *                     bias_trace_view[ix_tmp] = 1.0 - bias_trace_view[ix_tmp]
  *                     ix_tmp += 1
  */
         while (1) {
           __pyx_t_17 = (__pyx_v_ix_tmp < __pyx_v_num_draws);
           if (!__pyx_t_17) break;
 
-          /* "cssm.pyx":3964
+          /* "cssm.pyx":4179
  *                 ix_tmp = 0
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 1.0 - bias_trace_view[ix_tmp]             # <<<<<<<<<<<<<<
  *                     ix_tmp += 1
  * 
  */
           __pyx_t_19 = __pyx_v_ix_tmp;
           __pyx_t_18 = __pyx_v_ix_tmp;
           *((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_18 * __pyx_v_bias_trace_view.strides[0]) )) = (1.0 - (*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_19 * __pyx_v_bias_trace_view.strides[0]) ))));
 
-          /* "cssm.pyx":3965
+          /* "cssm.pyx":4180
  *                 while ix_tmp < num_draws:
  *                     bias_trace_view[ix_tmp] = 1.0 - bias_trace_view[ix_tmp]
  *                     ix_tmp += 1             # <<<<<<<<<<<<<<
  * 
  *                 #print('new bias_trace: ', bias_trace)
  */
           __pyx_v_ix_tmp = (__pyx_v_ix_tmp + 1);
         }
       }
       __pyx_L21:;
 
-      /* "cssm.pyx":3970
+      /* "cssm.pyx":4185
  * 
  *             # Random walks until the y_l corresponding to y_h hits bound
  *             ix = 0             # <<<<<<<<<<<<<<
  *             while (y_l >= ((-1) * boundary_view[ix])) and (y_l <= boundary_view[ix]) and (t_l <= deadline_tmp):
  *                 # Compute local position dependence
  */
       __pyx_v_ix = 0;
 
-      /* "cssm.pyx":3971
+      /* "cssm.pyx":4186
  *             # Random walks until the y_l corresponding to y_h hits bound
  *             ix = 0
  *             while (y_l >= ((-1) * boundary_view[ix])) and (y_l <= boundary_view[ix]) and (t_l <= deadline_tmp):             # <<<<<<<<<<<<<<
  *                 # Compute local position dependence
  *                 # AF-todo: can't understand what the idea here is anymore
  */
       while (1) {
@@ -69072,27 +73246,27 @@
           goto __pyx_L30_bool_binop_done;
         }
         __pyx_t_24 = (__pyx_v_t_l <= __pyx_v_deadline_tmp);
         __pyx_t_17 = __pyx_t_24;
         __pyx_L30_bool_binop_done:;
         if (!__pyx_t_17) break;
 
-        /* "cssm.pyx":3975
+        /* "cssm.pyx":4190
  *                 # AF-todo: can't understand what the idea here is anymore
  *                 # especially why bias_trace_view is flipped (-1) here
  *                 tmp_pos_dep = (1 + (d_view[k] * (bias_trace_view[ix] - 1.0))) / (2 - d_view[k])             # <<<<<<<<<<<<<<
  * 
  *                 if (bias_trace_view[ix] < 1) and (bias_trace_view[ix] > 0):
  */
         __pyx_t_19 = __pyx_v_k;
         __pyx_t_18 = __pyx_v_ix;
         __pyx_t_23 = __pyx_v_k;
         __pyx_v_tmp_pos_dep = ((1.0 + ((*((float *) ( /* dim=0 */ (__pyx_v_d_view.data + __pyx_t_19 * __pyx_v_d_view.strides[0]) ))) * ((*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_18 * __pyx_v_bias_trace_view.strides[0]) ))) - 1.0))) / ((double)(2.0 - (*((float *) ( /* dim=0 */ (__pyx_v_d_view.data + __pyx_t_23 * __pyx_v_d_view.strides[0]) ))))));
 
-        /* "cssm.pyx":3977
+        /* "cssm.pyx":4192
  *                 tmp_pos_dep = (1 + (d_view[k] * (bias_trace_view[ix] - 1.0))) / (2 - d_view[k])
  * 
  *                 if (bias_trace_view[ix] < 1) and (bias_trace_view[ix] > 0):             # <<<<<<<<<<<<<<
  *                     # Before high-dim choice is taken
  *                     y_l += tmp_pos_dep * (v_l * delta_t) # Add drift
  */
         __pyx_t_23 = __pyx_v_ix;
@@ -69104,684 +73278,684 @@
         }
         __pyx_t_23 = __pyx_v_ix;
         __pyx_t_24 = ((*((float *) ( /* dim=0 */ (__pyx_v_bias_trace_view.data + __pyx_t_23 * __pyx_v_bias_trace_view.strides[0]) ))) > 0.0);
         __pyx_t_17 = __pyx_t_24;
         __pyx_L34_bool_binop_done:;
         if (__pyx_t_17) {
 
-          /* "cssm.pyx":3979
+          /* "cssm.pyx":4194
  *                 if (bias_trace_view[ix] < 1) and (bias_trace_view[ix] > 0):
  *                     # Before high-dim choice is taken
  *                     y_l += tmp_pos_dep * (v_l * delta_t) # Add drift             # <<<<<<<<<<<<<<
  *                     y_l += tmp_pos_dep * sqrt_st * gaussian_values[m] # Add noise
  *                 else:
  */
           __pyx_v_y_l = (__pyx_v_y_l + (__pyx_v_tmp_pos_dep * (__pyx_v_v_l * __pyx_v_delta_t)));
 
-          /* "cssm.pyx":3980
+          /* "cssm.pyx":4195
  *                     # Before high-dim choice is taken
  *                     y_l += tmp_pos_dep * (v_l * delta_t) # Add drift
  *                     y_l += tmp_pos_dep * sqrt_st * gaussian_values[m] # Add noise             # <<<<<<<<<<<<<<
  *                 else:
  *                     # After high-dim choice is taken
  */
           __pyx_t_23 = __pyx_v_m;
           __pyx_v_y_l = (__pyx_v_y_l + ((__pyx_v_tmp_pos_dep * __pyx_v_sqrt_st) * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_23 * __pyx_v_gaussian_values.strides[0]) )))));
 
-          /* "cssm.pyx":3977
+          /* "cssm.pyx":4192
  *                 tmp_pos_dep = (1 + (d_view[k] * (bias_trace_view[ix] - 1.0))) / (2 - d_view[k])
  * 
  *                 if (bias_trace_view[ix] < 1) and (bias_trace_view[ix] > 0):             # <<<<<<<<<<<<<<
  *                     # Before high-dim choice is taken
  *                     y_l += tmp_pos_dep * (v_l * delta_t) # Add drift
  */
           goto __pyx_L33;
         }
 
-        /* "cssm.pyx":3983
+        /* "cssm.pyx":4198
  *                 else:
  *                     # After high-dim choice is taken
  *                     y_l += (v_l * delta_t) # Add drift             # <<<<<<<<<<<<<<
  *                     y_l += sqrt_st * gaussian_values[m] # Add noise
  * 
  */
         /*else*/ {
           __pyx_v_y_l = (__pyx_v_y_l + (__pyx_v_v_l * __pyx_v_delta_t));
 
-          /* "cssm.pyx":3984
+          /* "cssm.pyx":4199
  *                     # After high-dim choice is taken
  *                     y_l += (v_l * delta_t) # Add drift
  *                     y_l += sqrt_st * gaussian_values[m] # Add noise             # <<<<<<<<<<<<<<
  * 
  *                 t_l += delta_t # update time for low_dim choice
  */
           __pyx_t_23 = __pyx_v_m;
           __pyx_v_y_l = (__pyx_v_y_l + (__pyx_v_sqrt_st * (*((float *) ( /* dim=0 */ (__pyx_v_gaussian_values.data + __pyx_t_23 * __pyx_v_gaussian_values.strides[0]) )))));
         }
         __pyx_L33:;
 
-        /* "cssm.pyx":3986
+        /* "cssm.pyx":4201
  *                     y_l += sqrt_st * gaussian_values[m] # Add noise
  * 
  *                 t_l += delta_t # update time for low_dim choice             # <<<<<<<<<<<<<<
  *                 ix += 1 # update time index
  *                 m += 1 # update rv couter
  */
         __pyx_v_t_l = (__pyx_v_t_l + __pyx_v_delta_t);
 
-        /* "cssm.pyx":3987
+        /* "cssm.pyx":4202
  * 
  *                 t_l += delta_t # update time for low_dim choice
  *                 ix += 1 # update time index             # <<<<<<<<<<<<<<
  *                 m += 1 # update rv couter
  * 
  */
         __pyx_v_ix = (__pyx_v_ix + 1);
 
-        /* "cssm.pyx":3988
+        /* "cssm.pyx":4203
  *                 t_l += delta_t # update time for low_dim choice
  *                 ix += 1 # update time index
  *                 m += 1 # update rv couter             # <<<<<<<<<<<<<<
  * 
  *                 if m == num_draws:
  */
         __pyx_v_m = (__pyx_v_m + 1);
 
-        /* "cssm.pyx":3990
+        /* "cssm.pyx":4205
  *                 m += 1 # update rv couter
  * 
  *                 if m == num_draws:             # <<<<<<<<<<<<<<
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0
  */
         __pyx_t_17 = (__pyx_v_m == __pyx_v_num_draws);
         if (__pyx_t_17) {
 
-          /* "cssm.pyx":3991
+          /* "cssm.pyx":4206
  * 
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)             # <<<<<<<<<<<<<<
  *                     m = 0
  * 
  */
-          __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 3991, __pyx_L1_error)
+          __pyx_t_2 = __pyx_f_4cssm_draw_gaussian(__pyx_v_num_draws); if (unlikely(!__pyx_t_2.memview)) __PYX_ERR(0, 4206, __pyx_L1_error)
           __PYX_XCLEAR_MEMVIEW(&__pyx_v_gaussian_values, 1);
           __pyx_v_gaussian_values = __pyx_t_2;
           __pyx_t_2.memview = NULL;
           __pyx_t_2.data = NULL;
 
-          /* "cssm.pyx":3992
+          /* "cssm.pyx":4207
  *                 if m == num_draws:
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0             # <<<<<<<<<<<<<<
  * 
  *             if smooth:
  */
           __pyx_v_m = 0;
 
-          /* "cssm.pyx":3990
+          /* "cssm.pyx":4205
  *                 m += 1 # update rv couter
  * 
  *                 if m == num_draws:             # <<<<<<<<<<<<<<
  *                     gaussian_values = draw_gaussian(num_draws)
  *                     m = 0
  */
         }
       }
 
-      /* "cssm.pyx":3994
+      /* "cssm.pyx":4209
  *                     m = 0
  * 
  *             if smooth:             # <<<<<<<<<<<<<<
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  */
-      __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_v_smooth); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 3994, __pyx_L1_error)
+      __pyx_t_17 = __Pyx_PyObject_IsTrue(__pyx_v_smooth); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 4209, __pyx_L1_error)
       if (__pyx_t_17) {
 
-        /* "cssm.pyx":3995
+        /* "cssm.pyx":4210
  * 
  *             if smooth:
  *                 if t_h == 0.0:             # <<<<<<<<<<<<<<
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  */
         __pyx_t_17 = (__pyx_v_t_h == 0.0);
         if (__pyx_t_17) {
 
-          /* "cssm.pyx":3996
+          /* "cssm.pyx":4211
  *             if smooth:
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t             # <<<<<<<<<<<<<<
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  */
-          __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3996, __pyx_L1_error)
+          __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4211, __pyx_L1_error)
           __pyx_v_smooth_u = ((__pyx_t_22 * 0.5) * __pyx_v_delta_t);
 
-          /* "cssm.pyx":3995
+          /* "cssm.pyx":4210
  * 
  *             if smooth:
  *                 if t_h == 0.0:             # <<<<<<<<<<<<<<
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  */
           goto __pyx_L38;
         }
 
-        /* "cssm.pyx":3997
+        /* "cssm.pyx":4212
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:             # <<<<<<<<<<<<<<
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  *                 else:
  */
         __pyx_t_17 = (fmax(__pyx_v_t_h, __pyx_v_t_l) < __pyx_v_deadline_tmp);
         if (__pyx_t_17) {
 
-          /* "cssm.pyx":3998
+          /* "cssm.pyx":4213
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:
  *                     smooth_u = (0.5 - random_uniform()) * delta_t             # <<<<<<<<<<<<<<
  *                 else:
  *                     smooth_u = 0.0
  */
-          __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 3998, __pyx_L1_error)
+          __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4213, __pyx_L1_error)
           __pyx_v_smooth_u = ((0.5 - __pyx_t_22) * __pyx_v_delta_t);
 
-          /* "cssm.pyx":3997
+          /* "cssm.pyx":4212
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  *                 elif fmax(t_h, t_l) < deadline_tmp:             # <<<<<<<<<<<<<<
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  *                 else:
  */
           goto __pyx_L38;
         }
 
-        /* "cssm.pyx":4000
+        /* "cssm.pyx":4215
  *                     smooth_u = (0.5 - random_uniform()) * delta_t
  *                 else:
  *                     smooth_u = 0.0             # <<<<<<<<<<<<<<
  *             else:
  *                 smooth_u = 0.0
  */
         /*else*/ {
           __pyx_v_smooth_u = 0.0;
         }
         __pyx_L38:;
 
-        /* "cssm.pyx":3994
+        /* "cssm.pyx":4209
  *                     m = 0
  * 
  *             if smooth:             # <<<<<<<<<<<<<<
  *                 if t_h == 0.0:
  *                     smooth_u = random_uniform() * 0.5 * delta_t
  */
         goto __pyx_L37;
       }
 
-      /* "cssm.pyx":4002
+      /* "cssm.pyx":4217
  *                     smooth_u = 0.0
  *             else:
  *                 smooth_u = 0.0             # <<<<<<<<<<<<<<
  * 
  *             rts_view[n, k, 0] = fmax(t_h, t_l) + t_view[k]
  */
       /*else*/ {
         __pyx_v_smooth_u = 0.0;
       }
       __pyx_L37:;
 
-      /* "cssm.pyx":4004
+      /* "cssm.pyx":4219
  *                 smooth_u = 0.0
  * 
  *             rts_view[n, k, 0] = fmax(t_h, t_l) + t_view[k]             # <<<<<<<<<<<<<<
  * 
  *             # The probability of making a 'mistake' 1 - (relative y position)
  */
       __pyx_t_23 = __pyx_v_k;
       __pyx_t_18 = __pyx_v_n;
       __pyx_t_19 = __pyx_v_k;
       __pyx_t_25 = 0;
       *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_18 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_19 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_25 * __pyx_v_rts_view.strides[2]) )) = (fmax(__pyx_v_t_h, __pyx_v_t_l) + (*((float *) ( /* dim=0 */ (__pyx_v_t_view.data + __pyx_t_23 * __pyx_v_t_view.strides[0]) ))));
 
-      /* "cssm.pyx":4009
+      /* "cssm.pyx":4224
  *             # y at upper bound --> choices_view[n, k, 0] add one deterministically
  *             # y at lower bound --> choice_view[n, k, 0] stays the same deterministically
  *             if random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 1
  * 
  */
-      __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4009, __pyx_L1_error)
+      __pyx_t_22 = __pyx_f_4cssm_random_uniform(); if (unlikely(__pyx_t_22 == ((float)-1) && PyErr_Occurred())) __PYX_ERR(0, 4224, __pyx_L1_error)
       __pyx_t_23 = __pyx_v_ix;
       __pyx_t_25 = __pyx_v_ix;
       __pyx_t_17 = (__pyx_t_22 <= ((__pyx_v_y_l + (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_23 * __pyx_v_boundary_view.strides[0]) )))) / (2.0 * (*((float *) ( /* dim=0 */ (__pyx_v_boundary_view.data + __pyx_t_25 * __pyx_v_boundary_view.strides[0]) ))))));
       if (__pyx_t_17) {
 
-        /* "cssm.pyx":4010
+        /* "cssm.pyx":4225
  *             # y at lower bound --> choice_view[n, k, 0] stays the same deterministically
  *             if random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
  *                 choices_view[n, k, 0] += 1             # <<<<<<<<<<<<<<
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):
  */
         __pyx_t_25 = __pyx_v_n;
         __pyx_t_23 = __pyx_v_k;
         __pyx_t_19 = 0;
         *((int *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_choices_view.data + __pyx_t_25 * __pyx_v_choices_view.strides[0]) ) + __pyx_t_23 * __pyx_v_choices_view.strides[1]) ) + __pyx_t_19 * __pyx_v_choices_view.strides[2]) )) += 1;
 
-        /* "cssm.pyx":4009
+        /* "cssm.pyx":4224
  *             # y at upper bound --> choices_view[n, k, 0] add one deterministically
  *             # y at lower bound --> choice_view[n, k, 0] stays the same deterministically
  *             if random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):             # <<<<<<<<<<<<<<
  *                 choices_view[n, k, 0] += 1
  * 
  */
       }
 
-      /* "cssm.pyx":4012
+      /* "cssm.pyx":4227
  *                 choices_view[n, k, 0] += 1
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):             # <<<<<<<<<<<<<<
  *                 rts_view[n, k, 0] = -999
  * 
  */
       __pyx_t_19 = __pyx_v_n;
       __pyx_t_23 = __pyx_v_k;
       __pyx_t_25 = 0;
       __pyx_t_18 = __pyx_v_k;
       __pyx_t_26 = __pyx_v_k;
       __pyx_t_17 = (((*((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_19 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_23 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_25 * __pyx_v_rts_view.strides[2]) ))) >= (*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_18 * __pyx_v_deadline_view.strides[0]) )))) | ((*((float *) ( /* dim=0 */ (__pyx_v_deadline_view.data + __pyx_t_26 * __pyx_v_deadline_view.strides[0]) ))) <= 0.0));
       if (__pyx_t_17) {
 
-        /* "cssm.pyx":4013
+        /* "cssm.pyx":4228
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):
  *                 rts_view[n, k, 0] = -999             # <<<<<<<<<<<<<<
  * 
  *     if return_option == 'full':
  */
         __pyx_t_26 = __pyx_v_n;
         __pyx_t_18 = __pyx_v_k;
         __pyx_t_25 = 0;
         *((float *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_rts_view.data + __pyx_t_26 * __pyx_v_rts_view.strides[0]) ) + __pyx_t_18 * __pyx_v_rts_view.strides[1]) ) + __pyx_t_25 * __pyx_v_rts_view.strides[2]) )) = -999.0;
 
-        /* "cssm.pyx":4012
+        /* "cssm.pyx":4227
  *                 choices_view[n, k, 0] += 1
  * 
  *             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):             # <<<<<<<<<<<<<<
  *                 rts_view[n, k, 0] = -999
  * 
  */
       }
     }
   }
 
-  /* "cssm.pyx":4015
+  /* "cssm.pyx":4230
  *                 rts_view[n, k, 0] = -999
  * 
  *     if return_option == 'full':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'metadata': {'vh': vh,
  *                                                             'vl1': vl1,
  */
-  __pyx_t_17 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_full, Py_EQ)); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 4015, __pyx_L1_error)
+  __pyx_t_17 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_full, Py_EQ)); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 4230, __pyx_L1_error)
   if (__pyx_t_17) {
 
-    /* "cssm.pyx":4016
+    /* "cssm.pyx":4231
  * 
  *     if return_option == 'full':
  *         return {'rts': rts, 'choices': choices, 'metadata': {'vh': vh,             # <<<<<<<<<<<<<<
  *                                                             'vl1': vl1,
  *                                                             'vl2': vl2,
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4016, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4231, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_vh, ((PyObject *)__pyx_v_vh)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_vh, ((PyObject *)__pyx_v_vh)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4017
+    /* "cssm.pyx":4232
  *     if return_option == 'full':
  *         return {'rts': rts, 'choices': choices, 'metadata': {'vh': vh,
  *                                                             'vl1': vl1,             # <<<<<<<<<<<<<<
  *                                                             'vl2': vl2,
  *                                                             'a': a,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_vl1, ((PyObject *)__pyx_v_vl1)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_vl1, ((PyObject *)__pyx_v_vl1)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4018
+    /* "cssm.pyx":4233
  *         return {'rts': rts, 'choices': choices, 'metadata': {'vh': vh,
  *                                                             'vl1': vl1,
  *                                                             'vl2': vl2,             # <<<<<<<<<<<<<<
  *                                                             'a': a,
  *                                                             'zh': zh,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_vl2, ((PyObject *)__pyx_v_vl2)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_vl2, ((PyObject *)__pyx_v_vl2)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4019
+    /* "cssm.pyx":4234
  *                                                             'vl1': vl1,
  *                                                             'vl2': vl2,
  *                                                             'a': a,             # <<<<<<<<<<<<<<
  *                                                             'zh': zh,
  *                                                             'zl1': zl1,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_a, ((PyObject *)__pyx_v_a)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4020
+    /* "cssm.pyx":4235
  *                                                             'vl2': vl2,
  *                                                             'a': a,
  *                                                             'zh': zh,             # <<<<<<<<<<<<<<
  *                                                             'zl1': zl1,
  *                                                             'zl2': zl2,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_zh, ((PyObject *)__pyx_v_zh)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_zh, ((PyObject *)__pyx_v_zh)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4021
+    /* "cssm.pyx":4236
  *                                                             'a': a,
  *                                                             'zh': zh,
  *                                                             'zl1': zl1,             # <<<<<<<<<<<<<<
  *                                                             'zl2': zl2,
  *                                                             'd': d,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_zl1, ((PyObject *)__pyx_v_zl1)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_zl1, ((PyObject *)__pyx_v_zl1)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4022
+    /* "cssm.pyx":4237
  *                                                             'zh': zh,
  *                                                             'zl1': zl1,
  *                                                             'zl2': zl2,             # <<<<<<<<<<<<<<
  *                                                             'd': d,
  *                                                             't': t,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_zl2, ((PyObject *)__pyx_v_zl2)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_zl2, ((PyObject *)__pyx_v_zl2)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4023
+    /* "cssm.pyx":4238
  *                                                             'zl1': zl1,
  *                                                             'zl2': zl2,
  *                                                             'd': d,             # <<<<<<<<<<<<<<
  *                                                             't': t,
  *                                                             'deadline': deadline,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_d, ((PyObject *)__pyx_v_d)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_d, ((PyObject *)__pyx_v_d)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4024
+    /* "cssm.pyx":4239
  *                                                             'zl2': zl2,
  *                                                             'd': d,
  *                                                             't': t,             # <<<<<<<<<<<<<<
  *                                                             'deadline': deadline,
  *                                                             's': s,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_t, ((PyObject *)__pyx_v_t)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_t, ((PyObject *)__pyx_v_t)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4025
+    /* "cssm.pyx":4240
  *                                                             'd': d,
  *                                                             't': t,
  *                                                             'deadline': deadline,             # <<<<<<<<<<<<<<
  *                                                             's': s,
  *                                                             **boundary_params,
  */
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_deadline, ((PyObject *)__pyx_v_deadline)) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
 
-    /* "cssm.pyx":4026
+    /* "cssm.pyx":4241
  *                                                             't': t,
  *                                                             'deadline': deadline,
  *                                                             's': s,             # <<<<<<<<<<<<<<
  *                                                             **boundary_params,
  *                                                             'delta_t': delta_t,
  */
-    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_s); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4026, __pyx_L1_error)
+    __pyx_t_4 = PyFloat_FromDouble(__pyx_v_s); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 4241, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_s, __pyx_t_4) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_u_s, __pyx_t_4) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_9 = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4027
+    /* "cssm.pyx":4242
  *                                                             'deadline': deadline,
  *                                                             's': s,
  *                                                             **boundary_params,             # <<<<<<<<<<<<<<
  *                                                             'delta_t': delta_t,
  *                                                             'max_t': max_t,
  */
     if (unlikely(__pyx_v_boundary_params == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument after ** must be a mapping, not NoneType");
-      __PYX_ERR(0, 4027, __pyx_L1_error)
+      __PYX_ERR(0, 4242, __pyx_L1_error)
     }
     if (unlikely(PyDict_Update(__pyx_t_9, __pyx_v_boundary_params) < 0)) {
       if (PyErr_ExceptionMatches(PyExc_AttributeError)) __Pyx_RaiseMappingExpectedError(__pyx_v_boundary_params);
-      __PYX_ERR(0, 4027, __pyx_L1_error)
+      __PYX_ERR(0, 4242, __pyx_L1_error)
     }
 
-    /* "cssm.pyx":4028
+    /* "cssm.pyx":4243
  *                                                             's': s,
  *                                                             **boundary_params,
  *                                                             'delta_t': delta_t,             # <<<<<<<<<<<<<<
  *                                                             'max_t': max_t,
  *                                                             'n_samples': n_samples,
  */
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4028, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4243, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_delta_t, __pyx_t_3) < 0) __PYX_ERR(0, 4028, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_delta_t, __pyx_t_3) < 0) __PYX_ERR(0, 4243, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4029
+    /* "cssm.pyx":4244
  *                                                             **boundary_params,
  *                                                             'delta_t': delta_t,
  *                                                             'max_t': max_t,             # <<<<<<<<<<<<<<
  *                                                             'n_samples': n_samples,
  *                                                             'n_trials': n_trials,
  */
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4029, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_max_t); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4244, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_max_t, __pyx_t_3) < 0) __PYX_ERR(0, 4029, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_max_t, __pyx_t_3) < 0) __PYX_ERR(0, 4244, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4030
+    /* "cssm.pyx":4245
  *                                                             'delta_t': delta_t,
  *                                                             'max_t': max_t,
  *                                                             'n_samples': n_samples,             # <<<<<<<<<<<<<<
  *                                                             'n_trials': n_trials,
  *                                                             'simulator': 'ddm_flexbound_mic2_adj',
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4030, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4245, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_samples, __pyx_t_3) < 0) __PYX_ERR(0, 4030, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_samples, __pyx_t_3) < 0) __PYX_ERR(0, 4245, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4031
+    /* "cssm.pyx":4246
  *                                                             'max_t': max_t,
  *                                                             'n_samples': n_samples,
  *                                                             'n_trials': n_trials,             # <<<<<<<<<<<<<<
  *                                                             'simulator': 'ddm_flexbound_mic2_adj',
  *                                                             'boundary_fun_type': boundary_fun.__name__,
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4031, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_trials, __pyx_t_3) < 0) __PYX_ERR(0, 4031, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_trials, __pyx_t_3) < 0) __PYX_ERR(0, 4246, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 4032, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 4247, __pyx_L1_error)
 
-    /* "cssm.pyx":4033
+    /* "cssm.pyx":4248
  *                                                             'n_trials': n_trials,
  *                                                             'simulator': 'ddm_flexbound_mic2_adj',
  *                                                             'boundary_fun_type': boundary_fun.__name__,             # <<<<<<<<<<<<<<
  *                                                             'possible_choices': [0, 1, 2, 3],
  *                                                             'trajectory': 'This simulator does not yet allow for trajectory simulation',
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4033, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_boundary_fun_type, __pyx_t_3) < 0) __PYX_ERR(0, 4033, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_boundary_fun_type, __pyx_t_3) < 0) __PYX_ERR(0, 4248, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4034
+    /* "cssm.pyx":4249
  *                                                             'simulator': 'ddm_flexbound_mic2_adj',
  *                                                             'boundary_fun_type': boundary_fun.__name__,
  *                                                             'possible_choices': [0, 1, 2, 3],             # <<<<<<<<<<<<<<
  *                                                             'trajectory': 'This simulator does not yet allow for trajectory simulation',
  *                                                             'boundary': boundary}}
  */
-    __pyx_t_3 = PyList_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4034, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_0)) __PYX_ERR(0, 4034, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_0)) __PYX_ERR(0, 4249, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_int_1)) __PYX_ERR(0, 4034, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_int_1)) __PYX_ERR(0, 4249, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_int_2)) __PYX_ERR(0, 4034, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_int_2)) __PYX_ERR(0, 4249, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 3, __pyx_int_3)) __PYX_ERR(0, 4034, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_possible_choices, __pyx_t_3) < 0) __PYX_ERR(0, 4034, __pyx_L1_error)
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 3, __pyx_int_3)) __PYX_ERR(0, 4249, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_possible_choices, __pyx_t_3) < 0) __PYX_ERR(0, 4249, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_trajectory, __pyx_kp_u_This_simulator_does_not_yet_allo) < 0) __PYX_ERR(0, 4035, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_trajectory, __pyx_kp_u_This_simulator_does_not_yet_allo) < 0) __PYX_ERR(0, 4250, __pyx_L1_error)
 
-    /* "cssm.pyx":4036
+    /* "cssm.pyx":4251
  *                                                             'possible_choices': [0, 1, 2, 3],
  *                                                             'trajectory': 'This simulator does not yet allow for trajectory simulation',
  *                                                             'boundary': boundary}}             # <<<<<<<<<<<<<<
  *     elif return_option == 'minimal':
  *         return {'rts': rts, 'choices': choices, 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  */
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_boundary, __pyx_v_boundary) < 0) __PYX_ERR(0, 4036, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_9) < 0) __PYX_ERR(0, 4016, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_boundary, __pyx_v_boundary) < 0) __PYX_ERR(0, 4251, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_9) < 0) __PYX_ERR(0, 4231, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "cssm.pyx":4015
+    /* "cssm.pyx":4230
  *                 rts_view[n, k, 0] = -999
  * 
  *     if return_option == 'full':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'metadata': {'vh': vh,
  *                                                             'vl1': vl1,
  */
   }
 
-  /* "cssm.pyx":4037
+  /* "cssm.pyx":4252
  *                                                             'trajectory': 'This simulator does not yet allow for trajectory simulation',
  *                                                             'boundary': boundary}}
  *     elif return_option == 'minimal':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                                                              'possible_choices': [0, 1, 2, 3],
  */
-  __pyx_t_17 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_minimal, Py_EQ)); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 4037, __pyx_L1_error)
+  __pyx_t_17 = (__Pyx_PyUnicode_Equals(__pyx_v_return_option, __pyx_n_u_minimal, Py_EQ)); if (unlikely((__pyx_t_17 < 0))) __PYX_ERR(0, 4252, __pyx_L1_error)
   if (likely(__pyx_t_17)) {
 
-    /* "cssm.pyx":4038
+    /* "cssm.pyx":4253
  *                                                             'boundary': boundary}}
  *     elif return_option == 'minimal':
  *         return {'rts': rts, 'choices': choices, 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',             # <<<<<<<<<<<<<<
  *                                                              'possible_choices': [0, 1, 2, 3],
  *                                                              'boundary_fun_type': boundary_fun.__name__,
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4038, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
-    __pyx_t_9 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_rts, __pyx_v_rts) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_choices, __pyx_v_choices) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyDict_NewPresized(5); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_simulator, __pyx_n_u_ddm_flexbound_mic2_adj) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
 
-    /* "cssm.pyx":4039
+    /* "cssm.pyx":4254
  *     elif return_option == 'minimal':
  *         return {'rts': rts, 'choices': choices, 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                                                              'possible_choices': [0, 1, 2, 3],             # <<<<<<<<<<<<<<
  *                                                              'boundary_fun_type': boundary_fun.__name__,
  *                                                              'n_samples': n_samples,
  */
-    __pyx_t_3 = PyList_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4039, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4254, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_0)) __PYX_ERR(0, 4039, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_int_0)) __PYX_ERR(0, 4254, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_int_1)) __PYX_ERR(0, 4039, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_int_1)) __PYX_ERR(0, 4254, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_int_2)) __PYX_ERR(0, 4039, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 2, __pyx_int_2)) __PYX_ERR(0, 4254, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 3, __pyx_int_3)) __PYX_ERR(0, 4039, __pyx_L1_error);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_possible_choices, __pyx_t_3) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 3, __pyx_int_3)) __PYX_ERR(0, 4254, __pyx_L1_error);
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_possible_choices, __pyx_t_3) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4040
+    /* "cssm.pyx":4255
  *         return {'rts': rts, 'choices': choices, 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                                                              'possible_choices': [0, 1, 2, 3],
  *                                                              'boundary_fun_type': boundary_fun.__name__,             # <<<<<<<<<<<<<<
  *                                                              'n_samples': n_samples,
  *                                                              'n_trials': n_trials,
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4040, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_boundary_fun, __pyx_n_s_name_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4255, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_boundary_fun_type, __pyx_t_3) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_boundary_fun_type, __pyx_t_3) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4041
+    /* "cssm.pyx":4256
  *                                                              'possible_choices': [0, 1, 2, 3],
  *                                                              'boundary_fun_type': boundary_fun.__name__,
  *                                                              'n_samples': n_samples,             # <<<<<<<<<<<<<<
  *                                                              'n_trials': n_trials,
  *                                                              }}
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4041, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_samples); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_samples, __pyx_t_3) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_samples, __pyx_t_3) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "cssm.pyx":4042
+    /* "cssm.pyx":4257
  *                                                              'boundary_fun_type': boundary_fun.__name__,
  *                                                              'n_samples': n_samples,
  *                                                              'n_trials': n_trials,             # <<<<<<<<<<<<<<
  *                                                              }}
  *     else:
  */
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4042, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_n_trials); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 4257, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_trials, __pyx_t_3) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_9, __pyx_n_u_n_trials, __pyx_t_3) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_9) < 0) __PYX_ERR(0, 4038, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_5, __pyx_n_u_metadata, __pyx_t_9) < 0) __PYX_ERR(0, 4253, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "cssm.pyx":4037
+    /* "cssm.pyx":4252
  *                                                             'trajectory': 'This simulator does not yet allow for trajectory simulation',
  *                                                             'boundary': boundary}}
  *     elif return_option == 'minimal':             # <<<<<<<<<<<<<<
  *         return {'rts': rts, 'choices': choices, 'metadata': {'simulator': 'ddm_flexbound_mic2_adj',
  *                                                              'possible_choices': [0, 1, 2, 3],
  */
   }
 
-  /* "cssm.pyx":4045
+  /* "cssm.pyx":4260
  *                                                              }}
  *     else:
  *         raise ValueError('return_option must be either "full" or "minimal"')             # <<<<<<<<<<<<<<
  * # -----------------------------------------------------------------------------------------------
  */
   /*else*/ {
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4045, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 4260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 4045, __pyx_L1_error)
+    __PYX_ERR(0, 4260, __pyx_L1_error)
   }
 
-  /* "cssm.pyx":3839
+  /* "cssm.pyx":4054
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_tradeoff(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                            np.ndarray[float, ndim = 1] vl1,
  *                            np.ndarray[float, ndim = 1] vl2,
  */
 
@@ -70851,29 +75025,31 @@
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
-    {&__pyx_n_s__60, __pyx_k__60, sizeof(__pyx_k__60), 0, 0, 1, 1},
+    {&__pyx_n_s__66, __pyx_k__66, sizeof(__pyx_k__66), 0, 0, 1, 1},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
     {&__pyx_n_u_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 1, 0, 1},
     {&__pyx_n_s_a_view, __pyx_k_a_view, sizeof(__pyx_k_a_view), 0, 0, 1, 1},
     {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
+    {&__pyx_n_s_abs, __pyx_k_abs, sizeof(__pyx_k_abs), 0, 0, 1, 1},
     {&__pyx_n_s_add, __pyx_k_add, sizeof(__pyx_k_add), 0, 0, 1, 1},
     {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
     {&__pyx_n_s_alpha, __pyx_k_alpha, sizeof(__pyx_k_alpha), 0, 0, 1, 1},
     {&__pyx_n_u_alpha, __pyx_k_alpha, sizeof(__pyx_k_alpha), 0, 1, 0, 1},
     {&__pyx_n_s_alpha_stable_values, __pyx_k_alpha_stable_values, sizeof(__pyx_k_alpha_stable_values), 0, 0, 1, 1},
     {&__pyx_n_s_alpha_view, __pyx_k_alpha_view, sizeof(__pyx_k_alpha_view), 0, 0, 1, 1},
     {&__pyx_kp_u_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 1, 0, 0},
     {&__pyx_n_s_arange, __pyx_k_arange, sizeof(__pyx_k_arange), 0, 0, 1, 1},
     {&__pyx_n_s_argmax, __pyx_k_argmax, sizeof(__pyx_k_argmax), 0, 0, 1, 1},
+    {&__pyx_n_s_argmin, __pyx_k_argmin, sizeof(__pyx_k_argmin), 0, 0, 1, 1},
     {&__pyx_n_s_astype, __pyx_k_astype, sizeof(__pyx_k_astype), 0, 0, 1, 1},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
     {&__pyx_n_u_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 1, 0, 1},
     {&__pyx_n_s_b_view, __pyx_k_b_view, sizeof(__pyx_k_b_view), 0, 0, 1, 1},
     {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
     {&__pyx_n_s_bias_trace, __pyx_k_bias_trace, sizeof(__pyx_k_bias_trace), 0, 0, 1, 1},
@@ -70985,38 +75161,46 @@
     {&__pyx_n_s_ix_l, __pyx_k_ix_l, sizeof(__pyx_k_ix_l), 0, 0, 1, 1},
     {&__pyx_n_s_ix_tmp, __pyx_k_ix_tmp, sizeof(__pyx_k_ix_tmp), 0, 0, 1, 1},
     {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
     {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
     {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
     {&__pyx_n_s_keys, __pyx_k_keys, sizeof(__pyx_k_keys), 0, 0, 1, 1},
     {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
+    {&__pyx_n_s_lba_angle, __pyx_k_lba_angle, sizeof(__pyx_k_lba_angle), 0, 0, 1, 1},
+    {&__pyx_n_u_lba_angle, __pyx_k_lba_angle, sizeof(__pyx_k_lba_angle), 0, 1, 0, 1},
+    {&__pyx_n_s_lba_vanilla, __pyx_k_lba_vanilla, sizeof(__pyx_k_lba_vanilla), 0, 0, 1, 1},
+    {&__pyx_n_u_lba_vanilla, __pyx_k_lba_vanilla, sizeof(__pyx_k_lba_vanilla), 0, 1, 0, 1},
     {&__pyx_n_s_lca, __pyx_k_lca, sizeof(__pyx_k_lca), 0, 0, 1, 1},
     {&__pyx_n_u_lca, __pyx_k_lca, sizeof(__pyx_k_lca), 0, 1, 0, 1},
     {&__pyx_n_s_levy_flexbound, __pyx_k_levy_flexbound, sizeof(__pyx_k_levy_flexbound), 0, 0, 1, 1},
     {&__pyx_n_u_levy_flexbound, __pyx_k_levy_flexbound, sizeof(__pyx_k_levy_flexbound), 0, 1, 0, 1},
     {&__pyx_n_s_m, __pyx_k_m, sizeof(__pyx_k_m), 0, 0, 1, 1},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_max_t, __pyx_k_max_t, sizeof(__pyx_k_max_t), 0, 0, 1, 1},
     {&__pyx_n_u_max_t, __pyx_k_max_t, sizeof(__pyx_k_max_t), 0, 1, 0, 1},
     {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
     {&__pyx_n_u_metadata, __pyx_k_metadata, sizeof(__pyx_k_metadata), 0, 1, 0, 1},
+    {&__pyx_n_s_min, __pyx_k_min, sizeof(__pyx_k_min), 0, 0, 1, 1},
     {&__pyx_n_u_minimal, __pyx_k_minimal, sizeof(__pyx_k_minimal), 0, 1, 0, 1},
     {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
     {&__pyx_n_s_multiply, __pyx_k_multiply, sizeof(__pyx_k_multiply), 0, 0, 1, 1},
     {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
     {&__pyx_n_s_n_particles, __pyx_k_n_particles, sizeof(__pyx_k_n_particles), 0, 0, 1, 1},
     {&__pyx_n_s_n_samples, __pyx_k_n_samples, sizeof(__pyx_k_n_samples), 0, 0, 1, 1},
     {&__pyx_n_u_n_samples, __pyx_k_n_samples, sizeof(__pyx_k_n_samples), 0, 1, 0, 1},
     {&__pyx_n_s_n_trials, __pyx_k_n_trials, sizeof(__pyx_k_n_trials), 0, 0, 1, 1},
     {&__pyx_n_u_n_trials, __pyx_k_n_trials, sizeof(__pyx_k_n_trials), 0, 1, 0, 1},
+    {&__pyx_n_s_nact, __pyx_k_nact, sizeof(__pyx_k_nact), 0, 0, 1, 1},
     {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
     {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
     {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
+    {&__pyx_n_s_ndt, __pyx_k_ndt, sizeof(__pyx_k_ndt), 0, 0, 1, 1},
     {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
     {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
+    {&__pyx_n_s_normal, __pyx_k_normal, sizeof(__pyx_k_normal), 0, 0, 1, 1},
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_num_draws, __pyx_k_num_draws, sizeof(__pyx_k_num_draws), 0, 0, 1, 1},
     {&__pyx_n_s_num_steps, __pyx_k_num_steps, sizeof(__pyx_k_num_steps), 0, 0, 1, 1},
     {&__pyx_n_s_numbers, __pyx_k_numbers, sizeof(__pyx_k_numbers), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
     {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
     {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
@@ -71037,22 +75221,25 @@
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
     {&__pyx_n_s_race_model, __pyx_k_race_model, sizeof(__pyx_k_race_model), 0, 0, 1, 1},
     {&__pyx_n_u_race_model, __pyx_k_race_model, sizeof(__pyx_k_race_model), 0, 1, 0, 1},
+    {&__pyx_n_s_random, __pyx_k_random, sizeof(__pyx_k_random), 0, 0, 1, 1},
     {&__pyx_n_s_random_state, __pyx_k_random_state, sizeof(__pyx_k_random_state), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
     {&__pyx_n_s_register, __pyx_k_register, sizeof(__pyx_k_register), 0, 0, 1, 1},
     {&__pyx_n_s_return_option, __pyx_k_return_option, sizeof(__pyx_k_return_option), 0, 0, 1, 1},
     {&__pyx_kp_u_return_option_must_be_either_ful, __pyx_k_return_option_must_be_either_ful, sizeof(__pyx_k_return_option_must_be_either_ful), 0, 1, 0, 0},
+    {&__pyx_n_s_rlwm_lba_race, __pyx_k_rlwm_lba_race, sizeof(__pyx_k_rlwm_lba_race), 0, 0, 1, 1},
+    {&__pyx_n_u_rlwm_lba_race, __pyx_k_rlwm_lba_race, sizeof(__pyx_k_rlwm_lba_race), 0, 1, 0, 1},
     {&__pyx_n_s_rts, __pyx_k_rts, sizeof(__pyx_k_rts), 0, 0, 1, 1},
     {&__pyx_n_u_rts, __pyx_k_rts, sizeof(__pyx_k_rts), 0, 1, 0, 1},
     {&__pyx_n_s_rts_high, __pyx_k_rts_high, sizeof(__pyx_k_rts_high), 0, 0, 1, 1},
     {&__pyx_n_u_rts_high, __pyx_k_rts_high, sizeof(__pyx_k_rts_high), 0, 1, 0, 1},
     {&__pyx_n_s_rts_high_view, __pyx_k_rts_high_view, sizeof(__pyx_k_rts_high_view), 0, 0, 1, 1},
     {&__pyx_n_s_rts_low, __pyx_k_rts_low, sizeof(__pyx_k_rts_low), 0, 0, 1, 1},
     {&__pyx_n_u_rts_low, __pyx_k_rts_low, sizeof(__pyx_k_rts_low), 0, 1, 0, 1},
@@ -71060,14 +75247,16 @@
     {&__pyx_n_s_rts_view, __pyx_k_rts_view, sizeof(__pyx_k_rts_view), 0, 0, 1, 1},
     {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
     {&__pyx_n_u_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 1, 0, 1},
     {&__pyx_n_s_s_pre_high_level_choice, __pyx_k_s_pre_high_level_choice, sizeof(__pyx_k_s_pre_high_level_choice), 0, 0, 1, 1},
     {&__pyx_n_u_s_pre_high_level_choice, __pyx_k_s_pre_high_level_choice, sizeof(__pyx_k_s_pre_high_level_choice), 0, 1, 0, 1},
     {&__pyx_n_s_s_pre_high_level_choice_view, __pyx_k_s_pre_high_level_choice_view, sizeof(__pyx_k_s_pre_high_level_choice_view), 0, 0, 1, 1},
     {&__pyx_n_s_s_view, __pyx_k_s_view, sizeof(__pyx_k_s_view), 0, 0, 1, 1},
+    {&__pyx_n_s_sd, __pyx_k_sd, sizeof(__pyx_k_sd), 0, 0, 1, 1},
+    {&__pyx_n_u_sd, __pyx_k_sd, sizeof(__pyx_k_sd), 0, 1, 0, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
     {&__pyx_n_s_sign, __pyx_k_sign, sizeof(__pyx_k_sign), 0, 0, 1, 1},
     {&__pyx_n_u_simulator, __pyx_k_simulator, sizeof(__pyx_k_simulator), 0, 1, 0, 1},
     {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
     {&__pyx_n_s_smooth, __pyx_k_smooth, sizeof(__pyx_k_smooth), 0, 0, 1, 1},
@@ -71104,27 +75293,39 @@
     {&__pyx_n_s_t_par, __pyx_k_t_par, sizeof(__pyx_k_t_par), 0, 0, 1, 1},
     {&__pyx_n_s_t_particle, __pyx_k_t_particle, sizeof(__pyx_k_t_particle), 0, 0, 1, 1},
     {&__pyx_n_s_t_particle1, __pyx_k_t_particle1, sizeof(__pyx_k_t_particle1), 0, 0, 1, 1},
     {&__pyx_n_s_t_particle2, __pyx_k_t_particle2, sizeof(__pyx_k_t_particle2), 0, 0, 1, 1},
     {&__pyx_n_s_t_s, __pyx_k_t_s, sizeof(__pyx_k_t_s), 0, 0, 1, 1},
     {&__pyx_n_s_t_tmp, __pyx_k_t_tmp, sizeof(__pyx_k_t_tmp), 0, 0, 1, 1},
     {&__pyx_n_s_t_view, __pyx_k_t_view, sizeof(__pyx_k_t_view), 0, 0, 1, 1},
+    {&__pyx_n_s_tan, __pyx_k_tan, sizeof(__pyx_k_tan), 0, 0, 1, 1},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_test2, __pyx_k_test2, sizeof(__pyx_k_test2), 0, 0, 1, 1},
     {&__pyx_n_s_test_2, __pyx_k_test_2, sizeof(__pyx_k_test_2), 0, 0, 1, 1},
+    {&__pyx_n_s_theta, __pyx_k_theta, sizeof(__pyx_k_theta), 0, 0, 1, 1},
+    {&__pyx_n_u_theta, __pyx_k_theta, sizeof(__pyx_k_theta), 0, 1, 0, 1},
+    {&__pyx_n_s_theta_view, __pyx_k_theta_view, sizeof(__pyx_k_theta_view), 0, 0, 1, 1},
     {&__pyx_n_s_tmp_pos_dep, __pyx_k_tmp_pos_dep, sizeof(__pyx_k_tmp_pos_dep), 0, 0, 1, 1},
     {&__pyx_n_s_traj, __pyx_k_traj, sizeof(__pyx_k_traj), 0, 0, 1, 1},
     {&__pyx_n_s_traj_view, __pyx_k_traj_view, sizeof(__pyx_k_traj_view), 0, 0, 1, 1},
     {&__pyx_n_u_trajectory, __pyx_k_trajectory, sizeof(__pyx_k_trajectory), 0, 1, 0, 1},
     {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
     {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
+    {&__pyx_n_s_uniform, __pyx_k_uniform, sizeof(__pyx_k_uniform), 0, 0, 1, 1},
     {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
     {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
     {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
     {&__pyx_n_u_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 1, 0, 1},
+    {&__pyx_n_u_v_2, __pyx_k_v_2, sizeof(__pyx_k_v_2), 0, 1, 0, 1},
+    {&__pyx_n_s_v_RL, __pyx_k_v_RL, sizeof(__pyx_k_v_RL), 0, 0, 1, 1},
+    {&__pyx_n_u_v_RL_2, __pyx_k_v_RL_2, sizeof(__pyx_k_v_RL_2), 0, 1, 0, 1},
+    {&__pyx_n_s_v_RL_view, __pyx_k_v_RL_view, sizeof(__pyx_k_v_RL_view), 0, 0, 1, 1},
+    {&__pyx_n_s_v_WM, __pyx_k_v_WM, sizeof(__pyx_k_v_WM), 0, 0, 1, 1},
+    {&__pyx_n_u_v_WM_2, __pyx_k_v_WM_2, sizeof(__pyx_k_v_WM_2), 0, 1, 0, 1},
+    {&__pyx_n_s_v_WM_view, __pyx_k_v_WM_view, sizeof(__pyx_k_v_WM_view), 0, 0, 1, 1},
     {&__pyx_n_s_v_dict, __pyx_k_v_dict, sizeof(__pyx_k_v_dict), 0, 0, 1, 1},
     {&__pyx_n_s_v_l, __pyx_k_v_l, sizeof(__pyx_k_v_l), 0, 0, 1, 1},
     {&__pyx_n_s_v_l1, __pyx_k_v_l1, sizeof(__pyx_k_v_l1), 0, 0, 1, 1},
     {&__pyx_n_s_v_l2, __pyx_k_v_l2, sizeof(__pyx_k_v_l2), 0, 0, 1, 1},
     {&__pyx_n_s_v_view, __pyx_k_v_view, sizeof(__pyx_k_v_view), 0, 0, 1, 1},
     {&__pyx_n_s_version_info, __pyx_k_version_info, sizeof(__pyx_k_version_info), 0, 0, 1, 1},
     {&__pyx_n_s_vh, __pyx_k_vh, sizeof(__pyx_k_vh), 0, 0, 1, 1},
@@ -71132,14 +75333,20 @@
     {&__pyx_n_s_vh_view, __pyx_k_vh_view, sizeof(__pyx_k_vh_view), 0, 0, 1, 1},
     {&__pyx_n_s_vl1, __pyx_k_vl1, sizeof(__pyx_k_vl1), 0, 0, 1, 1},
     {&__pyx_n_u_vl1, __pyx_k_vl1, sizeof(__pyx_k_vl1), 0, 1, 0, 1},
     {&__pyx_n_s_vl1_view, __pyx_k_vl1_view, sizeof(__pyx_k_vl1_view), 0, 0, 1, 1},
     {&__pyx_n_s_vl2, __pyx_k_vl2, sizeof(__pyx_k_vl2), 0, 0, 1, 1},
     {&__pyx_n_u_vl2, __pyx_k_vl2, sizeof(__pyx_k_vl2), 0, 1, 0, 1},
     {&__pyx_n_s_vl2_view, __pyx_k_vl2_view, sizeof(__pyx_k_vl2_view), 0, 0, 1, 1},
+    {&__pyx_n_s_vs, __pyx_k_vs, sizeof(__pyx_k_vs), 0, 0, 1, 1},
+    {&__pyx_n_s_vs_RL, __pyx_k_vs_RL, sizeof(__pyx_k_vs_RL), 0, 0, 1, 1},
+    {&__pyx_n_s_vs_WM, __pyx_k_vs_WM, sizeof(__pyx_k_vs_WM), 0, 0, 1, 1},
+    {&__pyx_n_s_x_t, __pyx_k_x_t, sizeof(__pyx_k_x_t), 0, 0, 1, 1},
+    {&__pyx_n_s_x_t_RL, __pyx_k_x_t_RL, sizeof(__pyx_k_x_t_RL), 0, 0, 1, 1},
+    {&__pyx_n_s_x_t_WM, __pyx_k_x_t_WM, sizeof(__pyx_k_x_t_WM), 0, 0, 1, 1},
     {&__pyx_n_s_y, __pyx_k_y, sizeof(__pyx_k_y), 0, 0, 1, 1},
     {&__pyx_n_s_y_h, __pyx_k_y_h, sizeof(__pyx_k_y_h), 0, 0, 1, 1},
     {&__pyx_n_s_y_l, __pyx_k_y_l, sizeof(__pyx_k_y_l), 0, 0, 1, 1},
     {&__pyx_n_s_y_l1, __pyx_k_y_l1, sizeof(__pyx_k_y_l1), 0, 0, 1, 1},
     {&__pyx_n_s_y_l2, __pyx_k_y_l2, sizeof(__pyx_k_y_l2), 0, 0, 1, 1},
     {&__pyx_n_s_z, __pyx_k_z, sizeof(__pyx_k_z), 0, 0, 1, 1},
     {&__pyx_n_u_z, __pyx_k_z, sizeof(__pyx_k_z), 0, 1, 0, 1},
@@ -71151,14 +75358,15 @@
     {&__pyx_n_s_zh_view, __pyx_k_zh_view, sizeof(__pyx_k_zh_view), 0, 0, 1, 1},
     {&__pyx_n_s_zl1, __pyx_k_zl1, sizeof(__pyx_k_zl1), 0, 0, 1, 1},
     {&__pyx_n_u_zl1, __pyx_k_zl1, sizeof(__pyx_k_zl1), 0, 1, 0, 1},
     {&__pyx_n_s_zl1_view, __pyx_k_zl1_view, sizeof(__pyx_k_zl1_view), 0, 0, 1, 1},
     {&__pyx_n_s_zl2, __pyx_k_zl2, sizeof(__pyx_k_zl2), 0, 0, 1, 1},
     {&__pyx_n_u_zl2, __pyx_k_zl2, sizeof(__pyx_k_zl2), 0, 1, 0, 1},
     {&__pyx_n_s_zl2_view, __pyx_k_zl2_view, sizeof(__pyx_k_zl2_view), 0, 0, 1, 1},
+    {&__pyx_n_s_zs, __pyx_k_zs, sizeof(__pyx_k_zs), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 56, __pyx_L1_error)
@@ -71214,26 +75422,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-hclv6q0_/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-r0fkycoy/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
@@ -71560,34 +75768,70 @@
  *                                            np.ndarray[float, ndim = 1] vl2,
  */
   __pyx_tuple__55 = PyTuple_Pack(81, __pyx_n_s_vh, __pyx_n_s_vl1, __pyx_n_s_vl2, __pyx_n_s_a, __pyx_n_s_zh, __pyx_n_s_zl1, __pyx_n_s_zl2, __pyx_n_s_d, __pyx_n_s_g, __pyx_n_s_t, __pyx_n_s_deadline, __pyx_n_s_s, __pyx_n_s_delta_t, __pyx_n_s_max_t, __pyx_n_s_n_samples, __pyx_n_s_n_trials, __pyx_n_s_print_info, __pyx_n_s_boundary_fun, __pyx_n_s_boundary_multiplicative, __pyx_n_s_boundary_params, __pyx_n_s_random_state, __pyx_n_s_return_option, __pyx_n_s_smooth, __pyx_n_s_kwargs, __pyx_n_s_vh_view, __pyx_n_s_vl1_view, __pyx_n_s_vl2_view, __pyx_n_s_a_view, __pyx_n_s_zh_view, __pyx_n_s_zl1_view, __pyx_n_s_zl2_view, __pyx_n_s_d_view, __pyx_n_s_g_view, __pyx_n_s_t_view, __pyx_n_s_deadline_view, __pyx_n_s_rts, __pyx_n_s_choices, __pyx_n_s_rts_low, __pyx_n_s_rts_high, __pyx_n_s_rts_view, __pyx_n_s_rts_high_view, __pyx_n_s_rts_low_view, __pyx_n_s_choices_view, __pyx_n_s_traj, __pyx_n_s_traj_view, __pyx_n_s_delta_t_sqrt, __pyx_n_s_sqrt_st, __pyx_n_s_num_draws, __pyx_n_s_t_s, __pyx_n_s_boundary, __pyx_n_s_boundary_view, __pyx_n_s_bias_trace_l1, __pyx_n_s_bias_trace_l2, __pyx_n_s_bias_trace_l1_view, __pyx_n_s_bias_trace_l2_view, __pyx_n_s_y_h, __pyx_n_s_y_l, __pyx_n_s_y_l1, __pyx_n_s_y_l2, __pyx_n_s_v_l, __pyx_n_s_v_l1, __pyx_n_s_v_l2, __pyx_n_s_t_h, __pyx_n_s_t_l, __pyx_n_s_t_l1, __pyx_n_s_t_l2, __pyx_n_s_smooth_u, __pyx_n_s_deadline_tmp, __pyx_n_s_n, __pyx_n_s_ix, __pyx_n_s_ix1, __pyx_n_s_ix2, __pyx_n_s_ix_l, __pyx_n_s_ix_tmp, __pyx_n_s_ix1_tmp, __pyx_n_s_ix2_tmp, __pyx_n_s_k, __pyx_n_s_m, __pyx_n_s_gaussian_values, __pyx_n_s_boundary_params_tmp, __pyx_n_s_key); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 3046, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
   __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(23, 0, 0, 81, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_ddm_flexbound_mic2_ornstein_mult, 3046, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 3046, __pyx_L1_error)
 
-  /* "cssm.pyx":3328
+  /* "cssm.pyx":3327
+ * 
+ * # Simulate (rt, choice) tuples from: Vanilla LBA Model without ndt -----------------------------
+ * def lba_vanilla(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+  __pyx_tuple__57 = PyTuple_Pack(26, __pyx_n_s_v, __pyx_n_s_a, __pyx_n_s_z, __pyx_n_s_deadline, __pyx_n_s_sd, __pyx_n_s_ndt, __pyx_n_s_nact, __pyx_n_s_n_samples, __pyx_n_s_n_trials, __pyx_n_s_max_t, __pyx_n_s_kwargs, __pyx_n_s_v_view, __pyx_n_s_a_view, __pyx_n_s_z_view, __pyx_n_s_deadline_view, __pyx_n_s_rts, __pyx_n_s_rts_view, __pyx_n_s_choices, __pyx_n_s_choices_view, __pyx_n_s_n, __pyx_n_s_k, __pyx_n_s_i, __pyx_n_s_zs, __pyx_n_s_vs, __pyx_n_s_x_t, __pyx_n_s_v_dict); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__57);
+  __Pyx_GIVEREF(__pyx_tuple__57);
+  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(10, 0, 0, 26, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_lba_vanilla, 3327, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 3327, __pyx_L1_error)
+
+  /* "cssm.pyx":3394
+ * 
+ * # Simulate (rt, choice) tuples from: Collapsing bound angle LBA Model -----------------------------
+ * def lba_angle(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+  __pyx_tuple__59 = PyTuple_Pack(28, __pyx_n_s_v, __pyx_n_s_a, __pyx_n_s_z, __pyx_n_s_theta, __pyx_n_s_deadline, __pyx_n_s_sd, __pyx_n_s_ndt, __pyx_n_s_nact, __pyx_n_s_n_samples, __pyx_n_s_n_trials, __pyx_n_s_max_t, __pyx_n_s_kwargs, __pyx_n_s_v_view, __pyx_n_s_a_view, __pyx_n_s_z_view, __pyx_n_s_theta_view, __pyx_n_s_deadline_view, __pyx_n_s_rts, __pyx_n_s_rts_view, __pyx_n_s_choices, __pyx_n_s_choices_view, __pyx_n_s_n, __pyx_n_s_k, __pyx_n_s_i, __pyx_n_s_zs, __pyx_n_s_vs, __pyx_n_s_x_t, __pyx_n_s_v_dict); if (unlikely(!__pyx_tuple__59)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__59);
+  __Pyx_GIVEREF(__pyx_tuple__59);
+  __pyx_codeobj__60 = (PyObject*)__Pyx_PyCode_New(11, 0, 0, 28, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__59, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_lba_angle, 3394, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__60)) __PYX_ERR(0, 3394, __pyx_L1_error)
+
+  /* "cssm.pyx":3460
+ * 
+ * # Simulate (rt, choice) tuples from: RLWM LBA Race Model without ndt -----------------------------
+ * def rlwm_lba_race(np.ndarray[float, ndim = 2] v_RL, # RL drift parameters (np.array expect: one column of floats)             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] v_WM, # WM drift parameters (np.array expect: one column of floats)
+ *         np.ndarray[float, ndim = 2] a, # criterion height
+ */
+  __pyx_tuple__61 = PyTuple_Pack(30, __pyx_n_s_v_RL, __pyx_n_s_v_WM, __pyx_n_s_a, __pyx_n_s_z, __pyx_n_s_deadline, __pyx_n_s_sd, __pyx_n_s_ndt, __pyx_n_s_nact, __pyx_n_s_n_samples, __pyx_n_s_n_trials, __pyx_n_s_max_t, __pyx_n_s_kwargs, __pyx_n_s_v_RL_view, __pyx_n_s_v_WM_view, __pyx_n_s_a_view, __pyx_n_s_z_view, __pyx_n_s_deadline_view, __pyx_n_s_zs, __pyx_n_s_x_t_RL, __pyx_n_s_x_t_WM, __pyx_n_s_vs_RL, __pyx_n_s_vs_WM, __pyx_n_s_rts, __pyx_n_s_rts_view, __pyx_n_s_choices, __pyx_n_s_choices_view, __pyx_n_s_n, __pyx_n_s_k, __pyx_n_s_i, __pyx_n_s_v_dict); if (unlikely(!__pyx_tuple__61)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__61);
+  __Pyx_GIVEREF(__pyx_tuple__61);
+  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(11, 0, 0, 30, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__61, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_rlwm_lba_race, 3460, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 3460, __pyx_L1_error)
+
+  /* "cssm.pyx":3543
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                                         np.ndarray[float, ndim = 1] vl1,
  *                                                         np.ndarray[float, ndim = 1] vl2,
  */
-  __pyx_codeobj__57 = (PyObject*)__Pyx_PyCode_New(23, 0, 0, 81, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_ddm_flexbound_mic2_unnormalized, 3328, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__57)) __PYX_ERR(0, 3328, __pyx_L1_error)
+  __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(23, 0, 0, 81, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_ddm_flexbound_mic2_unnormalized, 3543, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(0, 3543, __pyx_L1_error)
 
-  /* "cssm.pyx":3839
+  /* "cssm.pyx":4054
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_tradeoff(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                            np.ndarray[float, ndim = 1] vl1,
  *                            np.ndarray[float, ndim = 1] vl2,
  */
-  __pyx_tuple__58 = PyTuple_Pack(61, __pyx_n_s_vh, __pyx_n_s_vl1, __pyx_n_s_vl2, __pyx_n_s_a, __pyx_n_s_zh, __pyx_n_s_zl1, __pyx_n_s_zl2, __pyx_n_s_d, __pyx_n_s_t, __pyx_n_s_deadline, __pyx_n_s_s, __pyx_n_s_delta_t, __pyx_n_s_max_t, __pyx_n_s_n_samples, __pyx_n_s_n_trials, __pyx_n_s_print_info, __pyx_n_s_boundary_fun, __pyx_n_s_boundary_multiplicative, __pyx_n_s_boundary_params, __pyx_n_s_random_state, __pyx_n_s_return_option, __pyx_n_s_smooth, __pyx_n_s_kwargs, __pyx_n_s_vh_view, __pyx_n_s_vl1_view, __pyx_n_s_vl2_view, __pyx_n_s_a_view, __pyx_n_s_zh_view, __pyx_n_s_zl1_view, __pyx_n_s_zl2_view, __pyx_n_s_d_view, __pyx_n_s_t_view, __pyx_n_s_deadline_view, __pyx_n_s_rts, __pyx_n_s_choices, __pyx_n_s_rts_view, __pyx_n_s_choices_view, __pyx_n_s_delta_t_sqrt, __pyx_n_s_sqrt_st, __pyx_n_s_num_draws, __pyx_n_s_t_s, __pyx_n_s_boundary, __pyx_n_s_boundary_view, __pyx_n_s_bias_trace, __pyx_n_s_bias_trace_view, __pyx_n_s_y_h, __pyx_n_s_y_l, __pyx_n_s_v_l, __pyx_n_s_t_h, __pyx_n_s_t_l, __pyx_n_s_tmp_pos_dep, __pyx_n_s_smooth_u, __pyx_n_s_deadline_tmp, __pyx_n_s_n, __pyx_n_s_ix, __pyx_n_s_ix_tmp, __pyx_n_s_k, __pyx_n_s_m, __pyx_n_s_gaussian_values, __pyx_n_s_boundary_params_tmp, __pyx_n_s_key); if (unlikely(!__pyx_tuple__58)) __PYX_ERR(0, 3839, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__58);
-  __Pyx_GIVEREF(__pyx_tuple__58);
-  __pyx_codeobj__59 = (PyObject*)__Pyx_PyCode_New(22, 0, 0, 61, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__58, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_ddm_flexbound_tradeoff, 3839, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__59)) __PYX_ERR(0, 3839, __pyx_L1_error)
+  __pyx_tuple__64 = PyTuple_Pack(61, __pyx_n_s_vh, __pyx_n_s_vl1, __pyx_n_s_vl2, __pyx_n_s_a, __pyx_n_s_zh, __pyx_n_s_zl1, __pyx_n_s_zl2, __pyx_n_s_d, __pyx_n_s_t, __pyx_n_s_deadline, __pyx_n_s_s, __pyx_n_s_delta_t, __pyx_n_s_max_t, __pyx_n_s_n_samples, __pyx_n_s_n_trials, __pyx_n_s_print_info, __pyx_n_s_boundary_fun, __pyx_n_s_boundary_multiplicative, __pyx_n_s_boundary_params, __pyx_n_s_random_state, __pyx_n_s_return_option, __pyx_n_s_smooth, __pyx_n_s_kwargs, __pyx_n_s_vh_view, __pyx_n_s_vl1_view, __pyx_n_s_vl2_view, __pyx_n_s_a_view, __pyx_n_s_zh_view, __pyx_n_s_zl1_view, __pyx_n_s_zl2_view, __pyx_n_s_d_view, __pyx_n_s_t_view, __pyx_n_s_deadline_view, __pyx_n_s_rts, __pyx_n_s_choices, __pyx_n_s_rts_view, __pyx_n_s_choices_view, __pyx_n_s_delta_t_sqrt, __pyx_n_s_sqrt_st, __pyx_n_s_num_draws, __pyx_n_s_t_s, __pyx_n_s_boundary, __pyx_n_s_boundary_view, __pyx_n_s_bias_trace, __pyx_n_s_bias_trace_view, __pyx_n_s_y_h, __pyx_n_s_y_l, __pyx_n_s_v_l, __pyx_n_s_t_h, __pyx_n_s_t_l, __pyx_n_s_tmp_pos_dep, __pyx_n_s_smooth_u, __pyx_n_s_deadline_tmp, __pyx_n_s_n, __pyx_n_s_ix, __pyx_n_s_ix_tmp, __pyx_n_s_k, __pyx_n_s_m, __pyx_n_s_gaussian_values, __pyx_n_s_boundary_params_tmp, __pyx_n_s_key); if (unlikely(!__pyx_tuple__64)) __PYX_ERR(0, 4054, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__64);
+  __Pyx_GIVEREF(__pyx_tuple__64);
+  __pyx_codeobj__65 = (PyObject*)__Pyx_PyCode_New(22, 0, 0, 61, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__64, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cssm_pyx, __pyx_n_s_ddm_flexbound_tradeoff, 4054, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__65)) __PYX_ERR(0, 4054, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -71841,41 +76085,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -73105,15 +77349,15 @@
  *                   return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 598, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_38__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_44__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound, __pyx_t_5) < 0) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":728
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flex(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
@@ -73145,15 +77389,15 @@
  *              return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults1, __pyx_t_5)->__pyx_arg_drift_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_40__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_46__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flex, __pyx_t_5) < 0) __PYX_ERR(0, 728, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1023
  * # @cythonwraparound(False)
  * 
  * def levy_flexbound(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
@@ -73172,15 +77416,15 @@
  *                    return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1036, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_42__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_48__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_levy_flexbound, __pyx_t_5) < 0) __PYX_ERR(0, 1023, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1162
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def full_ddm(np.ndarray[float, ndim = 1] v, # = 0,             # <<<<<<<<<<<<<<
@@ -73199,15 +77443,15 @@
  *              return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_44__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_50__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_full_ddm, __pyx_t_5) < 0) __PYX_ERR(0, 1162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1325
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_sdv(np.ndarray[float, ndim = 1] v,             # <<<<<<<<<<<<<<
@@ -73226,15 +77470,15 @@
  *             return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults4, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_46__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_52__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_sdv, __pyx_t_5) < 0) __PYX_ERR(0, 1325, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1474
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ornstein_uhlenbeck(np.ndarray[float, ndim = 1] v, # drift parameter             # <<<<<<<<<<<<<<
@@ -73253,15 +77497,15 @@
  *                        return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults5, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_48__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_54__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ornstein_uhlenbeck, __pyx_t_5) < 0) __PYX_ERR(0, 1474, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1640
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def race_model(np.ndarray[float, ndim = 2] v,  # np.array expected, one column of floats             # <<<<<<<<<<<<<<
@@ -73280,15 +77524,15 @@
  *                return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1652, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults6, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_50__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_56__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_race_model, __pyx_t_5) < 0) __PYX_ERR(0, 1640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1800
  * 
  * # Simulate (rt, choice) tuples from: Leaky Competing Accumulator Model -----------------------------
  * def lca(np.ndarray[float, ndim = 2] v, # drift parameters (np.array expect: one column of floats)             # <<<<<<<<<<<<<<
@@ -73307,15 +77551,15 @@
  *         return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1814, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults7, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_52__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_58__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_lca, __pyx_t_5) < 0) __PYX_ERR(0, 1800, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":1973
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_seq2(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
@@ -73334,15 +77578,15 @@
  *                        return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1990, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults8, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_54__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_60__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_seq2, __pyx_t_5) < 0) __PYX_ERR(0, 1973, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":2237
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_par2(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
@@ -73361,15 +77605,15 @@
  *                        return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults9, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_56__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_62__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_par2, __pyx_t_5) < 0) __PYX_ERR(0, 2237, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":2469
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_ornstein(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
@@ -73388,15 +77632,15 @@
  *                                 return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2489, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults10, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_58__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_64__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_mic2_ornstein, __pyx_t_5) < 0) __PYX_ERR(0, 2469, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":2759
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
@@ -73415,15 +77659,15 @@
  *                                   return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 2777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults11, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_60__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_66__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_mic2_multinoise, __pyx_t_5) < 0) __PYX_ERR(0, 2759, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
   /* "cssm.pyx":3046
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
@@ -73442,81 +77686,324 @@
  *                                            return_option = 'full',
  */
   __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3065, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_CyFunction_Defaults(__pyx_defaults12, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_62__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_68__defaults__);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_mic2_ornstein_mult, __pyx_t_5) < 0) __PYX_ERR(0, 3046, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "cssm.pyx":3328
+  /* "cssm.pyx":3332
+ *         np.ndarray[float, ndim = 1] deadline,
+ *         float sd, # std dev of Normal from where we sample vs
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues             # <<<<<<<<<<<<<<
+ *         int nact = 3,
+ *         int n_samples = 2000,
+ */
+  __pyx_t_5 = PyFloat_FromDouble(((float)0.0)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3332, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "cssm.pyx":3333
+ *         float sd, # std dev of Normal from where we sample vs
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+ *         int nact = 3,             # <<<<<<<<<<<<<<
+ *         int n_samples = 2000,
+ *         int n_trials = 1,
+ */
+  __pyx_t_4 = __Pyx_PyInt_From_int(((int)3)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3333, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+
+  /* "cssm.pyx":3334
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+ *         int nact = 3,
+ *         int n_samples = 2000,             # <<<<<<<<<<<<<<
+ *         int n_trials = 1,
+ *         float max_t = 20,
+ */
+  __pyx_t_9 = __Pyx_PyInt_From_int(((int)0x7D0)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3334, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+
+  /* "cssm.pyx":3335
+ *         int nact = 3,
+ *         int n_samples = 2000,
+ *         int n_trials = 1,             # <<<<<<<<<<<<<<
+ *         float max_t = 20,
+ *         **kwargs
+ */
+  __pyx_t_10 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3335, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+
+  /* "cssm.pyx":3336
+ *         int n_samples = 2000,
+ *         int n_trials = 1,
+ *         float max_t = 20,             # <<<<<<<<<<<<<<
+ *         **kwargs
+ *         ):
+ */
+  __pyx_t_11 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 3336, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+
+  /* "cssm.pyx":3327
+ * 
+ * # Simulate (rt, choice) tuples from: Vanilla LBA Model without ndt -----------------------------
+ * def lba_vanilla(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+  __pyx_t_7 = PyTuple_New(5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_5)) __PYX_ERR(0, 3327, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_4)) __PYX_ERR(0, 3327, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_9);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_t_9)) __PYX_ERR(0, 3327, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_10);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 3, __pyx_t_10)) __PYX_ERR(0, 3327, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_11);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 4, __pyx_t_11)) __PYX_ERR(0, 3327, __pyx_L1_error);
+  __pyx_t_5 = 0;
+  __pyx_t_4 = 0;
+  __pyx_t_9 = 0;
+  __pyx_t_10 = 0;
+  __pyx_t_11 = 0;
+  __pyx_t_11 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_35lba_vanilla, 0, __pyx_n_s_lba_vanilla, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 3327, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_11, __pyx_t_7);
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lba_vanilla, __pyx_t_11) < 0) __PYX_ERR(0, 3327, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+
+  /* "cssm.pyx":3400
+ *         np.ndarray[float, ndim = 1] deadline,
+ *         float sd, # std dev
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues             # <<<<<<<<<<<<<<
+ *         int nact = 3,
+ *         int n_samples = 2000,
+ */
+  __pyx_t_11 = PyFloat_FromDouble(((float)0.0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 3400, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+
+  /* "cssm.pyx":3401
+ *         float sd, # std dev
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+ *         int nact = 3,             # <<<<<<<<<<<<<<
+ *         int n_samples = 2000,
+ *         int n_trials = 1,
+ */
+  __pyx_t_7 = __Pyx_PyInt_From_int(((int)3)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3401, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+
+  /* "cssm.pyx":3402
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+ *         int nact = 3,
+ *         int n_samples = 2000,             # <<<<<<<<<<<<<<
+ *         int n_trials = 1,
+ *         float max_t = 20,
+ */
+  __pyx_t_10 = __Pyx_PyInt_From_int(((int)0x7D0)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3402, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+
+  /* "cssm.pyx":3403
+ *         int nact = 3,
+ *         int n_samples = 2000,
+ *         int n_trials = 1,             # <<<<<<<<<<<<<<
+ *         float max_t = 20,
+ *         **kwargs
+ */
+  __pyx_t_9 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3403, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+
+  /* "cssm.pyx":3404
+ *         int n_samples = 2000,
+ *         int n_trials = 1,
+ *         float max_t = 20,             # <<<<<<<<<<<<<<
+ *         **kwargs
+ *         ):
+ */
+  __pyx_t_4 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3404, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+
+  /* "cssm.pyx":3394
+ * 
+ * # Simulate (rt, choice) tuples from: Collapsing bound angle LBA Model -----------------------------
+ * def lba_angle(np.ndarray[float, ndim = 2] v,             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] a,
+ *         np.ndarray[float, ndim = 2] z,
+ */
+  __pyx_t_5 = PyTuple_New(5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_11);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_11)) __PYX_ERR(0, 3394, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_7);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_7)) __PYX_ERR(0, 3394, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_10);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_10)) __PYX_ERR(0, 3394, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_9);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_9)) __PYX_ERR(0, 3394, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_5, 4, __pyx_t_4)) __PYX_ERR(0, 3394, __pyx_L1_error);
+  __pyx_t_11 = 0;
+  __pyx_t_7 = 0;
+  __pyx_t_10 = 0;
+  __pyx_t_9 = 0;
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_37lba_angle, 0, __pyx_n_s_lba_angle, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__60)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3394, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_4, __pyx_t_5);
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lba_angle, __pyx_t_4) < 0) __PYX_ERR(0, 3394, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+  /* "cssm.pyx":3466
+ *         np.ndarray[float, ndim = 1] deadline,
+ *         float sd, # std dev of Normal from where we sample vs
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues             # <<<<<<<<<<<<<<
+ *         int nact = 3,
+ *         int n_samples = 2000,
+ */
+  __pyx_t_4 = PyFloat_FromDouble(((float)0.0)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3466, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+
+  /* "cssm.pyx":3467
+ *         float sd, # std dev of Normal from where we sample vs
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+ *         int nact = 3,             # <<<<<<<<<<<<<<
+ *         int n_samples = 2000,
+ *         int n_trials = 1,
+ */
+  __pyx_t_5 = __Pyx_PyInt_From_int(((int)3)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3467, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+
+  /* "cssm.pyx":3468
+ *         float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+ *         int nact = 3,
+ *         int n_samples = 2000,             # <<<<<<<<<<<<<<
+ *         int n_trials = 1,
+ *         float max_t = 20,
+ */
+  __pyx_t_9 = __Pyx_PyInt_From_int(((int)0x7D0)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 3468, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_9);
+
+  /* "cssm.pyx":3469
+ *         int nact = 3,
+ *         int n_samples = 2000,
+ *         int n_trials = 1,             # <<<<<<<<<<<<<<
+ *         float max_t = 20,
+ *         **kwargs
+ */
+  __pyx_t_10 = __Pyx_PyInt_From_int(((int)1)); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 3469, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_10);
+
+  /* "cssm.pyx":3470
+ *         int n_samples = 2000,
+ *         int n_trials = 1,
+ *         float max_t = 20,             # <<<<<<<<<<<<<<
+ *         **kwargs
+ *         ):
+ */
+  __pyx_t_7 = PyFloat_FromDouble(((float)20.0)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3470, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+
+  /* "cssm.pyx":3460
+ * 
+ * # Simulate (rt, choice) tuples from: RLWM LBA Race Model without ndt -----------------------------
+ * def rlwm_lba_race(np.ndarray[float, ndim = 2] v_RL, # RL drift parameters (np.array expect: one column of floats)             # <<<<<<<<<<<<<<
+ *         np.ndarray[float, ndim = 2] v_WM, # WM drift parameters (np.array expect: one column of floats)
+ *         np.ndarray[float, ndim = 2] a, # criterion height
+ */
+  __pyx_t_11 = PyTuple_New(5); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_GIVEREF(__pyx_t_4);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_4)) __PYX_ERR(0, 3460, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_5)) __PYX_ERR(0, 3460, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_9);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_t_9)) __PYX_ERR(0, 3460, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_10);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 3, __pyx_t_10)) __PYX_ERR(0, 3460, __pyx_L1_error);
+  __Pyx_GIVEREF(__pyx_t_7);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_11, 4, __pyx_t_7)) __PYX_ERR(0, 3460, __pyx_L1_error);
+  __pyx_t_4 = 0;
+  __pyx_t_5 = 0;
+  __pyx_t_9 = 0;
+  __pyx_t_10 = 0;
+  __pyx_t_7 = 0;
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_39rlwm_lba_race, 0, __pyx_n_s_rlwm_lba_race, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3460, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_t_11);
+  __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rlwm_lba_race, __pyx_t_7) < 0) __PYX_ERR(0, 3460, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "cssm.pyx":3543
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                                                         np.ndarray[float, ndim = 1] vl1,
  *                                                         np.ndarray[float, ndim = 1] vl2,
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_35ddm_flexbound_mic2_unnormalized_ornstein_multinoise, 0, __pyx_n_s_ddm_flexbound_mic2_unnormalized, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__57)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3328, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_5, sizeof(__pyx_defaults13), 1)) __PYX_ERR(0, 3328, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_41ddm_flexbound_mic2_unnormalized_ornstein_multinoise, 0, __pyx_n_s_ddm_flexbound_mic2_unnormalized, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__63)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 3543, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults13), 1)) __PYX_ERR(0, 3543, __pyx_L1_error)
 
-  /* "cssm.pyx":3347
+  /* "cssm.pyx":3562
  *                                                         boundary_fun = None, # function of t (and potentially other parameters) that takes in (t, *args)
  *                                                         boundary_multiplicative = True,
  *                                                         boundary_params = {},             # <<<<<<<<<<<<<<
  *                                                         random_state = None,
  *                                                         return_option = 'full',
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3347, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_64__defaults__);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_mic2_unnormalized, __pyx_t_5) < 0) __PYX_ERR(0, 3328, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 3562, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_CyFunction_Defaults(__pyx_defaults13, __pyx_t_7)->__pyx_arg_boundary_params = __pyx_t_11;
+  __Pyx_GIVEREF(__pyx_t_11);
+  __pyx_t_11 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_4cssm_70__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_mic2_unnormalized, __pyx_t_7) < 0) __PYX_ERR(0, 3543, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "cssm.pyx":3839
+  /* "cssm.pyx":4054
  * # @cythonboundscheck(False)
  * # @cythonwraparound(False)
  * def ddm_flexbound_tradeoff(np.ndarray[float, ndim = 1] vh,             # <<<<<<<<<<<<<<
  *                            np.ndarray[float, ndim = 1] vl1,
  *                            np.ndarray[float, ndim = 1] vl2,
  */
-  __pyx_t_5 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_37ddm_flexbound_tradeoff, 0, __pyx_n_s_ddm_flexbound_tradeoff, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__59)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 3839, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_5, sizeof(__pyx_defaults14), 1)) __PYX_ERR(0, 3839, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4cssm_43ddm_flexbound_tradeoff, 0, __pyx_n_s_ddm_flexbound_tradeoff, NULL, __pyx_n_s_cssm, __pyx_d, ((PyObject *)__pyx_codeobj__65)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 4054, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (!__Pyx_CyFunction_InitDefaults(__pyx_t_7, sizeof(__pyx_defaults14), 1)) __PYX_ERR(0, 4054, __pyx_L1_error)
 
-  /* "cssm.pyx":3857
+  /* "cssm.pyx":4072
  *                            boundary_fun = None, # function of t (and potentially other parameters) that takes in (t, *args)
  *                            boundary_multiplicative = True,
  *                            boundary_params = {},             # <<<<<<<<<<<<<<
  *                            random_state = None,
  *                            return_option = 'full',
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 3857, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_t_5)->__pyx_arg_boundary_params = __pyx_t_4;
-  __Pyx_GIVEREF(__pyx_t_4);
-  __pyx_t_4 = 0;
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_5, __pyx_pf_4cssm_66__defaults__);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_tradeoff, __pyx_t_5) < 0) __PYX_ERR(0, 3839, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 4072, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_11);
+  __Pyx_CyFunction_Defaults(__pyx_defaults14, __pyx_t_7)->__pyx_arg_boundary_params = __pyx_t_11;
+  __Pyx_GIVEREF(__pyx_t_11);
+  __pyx_t_11 = 0;
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_7, __pyx_pf_4cssm_72__defaults__);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ddm_flexbound_tradeoff, __pyx_t_7) < 0) __PYX_ERR(0, 4054, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "cssm.pyx":1
  * # Globaly settings for cython             # <<<<<<<<<<<<<<
  * # cython: cdivision=True
  * # cython: wraparound=False
  */
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test_2, __pyx_t_5) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test_2, __pyx_t_7) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
@@ -77192,14 +81679,20 @@
   static void __Pyx_RaiseMappingExpectedError(PyObject* arg) {
     __Pyx_TypeName arg_type_name = __Pyx_PyType_GetName(Py_TYPE(arg));
     PyErr_Format(PyExc_TypeError,
         "'" __Pyx_FMT_TYPENAME "' object is not a mapping", arg_type_name);
     __Pyx_DECREF_TypeName(arg_type_name);
 }
 
+/* BufferFallbackError */
+  static void __Pyx_RaiseBufferFallbackError(void) {
+  PyErr_SetString(PyExc_ValueError,
+     "Buffer acquisition failed on assignment; and then reacquiring the old buffer failed too!");
+}
+
 /* PyObject_GenericGetAttrNoDict */
   #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
     __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
                  "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
@@ -77687,18 +82180,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -77744,23 +82237,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -78752,15 +83245,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -79836,14 +84329,26 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* MemviewDtypeToObject */
+  static CYTHON_INLINE PyObject *__pyx_memview_get_float(const char *itemp) {
+    return (PyObject *) PyFloat_FromDouble(*(float *) itemp);
+}
+static CYTHON_INLINE int __pyx_memview_set_float(const char *itemp, PyObject *obj) {
+    float value = __pyx_PyFloat_AsFloat(obj);
+    if (unlikely((value == (float)-1) && PyErr_Occurred()))
+        return 0;
+    *(float *) itemp = value;
+    return 1;
+}
+
 /* Declarations */
   #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
@@ -81422,15 +85927,15 @@
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
         Py_XDECREF(name);
-        name = __Pyx_NewRef(__pyx_n_s__60);
+        name = __Pyx_NewRef(__pyx_n_s__66);
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
   static unsigned long __Pyx_get_runtime_version(void) {
```

### Comparing `ssm-simulators-0.7.0/src/cssm.pyx` & `ssm_simulators-0.7.2/src/cssm.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -2178,27 +2178,27 @@
                 elif t_particle < deadline_tmp:
                     smooth_u = (0.5 - random_uniform()) * delta_t
                 else:
                     smooth_u = 0.0
             else:
                 smooth_u = 0.0
 
-                rts_view[n, k, 0] = t_particle + t_view[k] + smooth_u
+            rts_view[n, k, 0] = t_particle + t_view[k] + smooth_u
 
-                # The probability of making a 'mistake' 1 - (relative y position)
-                # y at upper bound --> choices_view[n, k, 0] add one deterministically
-                # y at lower bound --> choice_view[n, k, 0] stays the same deterministically
-                
-                # If boundary is negative (or 0) already, we flip a coin
-                if boundary_view[ix] <= 0:
-                    if random_uniform() <= 0.5:
-                        choices_view[n, k, 0] += 1
-                # Otherwise apply rule from above
-                elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
+            # The probability of making a 'mistake' 1 - (relative y position)
+            # y at upper bound --> choices_view[n, k, 0] add one deterministically
+            # y at lower bound --> choice_view[n, k, 0] stays the same deterministically
+            
+            # If boundary is negative (or 0) already, we flip a coin
+            if boundary_view[ix] <= 0:
+                if random_uniform() <= 0.5:
                     choices_view[n, k, 0] += 1
+            # Otherwise apply rule from above
+            elif random_uniform() <= ((y_l + boundary_view[ix]) / (2 * boundary_view[ix])):
+                choices_view[n, k, 0] += 1
 
             if (rts_view[n, k, 0] >= deadline_view[k]) | (deadline_view[k] <= 0):
                     rts_view[n, k, 0] = -999
 
     if return_option == 'full':
         return {'rts': rts, 'choices': choices, 'metadata': {'vh': vh,
                                                             'vl1': vl1,
@@ -2534,15 +2534,15 @@
     # Y particle trace
     bias_trace_l1 = np.zeros(num_draws, dtype = DTYPE)
     bias_trace_l2 = np.zeros(num_draws, dtype = DTYPE)
     cdef float[:] bias_trace_l1_view = bias_trace_l1
     cdef float[:] bias_trace_l2_view = bias_trace_l2
 
     cdef float y_h, y_l, y_l1, y_l2
-    cdef float v_l, v_l1, v_l2, 
+    cdef float v_l, v_l1, v_l2,
     cdef float t_h, t_l, t_l1, t_l2, smooth_u, deadline_tmp
     cdef Py_ssize_t n, ix, ix1, ix2, ix_l, ix_tmp, ix1_tmp, ix2_tmp, k
     cdef Py_ssize_t m = 0
     cdef float[:] gaussian_values = draw_gaussian(num_draws)
 
     for k in range(n_trials):
         # Precompute boundary evaluations
@@ -3318,14 +3318,229 @@
                              'n_samples': n_samples,
                              'n_trials': n_trials,
                              }}
     else:
         raise ValueError('return_option must be either "full" or "minimal"')
 # ----------------------------------------------------------------------------------------------------
 
+
+# Simulate (rt, choice) tuples from: Vanilla LBA Model without ndt -----------------------------
+def lba_vanilla(np.ndarray[float, ndim = 2] v, 
+        np.ndarray[float, ndim = 2] a, 
+        np.ndarray[float, ndim = 2] z, 
+        np.ndarray[float, ndim = 1] deadline,
+        float sd, # std dev of Normal from where we sample vs
+        float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+        int nact = 3,
+        int n_samples = 2000,
+        int n_trials = 1,
+        float max_t = 20,
+        **kwargs
+        ):
+
+    # v_t = np.random.normal(v, sd)
+    # print(len(z), nact, np.array([z]*nact).transpose().shape)
+    # z_t = np.random.uniform(np.zeros((len(z), nact)), np.array([z]*nact).transpose(), (len(z), nact))
+
+    # Param views
+    cdef float[:, :] v_view = v
+    cdef float[:, :] a_view = a
+    cdef float[:, :] z_view = z
+
+    cdef float[:] deadline_view = deadline
+
+    rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+    cdef float[:, :, :] rts_view = rts
+    
+    choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+    cdef int[:, :, :] choices_view = choices
+    
+    cdef Py_ssize_t n, k, i
+
+    for k in range(n_trials):
+        
+        for n in range(n_samples):
+            zs = np.random.uniform(0, z_view[k], nact)
+
+            vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs
+
+            x_t = ([a_view[k]]*nact - zs)/vs
+        
+            choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n
+            rts_view[n, k, 0] = np.min(x_t) + ndt  # store reaction time for sample n
+
+            # If the rt exceeds the deadline, set rt to -999
+            if rts_view[n, k, 0] >= deadline_view[k]:
+                rts_view[n, k, 0] = -999
+        
+
+    v_dict = {}    
+    for i in range(nact):
+        v_dict['v_' + str(i)] = v[:, i]
+
+    return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+                                                         'a': a,
+                                                         'z': z,
+                                                         'deadline': deadline,
+                                                         'sd': sd,
+                                                         'n_samples': n_samples,
+                                                         'simulator' : 'lba_vanilla',
+                                                         'possible_choices': list(np.arange(0, nact, 1)),
+                                                         'max_t': max_t,
+                                                         }}
+
+
+
+# Simulate (rt, choice) tuples from: Collapsing bound angle LBA Model -----------------------------
+def lba_angle(np.ndarray[float, ndim = 2] v, 
+        np.ndarray[float, ndim = 2] a, 
+        np.ndarray[float, ndim = 2] z,  
+        np.ndarray[float, ndim = 2] theta,
+        np.ndarray[float, ndim = 1] deadline,
+        float sd, # std dev 
+        float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+        int nact = 3,
+        int n_samples = 2000,
+        int n_trials = 1,
+        float max_t = 20,
+        **kwargs
+        ):
+
+    # Param views
+    cdef float[:, :] v_view = v
+    cdef float[:, :] a_view = a
+    cdef float[:, :] z_view = z
+    cdef float[:, :] theta_view = theta
+
+    cdef float[:] deadline_view = deadline
+
+    rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+    cdef float[:, :, :] rts_view = rts
+    
+    choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+    cdef int[:, :, :] choices_view = choices
+    
+    cdef Py_ssize_t n, k, i
+
+    for k in range(n_trials):
+        
+        for n in range(n_samples):
+            zs = np.random.uniform(0, z_view[k], nact)
+
+            vs = np.abs(np.random.normal(v_view[k], sd)) # np.abs() to avoid negative vs
+            x_t = ([a_view[k]]*nact - zs)/(vs + np.tan(theta_view[k, 0]))
+        
+            choices_view[n, k, 0] = np.argmin(x_t) # store choices for sample n
+            rts_view[n, k, 0] = np.min(x_t) + ndt # store reaction time for sample n
+
+            # If the rt exceeds the deadline, set rt to -999
+            if rts_view[n, k, 0] >= deadline_view[k]:
+                rts_view[n, k, 0] = -999
+
+            # if np.min(x_t) <= 0:
+            #     print("\n ssms sim error: ", a[k], zs, vs, np.tan(theta[k]))
+    
+    v_dict = {}  
+    for i in range(nact):
+        v_dict['v_' + str(i)] = v[:, i]
+
+    return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+                                                         'a': a,
+                                                         'z': z,
+                                                         'theta': theta,
+                                                         'deadline': deadline,
+                                                         'sd': sd,
+                                                         'n_samples': n_samples,
+                                                         'simulator' : 'lba_angle',
+                                                         'possible_choices': list(np.arange(0, nact, 1)),
+                                                         'max_t': max_t,
+                                                         }}
+
+
+# Simulate (rt, choice) tuples from: RLWM LBA Race Model without ndt -----------------------------
+def rlwm_lba_race(np.ndarray[float, ndim = 2] v_RL, # RL drift parameters (np.array expect: one column of floats)
+        np.ndarray[float, ndim = 2] v_WM, # WM drift parameters (np.array expect: one column of floats)
+        np.ndarray[float, ndim = 2] a, # criterion height
+        np.ndarray[float, ndim = 2] z, # initial bias parameters (np.array expect: one column of floats)
+        np.ndarray[float, ndim = 1] deadline,
+        float sd, # std dev of Normal from where we sample vs
+        float ndt = 0, # ndt is supposed to be 0 by default because of parameter identifiability issues
+        int nact = 3,
+        int n_samples = 2000,
+        int n_trials = 1,
+        float max_t = 20,
+        **kwargs
+        ):
+
+    # v_t = np.random.normal(v, sd)
+    # print(len(z), nact, np.array([z]*nact).transpose().shape)
+    # z_t = np.random.uniform(np.zeros((len(z), nact)), np.array([z]*nact).transpose(), (len(z), nact))
+
+    # Param views
+    cdef float[:, :] v_RL_view = v_RL
+    cdef float[:, :] v_WM_view = v_WM
+    cdef float[:, :] a_view = a
+    cdef float[:, :] z_view = z
+
+    cdef float[:] deadline_view = deadline
+
+    cdef np.ndarray[float, ndim = 1] zs
+    cdef np.ndarray[double, ndim = 2] x_t_RL
+    cdef np.ndarray[double, ndim = 2] x_t_WM
+    cdef np.ndarray[double, ndim = 1] vs_RL
+    cdef np.ndarray[double, ndim = 1] vs_WM
+
+    rts = np.zeros((n_samples, n_trials, 1), dtype = DTYPE)
+    cdef float[:, :, :] rts_view = rts
+    
+    choices = np.zeros((n_samples, n_trials, 1), dtype = np.intc)
+    cdef int[:, :, :] choices_view = choices
+    
+    cdef Py_ssize_t n, k, i
+
+    for k in range(n_trials):
+        
+        for n in range(n_samples):
+            zs = np.random.uniform(0, z_view[k], nact).astype(DTYPE)
+
+            vs_RL = np.abs(np.random.normal(v_RL_view[k], sd)) # np.abs() to avoid negative vs
+            vs_WM = np.abs(np.random.normal(v_WM_view[k], sd)) # np.abs() to avoid negative vs
+
+            x_t_RL = ([a_view[k]]*nact - zs)/vs_RL
+            x_t_WM = ([a_view[k]]*nact - zs)/vs_WM
+
+            if np.min(x_t_RL) <= np.min(x_t_WM):
+                rts_view[n, k, 0] = np.min(x_t_RL) + ndt  # store reaction time for sample n
+                choices_view[n, k, 0] = np.argmin(x_t_RL) # store choices for sample n
+            else:
+                rts_view[n, k, 0] = np.min(x_t_WM) + ndt  # store reaction time for sample n
+                choices_view[n, k, 0] = np.argmin(x_t_WM) # store choices for sample n  
+            
+            # If the rt exceeds the deadline, set rt to -999
+            if rts_view[n, k, 0] >= deadline_view[k]:
+                rts_view[n, k, 0] = -999
+        
+
+    v_dict = {}    
+    for i in range(nact):
+        v_dict['v_RL_' + str(i)] = v_RL[:, i]
+        v_dict['v_WM_' + str(i)] = v_WM[:, i]
+
+    return {'rts': rts, 'choices': choices, 'metadata': {**v_dict,
+                                                         'a': a,
+                                                         'z': z,
+                                                         'deadline': deadline,
+                                                         'sd': sd,
+                                                         'n_samples': n_samples,
+                                                         'simulator' : 'rlwm_lba_race',
+                                                         'possible_choices': list(np.arange(0, nact, 1)),
+                                                         'max_t': max_t,
+                                                         }}
+# ----------------------------------------------------------------------------------------------------
+
 # Simulate (rt, choice) tuples from: DDM WITH FLEXIBLE BOUNDARIES ------------------------------------
 # @cythonboundscheck(False)
 # @cythonwraparound(False)
 def ddm_flexbound_mic2_unnormalized_ornstein_multinoise(np.ndarray[float, ndim = 1] vh, 
                                                         np.ndarray[float, ndim = 1] vl1,
                                                         np.ndarray[float, ndim = 1] vl2,
                                                         np.ndarray[float, ndim = 1] a,
```

### Comparing `ssm-simulators-0.7.0/ssm_simulators.egg-info/PKG-INFO` & `ssm_simulators-0.7.2/ssm_simulators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: ssm-simulators
-Version: 0.7.0
+Version: 0.7.2
 Summary: SSMS is a package collecting simulators and training data generators for a bunch of generative models of interest in the cognitive science / neuroscience and approximate bayesian computation communities
 Author-email: Alexander Fenger <alexander_fengler@brown.edu>
 Project-URL: Homepage, https://github.com/AlexanderFengler/ssm-simulators
 Project-URL: Bug Tracker, https://github.com/AlexanderFengler/ssm-simulators/issues
 Keywords: simulators,generative models,cognitive science,neuroscience
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: <3.12,>3.8
+Requires-Python: <3.12,>3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: scipy>=1.6.3
-Requires-Dist: cython>=0.29.23
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: scikit-learn>=0.24.0
 Requires-Dist: psutil>=5.0.0
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `ssm-simulators-0.7.0/ssm_simulators.egg-info/SOURCES.txt` & `ssm_simulators-0.7.2/ssm_simulators.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.py
 notebooks/basic_tutorial copy.ipynb
 notebooks/basic_tutorial.ipynb
 notebooks/basic_tutorial_tmp.ipynb
 notebooks/essential_tests.ipynb
 notebooks/test_deadline.ipynb
 notebooks/test_mic2_ornstein.ipynb
+notebooks/test_seq2.ipynb
 src/cssm.cpp
 src/cssm.pyx
 ssm_simulators.egg-info/PKG-INFO
 ssm_simulators.egg-info/SOURCES.txt
 ssm_simulators.egg-info/dependency_links.txt
 ssm_simulators.egg-info/requires.txt
 ssm_simulators.egg-info/top_level.txt
```

### Comparing `ssm-simulators-0.7.0/ssms/basic_simulators/boundary_functions.py` & `ssm_simulators-0.7.2/ssms/basic_simulators/boundary_functions.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/ssms/basic_simulators/drift_functions.py` & `ssm_simulators-0.7.2/ssms/basic_simulators/drift_functions.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/ssms/basic_simulators/simulator.py` & `ssm_simulators-0.7.2/ssms/basic_simulators/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 def make_boundary_dict(model_config, model, theta):
     boundary_name = model_config[model]["boundary_name"]
     boundary_params = {
         param_name: value
         for param_name, value in theta.items()
         if param_name in boundary_config[boundary_name]["params"]
     }
+
     boundary_fun = boundary_config[boundary_name]["fun"]
     boundary_multiplicative = boundary_config[boundary_name]["multiplicative"]
     boundary_dict = {
         "boundary_params": boundary_params,
         "boundary_fun": boundary_fun,
         "boundary_multiplicative": boundary_multiplicative,
     }
@@ -295,14 +296,43 @@
 
     for choice in choice_codes:
         counts[:, cnt] = np.histogram(out[:, 0][out[:, 1] == choice], bins=bins)[0]
         cnt += 1
     return counts
 
 
+def validate_ssm_parameters(model, theta):
+
+    def check_num_drifts_and_actions(drifts, num_actions):
+        drifts = np.array(drifts)
+        if drifts.shape[1] != num_actions:
+            raise ValueError("Number of drift rates does not match number of actions")
+
+    def check_lba_drifts_sum(drifts):
+        v_sum = np.sum(drifts, axis=1)
+        if np.any(v_sum <= 0.99) or np.any(v_sum >= 1.01):
+            raise ValueError("Drift rates do not sum to 1 for each trial")
+
+    def check_if_z_gt_a(z, a):
+        if np.any(z >= a):
+            raise ValueError("Starting point z >= a for at least one trial")
+
+    if model in ["lba_3_v1", "lba_angle_3_v1", "rlwm_lba_race_v1"]:
+        if model in ["lba_3_v1", "lba_angle_3_v1"]:
+            # check_num_drifts_and_actions(theta['v'], model_config[model]['nchoices'])
+            check_lba_drifts_sum(theta["v"])
+            check_if_z_gt_a(theta["z"], theta["a"])
+        elif model in ["rlwm_lba_race_v1"]:
+            # check_num_drifts_and_actions(theta['v_RL'], model_config[model]['nchoices'])
+            # check_num_drifts_and_actions(theta['v_WM'], model_config[model]['nchoices'])
+            check_lba_drifts_sum(theta["v_RL"])
+            check_lba_drifts_sum(theta["v_WM"])
+            check_if_z_gt_a(theta["z"], theta["a"])
+
+
 def simulator(
     theta,
     model="angle",
     n_samples=1000,
     delta_t=0.001,
     max_t=20,
     no_noise=False,
@@ -454,14 +484,15 @@
         "4_particles": np.tile(
             np.array(
                 [1.0] * 4,
                 dtype=np.float32,
             ),
             (n_trials, 1),
         ),
+        "lba_based_models": 0.1,
     }
 
     if no_noise:
         noise_dict = {key: value * 0.0 for key, value in noise_dict.items()}
 
     if model in [
         "glob",
@@ -488,14 +519,43 @@
 
     if model in ["ds_conflict_drift", "ds_conflict_drift_angle"]:
         sim_param_dict["s"] = noise_dict["1_particles"]
         theta["v"] = np.tile(np.array([0], dtype=np.float32), n_trials)
 
     # Multi-particle models
 
+    #   LBA-based models
+
+    # lba_sd = 0.1
+    if model == "lba_3_v1":
+        sim_param_dict["sd"] = noise_dict["lba_based_models"]
+        theta["v"] = np.column_stack([theta["v0"], theta["v1"], theta["v2"]])
+        theta["a"] = np.expand_dims(theta["a"], axis=1)
+        theta["z"] = np.expand_dims(theta["z"], axis=1)
+
+    if model == "lba_angle_3_v1":
+        sim_param_dict["sd"] = noise_dict["lba_based_models"]
+        theta["v"] = np.column_stack([theta["v0"], theta["v1"], theta["v2"]])
+        theta["a"] = np.expand_dims(theta["a"], axis=1)
+        theta["z"] = np.expand_dims(theta["z"], axis=1)
+        theta["theta"] = np.expand_dims(theta["theta"], axis=1)
+
+    if model == "rlwm_lba_race_v1":
+        sim_param_dict["sd"] = noise_dict["lba_based_models"]
+        theta["v_RL"] = np.column_stack(
+            [theta["v_RL_0"], theta["v_RL_1"], theta["v_RL_2"]]
+        )
+        theta["v_WM"] = np.column_stack(
+            [theta["v_WM_0"], theta["v_WM_1"], theta["v_WM_2"]]
+        )
+        theta["a"] = np.expand_dims(theta["a"], axis=1)
+        theta["z"] = np.expand_dims(theta["z"], axis=1)
+
+    validate_ssm_parameters(model, theta)
+
     # 2 Choice
     if model == "race_2":
         sim_param_dict["s"] = noise_dict["2_particles"]
         theta["z"] = np.column_stack([theta["z0"], theta["z1"]])
         theta["v"] = np.column_stack([theta["v0"], theta["v1"]])
         theta["t"] = np.expand_dims(theta["t"], axis=1)
         theta["a"] = np.expand_dims(theta["a"], axis=1)
@@ -755,14 +815,15 @@
         sim_param_dict["s"] = noise_dict["1_particles"]
         theta["zh"], theta["zl1"], theta["zl2"] = [z_vec, z_vec, z_vec]
 
     # print(theta)
     # print(boundary_dict)
     # print(drift_dict)
     # print(sim_param_dict)
+
     # Call to the simulator
     x = model_config[model]["simulator"](
         **theta,
         **boundary_dict,
         **drift_dict,
         **sim_param_dict,
     )
```

### Comparing `ssm-simulators-0.7.0/ssms/config/config.py` & `ssm_simulators-0.7.2/ssms/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,59 @@
         "boundary_name": "constant",
         "boundary": bf.constant,
         "n_params": 5,
         "default_params": [0.0, 1.0, 0.5, 1e-3, 1e-3],
         "nchoices": 2,
         "simulator": cssm.ddm_sdv,
     },
+    "lba_3_v1": {
+        "name": "lba_3_v1",  # LBA_3 without ndt; sum of all v = 1
+        "params": ["v0", "v1", "v2", "a", "z"],
+        "param_bounds": [[0.0, 0.0, 0.0, 0.1, 0.1], [1.0, 1.0, 1.0, 1.1, 0.50]],
+        "boundary_name": "constant",
+        "boundary": bf.constant,
+        "n_params": 5,
+        "default_params": [0.5, 0.3, 0.2, 0.5, 0.2],
+        "nchoices": 3,
+        "simulator": cssm.lba_vanilla,
+    },
+    "lba_angle_3_v1": {
+        "name": "lba_angle_3_v1",  # LBA_Angle_3 without ndt; sum of all v = 1
+        "params": ["v0", "v1", "v2", "a", "z", "theta"],
+        "param_bounds": [[0.0, 0.0, 0.0, 0.1, 0.0, 0], [1.0, 1.0, 1.0, 1.1, 0.5, 1.3]],
+        "boundary_name": "constant",
+        "boundary": bf.constant,
+        "n_params": 6,
+        "default_params": [0.5, 0.3, 0.2, 0.5, 0.2, 0.0],
+        "nchoices": 3,
+        "simulator": cssm.lba_angle,
+    },
+    "rlwm_lba_race_v1": {
+        "name": "rlwm_lba_race_wo_ndt_v1",  # RLWM_Race_LBA_3 without ndt; sum of all v_RL = 1 and sum of all v_WM = 1
+        "params": [
+            "v_RL_0",
+            "v_RL_1",
+            "v_RL_2",
+            "v_WM_0",
+            "v_WM_1",
+            "v_WM_2",
+            "a",
+            "z",
+        ],
+        "param_bounds": [
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.05, 0.0],
+            [1.0, 1.0, 1.0, 1.0, 1.0, 1.0, 1.1, 0.5],
+        ],
+        "boundary_name": "constant",
+        "boundary": bf.constant,
+        "n_params": 8,
+        "default_params": [0.5, 0.3, 0.2, 0.5, 0.3, 0.2, 0.5, 0.2],
+        "nchoices": 3,
+        "simulator": cssm.rlwm_lba_race,
+    },
     "race_2": {
         "name": "race_2",
         "params": ["v0", "v1", "a", "z0", "z1", "t"],
         "param_bounds": [
             [0.0, 0.0, 1.0, 0.0, 0.0, 0.0],
             [2.5, 2.5, 3.0, 0.9, 0.9, 2.0],
         ],
@@ -710,15 +755,15 @@
             [-4.0, -4.0, -4.0, 0.3, 0.0, 0.31, 0.31],
             [4.0, 4.0, 4.0, 2.5, 2.0, 4.99, 6.99],
         ],
         "boundary_name": "weibull_cdf",
         "boundary": bf.weibull_cdf,
         "boundary_multiplicative": True,
         "n_params": 7,
-        "default_params": [0.0, 0.0, 0.0, 1.0, 1.0, 0.0],
+        "default_params": [0.0, 0.0, 0.0, 1.0, 1.0, 0.0, 3.0],
         "nchoices": 4,
         "simulator": cssm.ddm_flexbound_par2,
     },
     "ddm_seq2": {
         "name": "ddm_seq2",
         "params": ["vh", "vl1", "vl2", "a", "zh", "zl1", "zl2", "t"],
         "param_bounds": [
```

### Comparing `ssm-simulators-0.7.0/ssms/dataset_generators/lan_mlp.py` & `ssm_simulators-0.7.2/ssms/dataset_generators/lan_mlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -244,39 +244,63 @@
         rt_tmp = np.random.uniform(low=-1.0, high=0.0001, size=n_unif_down)
 
         out[(n_kde + n_unif_up) :, -3] = rt_tmp
         out[(n_kde + n_unif_up) :, -2] = choice_tmp
         out[(n_kde + n_unif_up) :, -1] = self.generator_config["negative_rt_cutoff"]
         return out.astype(np.float32)
 
+    def parameter_transform_for_data_gen(self, theta):
+        """
+        Function to impose constraints on the parameters for data generation.
+        """
+
+        # For LBA-based models, we need to ensure that the drift rates sum to 1
+        if self.model_config["name"] == "rlwm_lba_race_wo_ndt_v1":
+            # normalize the RL drift rates
+            theta[0:3] = theta[0:3] / np.sum(theta[0:3])
+
+            # normalize the WM drift rates
+            theta[3:6] = theta[3:6] / np.sum(theta[3:6])
+
+            # ensure that a is always greater than z
+            if theta[6] <= theta[7]:
+                tmp = theta[6]
+                theta[6] = theta[7]
+                theta[7] = tmp
+
+        return theta
+
     def _mlp_get_processed_data_for_theta(self, random_seed_tuple):
         np.random.seed(random_seed_tuple[0])
         keep = 0
         while not keep:
             theta = np.float32(
                 np.random.uniform(
                     low=self.model_config["param_bounds"][0],
                     high=self.model_config["param_bounds"][1],
                 )
             )
+
+            theta = self.parameter_transform_for_data_gen(theta)
+
             theta_dict = {
                 name: val for name, val in zip(self.model_config["params"], theta)
             }
 
             simulations = self.get_simulations(
                 theta=theta_dict, random_seed=random_seed_tuple[1]
             )
             keep, stats = self._filter_simulations(simulations)
 
         kde_data = self._make_kde_data(simulations=simulations, theta=theta)
 
         if len(simulations["metadata"]["possible_choices"]) == 2:
-            cpn_labels = np.expand_dims(simulations["choice_p"][0, 0], axis=0)
+            cpn_labels = np.expand_dims(simulations["choice_p"][0, 1], axis=0)
             cpn_no_omission_labels = np.expand_dims(
-                simulations["choice_p_no_omission"][0, 0], axis=0
+                simulations["choice_p_no_omission"][0, 1], axis=0
             )
         else:
             cpn_labels = simulations["choice_p"]
             cpn_no_omission_labels = simulations["choice_p_no_omission"]
 
         return {
             "lan_data": kde_data[:, :-1],
@@ -309,71 +333,32 @@
         }
 
         # Run the simulator
         simulations = self.get_simulations(
             theta=theta_dict, random_seed=random_seed_tuple[1]
         )
 
-        # Compute the choice probabilities
-        out_dict = {}
-        out_dict["choice_p"] = np.zeros(
-            (1, len(simulations["metadata"]["possible_choices"]))
-        )
-        out_dict["choice_p_no_omission"] = np.zeros(
-            (1, len(simulations["metadata"]["possible_choices"]))
-        )
-        out_dict["omission_p"] = {}
-        out_dict["theta"] = np.expand_dims(theta, axis=0)
-
-        for k, choice in enumerate(simulations["metadata"]["possible_choices"]):
-            out_dict["choice_p"][k] = np.array(
-                [
-                    (simulations["choices"] == choice).sum()
-                    / simulations["choices"].flatten().shape[0]
-                ]
-            )
-            out_dict["choice_p_no_omission"][k] = np.array(
-                [
-                    (simulations["choices"][simulations["rts"] != -999] == choice).sum()
-                    / simulations["choices"].flatten().shape[0]
-                ]
+        if len(simulations["metadata"]["possible_choices"]) == 2:
+            cpn_labels = np.expand_dims(simulations["choice_p"][0, 1], axis=0)
+            cpn_no_omission_labels = np.expand_dims(
+                simulations["choice_p_no_omission"][0, 1], axis=0
             )
-
-        out_dict["omission_p"] = np.expand_dims(
-            np.array(
-                [
-                    (simulations["rts"] == -999).sum()
-                    / simulations["choices"].flatten().shape[0]
-                ]
-            ),
-            axis=0,
-        )
-        out_dict["nogo_p"] = np.expand_dims(
-            np.array(
-                [
-                    (simulations["rts"] == -999)
-                    | (
-                        simulations["choices"]
-                        != simulations["metadata"]["possible_choices"][0]
-                    )
-                ]
-            ),
-            axis=0,
-        )
-        out_dict["go_p"] = 1 - out_dict["nogo_p"]
+        else:
+            cpn_labels = simulations["choice_p"]
+            cpn_no_omission_labels = simulations["choice_p_no_omission"]
 
         return {
             "cpn_data": np.expand_dims(theta, axis=0),
-            "cpn_labels": out_dict["choice_p"],
+            "cpn_labels": cpn_labels,
             "cpn_no_omission_data": np.expand_dims(theta, axis=0),
-            "cpn_no_omission_labels": out_dict["choice_p_no_omission"],
+            "cpn_no_omission_labels": cpn_no_omission_labels,
             "opn_data": np.expand_dims(theta, axis=0),
-            "opn_labels": out_dict["omission_p"],
+            "opn_labels": simulations["omission_p"],
             "gonogo_data": np.expand_dims(theta, axis=0),
-            "gonogo_labels": out_dict["nogo_p"],
+            "gonogo_labels": simulations["nogo_p"],
             "theta": np.expand_dims(theta, axis=0),
         }
 
     def _get_rejected_parameter_setups(self, random_seed_tuple):
         np.random.seed(random_seed_tuple[0])
         rejected_thetas = []
         keep = 1
```

### Comparing `ssm-simulators-0.7.0/ssms/dataset_generators/snpe.py` & `ssm_simulators-0.7.2/ssms/dataset_generators/snpe.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/ssms/support_utils/kde_class.py` & `ssm_simulators-0.7.2/ssms/support_utils/kde_class.py`

 * *Files identical despite different names*

### Comparing `ssm-simulators-0.7.0/tests/test_simulator.py` & `ssm_simulators-0.7.2/tests/test_simulator.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,31 +14,22 @@
     # Prepare input data for each model
     for key in model_config.keys():
         # Get model parameter names
         model_param_list = model_config[key]["params"]
 
         # Dictionary with all scalar values
         theta_dict_all_scalars = {
-            param: np.mean(
-                [
-                    model_config[key]["param_bounds"][0][i],
-                    model_config[key]["param_bounds"][1][i],
-                ]
-            )
+            param: model_config[key]["default_params"][i]
             for i, param in enumerate(model_param_list)
         }
+
         # Dictionary with all vectors
         theta_dict_all_vectors = {
             param: np.tile(
-                np.mean(
-                    [
-                        model_config[key]["param_bounds"][0][i],
-                        model_config[key]["param_bounds"][1][i],
-                    ]
-                ),
+                np.array(model_config[key]["default_params"][i]),
                 100,
             )
             for i, param in enumerate(model_param_list)
         }
 
         # Dictionary with mix of scalars and vectors
         theta_dict_sca_vec = deepcopy(theta_dict_all_vectors)
@@ -59,20 +50,15 @@
             theta_dict_uneven[tmp_key] = np.concatenate(
                 [theta_dict_all_vectors[tmp_key], np.zeros(2)]
             )
             cnt += 1
 
         # Input is list
         theta_list = [
-            np.mean(
-                [
-                    model_config[key]["param_bounds"][0][i],
-                    model_config[key]["param_bounds"][1][i],
-                ]
-            )
+            model_config[key]["default_params"][i]
             for i, param in enumerate(model_param_list)
         ]
 
         # Input is numpy array
         theta_nparray = np.array(theta_list)
 
         # Input is pd.DataFrame
@@ -88,26 +74,27 @@
             "theta_dict_sca_vec": theta_dict_sca_vec,
             "theta_dict_uneven": theta_dict_uneven,
             "theta_list": theta_list,
             "theta_nparray": theta_nparray,
             "theta_pd_1": theta_pd_1,
             "theta_pd_n": theta_pd_n,
         }
+
     return data
 
 
 def test_simulator_runs(sim_input_data):
     """Test that simulator runs for all models"""
     # Go over model names
     for key in model_config.keys():
         # Go over different types of input data
         # (listed above in sim_input_data() fixture)
         for subkey in sim_input_data[key].keys():
-            print(subkey)
-            print(key)
+            print(key, " -> ", subkey)
+
             # Go over different number of samples
             if subkey == "theta_dict_uneven":
                 for n_samples in [1, 10]:
                     try:
                         out = simulator(
                             model=key, theta=sim_input_data[key][subkey], n_samples=1
                         )
```

