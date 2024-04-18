# Comparing `tmp/plorts-0.7.5.tar.gz` & `tmp/plorts-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plorts-0.7.5.tar", last modified: Tue Oct 11 00:24:11 2022, max compression
+gzip compressed data, was "plorts-0.7.6.tar", last modified: Thu Apr 18 01:49:03 2024, max compression
```

## Comparing `plorts-0.7.5.tar` & `plorts-0.7.6.tar`

### file list

```diff
@@ -1,29 +1,19 @@
-drwxr-xr-x   0 bspang     (501) staff       (20)        0 2022-10-11 00:24:11.958435 plorts-0.7.5/
--rw-r--r--   0 bspang     (501) staff       (20)     1055 2019-07-02 20:16:11.000000 plorts-0.7.5/LICENSE
--rw-r--r--   0 bspang     (501) staff       (20)       25 2019-10-03 21:21:12.000000 plorts-0.7.5/MANIFEST.in
--rw-r--r--   0 bspang     (501) staff       (20)     1422 2022-10-11 00:24:11.958608 plorts-0.7.5/PKG-INFO
--rw-r--r--   0 bspang     (501) staff       (20)      574 2020-11-29 19:54:05.000000 plorts-0.7.5/README.md
-drwxr-xr-x   0 bspang     (501) staff       (20)        0 2022-10-11 00:24:11.955981 plorts-0.7.5/plorts/
--rw-r--r--   0 bspang     (501) staff       (20)      294 2019-07-04 18:26:07.000000 plorts-0.7.5/plorts/__init__.py
--rw-r--r--   0 bspang     (501) staff       (20)     3976 2019-10-03 23:37:14.000000 plorts-0.7.5/plorts/legend.py
--rw-r--r--   0 bspang     (501) staff       (20)     2127 2019-07-04 19:31:55.000000 plorts-0.7.5/plorts/palettes.py
--rw-r--r--   0 bspang     (501) staff       (20)       29 2019-07-02 20:16:11.000000 plorts-0.7.5/plorts/plorts-col.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)      243 2019-10-03 22:56:50.000000 plorts-0.7.5/plorts/plorts-cool.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)       28 2019-07-02 20:16:11.000000 plorts-0.7.5/plorts/plorts-halfcol.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)      244 2019-10-03 22:56:54.000000 plorts-0.7.5/plorts/plorts-neon.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)       29 2019-07-02 20:16:11.000000 plorts-0.7.5/plorts/plorts-onehalfcol.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)      151 2019-07-02 20:16:11.000000 plorts-0.7.5/plorts/plorts-print.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)       28 2019-07-02 20:16:11.000000 plorts-0.7.5/plorts/plorts-twocol.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)      244 2019-10-03 22:56:46.000000 plorts-0.7.5/plorts/plorts-warm.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)      175 2019-07-02 20:16:11.000000 plorts-0.7.5/plorts/plorts-web.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)      576 2020-12-22 22:29:08.000000 plorts-0.7.5/plorts/plorts.mplstyle
--rw-r--r--   0 bspang     (501) staff       (20)     7800 2022-10-11 00:23:01.000000 plorts-0.7.5/plorts/plotting.py
--rw-r--r--   0 bspang     (501) staff       (20)     3286 2021-05-05 18:34:17.000000 plorts-0.7.5/plorts/style.py
-drwxr-xr-x   0 bspang     (501) staff       (20)        0 2022-10-11 00:24:11.958187 plorts-0.7.5/plorts.egg-info/
--rw-r--r--   0 bspang     (501) staff       (20)     1422 2022-10-11 00:24:11.000000 plorts-0.7.5/plorts.egg-info/PKG-INFO
--rw-r--r--   0 bspang     (501) staff       (20)      572 2022-10-11 00:24:11.000000 plorts-0.7.5/plorts.egg-info/SOURCES.txt
--rw-r--r--   0 bspang     (501) staff       (20)        1 2022-10-11 00:24:11.000000 plorts-0.7.5/plorts.egg-info/dependency_links.txt
--rw-r--r--   0 bspang     (501) staff       (20)       17 2022-10-11 00:24:11.000000 plorts-0.7.5/plorts.egg-info/requires.txt
--rw-r--r--   0 bspang     (501) staff       (20)        7 2022-10-11 00:24:11.000000 plorts-0.7.5/plorts.egg-info/top_level.txt
--rw-r--r--   0 bspang     (501) staff       (20)       67 2022-10-11 00:24:11.959287 plorts-0.7.5/setup.cfg
--rw-r--r--   0 bspang     (501) staff       (20)     2833 2019-10-03 21:20:49.000000 plorts-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:49:03.624167 plorts-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-18 01:48:59.000000 plorts-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-18 01:49:03.624167 plorts-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-18 01:48:59.000000 plorts-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:49:03.624167 plorts-0.7.6/plorts/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-18 01:48:59.000000 plorts-0.7.6/plorts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 01:48:59.000000 plorts-0.7.6/plorts/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-18 01:48:59.000000 plorts-0.7.6/plorts/legend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-18 01:48:59.000000 plorts-0.7.6/plorts/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7800 2024-04-18 01:48:59.000000 plorts-0.7.6/plorts/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-18 01:48:59.000000 plorts-0.7.6/plorts/style.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:49:03.624167 plorts-0.7.6/plorts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-18 01:49:03.000000 plorts-0.7.6/plorts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-18 01:49:03.000000 plorts-0.7.6/plorts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:49:03.000000 plorts-0.7.6/plorts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 01:49:03.000000 plorts-0.7.6/plorts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:49:03.000000 plorts-0.7.6/plorts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 01:49:03.628167 plorts-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-18 01:48:59.000000 plorts-0.7.6/setup.py
```

### Comparing `plorts-0.7.5/LICENSE` & `plorts-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `plorts-0.7.5/PKG-INFO` & `plorts-0.7.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: plorts
-Version: 0.7.5
+Version: 0.7.6
 Summary: Graphing wrapper around matplotlib
 Home-page: https://github.com/brucespang/plorts
 Author: Bruce Spang
 Author-email: bruce@brucespang.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
 
 # Plorts - Niceish python plots
 
 [![Documentation Status](https://readthedocs.org/projects/plorts/badge/?version=latest)](https://plorts.readthedocs.io/en/latest/?badge=latest)
 
 
-Like seaborn but with less stuff and also it starts faster
+A thin wrapper around matplotlib that handles a lot of common plots I need to make.
 
 ```
 $ pip install plorts
 ```
 
 ## Examples
 
@@ -39,9 +40,7 @@
 ![](output/line-plot.png)
 ![](output/scatter-plot.png)
 ![](output/stack-plot.png)
 ![](output/boxplot.png)
 ![](output/histogram.png)
 ![](output/cdf.png)
 ![](output/pdf.png)
-
-
```

### Comparing `plorts-0.7.5/README.md` & `plorts-0.7.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Plorts - Niceish python plots
 
 [![Documentation Status](https://readthedocs.org/projects/plorts/badge/?version=latest)](https://plorts.readthedocs.io/en/latest/?badge=latest)
 
 
-Like seaborn but with less stuff and also it starts faster
+A thin wrapper around matplotlib that handles a lot of common plots I need to make.
 
 ```
 $ pip install plorts
 ```
 
 ## Examples
```

### Comparing `plorts-0.7.5/plorts/legend.py` & `plorts-0.7.6/plorts/legend.py`

 * *Files identical despite different names*

### Comparing `plorts-0.7.5/plorts/palettes.py` & `plorts-0.7.6/plorts/palettes.py`

 * *Files identical despite different names*

### Comparing `plorts-0.7.5/plorts/plotting.py` & `plorts-0.7.6/plorts/plotting.py`

 * *Files identical despite different names*

### Comparing `plorts-0.7.5/plorts/style.py` & `plorts-0.7.6/plorts/style.py`

 * *Files identical despite different names*

### Comparing `plorts-0.7.5/plorts.egg-info/PKG-INFO` & `plorts-0.7.6/plorts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: plorts
-Version: 0.7.5
+Version: 0.7.6
 Summary: Graphing wrapper around matplotlib
 Home-page: https://github.com/brucespang/plorts
 Author: Bruce Spang
 Author-email: bruce@brucespang.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: numpy
 
 # Plorts - Niceish python plots
 
 [![Documentation Status](https://readthedocs.org/projects/plorts/badge/?version=latest)](https://plorts.readthedocs.io/en/latest/?badge=latest)
 
 
-Like seaborn but with less stuff and also it starts faster
+A thin wrapper around matplotlib that handles a lot of common plots I need to make.
 
 ```
 $ pip install plorts
 ```
 
 ## Examples
 
@@ -39,9 +40,7 @@
 ![](output/line-plot.png)
 ![](output/scatter-plot.png)
 ![](output/stack-plot.png)
 ![](output/boxplot.png)
 ![](output/histogram.png)
 ![](output/cdf.png)
 ![](output/pdf.png)
-
-
```

### Comparing `plorts-0.7.5/setup.py` & `plorts-0.7.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,82 @@
 """A setuptools based setup module.
 
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
+import re
+
 # To use a consistent encoding
 from codecs import open
 from os import path
 
+# Always prefer setuptools over distutils
+from setuptools import find_packages, setup
+
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-# Get the version from the VERSION file
-with open(path.join(here, 'VERSION'), encoding='utf-8') as f:
-    version = f.read()
+# Get the version from the version file
+version_filename = "plorts/_version.py"
+version_file = open(version_filename, "rt").read()
+version_regex = r"^__version__ = ['\"]([^'\"]*)['\"]"
+mo = re.search(version_regex, version_file, re.M)
+if mo:
+    version_string = mo.group(1)
+else:
+    raise RuntimeError("Unable to find version string in %s." % (version_filename,))
 
-setup(
-    name='plorts',
 
+setup(
+    name="plorts",
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version=version,
-
-    description='Graphing wrapper around matplotlib',
+    version=version_string,
+    description="Graphing wrapper around matplotlib",
     long_description=long_description,
-
     # The project's main homepage.
-    url='https://github.com/brucespang/plorts',
-
+    url="https://github.com/brucespang/plorts",
     # Author details
-    author='Bruce Spang',
-    author_email='bruce@brucespang.com',
-
+    author="Bruce Spang",
+    author_email="bruce@brucespang.com",
     # Choose your license
-    license='MIT',
-
+    license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 4 - Beta',
-
+        "Development Status :: 4 - Beta",
         # Indicate who your project is intended for
-        'Intended Audience :: Science/Research',
-
-        'Topic :: Multimedia :: Graphics',
-        'Topic :: Scientific/Engineering :: Visualization',
-
+        "Intended Audience :: Science/Research",
+        "Topic :: Multimedia :: Graphics",
+        "Topic :: Scientific/Engineering :: Visualization",
         # Pick your license as you wish (should match "license" above)
-        'License :: OSI Approved :: MIT License',
-
+        "License :: OSI Approved :: MIT License",
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
+        "Programming Language :: Python :: 2",
+        "Programming Language :: Python :: 2.6",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
     ],
-
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
-    packages=find_packages(exclude=['contrib', 'docs', 'tests']),
-
+    packages=find_packages(exclude=["contrib", "docs", "tests"]),
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['matplotlib','numpy'],
-
+    install_requires=["matplotlib", "numpy"],
     # include matplotlib style files
     include_package_data=True,
 )
```

