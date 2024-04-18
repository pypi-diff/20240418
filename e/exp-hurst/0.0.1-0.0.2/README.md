# Comparing `tmp/exp_hurst-0.0.1.tar.gz` & `tmp/exp_hurst-0.0.2.tar.gz`

## Comparing `exp_hurst-0.0.1.tar` & `exp_hurst-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exp_hurst-0.0.1/src/exp_hurst/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 exp_hurst-0.0.1/src/exp_hurst/exp_hurst.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 exp_hurst-0.0.1/LICENSE
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 exp_hurst-0.0.1/README.md
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 exp_hurst-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 exp_hurst-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exp_hurst-0.0.2/src/exp_hurst/__init__.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 exp_hurst-0.0.2/src/exp_hurst/exp_hurst.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 exp_hurst-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 exp_hurst-0.0.2/README.md
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 exp_hurst-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 exp_hurst-0.0.2/PKG-INFO
```

### Comparing `exp_hurst-0.0.1/LICENSE` & `exp_hurst-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exp_hurst-0.0.1/README.md` & `exp_hurst-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Hurst Exponent Package
 
 ## Description
 The function hurst takes a np.array of numbers and returns the Hurst exponent of the time series. The Hurst exponent is a measure of randomness of a time series. It is used in the study of long-term memory of time series. The value of the Hurst exponent is between 0 and 1. A value of 0.5 indicates that the time series is random. A value greater than 0.5 indicates that the time series is trending. A value less than 0.5 indicates that the time series is mean reverting.
 
 ## Installation
 ```bash
-pip install hurst
+pip install exp_hurst
 ```
 
 ## Requirements
 - numpy
 - mmq
 
 ## Usage
```

### Comparing `exp_hurst-0.0.1/PKG-INFO` & `exp_hurst-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: exp_hurst
-Version: 0.0.1
+Version: 0.0.2
 Summary: It computes the Hurst exponent of a time series.
 Author-email: Igor Jasenovski <igormjsk@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -13,15 +13,15 @@
 # Hurst Exponent Package
 
 ## Description
 The function hurst takes a np.array of numbers and returns the Hurst exponent of the time series. The Hurst exponent is a measure of randomness of a time series. It is used in the study of long-term memory of time series. The value of the Hurst exponent is between 0 and 1. A value of 0.5 indicates that the time series is random. A value greater than 0.5 indicates that the time series is trending. A value less than 0.5 indicates that the time series is mean reverting.
 
 ## Installation
 ```bash
-pip install hurst
+pip install exp_hurst
 ```
 
 ## Requirements
 - numpy
 - mmq
 
 ## Usage
```

