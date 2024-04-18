# Comparing `tmp/polynomial_generator-0.1.2a0.tar.gz` & `tmp/polynomial_generator-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polynomial_generator-0.1.2a0.tar", max compression
+gzip compressed data, was "polynomial_generator-0.1.2a1.tar", max compression
```

## Comparing `polynomial_generator-0.1.2a0.tar` & `polynomial_generator-0.1.2a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-04-11 11:14:32.772378 polynomial_generator-0.1.2a0/LICENSE
--rw-r--r--   0        0        0     2906 2024-04-11 11:39:05.819216 polynomial_generator-0.1.2a0/README.md
--rw-r--r--   0        0        0       55 2024-04-11 11:31:25.208211 polynomial_generator-0.1.2a0/polynomial_generator/__init__.py
--rw-r--r--   0        0        0     2330 2024-04-11 11:14:32.784378 polynomial_generator-0.1.2a0/polynomial_generator/polynomial.py
--rw-r--r--   0        0        0     2972 2024-04-11 11:30:47.239593 polynomial_generator-0.1.2a0/polynomial_generator/polynomial_app.py
--rw-r--r--   0        0        0      868 2024-04-11 11:30:51.899670 polynomial_generator-0.1.2a0/polynomial_generator/polynomial_cli.py
--rw-r--r--   0        0        0      599 2024-04-11 11:32:20.805101 polynomial_generator-0.1.2a0/polynomial_generator/pyinstaller_script.py
--rw-r--r--   0        0        0      654 2024-04-11 11:40:47.628681 polynomial_generator-0.1.2a0/pyproject.toml
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 polynomial_generator-0.1.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-11 11:14:32.772378 polynomial_generator-0.1.2a1/LICENSE
+-rw-r--r--   0        0        0     2906 2024-04-18 08:34:06.795630 polynomial_generator-0.1.2a1/README.md
+-rw-r--r--   0        0        0       55 2024-04-18 08:34:06.795630 polynomial_generator-0.1.2a1/polynomial_generator/__init__.py
+-rw-r--r--   0        0        0     2330 2024-04-11 11:14:32.784378 polynomial_generator-0.1.2a1/polynomial_generator/polynomial.py
+-rw-r--r--   0        0        0     2972 2024-04-18 08:34:06.795630 polynomial_generator-0.1.2a1/polynomial_generator/polynomial_app.py
+-rw-r--r--   0        0        0      868 2024-04-18 08:34:06.795630 polynomial_generator-0.1.2a1/polynomial_generator/polynomial_cli.py
+-rw-r--r--   0        0        0      599 2024-04-18 08:34:06.795630 polynomial_generator-0.1.2a1/polynomial_generator/pyinstaller_script.py
+-rw-r--r--   0        0        0     1567 2024-04-18 08:34:52.496136 polynomial_generator-0.1.2a1/pyproject.toml
+-rw-r--r--   0        0        0     4452 1970-01-01 00:00:00.000000 polynomial_generator-0.1.2a1/PKG-INFO
```

### Comparing `polynomial_generator-0.1.2a0/LICENSE` & `polynomial_generator-0.1.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.2a0/README.md` & `polynomial_generator-0.1.2a1/README.md`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.2a0/polynomial_generator/polynomial.py` & `polynomial_generator-0.1.2a1/polynomial_generator/polynomial.py`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.2a0/polynomial_generator/polynomial_app.py` & `polynomial_generator-0.1.2a1/polynomial_generator/polynomial_app.py`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.2a0/polynomial_generator/polynomial_cli.py` & `polynomial_generator-0.1.2a1/polynomial_generator/polynomial_cli.py`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.2a0/polynomial_generator/pyinstaller_script.py` & `polynomial_generator-0.1.2a1/polynomial_generator/pyinstaller_script.py`

 * *Files identical despite different names*

### Comparing `polynomial_generator-0.1.2a0/PKG-INFO` & `polynomial_generator-0.1.2a1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,40 @@
 Metadata-Version: 2.1
 Name: polynomial-generator
-Version: 0.1.2a0
+Version: 0.1.2a1
 Summary: A Python package for generating polynomial expressions
+Home-page: https://github.com/Hermann-web/polynomial-generator
 License: MIT
+Keywords: polynomial,generator,mathematics,CLI,GUI
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
+Maintainer: Hermann Agossou
+Maintainer-email: agossouhermann7@gmail.com
 Requires-Python: >=3.8,<3.13
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: MacOS X
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Environment :: X11 Applications :: GTK
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Documentation, https://github.com/Hermann-web/polynomial-generator
+Project-URL: Repository, https://github.com/Hermann-web/polynomial-generator
 Description-Content-Type: text/markdown
 
 # Polynomial Generator
 
 [![License](https://img.shields.io/github/license/hermann-web/polynomial-generator)](LICENSE)
 [![Release](https://img.shields.io/github/v/release/hermann-web/polynomial-generator)](https://github.com/hermann-web/polynomial-generator/releases)
```

