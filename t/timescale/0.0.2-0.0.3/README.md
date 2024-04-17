# Comparing `tmp/timescale-0.0.2.tar.gz` & `tmp/timescale-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timescale-0.0.2.tar", last modified: Fri Aug 25 16:40:07 2023, max compression
+gzip compressed data, was "timescale-0.0.3.tar", last modified: Wed Apr 17 22:06:00 2024, max compression
```

## Comparing `timescale-0.0.2.tar` & `timescale-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 16:40:07.147912 timescale-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (998)      955 2023-08-25 16:39:55.000000 timescale-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (998)     5545 2023-08-25 16:39:55.000000 timescale-0.0.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (998)      620 2023-08-25 16:39:55.000000 timescale-0.0.2/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (998)     1074 2023-08-25 16:39:55.000000 timescale-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (998)      132 2023-08-25 16:39:55.000000 timescale-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (998)     3422 2023-08-25 16:40:07.147912 timescale-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (998)     2587 2023-08-25 16:39:55.000000 timescale-0.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (998)       36 2023-08-25 16:39:55.000000 timescale-0.0.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (998)       48 2023-08-25 16:39:55.000000 timescale-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (998)       38 2023-08-25 16:40:07.147912 timescale-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (998)     2200 2023-08-25 16:39:55.000000 timescale-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 16:40:07.147912 timescale-0.0.2/timescale/
--rw-r--r--   0 runner    (1001) docker     (998)      410 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 16:40:07.147912 timescale-0.0.2/timescale/data/
--rwxr-xr-x   0 runner    (1001) docker     (998)    12600 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (998)    30345 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/historic_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (998)   130160 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/iers_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (998)    10666 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/leap-seconds.list
--rwxr-xr-x   0 runner    (1001) docker     (998)   156360 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/merged_deltat.data
--rwxr-xr-x   0 runner    (1001) docker     (998)    34592 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/ser7.dat
--rw-r--r--   0 runner    (1001) docker     (998)     5849 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/tab5.2e.txt
--rw-r--r--   0 runner    (1001) docker     (998)   145678 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/tab5.3a.txt
--rw-r--r--   0 runner    (1001) docker     (998)   113660 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/data/tab5.3b.txt
--rw-r--r--   0 runner    (1001) docker     (998)    17871 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/eop.py
--rw-r--r--   0 runner    (1001) docker     (998)    61985 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/time.py
--rw-r--r--   0 runner    (1001) docker     (998)    50772 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/utilities.py
--rw-r--r--   0 runner    (1001) docker     (998)      390 2023-08-25 16:39:55.000000 timescale-0.0.2/timescale/version.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 16:40:07.147912 timescale-0.0.2/timescale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (998)     3422 2023-08-25 16:40:07.000000 timescale-0.0.2/timescale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (998)      669 2023-08-25 16:40:07.000000 timescale-0.0.2/timescale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 16:40:07.000000 timescale-0.0.2/timescale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (998)       48 2023-08-25 16:40:07.000000 timescale-0.0.2/timescale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (998)       15 2023-08-25 16:40:07.000000 timescale-0.0.2/timescale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (998)        6 2023-08-25 16:39:55.000000 timescale-0.0.2/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:06:00.126235 timescale-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-17 22:05:49.000000 timescale-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-04-17 22:05:49.000000 timescale-0.0.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-17 22:05:49.000000 timescale-0.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-17 22:05:49.000000 timescale-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 22:05:49.000000 timescale-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-17 22:06:00.126235 timescale-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-17 22:05:49.000000 timescale-0.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 22:05:49.000000 timescale-0.0.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 22:05:49.000000 timescale-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 22:06:00.126235 timescale-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-17 22:05:49.000000 timescale-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:06:00.118235 timescale-0.0.3/timescale/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:06:00.126235 timescale-0.0.3/timescale/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12600 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)  3597756 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/finals.all
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30345 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/historic_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)   130160 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/iers_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5068 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/leap-seconds.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    79520 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/mean-pole.tab
+-rwxr-xr-x   0 runner    (1001) docker     (127)   160980 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/merged_deltat.data
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34592 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/ser7.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/tab5.2e.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   145678 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/tab5.3a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   113660 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/data/tab5.3b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17867 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/eop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    64917 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51959 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-17 22:05:49.000000 timescale-0.0.3/timescale/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 22:06:00.126235 timescale-0.0.3/timescale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-17 22:06:00.000000 timescale-0.0.3/timescale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-17 22:06:00.000000 timescale-0.0.3/timescale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 22:06:00.000000 timescale-0.0.3/timescale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 22:06:00.000000 timescale-0.0.3/timescale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 22:06:00.000000 timescale-0.0.3/timescale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 22:05:49.000000 timescale-0.0.3/version.txt
```

### Comparing `timescale-0.0.2/.gitignore` & `timescale-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/CODE_OF_CONDUCT.rst` & `timescale-0.0.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/CONTRIBUTORS.rst` & `timescale-0.0.3/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/LICENSE` & `timescale-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/PKG-INFO` & `timescale-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timescale
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python tools for time and astronomical calculations.
 Home-page: https://github.com/tsutterley/timescale
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Time,leap seconds,TAI,GPS,UT1,TT
 Classifier: Development Status :: 3 - Alpha
@@ -15,24 +15,30 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: numpy
+Requires-Dist: python-dateutil
+Requires-Dist: scipy
+Requires-Dist: setuptools_scm
 
 =========
 timescale
 =========
 
 |Language|
 |License|
 |PyPI Version|
 |Anaconda-Server|
 |Documentation Status|
+|zenodo|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/pyTMD?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/github/license/tsutterley/timescale
    :target: https://github.com/tsutterley/timescale/blob/main/LICENSE
 
@@ -41,14 +47,17 @@
 
 .. |Anaconda-Server| image:: https://img.shields.io/conda/vn/conda-forge/timescale
    :target: https://anaconda.org/conda-forge/timescale
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/timescale/badge/?version=latest
    :target: https://timescale.readthedocs.io/en/latest/?badge=latest
 
+.. |zenodo| image:: https://zenodo.org/badge/681330279.svg
+   :target: https://zenodo.org/badge/latestdoi/681330279
+
 Python tools for time and astronomical calculations
 
 Dependencies
 ############
 
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
```

### Comparing `timescale-0.0.2/README.rst` & `timescale-0.0.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 =========
 
 |Language|
 |License|
 |PyPI Version|
 |Anaconda-Server|
 |Documentation Status|
+|zenodo|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/pyTMD?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/github/license/tsutterley/timescale
    :target: https://github.com/tsutterley/timescale/blob/main/LICENSE
 
@@ -19,14 +20,17 @@
 
 .. |Anaconda-Server| image:: https://img.shields.io/conda/vn/conda-forge/timescale
    :target: https://anaconda.org/conda-forge/timescale
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/timescale/badge/?version=latest
    :target: https://timescale.readthedocs.io/en/latest/?badge=latest
 
+.. |zenodo| image:: https://zenodo.org/badge/681330279.svg
+   :target: https://zenodo.org/badge/latestdoi/681330279
+
 Python tools for time and astronomical calculations
 
 Dependencies
 ############
 
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
```

### Comparing `timescale-0.0.2/setup.py` & `timescale-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/data/deltat.data` & `timescale-0.0.3/timescale/data/deltat.data`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/data/historic_deltat.data` & `timescale-0.0.3/timescale/data/historic_deltat.data`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/data/iers_deltat.data` & `timescale-0.0.3/timescale/data/iers_deltat.data`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/data/merged_deltat.data` & `timescale-0.0.3/timescale/data/merged_deltat.data`

 * *Files 2% similar despite different names*

```diff
@@ -7812,7 +7812,238 @@
  2023  8 18 69.1890
  2023  8 19 69.1886
  2023  8 20 69.1883
  2023  8 21 69.1879
  2023  8 22 69.1874
  2023  8 23 69.1868
  2023  8 24 69.1861
+ 2023  8 25 69.1853
+ 2023  8 26 69.1843
+ 2023  8 27 69.1832
+ 2023  8 28 69.1823
+ 2023  8 29 69.1815
+ 2023  8 30 69.1811
+ 2023  8 31 69.1812
+ 2023  9  1 69.1814
+ 2023  9  2 69.1818
+ 2023  9  3 69.1821
+ 2023  9  4 69.1822
+ 2023  9  5 69.1820
+ 2023  9  6 69.1813
+ 2023  9  7 69.1805
+ 2023  9  8 69.1796
+ 2023  9  9 69.1786
+ 2023  9 10 69.1777
+ 2023  9 11 69.1768
+ 2023  9 12 69.1760
+ 2023  9 13 69.1754
+ 2023  9 14 69.1751
+ 2023  9 15 69.1749
+ 2023  9 16 69.1748
+ 2023  9 17 69.1748
+ 2023  9 18 69.1746
+ 2023  9 19 69.1743
+ 2023  9 20 69.1739
+ 2023  9 21 69.1735
+ 2023  9 22 69.1728
+ 2023  9 23 69.1721
+ 2023  9 24 69.1713
+ 2023  9 25 69.1707
+ 2023  9 26 69.1703
+ 2023  9 27 69.1701
+ 2023  9 28 69.1704
+ 2023  9 29 69.1710
+ 2023  9 30 69.1717
+ 2023 10  1 69.1723
+ 2023 10  2 69.1727
+ 2023 10  3 69.1727
+ 2023 10  4 69.1725
+ 2023 10  5 69.1720
+ 2023 10  6 69.1713
+ 2023 10  7 69.1706
+ 2023 10  8 69.1701
+ 2023 10  9 69.1696
+ 2023 10 10 69.1694
+ 2023 10 11 69.1693
+ 2023 10 12 69.1694
+ 2023 10 13 69.1697
+ 2023 10 14 69.1700
+ 2023 10 15 69.1704
+ 2023 10 16 69.1706
+ 2023 10 17 69.1707
+ 2023 10 18 69.1706
+ 2023 10 19 69.1704
+ 2023 10 20 69.1701
+ 2023 10 21 69.1698
+ 2023 10 22 69.1696
+ 2023 10 23 69.1695
+ 2023 10 24 69.1697
+ 2023 10 25 69.1703
+ 2023 10 26 69.1710
+ 2023 10 27 69.1718
+ 2023 10 28 69.1725
+ 2023 10 29 69.1730
+ 2023 10 30 69.1731
+ 2023 10 31 69.1730
+ 2023 11  1 69.1727
+ 2023 11  2 69.1723
+ 2023 11  3 69.1717
+ 2023 11  4 69.1713
+ 2023 11  5 69.1710
+ 2023 11  6 69.1709
+ 2023 11  7 69.1710
+ 2023 11  8 69.1712
+ 2023 11  9 69.1716
+ 2023 11 10 69.1721
+ 2023 11 11 69.1726
+ 2023 11 12 69.1731
+ 2023 11 13 69.1734
+ 2023 11 14 69.1735
+ 2023 11 15 69.1734
+ 2023 11 16 69.1732
+ 2023 11 17 69.1732
+ 2023 11 18 69.1729
+ 2023 11 19 69.1727
+ 2023 11 20 69.1727
+ 2023 11 21 69.1729
+ 2023 11 22 69.1733
+ 2023 11 23 69.1737
+ 2023 11 24 69.1742
+ 2023 11 25 69.1745
+ 2023 11 26 69.1746
+ 2023 11 27 69.1745
+ 2023 11 28 69.1742
+ 2023 11 29 69.1736
+ 2023 11 30 69.1730
+ 2023 12  1 69.1724
+ 2023 12  2 69.1720
+ 2023 12  3 69.1717
+ 2023 12  4 69.1716
+ 2023 12  5 69.1716
+ 2023 12  6 69.1717
+ 2023 12  7 69.1720
+ 2023 12  8 69.1724
+ 2023 12  9 69.1726
+ 2023 12 10 69.1728
+ 2023 12 11 69.1728
+ 2023 12 12 69.1726
+ 2023 12 13 69.1723
+ 2023 12 14 69.1720
+ 2023 12 15 69.1715
+ 2023 12 16 69.1713
+ 2023 12 17 69.1714
+ 2023 12 18 69.1717
+ 2023 12 19 69.1723
+ 2023 12 20 69.1730
+ 2023 12 21 69.1739
+ 2023 12 22 69.1746
+ 2023 12 23 69.1753
+ 2023 12 24 69.1756
+ 2023 12 25 69.1756
+ 2023 12 26 69.1755
+ 2023 12 27 69.1755
+ 2023 12 28 69.1754
+ 2023 12 29 69.1751
+ 2023 12 30 69.1750
+ 2023 12 31 69.1751
+ 2024  1  1 69.1752
+ 2024  1  2 69.1755
+ 2024  1  3 69.1759
+ 2024  1  4 69.1763
+ 2024  1  5 69.1767
+ 2024  1  6 69.1770
+ 2024  1  7 69.1772
+ 2024  1  8 69.1772
+ 2024  1  9 69.1769
+ 2024  1 10 69.1766
+ 2024  1 11 69.1762
+ 2024  1 12 69.1758
+ 2024  1 13 69.1757
+ 2024  1 14 69.1758
+ 2024  1 15 69.1762
+ 2024  1 16 69.1768
+ 2024  1 17 69.1774
+ 2024  1 18 69.1779
+ 2024  1 19 69.1783
+ 2024  1 20 69.1784
+ 2024  1 21 69.1784
+ 2024  1 22 69.1781
+ 2024  1 23 69.1778
+ 2024  1 24 69.1775
+ 2024  1 25 69.1773
+ 2024  1 26 69.1771
+ 2024  1 27 69.1772
+ 2024  1 28 69.1775
+ 2024  1 29 69.1779
+ 2024  1 30 69.1785
+ 2024  1 31 69.1791
+ 2024  2  1 69.1797
+ 2024  2  2 69.1803
+ 2024  2  3 69.1806
+ 2024  2  4 69.1808
+ 2024  2  5 69.1808
+ 2024  2  6 69.1807
+ 2024  2  7 69.1805
+ 2024  2  8 69.1804
+ 2024  2  9 69.1805
+ 2024  2 10 69.1808
+ 2024  2 11 69.1816
+ 2024  2 12 69.1826
+ 2024  2 13 69.1838
+ 2024  2 14 69.1848
+ 2024  2 15 69.1858
+ 2024  2 16 69.1864
+ 2024  2 17 69.1868
+ 2024  2 18 69.1869
+ 2024  2 19 69.1868
+ 2024  2 20 69.1865
+ 2024  2 21 69.1862
+ 2024  2 22 69.1860
+ 2024  2 23 69.1858
+ 2024  2 24 69.1857
+ 2024  2 25 69.1859
+ 2024  2 26 69.1861
+ 2024  2 27 69.1865
+ 2024  2 28 69.1868
+ 2024  2 29 69.1871
+ 2024  3  1 69.1874
+ 2024  3  2 69.1875
+ 2024  3  3 69.1875
+ 2024  3  4 69.1873
+ 2024  3  5 69.1870
+ 2024  3  6 69.1866
+ 2024  3  7 69.1865
+ 2024  3  8 69.1867
+ 2024  3  9 69.1872
+ 2024  3 10 69.1882
+ 2024  3 11 69.1894
+ 2024  3 12 69.1906
+ 2024  3 13 69.1917
+ 2024  3 14 69.1925
+ 2024  3 15 69.1931
+ 2024  3 16 69.1933
+ 2024  3 17 69.1933
+ 2024  3 18 69.1931
+ 2024  3 19 69.1931
+ 2024  3 20 69.1932
+ 2024  3 21 69.1934
+ 2024  3 22 69.1938
+ 2024  3 23 69.1943
+ 2024  3 24 69.1949
+ 2024  3 25 69.1956
+ 2024  3 26 69.1965
+ 2024  3 27 69.1972
+ 2024  3 28 69.1978
+ 2024  3 29 69.1982
+ 2024  3 30 69.1985
+ 2024  3 31 69.1985
+ 2024  4  1 69.1983
+ 2024  4  2 69.1980
+ 2024  4  3 69.1977
+ 2024  4  4 69.1975
+ 2024  4  5 69.1977
+ 2024  4  6 69.1982
+ 2024  4  7 69.1989
+ 2024  4  8 69.1999
+ 2024  4  9 69.2008
+ 2024  4 10 69.2015
+ 2024  4 11 69.2019
```

### Comparing `timescale-0.0.2/timescale/data/ser7.dat` & `timescale-0.0.3/timescale/data/ser7.dat`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
                                                                                
       **********************************************************************   
       *                                                                    *   
       *                   I E R S   B U L L E T I N - A                    *   
       *                                                                    *   
       *           Rapid Service/Prediction of Earth Orientation            *   
       **********************************************************************   
-      24 August 2023                                      Vol. XXXVI No. 034   
+      11 April 2024                                      Vol. XXXVII No. 015   
       ______________________________________________________________________   
       GENERAL INFORMATION:                                                     
          MJD = Julian Date - 2 400 000.5 days                                  
          UT2-UT1 = 0.022 sin(2*pi*T) - 0.012 cos(2*pi*T)                       
                                      - 0.006 sin(4*pi*T) + 0.007 cos(4*pi*T)   
             where pi = 3.14159265... and T is the date in Besselian years.     
          TT = TAI + 32.184 seconds                                             
          DUT1= (UT1-UTC) transmitted with time signals                         
              =  0.0 seconds beginning 28 July 2022 at 0000 UTC                 
          Beginning 1 January 2017:                                             
             TAI-UTC = 37.000 000 seconds                                       
      ***********************************************************************
      * ANNOUNCEMENTS:                                                      *
      *                                                                     *
-     * NO leap second will be introduced at the end of December 2023.      *
+     * NO leap second will be introduced at the end of June 2024.          *
      *                                                                     *
      * The primary source for IERS Rapid Service/Prediction Center (RS/PC) *
      * data products is the official IERS RS/PC website:                   *
      *   https://maia.usno.navy.mil                                        *
      *                                                                     *
      * IERS RS/PC products are also available from:                        *
      *   NASA CDDIS: https://cddis.nasa.gov/archive/products/iers/         *
@@ -49,425 +49,425 @@
      ________________________________________________________________________  
                                                                                
       COMBINED EARTH ORIENTATION PARAMETERS:                                   
                                                                                
                               IERS Rapid Service                               
               MJD      x    error     y    error   UT1-UTC   error             
                        "      "       "      "        s        s               
-   23  8 18  60174 0.28523 .00009 0.44297 .00009 -0.004979 0.000019          
-   23  8 19  60175 0.28654 .00009 0.44065 .00009 -0.004605 0.000017          
-   23  8 20  60176 0.28771 .00009 0.43816 .00009 -0.004266 0.000014          
-   23  8 21  60177 0.28867 .00009 0.43539 .00009 -0.003851 0.000013          
-   23  8 22  60178 0.28982 .00009 0.43245 .00009 -0.003363 0.000010          
-   23  8 23  60179 0.29125 .00009 0.42978 .00009 -0.002823 0.000010          
-   23  8 24  60180 0.29262 .00009 0.42735 .00009 -0.002133 0.000008          
+   24  4  5  60405 -.01044 .00009 0.34883 .00009 -0.013665 0.000010          
+   24  4  6  60406 -.00963 .00009 0.35130 .00009 -0.014155 0.000011          
+   24  4  7  60407 -.00920 .00009 0.35382 .00009 -0.014948 0.000009          
+   24  4  8  60408 -.00911 .00009 0.35640 .00009 -0.015943 0.000010          
+   24  4  9  60409 -.00915 .00009 0.35881 .00009 -0.016785 0.000010          
+   24  4 10  60410 -.00873 .00009 0.36071 .00009 -0.017470 0.000010          
+   24  4 11  60411 -.00794 .00009 0.36266 .00009 -0.017865 0.000009          
                                                                                
       _______________________________________________________________________  
                                                                                
       PREDICTIONS:                                                             
       The following formulas will not reproduce the predictions given below,   
       but may be used to extend the predictions beyond the end of this table.  
                                                                                
-      x =  0.1388 + 0.0905 cos A + 0.0339 sin A + 0.0652 cos C + 0.0449 sin C  
-      y =  0.3484 + 0.0358 cos A - 0.0819 sin A + 0.0449 cos C - 0.0652 sin C  
-         UT1-UTC = -0.0375 + 0.00008 (MJD - 60188) - (UT2-UT1)                 
+      x =  0.1477 - 0.0896 cos A + 0.0473 sin A - 0.0615 cos C - 0.0334 sin C  
+      y =  0.3534 + 0.0417 cos A + 0.0797 sin A - 0.0334 cos C + 0.0615 sin C  
+         UT1-UTC =  0.0186 + 0.00008 (MJD - 60419) - (UT2-UT1)                 
                                                                                
-      where A = 2*pi*(MJD-60180)/365.25 and C = 2*pi*(MJD-60180)/435.          
+      where A = 2*pi*(MJD-60411)/365.25 and C = 2*pi*(MJD-60411)/435.          
                                                                                
-         TAI-UTC(MJD 60181) = 37.0                                             
+         TAI-UTC(MJD 60412) = 37.0                                             
       The accuracy may be estimated from the expressions:                      
-      S x,y = 0.00068 (MJD-60180)**0.80   S t = 0.00025 (MJD-60180)**0.75      
+      S x,y = 0.00068 (MJD-60411)**0.80   S t = 0.00025 (MJD-60411)**0.75      
       Estimated accuracies are:  Predictions     10 d   20 d   30 d   40 d     
                                  Polar coord's  0.004  0.007  0.010  0.013     
                                  UT1-UTC        0.0014 0.0024 0.0032 0.0040    
                                                                                
                     MJD      x(arcsec)   y(arcsec)   UT1-UTC(sec)              
-       2023  8 25  60181       0.2938      0.4250     -0.00128         
-       2023  8 26  60182       0.2948      0.4227     -0.00026         
-       2023  8 27  60183       0.2957      0.4203      0.00083         
-       2023  8 28  60184       0.2965      0.4180      0.00186         
-       2023  8 29  60185       0.2972      0.4156      0.00266         
-       2023  8 30  60186       0.2980      0.4131      0.00311         
-       2023  8 31  60187       0.2987      0.4107      0.00317         
-       2023  9  1  60188       0.2994      0.4082      0.00295         
-       2023  9  2  60189       0.3001      0.4058      0.00258         
-       2023  9  3  60190       0.3008      0.4034      0.00228         
-       2023  9  4  60191       0.3014      0.4009      0.00220         
-       2023  9  5  60192       0.3020      0.3984      0.00242         
-       2023  9  6  60193       0.3025      0.3960      0.00292         
-       2023  9  7  60194       0.3030      0.3935      0.00366         
-       2023  9  8  60195       0.3035      0.3910      0.00452         
-       2023  9  9  60196       0.3039      0.3886      0.00541         
-       2023  9 10  60197       0.3042      0.3861      0.00624         
-       2023  9 11  60198       0.3045      0.3837      0.00694         
-       2023  9 12  60199       0.3047      0.3813      0.00748         
-       2023  9 13  60200       0.3049      0.3788      0.00780         
-       2023  9 14  60201       0.3050      0.3764      0.00790         
-       2023  9 15  60202       0.3051      0.3739      0.00781         
-       2023  9 16  60203       0.3051      0.3714      0.00757         
-       2023  9 17  60204       0.3052      0.3690      0.00724         
-       2023  9 18  60205       0.3052      0.3665      0.00691         
-       2023  9 19  60206       0.3051      0.3640      0.00664         
-       2023  9 20  60207       0.3050      0.3616      0.00651         
-       2023  9 21  60208       0.3049      0.3591      0.00653         
-       2023  9 22  60209       0.3047      0.3567      0.00669         
-       2023  9 23  60210       0.3044      0.3542      0.00694         
-       2023  9 24  60211       0.3042      0.3518      0.00718         
-       2023  9 25  60212       0.3038      0.3494      0.00729         
-       2023  9 26  60213       0.3035      0.3469      0.00713         
-       2023  9 27  60214       0.3031      0.3445      0.00665         
-       2023  9 28  60215       0.3026      0.3421      0.00585         
-       2023  9 29  60216       0.3021      0.3397      0.00483         
-       2023  9 30  60217       0.3016      0.3373      0.00377         
-       2023 10  1  60218       0.3010      0.3349      0.00282         
-       2023 10  2  60219       0.3004      0.3325      0.00212         
-       2023 10  3  60220       0.2998      0.3301      0.00171         
-       2023 10  4  60221       0.2991      0.3278      0.00158         
-       2023 10  5  60222       0.2984      0.3254      0.00166         
-       2023 10  6  60223       0.2976      0.3231      0.00184         
-       2023 10  7  60224       0.2968      0.3208      0.00202         
-       2023 10  8  60225       0.2960      0.3185      0.00213         
-       2023 10  9  60226       0.2951      0.3162      0.00209         
-       2023 10 10  60227       0.2942      0.3139      0.00188         
-       2023 10 11  60228       0.2932      0.3116      0.00149         
-       2023 10 12  60229       0.2923      0.3094      0.00092         
-       2023 10 13  60230       0.2912      0.3071      0.00022         
-       2023 10 14  60231       0.2902      0.3049     -0.00057         
-       2023 10 15  60232       0.2891      0.3027     -0.00135         
-       2023 10 16  60233       0.2879      0.3005     -0.00205         
-       2023 10 17  60234       0.2868      0.2984     -0.00259         
-       2023 10 18  60235       0.2855      0.2962     -0.00295         
-       2023 10 19  60236       0.2843      0.2941     -0.00312         
-       2023 10 20  60237       0.2830      0.2920     -0.00316         
-       2023 10 21  60238       0.2817      0.2899     -0.00316         
-       2023 10 22  60239       0.2804      0.2879     -0.00325         
-       2023 10 23  60240       0.2790      0.2858     -0.00356         
-       2023 10 24  60241       0.2776      0.2838     -0.00417         
-       2023 10 25  60242       0.2761      0.2818     -0.00510         
-       2023 10 26  60243       0.2747      0.2799     -0.00631         
-       2023 10 27  60244       0.2731      0.2779     -0.00765         
-       2023 10 28  60245       0.2716      0.2760     -0.00896         
-       2023 10 29  60246       0.2700      0.2741     -0.01009         
-       2023 10 30  60247       0.2684      0.2723     -0.01092         
-       2023 10 31  60248       0.2668      0.2704     -0.01145         
-       2023 11  1  60249       0.2651      0.2686     -0.01172         
-       2023 11  2  60250       0.2635      0.2668     -0.01182         
-       2023 11  3  60251       0.2617      0.2650     -0.01186         
-       2023 11  4  60252       0.2600      0.2633     -0.01192         
-       2023 11  5  60253       0.2582      0.2616     -0.01207         
-       2023 11  6  60254       0.2564      0.2599     -0.01237         
-       2023 11  7  60255       0.2546      0.2583     -0.01282         
-       2023 11  8  60256       0.2528      0.2567     -0.01343         
-       2023 11  9  60257       0.2509      0.2551     -0.01417         
-       2023 11 10  60258       0.2490      0.2535     -0.01499         
-       2023 11 11  60259       0.2471      0.2520     -0.01581         
-       2023 11 12  60260       0.2451      0.2505     -0.01656         
-       2023 11 13  60261       0.2431      0.2490     -0.01717         
-       2023 11 14  60262       0.2412      0.2476     -0.01757         
-       2023 11 15  60263       0.2391      0.2462     -0.01776         
-       2023 11 16  60264       0.2371      0.2448     -0.01776         
-       2023 11 17  60265       0.2351      0.2435     -0.01768         
-       2023 11 18  60266       0.2330      0.2422     -0.01763         
-       2023 11 19  60267       0.2309      0.2409     -0.01773         
-       2023 11 20  60268       0.2288      0.2396     -0.01807         
-       2023 11 21  60269       0.2266      0.2384     -0.01868         
-       2023 11 22  60270       0.2245      0.2373     -0.01952         
-       2023 11 23  60271       0.2223      0.2361     -0.02050         
-       2023 11 24  60272       0.2202      0.2350     -0.02147         
-       2023 11 25  60273       0.2180      0.2339     -0.02231         
-       2023 11 26  60274       0.2157      0.2329     -0.02289         
-       2023 11 27  60275       0.2135      0.2319     -0.02319         
-       2023 11 28  60276       0.2113      0.2309     -0.02321         
-       2023 11 29  60277       0.2090      0.2300     -0.02304         
-       2023 11 30  60278       0.2068      0.2291     -0.02276         
-       2023 12  1  60279       0.2045      0.2283     -0.02248         
-       2023 12  2  60280       0.2022      0.2274     -0.02227         
-       2023 12  3  60281       0.1999      0.2266     -0.02219         
-       2023 12  4  60282       0.1976      0.2259     -0.02227         
-       2023 12  5  60283       0.1953      0.2252     -0.02250         
-       2023 12  6  60284       0.1930      0.2245     -0.02287         
-       2023 12  7  60285       0.1906      0.2239     -0.02333         
-       2023 12  8  60286       0.1883      0.2233     -0.02381         
-       2023 12  9  60287       0.1859      0.2227     -0.02426         
-       2023 12 10  60288       0.1836      0.2222     -0.02459         
-       2023 12 11  60289       0.1812      0.2217     -0.02480         
-       2023 12 12  60290       0.1789      0.2212     -0.02481         
-       2023 12 13  60291       0.1765      0.2208     -0.02463         
-       2023 12 14  60292       0.1741      0.2204     -0.02433         
-       2023 12 15  60293       0.1718      0.2201     -0.02403         
-       2023 12 16  60294       0.1694      0.2198     -0.02387         
-       2023 12 17  60295       0.1670      0.2195     -0.02395         
-       2023 12 18  60296       0.1646      0.2192     -0.02431         
-       2023 12 19  60297       0.1623      0.2190     -0.02491         
-       2023 12 20  60298       0.1599      0.2189     -0.02565         
-       2023 12 21  60299       0.1575      0.2188     -0.02641         
-       2023 12 22  60300       0.1551      0.2187     -0.02705         
-       2023 12 23  60301       0.1528      0.2186     -0.02746         
-       2023 12 24  60302       0.1504      0.2186     -0.02761         
-       2023 12 25  60303       0.1480      0.2186     -0.02750         
-       2023 12 26  60304       0.1457      0.2187     -0.02718         
-       2023 12 27  60305       0.1433      0.2188     -0.02674         
-       2023 12 28  60306       0.1410      0.2189     -0.02627         
-       2023 12 29  60307       0.1386      0.2191     -0.02585         
-       2023 12 30  60308       0.1363      0.2193     -0.02556         
-       2023 12 31  60309       0.1340      0.2196     -0.02542         
-       2024  1  1  60310       0.1317      0.2199     -0.02545         
-       2024  1  2  60311       0.1294      0.2202     -0.02562         
-       2024  1  3  60312       0.1271      0.2205     -0.02589         
-       2024  1  4  60313       0.1248      0.2209     -0.02622         
-       2024  1  5  60314       0.1225      0.2213     -0.02653         
-       2024  1  6  60315       0.1202      0.2218     -0.02676         
-       2024  1  7  60316       0.1180      0.2223     -0.02684         
-       2024  1  8  60317       0.1157      0.2228     -0.02675         
-       2024  1  9  60318       0.1135      0.2234     -0.02646         
-       2024  1 10  60319       0.1113      0.2240     -0.02604         
-       2024  1 11  60320       0.1091      0.2246     -0.02559         
-       2024  1 12  60321       0.1069      0.2253     -0.02525         
-       2024  1 13  60322       0.1047      0.2260     -0.02514         
-       2024  1 14  60323       0.1026      0.2267     -0.02534         
-       2024  1 15  60324       0.1004      0.2275     -0.02584         
-       2024  1 16  60325       0.0983      0.2283     -0.02651         
-       2024  1 17  60326       0.0962      0.2291     -0.02723         
-       2024  1 18  60327       0.0941      0.2300     -0.02784         
-       2024  1 19  60328       0.0921      0.2309     -0.02824         
-       2024  1 20  60329       0.0900      0.2318     -0.02836         
-       2024  1 21  60330       0.0880      0.2328     -0.02821         
-       2024  1 22  60331       0.0860      0.2338     -0.02786         
-       2024  1 23  60332       0.0840      0.2348     -0.02737         
-       2024  1 24  60333       0.0820      0.2359     -0.02685         
-       2024  1 25  60334       0.0801      0.2369     -0.02638         
-       2024  1 26  60335       0.0782      0.2381     -0.02603         
-       2024  1 27  60336       0.0763      0.2392     -0.02584         
-       2024  1 28  60337       0.0744      0.2404     -0.02583         
-       2024  1 29  60338       0.0726      0.2416     -0.02598         
-       2024  1 30  60339       0.0707      0.2428     -0.02626         
-       2024  1 31  60340       0.0689      0.2441     -0.02661         
-       2024  2  1  60341       0.0672      0.2453     -0.02696         
-       2024  2  2  60342       0.0654      0.2467     -0.02726         
-       2024  2  3  60343       0.0637      0.2480     -0.02744         
-       2024  2  4  60344       0.0620      0.2494     -0.02746         
-       2024  2  5  60345       0.0603      0.2508     -0.02731         
-       2024  2  6  60346       0.0587      0.2522     -0.02701         
-       2024  2  7  60347       0.0571      0.2536     -0.02665         
-       2024  2  8  60348       0.0555      0.2551     -0.02636         
-       2024  2  9  60349       0.0540      0.2566     -0.02628         
-       2024  2 10  60350       0.0524      0.2581     -0.02653         
-       2024  2 11  60351       0.0509      0.2596     -0.02712         
-       2024  2 12  60352       0.0495      0.2612     -0.02800         
-       2024  2 13  60353       0.0480      0.2628     -0.02899         
-       2024  2 14  60354       0.0466      0.2644     -0.02993         
-       2024  2 15  60355       0.0452      0.2660     -0.03066         
-       2024  2 16  60356       0.0439      0.2676     -0.03110         
-       2024  2 17  60357       0.0426      0.2693     -0.03126         
-       2024  2 18  60358       0.0413      0.2710     -0.03119         
-       2024  2 19  60359       0.0401      0.2727     -0.03098         
-       2024  2 20  60360       0.0388      0.2744     -0.03072         
-       2024  2 21  60361       0.0377      0.2761     -0.03052         
-       2024  2 22  60362       0.0365      0.2779     -0.03043         
-       2024  2 23  60363       0.0354      0.2797     -0.03052         
-       2024  2 24  60364       0.0343      0.2815     -0.03080         
-       2024  2 25  60365       0.0332      0.2833     -0.03127         
-       2024  2 26  60366       0.0322      0.2851     -0.03189         
-       2024  2 27  60367       0.0312      0.2869     -0.03261         
-       2024  2 28  60368       0.0303      0.2888     -0.03335         
-       2024  2 29  60369       0.0294      0.2907     -0.03402         
-       2024  3  1  60370       0.0285      0.2925     -0.03455         
-       2024  3  2  60371       0.0276      0.2944     -0.03490         
-       2024  3  3  60372       0.0268      0.2963     -0.03503         
-       2024  3  4  60373       0.0261      0.2982     -0.03498         
-       2024  3  5  60374       0.0253      0.3002     -0.03480         
-       2024  3  6  60375       0.0246      0.3021     -0.03464         
-       2024  3  7  60376       0.0239      0.3041     -0.03463         
-       2024  3  8  60377       0.0233      0.3060     -0.03492         
-       2024  3  9  60378       0.0227      0.3080     -0.03558         
-       2024  3 10  60379       0.0221      0.3100     -0.03659         
-       2024  3 11  60380       0.0216      0.3119     -0.03782         
-       2024  3 12  60381       0.0211      0.3139     -0.03907         
-       2024  3 13  60382       0.0207      0.3159     -0.04015         
-       2024  3 14  60383       0.0203      0.3179     -0.04091         
-       2024  3 15  60384       0.0199      0.3199     -0.04132         
-       2024  3 16  60385       0.0195      0.3220     -0.04142         
-       2024  3 17  60386       0.0192      0.3240     -0.04130         
-       2024  3 18  60387       0.0189      0.3260     -0.04107         
-       2024  3 19  60388       0.0187      0.3280     -0.04084         
-       2024  3 20  60389       0.0185      0.3300     -0.04069         
-       2024  3 21  60390       0.0183      0.3321     -0.04068         
-       2024  3 22  60391       0.0182      0.3341     -0.04083         
-       2024  3 23  60392       0.0181      0.3361     -0.04113         
-       2024  3 24  60393       0.0180      0.3382     -0.04156         
-       2024  3 25  60394       0.0180      0.3402     -0.04207         
-       2024  3 26  60395       0.0180      0.3422     -0.04261         
-       2024  3 27  60396       0.0181      0.3443     -0.04312         
-       2024  3 28  60397       0.0182      0.3463     -0.04353         
-       2024  3 29  60398       0.0183      0.3483     -0.04376         
-       2024  3 30  60399       0.0185      0.3503     -0.04377         
-       2024  3 31  60400       0.0186      0.3524     -0.04359         
-       2024  4  1  60401       0.0189      0.3544     -0.04330         
-       2024  4  2  60402       0.0191      0.3564     -0.04298         
-       2024  4  3  60403       0.0194      0.3584     -0.04272         
-       2024  4  4  60404       0.0198      0.3604     -0.04258         
-       2024  4  5  60405       0.0201      0.3624     -0.04274         
-       2024  4  6  60406       0.0205      0.3644     -0.04320         
-       2024  4  7  60407       0.0210      0.3663     -0.04401         
-       2024  4  8  60408       0.0214      0.3683     -0.04499         
-       2024  4  9  60409       0.0219      0.3703     -0.04585         
-       2024  4 10  60410       0.0225      0.3722     -0.04651         
-       2024  4 11  60411       0.0231      0.3742     -0.04688         
-       2024  4 12  60412       0.0237      0.3761     -0.04702         
-       2024  4 13  60413       0.0243      0.3780     -0.04702         
-       2024  4 14  60414       0.0250      0.3799     -0.04679         
-       2024  4 15  60415       0.0257      0.3818     -0.04652         
-       2024  4 16  60416       0.0264      0.3837     -0.04631         
-       2024  4 17  60417       0.0272      0.3856     -0.04622         
-       2024  4 18  60418       0.0280      0.3875     -0.04625         
-       2024  4 19  60419       0.0288      0.3893     -0.04648         
-       2024  4 20  60420       0.0297      0.3911     -0.04690         
-       2024  4 21  60421       0.0305      0.3930     -0.04759         
-       2024  4 22  60422       0.0315      0.3948     -0.04835         
-       2024  4 23  60423       0.0324      0.3965     -0.04909         
-       2024  4 24  60424       0.0334      0.3983     -0.04971         
-       2024  4 25  60425       0.0344      0.4001     -0.05015         
-       2024  4 26  60426       0.0355      0.4018     -0.05036         
-       2024  4 27  60427       0.0365      0.4035     -0.05037         
-       2024  4 28  60428       0.0376      0.4052     -0.05016         
-       2024  4 29  60429       0.0387      0.4069     -0.04986         
-       2024  4 30  60430       0.0399      0.4086     -0.04962         
-       2024  5  1  60431       0.0411      0.4102     -0.04948         
-       2024  5  2  60432       0.0423      0.4119     -0.04968         
-       2024  5  3  60433       0.0435      0.4135     -0.05014         
-       2024  5  4  60434       0.0448      0.4151     -0.05090         
-       2024  5  5  60435       0.0461      0.4166     -0.05187         
-       2024  5  6  60436       0.0474      0.4182     -0.05294         
-       2024  5  7  60437       0.0487      0.4197     -0.05386         
-       2024  5  8  60438       0.0501      0.4212     -0.05441         
-       2024  5  9  60439       0.0514      0.4227     -0.05464         
-       2024  5 10  60440       0.0528      0.4241     -0.05452         
-       2024  5 11  60441       0.0543      0.4256     -0.05420         
-       2024  5 12  60442       0.0557      0.4270     -0.05378         
-       2024  5 13  60443       0.0572      0.4284     -0.05323         
-       2024  5 14  60444       0.0587      0.4297     -0.05267         
-       2024  5 15  60445       0.0602      0.4311     -0.05222         
-       2024  5 16  60446       0.0617      0.4324     -0.05194         
-       2024  5 17  60447       0.0633      0.4337     -0.05185         
-       2024  5 18  60448       0.0649      0.4350     -0.05178         
-       2024  5 19  60449       0.0664      0.4362     -0.05178         
-       2024  5 20  60450       0.0681      0.4374     -0.05176         
-       2024  5 21  60451       0.0697      0.4386     -0.05171         
-       2024  5 22  60452       0.0713      0.4397     -0.05147         
-       2024  5 23  60453       0.0730      0.4409     -0.05104         
-       2024  5 24  60454       0.0747      0.4420     -0.05042         
-       2024  5 25  60455       0.0764      0.4431     -0.04963         
-       2024  5 26  60456       0.0781      0.4441     -0.04870         
-       2024  5 27  60457       0.0798      0.4451     -0.04775         
-       2024  5 28  60458       0.0816      0.4461     -0.04690         
-       2024  5 29  60459       0.0833      0.4471     -0.04625         
-       2024  5 30  60460       0.0851      0.4480     -0.04590         
-       2024  5 31  60461       0.0869      0.4490     -0.04575         
-       2024  6  1  60462       0.0887      0.4498     -0.04586         
-       2024  6  2  60463       0.0905      0.4507     -0.04599         
-       2024  6  3  60464       0.0923      0.4515     -0.04606         
-       2024  6  4  60465       0.0941      0.4523     -0.04595         
-       2024  6  5  60466       0.0959      0.4531     -0.04556         
-       2024  6  6  60467       0.0978      0.4538     -0.04492         
-       2024  6  7  60468       0.0996      0.4545     -0.04411         
-       2024  6  8  60469       0.1015      0.4552     -0.04318         
-       2024  6  9  60470       0.1034      0.4558     -0.04226         
-       2024  6 10  60471       0.1053      0.4565     -0.04139         
-       2024  6 11  60472       0.1071      0.4571     -0.04066         
-       2024  6 12  60473       0.1090      0.4576     -0.04012         
-       2024  6 13  60474       0.1109      0.4581     -0.03962         
-       2024  6 14  60475       0.1128      0.4586     -0.03928         
-       2024  6 15  60476       0.1147      0.4591     -0.03901         
-       2024  6 16  60477       0.1166      0.4595     -0.03870         
-       2024  6 17  60478       0.1186      0.4599     -0.03833         
-       2024  6 18  60479       0.1205      0.4603     -0.03781         
-       2024  6 19  60480       0.1224      0.4607     -0.03712         
-       2024  6 20  60481       0.1243      0.4610     -0.03624         
-       2024  6 21  60482       0.1262      0.4612     -0.03515         
-       2024  6 22  60483       0.1281      0.4615     -0.03398         
-       2024  6 23  60484       0.1301      0.4617     -0.03289         
-       2024  6 24  60485       0.1320      0.4619     -0.03187         
-       2024  6 25  60486       0.1339      0.4621     -0.03106         
-       2024  6 26  60487       0.1358      0.4622     -0.03056         
-       2024  6 27  60488       0.1377      0.4623     -0.03032         
-       2024  6 28  60489       0.1396      0.4624     -0.03034         
-       2024  6 29  60490       0.1415      0.4624     -0.03040         
-       2024  6 30  60491       0.1435      0.4624     -0.03029         
-       2024  7  1  60492       0.1454      0.4624     -0.02990         
-       2024  7  2  60493       0.1472      0.4623     -0.02921         
-       2024  7  3  60494       0.1491      0.4623     -0.02822         
-       2024  7  4  60495       0.1510      0.4621     -0.02707         
-       2024  7  5  60496       0.1529      0.4620     -0.02575         
-       2024  7  6  60497       0.1548      0.4618     -0.02439         
-       2024  7  7  60498       0.1566      0.4616     -0.02316         
-       2024  7  8  60499       0.1585      0.4614     -0.02208         
-       2024  7  9  60500       0.1603      0.4611     -0.02117         
-       2024  7 10  60501       0.1621      0.4608     -0.02048         
-       2024  7 11  60502       0.1640      0.4605     -0.01989         
-       2024  7 12  60503       0.1658      0.4602     -0.01936         
-       2024  7 13  60504       0.1676      0.4598     -0.01887         
-       2024  7 14  60505       0.1694      0.4594     -0.01836         
-       2024  7 15  60506       0.1712      0.4590     -0.01776         
-       2024  7 16  60507       0.1729      0.4585     -0.01700         
-       2024  7 17  60508       0.1747      0.4580     -0.01595         
-       2024  7 18  60509       0.1764      0.4575     -0.01467         
-       2024  7 19  60510       0.1781      0.4570     -0.01318         
-       2024  7 20  60511       0.1799      0.4564     -0.01157         
-       2024  7 21  60512       0.1816      0.4558     -0.01005         
-       2024  7 22  60513       0.1832      0.4552     -0.00873         
-       2024  7 23  60514       0.1849      0.4545     -0.00772         
-       2024  7 24  60515       0.1866      0.4538     -0.00699         
-       2024  7 25  60516       0.1882      0.4531     -0.00649         
-       2024  7 26  60517       0.1898      0.4524     -0.00604         
-       2024  7 27  60518       0.1914      0.4517     -0.00552         
-       2024  7 28  60519       0.1930      0.4509     -0.00482         
-       2024  7 29  60520       0.1946      0.4501     -0.00389         
-       2024  7 30  60521       0.1961      0.4493     -0.00272         
-       2024  7 31  60522       0.1976      0.4484     -0.00129         
-       2024  8  1  60523       0.1991      0.4475      0.00036         
-       2024  8  2  60524       0.2006      0.4466      0.00202         
-       2024  8  3  60525       0.2021      0.4457      0.00364         
-       2024  8  4  60526       0.2035      0.4448      0.00516         
-       2024  8  5  60527       0.2049      0.4438      0.00648         
-       2024  8  6  60528       0.2063      0.4428      0.00771         
-       2024  8  7  60529       0.2077      0.4418      0.00882         
-       2024  8  8  60530       0.2091      0.4408      0.00975         
-       2024  8  9  60531       0.2104      0.4397      0.01064         
-       2024  8 10  60532       0.2117      0.4387      0.01149         
-       2024  8 11  60533       0.2130      0.4376      0.01240         
-       2024  8 12  60534       0.2143      0.4364      0.01347         
-       2024  8 13  60535       0.2155      0.4353      0.01460         
-       2024  8 14  60536       0.2167      0.4342      0.01582         
-       2024  8 15  60537       0.2179      0.4330      0.01717         
-       2024  8 16  60538       0.2191      0.4318      0.01850         
-       2024  8 17  60539       0.2202      0.4306      0.01984         
-       2024  8 18  60540       0.2214      0.4294      0.02092         
-       2024  8 19  60541       0.2224      0.4281      0.02171         
-       2024  8 20  60542       0.2235      0.4269      0.02210         
-       2024  8 21  60543       0.2246      0.4256      0.02217         
-       2024  8 22  60544       0.2256      0.4243      0.02201         
-       2024  8 23  60545       0.2266      0.4230      0.02180         
+       2024  4 12  60412      -0.0071      0.3646     -0.01792         
+       2024  4 13  60413      -0.0062      0.3667     -0.01771         
+       2024  4 14  60414      -0.0052      0.3690     -0.01736         
+       2024  4 15  60415      -0.0043      0.3712     -0.01697         
+       2024  4 16  60416      -0.0033      0.3735     -0.01661         
+       2024  4 17  60417      -0.0024      0.3759     -0.01631         
+       2024  4 18  60418      -0.0015      0.3782     -0.01616         
+       2024  4 19  60419      -0.0006      0.3806     -0.01615         
+       2024  4 20  60420       0.0004      0.3828     -0.01629         
+       2024  4 21  60421       0.0014      0.3851     -0.01655         
+       2024  4 22  60422       0.0024      0.3873     -0.01687         
+       2024  4 23  60423       0.0035      0.3895     -0.01718         
+       2024  4 24  60424       0.0046      0.3917     -0.01738         
+       2024  4 25  60425       0.0057      0.3939     -0.01740         
+       2024  4 26  60426       0.0069      0.3960     -0.01722         
+       2024  4 27  60427       0.0082      0.3982     -0.01681         
+       2024  4 28  60428       0.0095      0.4003     -0.01626         
+       2024  4 29  60429       0.0108      0.4024     -0.01567         
+       2024  4 30  60430       0.0121      0.4045     -0.01516         
+       2024  5  1  60431       0.0135      0.4065     -0.01484         
+       2024  5  2  60432       0.0149      0.4086     -0.01480         
+       2024  5  3  60433       0.0163      0.4106     -0.01510         
+       2024  5  4  60434       0.0178      0.4126     -0.01570         
+       2024  5  5  60435       0.0193      0.4146     -0.01652         
+       2024  5  6  60436       0.0208      0.4165     -0.01736         
+       2024  5  7  60437       0.0224      0.4185     -0.01806         
+       2024  5  8  60438       0.0240      0.4204     -0.01847         
+       2024  5  9  60439       0.0256      0.4222     -0.01856         
+       2024  5 10  60440       0.0273      0.4241     -0.01833         
+       2024  5 11  60441       0.0289      0.4259     -0.01789         
+       2024  5 12  60442       0.0307      0.4277     -0.01734         
+       2024  5 13  60443       0.0324      0.4295     -0.01681         
+       2024  5 14  60444       0.0342      0.4312     -0.01636         
+       2024  5 15  60445       0.0360      0.4329     -0.01605         
+       2024  5 16  60446       0.0378      0.4346     -0.01587         
+       2024  5 17  60447       0.0396      0.4362     -0.01581         
+       2024  5 18  60448       0.0415      0.4379     -0.01586         
+       2024  5 19  60449       0.0434      0.4394     -0.01595         
+       2024  5 20  60450       0.0453      0.4410     -0.01604         
+       2024  5 21  60451       0.0473      0.4425     -0.01607         
+       2024  5 22  60452       0.0492      0.4440     -0.01595         
+       2024  5 23  60453       0.0512      0.4455     -0.01566         
+       2024  5 24  60454       0.0533      0.4469     -0.01517         
+       2024  5 25  60455       0.0553      0.4483     -0.01452         
+       2024  5 26  60456       0.0573      0.4497     -0.01377         
+       2024  5 27  60457       0.0594      0.4511     -0.01303         
+       2024  5 28  60458       0.0615      0.4524     -0.01241         
+       2024  5 29  60459       0.0636      0.4536     -0.01203         
+       2024  5 30  60460       0.0658      0.4549     -0.01193         
+       2024  5 31  60461       0.0679      0.4561     -0.01210         
+       2024  6  1  60462       0.0701      0.4573     -0.01247         
+       2024  6  2  60463       0.0723      0.4584     -0.01290         
+       2024  6  3  60464       0.0745      0.4595     -0.01323         
+       2024  6  4  60465       0.0767      0.4606     -0.01333         
+       2024  6  5  60466       0.0789      0.4616     -0.01312         
+       2024  6  6  60467       0.0812      0.4626     -0.01259         
+       2024  6  7  60468       0.0834      0.4636     -0.01182         
+       2024  6  8  60469       0.0857      0.4645     -0.01091         
+       2024  6  9  60470       0.0880      0.4654     -0.00998         
+       2024  6 10  60471       0.0903      0.4663     -0.00913         
+       2024  6 11  60472       0.0926      0.4671     -0.00842         
+       2024  6 12  60473       0.0949      0.4679     -0.00786         
+       2024  6 13  60474       0.0972      0.4686     -0.00744         
+       2024  6 14  60475       0.0995      0.4693     -0.00714         
+       2024  6 15  60476       0.1019      0.4700     -0.00690         
+       2024  6 16  60477       0.1042      0.4706     -0.00668         
+       2024  6 17  60478       0.1066      0.4712     -0.00639         
+       2024  6 18  60479       0.1089      0.4718     -0.00597         
+       2024  6 19  60480       0.1113      0.4723     -0.00538         
+       2024  6 20  60481       0.1136      0.4728     -0.00459         
+       2024  6 21  60482       0.1160      0.4733     -0.00362         
+       2024  6 22  60483       0.1184      0.4737     -0.00251         
+       2024  6 23  60484       0.1208      0.4741     -0.00138         
+       2024  6 24  60485       0.1231      0.4744     -0.00034         
+       2024  6 25  60486       0.1255      0.4747      0.00049         
+       2024  6 26  60487       0.1279      0.4750      0.00106         
+       2024  6 27  60488       0.1303      0.4753      0.00136         
+       2024  6 28  60489       0.1327      0.4754      0.00148         
+       2024  6 29  60490       0.1351      0.4756      0.00153         
+       2024  6 30  60491       0.1374      0.4757      0.00166         
+       2024  7  1  60492       0.1398      0.4758      0.00200         
+       2024  7  2  60493       0.1422      0.4759      0.00263         
+       2024  7  3  60494       0.1445      0.4759      0.00357         
+       2024  7  4  60495       0.1469      0.4759      0.00475         
+       2024  7  5  60496       0.1493      0.4758      0.00609         
+       2024  7  6  60497       0.1516      0.4757      0.00747         
+       2024  7  7  60498       0.1540      0.4756      0.00879         
+       2024  7  8  60499       0.1563      0.4754      0.00998         
+       2024  7  9  60500       0.1586      0.4752      0.01101         
+       2024  7 10  60501       0.1610      0.4749      0.01188         
+       2024  7 11  60502       0.1633      0.4747      0.01261         
+       2024  7 12  60503       0.1656      0.4744      0.01327         
+       2024  7 13  60504       0.1679      0.4740      0.01391         
+       2024  7 14  60505       0.1701      0.4736      0.01460         
+       2024  7 15  60506       0.1724      0.4732      0.01540         
+       2024  7 16  60507       0.1747      0.4727      0.01635         
+       2024  7 17  60508       0.1769      0.4723      0.01748         
+       2024  7 18  60509       0.1792      0.4717      0.01879         
+       2024  7 19  60510       0.1814      0.4712      0.02023         
+       2024  7 20  60511       0.1836      0.4706      0.02172         
+       2024  7 21  60512       0.1858      0.4700      0.02314         
+       2024  7 22  60513       0.1879      0.4693      0.02435         
+       2024  7 23  60514       0.1901      0.4686      0.02526         
+       2024  7 24  60515       0.1922      0.4679      0.02586         
+       2024  7 25  60516       0.1944      0.4671      0.02622         
+       2024  7 26  60517       0.1965      0.4663      0.02646         
+       2024  7 27  60518       0.1985      0.4655      0.02674         
+       2024  7 28  60519       0.2006      0.4646      0.02722         
+       2024  7 29  60520       0.2027      0.4638      0.02795         
+       2024  7 30  60521       0.2047      0.4628      0.02896         
+       2024  7 31  60522       0.2067      0.4619      0.03022         
+       2024  8  1  60523       0.2087      0.4609      0.03163         
+       2024  8  2  60524       0.2107      0.4599      0.03308         
+       2024  8  3  60525       0.2126      0.4589      0.03448         
+       2024  8  4  60526       0.2145      0.4578      0.03575         
+       2024  8  5  60527       0.2164      0.4567      0.03685         
+       2024  8  6  60528       0.2183      0.4556      0.03775         
+       2024  8  7  60529       0.2201      0.4544      0.03850         
+       2024  8  8  60530       0.2220      0.4532      0.03913         
+       2024  8  9  60531       0.2238      0.4520      0.03970         
+       2024  8 10  60532       0.2255      0.4508      0.04028         
+       2024  8 11  60533       0.2273      0.4495      0.04095         
+       2024  8 12  60534       0.2290      0.4482      0.04173         
+       2024  8 13  60535       0.2307      0.4469      0.04267         
+       2024  8 14  60536       0.2324      0.4456      0.04376         
+       2024  8 15  60537       0.2340      0.4442      0.04499         
+       2024  8 16  60538       0.2356      0.4428      0.04628         
+       2024  8 17  60539       0.2372      0.4414      0.04753         
+       2024  8 18  60540       0.2388      0.4400      0.04860         
+       2024  8 19  60541       0.2403      0.4385      0.04937         
+       2024  8 20  60542       0.2418      0.4370      0.04979         
+       2024  8 21  60543       0.2433      0.4355      0.04987         
+       2024  8 22  60544       0.2447      0.4340      0.04975         
+       2024  8 23  60545       0.2461      0.4324      0.04960         
+       2024  8 24  60546       0.2475      0.4308      0.04960         
+       2024  8 25  60547       0.2489      0.4293      0.04987         
+       2024  8 26  60548       0.2502      0.4276      0.05045         
+       2024  8 27  60549       0.2515      0.4260      0.05130         
+       2024  8 28  60550       0.2527      0.4244      0.05233         
+       2024  8 29  60551       0.2539      0.4227      0.05342         
+       2024  8 30  60552       0.2551      0.4210      0.05446         
+       2024  8 31  60553       0.2563      0.4193      0.05538         
+       2024  9  1  60554       0.2574      0.4176      0.05612         
+       2024  9  2  60555       0.2585      0.4158      0.05667         
+       2024  9  3  60556       0.2595      0.4141      0.05704         
+       2024  9  4  60557       0.2606      0.4123      0.05727         
+       2024  9  5  60558       0.2616      0.4105      0.05742         
+       2024  9  6  60559       0.2625      0.4087      0.05756         
+       2024  9  7  60560       0.2634      0.4069      0.05776         
+       2024  9  8  60561       0.2643      0.4051      0.05807         
+       2024  9  9  60562       0.2652      0.4033      0.05852         
+       2024  9 10  60563       0.2660      0.4014      0.05913         
+       2024  9 11  60564       0.2668      0.3996      0.05987         
+       2024  9 12  60565       0.2675      0.3977      0.06070         
+       2024  9 13  60566       0.2682      0.3958      0.06152         
+       2024  9 14  60567       0.2689      0.3939      0.06221         
+       2024  9 15  60568       0.2696      0.3920      0.06266         
+       2024  9 16  60569       0.2702      0.3901      0.06275         
+       2024  9 17  60570       0.2707      0.3882      0.06246         
+       2024  9 18  60571       0.2713      0.3863      0.06188         
+       2024  9 19  60572       0.2718      0.3844      0.06115         
+       2024  9 20  60573       0.2723      0.3824      0.06049         
+       2024  9 21  60574       0.2727      0.3805      0.06007         
+       2024  9 22  60575       0.2731      0.3785      0.05997         
+       2024  9 23  60576       0.2734      0.3766      0.06019         
+       2024  9 24  60577       0.2738      0.3746      0.06063         
+       2024  9 25  60578       0.2741      0.3727      0.06119         
+       2024  9 26  60579       0.2743      0.3707      0.06172         
+       2024  9 27  60580       0.2745      0.3687      0.06215         
+       2024  9 28  60581       0.2747      0.3668      0.06242         
+       2024  9 29  60582       0.2749      0.3648      0.06250         
+       2024  9 30  60583       0.2750      0.3628      0.06240         
+       2024 10  1  60584       0.2750      0.3609      0.06215         
+       2024 10  2  60585       0.2751      0.3589      0.06181         
+       2024 10  3  60586       0.2751      0.3569      0.06144         
+       2024 10  4  60587       0.2750      0.3550      0.06111         
+       2024 10  5  60588       0.2750      0.3530      0.06089         
+       2024 10  6  60589       0.2749      0.3510      0.06082         
+       2024 10  7  60590       0.2747      0.3491      0.06092         
+       2024 10  8  60591       0.2746      0.3471      0.06116         
+       2024 10  9  60592       0.2744      0.3452      0.06152         
+       2024 10 10  60593       0.2741      0.3432      0.06191         
+       2024 10 11  60594       0.2739      0.3413      0.06224         
+       2024 10 12  60595       0.2736      0.3393      0.06239         
+       2024 10 13  60596       0.2732      0.3374      0.06226         
+       2024 10 14  60597       0.2728      0.3355      0.06179         
+       2024 10 15  60598       0.2724      0.3336      0.06101         
+       2024 10 16  60599       0.2720      0.3317      0.06002         
+       2024 10 17  60600       0.2715      0.3298      0.05902         
+       2024 10 18  60601       0.2710      0.3279      0.05821         
+       2024 10 19  60602       0.2705      0.3260      0.05772         
+       2024 10 20  60603       0.2699      0.3241      0.05761         
+       2024 10 21  60604       0.2693      0.3223      0.05781         
+       2024 10 22  60605       0.2686      0.3204      0.05820         
+       2024 10 23  60606       0.2680      0.3186      0.05863         
+       2024 10 24  60607       0.2673      0.3168      0.05899         
+       2024 10 25  60608       0.2665      0.3149      0.05921         
+       2024 10 26  60609       0.2658      0.3131      0.05925         
+       2024 10 27  60610       0.2650      0.3114      0.05913         
+       2024 10 28  60611       0.2642      0.3096      0.05887         
+       2024 10 29  60612       0.2633      0.3078      0.05851         
+       2024 10 30  60613       0.2624      0.3061      0.05813         
+       2024 10 31  60614       0.2615      0.3044      0.05779         
+       2024 11  1  60615       0.2606      0.3027      0.05755         
+       2024 11  2  60616       0.2596      0.3010      0.05748         
+       2024 11  3  60617       0.2586      0.2993      0.05759         
+       2024 11  4  60618       0.2576      0.2976      0.05788         
+       2024 11  5  60619       0.2566      0.2960      0.05830         
+       2024 11  6  60620       0.2555      0.2943      0.05878         
+       2024 11  7  60621       0.2544      0.2927      0.05923         
+       2024 11  8  60622       0.2532      0.2911      0.05956         
+       2024 11  9  60623       0.2521      0.2896      0.05966         
+       2024 11 10  60624       0.2509      0.2880      0.05950         
+       2024 11 11  60625       0.2497      0.2865      0.05907         
+       2024 11 12  60626       0.2485      0.2850      0.05841         
+       2024 11 13  60627       0.2472      0.2835      0.05764         
+       2024 11 14  60628       0.2459      0.2820      0.05691         
+       2024 11 15  60629       0.2446      0.2806      0.05639         
+       2024 11 16  60630       0.2433      0.2792      0.05618         
+       2024 11 17  60631       0.2420      0.2778      0.05630         
+       2024 11 18  60632       0.2406      0.2764      0.05670         
+       2024 11 19  60633       0.2392      0.2750      0.05725         
+       2024 11 20  60634       0.2378      0.2737      0.05774         
+       2024 11 21  60635       0.2364      0.2724      0.05807         
+       2024 11 22  60636       0.2349      0.2711      0.05824         
+       2024 11 23  60637       0.2334      0.2698      0.05824         
+       2024 11 24  60638       0.2320      0.2686      0.05801         
+       2024 11 25  60639       0.2305      0.2674      0.05778         
+       2024 11 26  60640       0.2289      0.2662      0.05742         
+       2024 11 27  60641       0.2274      0.2650      0.05720         
+       2024 11 28  60642       0.2258      0.2639      0.05698         
+       2024 11 29  60643       0.2242      0.2628      0.05691         
+       2024 11 30  60644       0.2227      0.2617      0.05701         
+       2024 12  1  60645       0.2210      0.2606      0.05732         
+       2024 12  2  60646       0.2194      0.2596      0.05786         
+       2024 12  3  60647       0.2178      0.2586      0.05841         
+       2024 12  4  60648       0.2161      0.2576      0.05889         
+       2024 12  5  60649       0.2145      0.2566      0.05924         
+       2024 12  6  60650       0.2128      0.2557      0.05932         
+       2024 12  7  60651       0.2111      0.2548      0.05919         
+       2024 12  8  60652       0.2094      0.2539      0.05869         
+       2024 12  9  60653       0.2077      0.2531      0.05803         
+       2024 12 10  60654       0.2060      0.2523      0.05729         
+       2024 12 11  60655       0.2042      0.2515      0.05653         
+       2024 12 12  60656       0.2025      0.2507      0.05598         
+       2024 12 13  60657       0.2008      0.2500      0.05575         
+       2024 12 14  60658       0.1990      0.2493      0.05586         
+       2024 12 15  60659       0.1972      0.2486      0.05620         
+       2024 12 16  60660       0.1955      0.2480      0.05671         
+       2024 12 17  60661       0.1937      0.2473      0.05725         
+       2024 12 18  60662       0.1919      0.2468      0.05769         
+       2024 12 19  60663       0.1901      0.2462      0.05785         
+       2024 12 20  60664       0.1883      0.2457      0.05777         
+       2024 12 21  60665       0.1865      0.2452      0.05755         
+       2024 12 22  60666       0.1847      0.2447      0.05718         
+       2024 12 23  60667       0.1829      0.2442      0.05678         
+       2024 12 24  60668       0.1811      0.2438      0.05643         
+       2024 12 25  60669       0.1792      0.2434      0.05610         
+       2024 12 26  60670       0.1774      0.2431      0.05592         
+       2024 12 27  60671       0.1756      0.2428      0.05591         
+       2024 12 28  60672       0.1738      0.2425      0.05605         
+       2024 12 29  60673       0.1720      0.2422      0.05628         
+       2024 12 30  60674       0.1701      0.2420      0.05660         
+       2024 12 31  60675       0.1683      0.2418      0.05702         
+       2025  1  1  60676       0.1665      0.2416      0.05735         
+       2025  1  2  60677       0.1647      0.2414      0.05738         
+       2025  1  3  60678       0.1629      0.2413      0.05715         
+       2025  1  4  60679       0.1611      0.2412      0.05661         
+       2025  1  5  60680       0.1593      0.2412      0.05581         
+       2025  1  6  60681       0.1575      0.2411      0.05484         
+       2025  1  7  60682       0.1557      0.2411      0.05381         
+       2025  1  8  60683       0.1539      0.2411      0.05296         
+       2025  1  9  60684       0.1521      0.2412      0.05238         
+       2025  1 10  60685       0.1503      0.2413      0.05208         
+       2025  1 11  60686       0.1485      0.2414      0.05207         
+       2025  1 12  60687       0.1468      0.2415      0.05218         
+       2025  1 13  60688       0.1450      0.2417      0.05235         
+       2025  1 14  60689       0.1433      0.2419      0.05245         
+       2025  1 15  60690       0.1415      0.2421      0.05233         
+       2025  1 16  60691       0.1398      0.2424      0.05201         
+       2025  1 17  60692       0.1381      0.2426      0.05151         
+       2025  1 18  60693       0.1364      0.2429      0.05086         
+       2025  1 19  60694       0.1347      0.2433      0.05024         
+       2025  1 20  60695       0.1330      0.2436      0.04967         
+       2025  1 21  60696       0.1313      0.2440      0.04919         
+       2025  1 22  60697       0.1296      0.2444      0.04893         
+       2025  1 23  60698       0.1280      0.2449      0.04882         
+       2025  1 24  60699       0.1263      0.2453      0.04892         
+       2025  1 25  60700       0.1247      0.2458      0.04932         
+       2025  1 26  60701       0.1231      0.2464      0.04970         
+       2025  1 27  60702       0.1215      0.2469      0.05021         
+       2025  1 28  60703       0.1199      0.2475      0.05065         
+       2025  1 29  60704       0.1184      0.2481      0.05100         
+       2025  1 30  60705       0.1168      0.2487      0.05100         
+       2025  1 31  60706       0.1153      0.2493      0.05064         
+       2025  2  1  60707       0.1138      0.2500      0.04996         
+       2025  2  2  60708       0.1123      0.2507      0.04911         
+       2025  2  3  60709       0.1108      0.2514      0.04811         
+       2025  2  4  60710       0.1093      0.2521      0.04718         
+       2025  2  5  60711       0.1079      0.2529      0.04650         
+       2025  2  6  60712       0.1064      0.2537      0.04602         
+       2025  2  7  60713       0.1050      0.2545      0.04580         
+       2025  2  8  60714       0.1037      0.2553      0.04583         
+       2025  2  9  60715       0.1023      0.2562      0.04596         
+       2025  2 10  60716       0.1009      0.2570      0.04612         
+       2025  2 11  60717       0.0996      0.2579      0.04615         
+       2025  2 12  60718       0.0983      0.2588      0.04601         
+       2025  2 13  60719       0.0970      0.2598      0.04558         
+       2025  2 14  60720       0.0958      0.2607      0.04499         
+       2025  2 15  60721       0.0945      0.2617      0.04422         
+       2025  2 16  60722       0.0933      0.2627      0.04339         
+       2025  2 17  60723       0.0921      0.2637      0.04255         
+       2025  2 18  60724       0.0909      0.2648      0.04178         
+       2025  2 19  60725       0.0898      0.2658      0.04119         
+       2025  2 20  60726       0.0887      0.2669      0.04086         
+       2025  2 21  60727       0.0875      0.2680      0.04078         
+       2025  2 22  60728       0.0865      0.2691      0.04079         
+       2025  2 23  60729       0.0854      0.2702      0.04090         
+       2025  2 24  60730       0.0844      0.2713      0.04102         
+       2025  2 25  60731       0.0834      0.2725      0.04099         
+       2025  2 26  60732       0.0824      0.2736      0.04071         
+       2025  2 27  60733       0.0814      0.2748      0.03998         
+       2025  2 28  60734       0.0805      0.2760      0.03896         
+       2025  3  1  60735       0.0796      0.2772      0.03763         
+       2025  3  2  60736       0.0787      0.2784      0.03622         
+       2025  3  3  60737       0.0779      0.2797      0.03484         
+       2025  3  4  60738       0.0771      0.2809      0.03371         
+       2025  3  5  60739       0.0763      0.2822      0.03297         
+       2025  3  6  60740       0.0755      0.2835      0.03249         
+       2025  3  7  60741       0.0747      0.2848      0.03226         
+       2025  3  8  60742       0.0740      0.2861      0.03215         
+       2025  3  9  60743       0.0733      0.2874      0.03207         
+       2025  3 10  60744       0.0727      0.2887      0.03183         
+       2025  3 11  60745       0.0720      0.2900      0.03143         
+       2025  3 12  60746       0.0714      0.2914      0.03081         
+       2025  3 13  60747       0.0709      0.2927      0.03000         
+       2025  3 14  60748       0.0703      0.2941      0.02909         
+       2025  3 15  60749       0.0698      0.2954      0.02809         
+       2025  3 16  60750       0.0693      0.2968      0.02704         
+       2025  3 17  60751       0.0688      0.2982      0.02601         
+       2025  3 18  60752       0.0684      0.2996      0.02509         
+       2025  3 19  60753       0.0680      0.3010      0.02433         
+       2025  3 20  60754       0.0676      0.3024      0.02367         
+       2025  3 21  60755       0.0672      0.3038      0.02319         
+       2025  3 22  60756       0.0669      0.3052      0.02274         
+       2025  3 23  60757       0.0666      0.3066      0.02228         
+       2025  3 24  60758       0.0663      0.3080      0.02167         
+       2025  3 25  60759       0.0661      0.3094      0.02083         
+       2025  3 26  60760       0.0659      0.3109      0.01970         
+       2025  3 27  60761       0.0657      0.3123      0.01830         
+       2025  3 28  60762       0.0655      0.3137      0.01665         
+       2025  3 29  60763       0.0654      0.3152      0.01479         
+       2025  3 30  60764       0.0653      0.3166      0.01299         
+       2025  3 31  60765       0.0652      0.3180      0.01146         
+       2025  4  1  60766       0.0652      0.3195      0.01025         
+       2025  4  2  60767       0.0652      0.3209      0.00953         
+       2025  4  3  60768       0.0652      0.3223      0.00904         
+       2025  4  4  60769       0.0652      0.3238      0.00889         
+       2025  4  5  60770       0.0653      0.3252      0.00879         
+       2025  4  6  60771       0.0654      0.3266      0.00866         
+       2025  4  7  60772       0.0655      0.3280      0.00845         
+       2025  4  8  60773       0.0656      0.3295      0.00797         
+       2025  4  9  60774       0.0658      0.3309      0.00731         
+       2025  4 10  60775       0.0660      0.3323      0.00657         
+       2025  4 11  60776       0.0663      0.3337      0.00579         
       These predictions are based on all announced leap seconds.               
                                                                                
       CELESTIAL POLE OFFSET SERIES:                                            
                            NEOS Celestial Pole Offset Series                   
                        MJD      dpsi    error     deps    error                
                                         (msec. of arc)                         
-                      60158  -116.22    1.03   -9.44    0.27   
-                      60159  -116.38    1.03   -9.21    0.27   
-                      60160  -116.88    1.03   -9.23    0.27   
-                      60161  -117.40    1.19   -9.42    0.12   
-                      60162  -117.79    0.88   -9.49    0.15   
-                      60163  -118.12    0.88   -9.35    0.15   
-                      60164  -118.42    0.41   -9.21    0.17   
+                      60389  -109.17    1.07   -9.25    0.23   
+                      60390  -108.89    1.07   -9.14    0.23   
+                      60391  -108.68    1.07   -8.97    0.23   
+                      60392  -108.60    0.32   -8.66    0.16   
+                      60393  -108.60    0.89   -8.31    0.04   
+                      60394  -108.58    0.89   -8.13    0.04   
+                      60395  -108.55    0.89   -8.22    0.04   
                                                             
                      IAU2000A Celestial Pole Offset Series  
                       MJD      dX     error     dY     error
                                     (msec. of arc)          
-                      60158    0.382  0.410   -0.258   0.270          
-                      60159    0.374  0.410   -0.246   0.270          
-                      60160    0.358  0.410   -0.229   0.270          
-                      60161    0.334  0.475   -0.212   0.121          
-                      60162    0.302  0.348   -0.195   0.150          
-                      60163    0.266  0.348   -0.180   0.150          
-                      60164    0.227  0.162   -0.166   0.169          
+                      60389    0.390  0.426   -0.109   0.228          
+                      60390    0.389  0.426   -0.098   0.228          
+                      60391    0.387  0.426   -0.085   0.228          
+                      60392    0.384  0.128   -0.070   0.160          
+                      60393    0.380  0.353   -0.053   0.039          
+                      60394    0.376  0.353   -0.036   0.039          
+                      60395    0.371  0.353   -0.018   0.039
```

### Comparing `timescale-0.0.2/timescale/data/tab5.2e.txt` & `timescale-0.0.3/timescale/data/tab5.2e.txt`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/data/tab5.3a.txt` & `timescale-0.0.3/timescale/data/tab5.3a.txt`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/data/tab5.3b.txt` & `timescale-0.0.3/timescale/data/tab5.3b.txt`

 * *Files identical despite different names*

### Comparing `timescale-0.0.2/timescale/eop.py` & `timescale-0.0.3/timescale/eop.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 u"""
 eop.py
-Written by Tyler Sutterley (08/2023)
+Written by Tyler Sutterley (04/2024)
 Utilities for maintaining and calculating Earth Orientation Parameters (EOP)
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
-    Forked 08/2023: forked from pyTMD EOP utility functions
+    Updated 04/2024: fixed annotations with multiple types
     Updated 04/2023: using pathlib to define and expand paths
         add wrapper function for interpolating daily EOP values
         have mean pole and finals file as attributes of EOP module
     Updated 03/2023: add secular pole model from IERS 2018 conventions
     Updated 11/2022: added encoding for writing ascii files
         use f-strings for formatting verbose or ascii output
     Updated 04/2022: updated docstrings to numpy documentation format
@@ -213,17 +213,17 @@
         return buffer
 
     # raise exception
     raise RuntimeError(f'Unable to download {FILE}')
 
 # PURPOSE: connects to servers and downloads finals files
 def update_finals_file(
-        username: str or None = None,
-        password: str or None = None,
-        timeout: int or None = 20,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = 20,
         verbose: bool = False,
         mode: oct = 0o775
     ):
     """
     Connects to servers and downloads finals EOP files
 
     Servers and Mirrors
```

### Comparing `timescale-0.0.2/timescale/time.py` & `timescale-0.0.3/timescale/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #!/usr/bin/env python
 u"""
 time.py
-Written by Tyler Sutterley (08/2023)
+Written by Tyler Sutterley (04/2024)
 Utilities for calculating time operations
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 04/2024: added quarter year approximate conversions
+        added _from_sec dictionary for named time units
+        replaced deprecated datetime.datetime.utcnow
+        updated urls and ftp links for updating the leap seconds list
+    Updated 02/2024: move the immutable parameters in timescale class
+    Updated 10/2023: add function to convert from calendar dates
+        add min, max and mean functions to Timescale class
     Forked 08/2023: forked from pyTMD time utility functions
     Updated 06/2023: improve conversion of timescale to datetime arrays
     Updated 05/2023: add timescale class for converting between time scales
         added timescale to_datetime function to create datetime arrays
         allow epoch arguments to be numpy datetime64 variables or strings
         function to convert a string with time zone information to datetime
     Updated 04/2023: using pathlib to define and expand paths
@@ -78,14 +85,18 @@
 _to_sec['mon'] = 30.0 * 86400.0
 _to_sec['month'] = 30.0 * 86400.0
 _to_sec['months'] = 30.0 * 86400.0
 _to_sec['common_year'] = 365.0 * 86400.0
 _to_sec['common_years'] = 365.0 * 86400.0
 _to_sec['year'] = 365.25 * 86400.0
 _to_sec['years'] = 365.25 * 86400.0
+_to_sec['quarter'] = 365.25 * 86400.0 / 4.0
+_to_sec['quarters'] = 365.25 * 86400.0 / 4.0
+# conversion factors from seconds to named time units
+_from_sec = {k: 1.0/v for k,v in _to_sec.items()}
 
 # standard epochs
 _mjd_epoch = (1858, 11, 17, 0, 0, 0)
 _ntp_epoch = (1900, 1, 1, 0, 0, 0)
 _unix_epoch = (1970, 1, 1, 0, 0, 0)
 _gps_epoch = (1980, 1, 6, 0, 0, 0)
 _tide_epoch = (1992, 1, 1, 0, 0, 0)
@@ -555,15 +566,15 @@
     # convert to array if only a single value was imported
     if (np.ndim(JD) == 0):
         JD = np.atleast_1d(JD)
         single_value = True
     else:
         single_value = False
 
-    # verify julian day
+    # verify Julian day
     JDO = np.floor(JD + 0.5)
     C = np.zeros_like(JD)
     # calculate C for dates before and after the switch to Gregorian
     IGREG = 2299161.0
     ind1, = np.nonzero(JDO < IGREG)
     C[ind1] = JDO[ind1] + 1524.0
     ind2, = np.nonzero(JDO >= IGREG)
@@ -619,56 +630,43 @@
 
     Attributes
     ----------
     leaps: np.ndarray
         Number of leap seconds
     MJD: np.ndarray
         Modified Julian Days
-    century: float
-        Days in a Julian century
-    day: float
-        Seconds in a day
-    turn: float
-        Fraction of a full turn
-    turndeg: float
-        Degrees in a full turn
-    tau: float
-        Radians in a full turn
-    deg2rad: float
-        Degrees to radians
-    deg2asec: float
-        Degrees to arcseconds
     """
+    # Julian century
+    century = 36525.0
+    # seconds per day
+    day = 86400.0
+    # 360 degrees
+    turn = 1.0
+    turndeg = 360.0
+    tau = 2.0*np.pi
+    # degrees to radians
+    deg2rad = np.pi/180.0
+    # degrees to arcseconds
+    deg2asec = 3600.0
+
     def __init__(self, MJD=None):
         # leap seconds
         self.leaps = None
         # modified Julian Days
         self.MJD = MJD
-        # Julian century
-        self.century = 36525.0
-        # seconds per day
-        self.day = 86400.0
-        # 360 degrees
-        self.turn = 1.0
-        self.turndeg = 360.0
-        self.tau = 2.0*np.pi
-        # degrees to radians
-        self.deg2rad = np.pi/180.0
-        # degrees to arcseconds
-        self.deg2asec = 3600.0
         # iterator
         self.__index__ = 0
 
     def from_deltatime(self,
             delta_time: np.ndarray,
             epoch: str | tuple | list | np.ndarray,
             standard: str = 'UTC'
         ):
         """
-        Converts a delta time array and into a ``timescale`` object
+        Converts a delta time array and into a ``Timescale`` object
 
         Parameters
         ----------
         delta_time: np.ndarray
             seconds since ``epoch``
         epoch: str, uuple, list or np.ndarray
             epoch for input ``delta_time``
@@ -707,34 +705,83 @@
         else:
             self.leaps = 0.0
         # convert time to days relative to Modified Julian days in UTC
         self.MJD = convert_delta_time(delta_time - self.leaps,
             epoch1=epoch, epoch2=_mjd_epoch, scale=(1.0/self.day))
         return self
 
+    def from_calendar(self,
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float = 0.0,
+        minute: np.ndarray | float = 0.0,
+        second: np.ndarray | float = 0.0,
+        ):
+        """
+        Converts calendar date arrays into a ``Timescale`` object
+
+        Parameters
+        ----------
+        year: np.ndarray
+            calendar year
+        month: np.ndarray
+            month of the year
+        day: np.ndarray
+            day of the month
+        hour: np.ndarray or float, default 0.0
+            hour of the day
+        minute: np.ndarray or float, default 0.0
+            minute of the hour
+        second: np.ndarray or float, default 0.0
+            second of the minute
+        """
+        # calculate date in Modified Julian Days (MJD) from calendar date
+        # MJD: days since November 17, 1858 (1858-11-17T00:00:00)
+        self.MJD = 367.0*year - \
+            np.floor(1.75*(year + np.floor((month + 9.0)/12.0))) - \
+            np.floor(0.75*(np.floor((year + (month - 9.0)/7.0)/100.0) + 1.0)) + \
+            np.floor(275.0*month/9.0) + day + hour/24.0 + minute/1440.0 + \
+            second/86400.0 + 1721028.5 - 2400000.5
+        return self
+
     def from_datetime(self, dtime: np.ndarray):
         """
-        Reads a ``datetime`` array and converts into a ``timescale`` object
+        Reads a ``datetime`` array and converts into a ``Timescale`` object
 
         Parameters
         ----------
         dtime: np.ndarray
             ``numpy.datetime64`` array
         """
         # convert delta time array from datetime object
         # to days relative to 1992-01-01T00:00:00
         self.MJD = convert_datetime(dtime, epoch=_mjd_epoch)/self.day
         return self
 
+    def from_list(self, temp):
+        """
+        Reads a list of ``Timescale`` objects and converts into a single
+        ``Timescale`` object
+
+        Parameters
+        ----------
+        temp: list
+            list of ``Timescale`` objects
+        """
+        # convert list of timescale objects to a single timescale object
+        self.MJD = np.array([t.MJD for t in temp])
+        return self
+
     def to_deltatime(self,
             epoch: str | tuple | list | np.ndarray,
             scale: float = 1.0
         ):
         """
-        Convert a ``timescale`` object to a delta time array
+        Convert a ``Timescale`` object to a delta time array
 
         Parameters
         ----------
         epoch: str, tuple, list, or np.ndarray
             epoch for output ``delta_time``
         scale: float, default 1.0
             scaling factor for converting time to output units
@@ -753,28 +800,41 @@
         # calculate the difference in epochs in days
         delta_time_epochs = (epoch - epoch1) / np.timedelta64(1, 'D')
         # return the date in time (default days) since epoch
         return scale*np.array(self.MJD - delta_time_epochs, dtype=np.float64)
 
     def to_datetime(self):
         """
-        Convert a ``timescale`` object to a ``datetime`` array
+        Convert a ``Timescale`` object to a ``datetime`` array
 
         Returns
         -------
         dtime: np.ndarray
             ``numpy.datetime64`` array
         """
         # convert Modified Julian Day epoch to datetime variable
         epoch = np.datetime64(datetime.datetime(*_mjd_epoch))
         # use nanoseconds to keep as much precision as possible
         delta_time = np.atleast_1d(self.MJD*self.day*1e9).astype(np.int64)
         # return the datetime array
         return np.array(epoch + delta_time.astype('timedelta64[ns]'))
 
+    def to_string(self, unit: str = 's', **kwargs):
+        """
+        Convert a ``Timescale`` object to a formatted string array
+
+        Parameters
+        ----------
+        unit: str, default 's'
+            datetime unit for output string array
+        **kwargs: dict
+            keyword arguments for datetime formatting
+        """
+        return np.datetime_as_string(self.to_datetime(), unit=unit, **kwargs)
+
     # PURPOSE: calculate the sum of a polynomial function of time
     def polynomial_sum(self, coefficients: list | np.ndarray, t: np.ndarray):
         """
         Calculates the sum of a polynomial function of time
 
         Parameters
         ----------
@@ -823,15 +883,15 @@
     def gps_week(self):
         """GPS week number since 1980-01-06T00:00:00
         """
         return ((self.tt - 2444244.5)//7).astype(np.int64)
 
     @timescale.utilities.reify
     def J2000(self):
-        """Seconds since 2000-01-0  1T12:00:00
+        """Seconds since 2000-01-01T12:00:00
         """
         return (self.tt - 2451545.0)*self.day
 
     @timescale.utilities.reify
     def st(self):
         """Greenwich Mean Sidereal Time (GMST) in fractions of a day
         from the Equinox Method
@@ -878,14 +938,29 @@
     @timescale.utilities.reify
     def year(self):
         """Universal Time (UT) as calendar year
         """
         Y, M, D, h, m, s = convert_julian(self.ut1, format='tuple')
         return convert_calendar_decimal(Y, M, D, hour=h, minute=m, second=s)
 
+    def min(self):
+        """Minimum time value as a ``Timescale`` object
+        """
+        return Timescale(MJD=np.nanmin(self.MJD))
+
+    def max(self):
+        """Maximum time value as a ``Timescale`` object
+        """
+        return Timescale(MJD=np.nanmax(self.MJD))
+
+    def mean(self):
+        """Mean time value as a ``Timescale`` object
+        """
+        return Timescale(MJD=np.nanmean(self.MJD))
+
     @property
     def turnasec(self):
         """Arcseconds in a full turn
         """
         return self.turndeg*self.deg2asec
 
     @property
@@ -898,33 +973,34 @@
     def masec2rad(self):
         """Microarcseconds to radians
         """
         return self.asec2rad/1.0e6
 
     @property
     def dtype(self):
-        """Main data type of ``timescale`` object"""
+        """Main data type of ``Timescale`` object"""
         return self.MJD.dtype
 
     @property
     def shape(self):
-        """Dimensions of ``timescale`` object
+        """Dimensions of ``Timescale`` object
         """
         return np.shape(self.MJD)
 
     @property
     def ndim(self):
-        """Number of dimensions in ``timescale`` object
+        """Number of dimensions in ``Timescale`` object
         """
         return np.ndim(self.MJD)
 
     def __str__(self):
-        """String representation of Timescale object
+        """String representation of the ``Timescale`` object
         """
-        return f"""Timescale object with {len(self)} time values"""
+        properties = ['timescale.time.Timescale']
+        return '\n'.join(properties)
 
     def __len__(self):
         """Number of time values
         """
         return len(np.atleast_1d(self.MJD))
 
     def __iter__(self):
@@ -932,15 +1008,15 @@
         """
         self.__index__ = 0
         return self
 
     def __next__(self):
         """Get the next time step
         """
-        temp = timescale()
+        temp = Timescale()
         try:
             temp.MJD = np.atleast_1d(self.MJD)[self.__index__].copy()
         except IndexError as exc:
             raise StopIteration from exc
         # add to index
         self.__index__ += 1
         return temp
@@ -971,15 +1047,15 @@
     ----------
     .. [1] J. Meeus, *Astronomical Algorithms*, 2nd edition, 477 pp., (1998).
     """
     # read delta time file
     delta_file = pathlib.Path(delta_file).expanduser().absolute()
     dinput = np.loadtxt(delta_file)
     # calculate Julian days and then convert to days since 1992-01-01T00:00:00
-    days = timescale.time.convert_calendar_dates(
+    days = convert_calendar_dates(
         dinput[:,0], dinput[:,1], dinput[:,2],
         epoch=_tide_epoch)
     # use scipy interpolating splines to interpolate delta times
     spl = scipy.interpolate.UnivariateSpline(days, dinput[:,3], k=1, s=0, ext=0)
     # return the delta time for the input date converted to days
     return spl(idays)/86400.0
 
@@ -1033,25 +1109,25 @@
     leap_secs = timescale.utilities.get_data_path(['data','leap-seconds.list'])
     # find line with file expiration as delta time
     with leap_secs.open(mode='r', encoding='utf8') as fid:
         secs, = [re.findall(r'\d+',i).pop() for i in fid.read().splitlines()
             if re.match(r'^(?=#@)',i)]
     # check that leap seconds file is still valid
     expiry = datetime.datetime(*_ntp_epoch) + datetime.timedelta(seconds=int(secs))
-    today = datetime.datetime.utcnow()
+    today = datetime.datetime.now(datetime.timezone.utc).replace(tzinfo=None)
     update_leap_seconds() if (expiry < today) else None
     # get leap seconds
     leap_UTC,TAI_UTC = np.loadtxt(leap_secs).T
     # TAI time is ahead of GPS by 19 seconds
     TAI_GPS = 19.0
     # convert leap second epochs from NTP to GPS
     # convert from time of 2nd leap second to time of 1st leap second
     leap_GPS = convert_delta_time(leap_UTC + TAI_UTC - TAI_GPS - 1,
         epoch1=_ntp_epoch, epoch2=_gps_epoch)
-    # return the GPS times of leap second occurance
+    # return the GPS times of leap second occurrence
     if truncate:
         return leap_GPS[leap_GPS >= 0].astype(np.float64)
     else:
         return leap_GPS.astype(np.float64)
 
 # PURPOSE: connects to servers and downloads leap second files
 def update_leap_seconds(
@@ -1062,16 +1138,17 @@
     """
     Connects to servers to download leap-seconds.list files from NIST servers
 
     - https://www.nist.gov/pml/time-and-frequency-division/leap-seconds-faqs
 
     Servers and Mirrors
 
-    - ftp://ftp.nist.gov/pub/time/leap-seconds.list
-    - https://www.ietf.org/timezones/data/leap-seconds.list
+    - ftp://ftp.boulder.nist.gov/pub/time/leap-seconds.list
+    - https://hpiers.obspm.fr/iers/bul/bulc/ntp/leap-seconds.list
+    - https://data.iana.org/time-zones/data/leap-seconds.list
 
     Parameters
     ----------
     timeout: int or None, default 20
         timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
@@ -1079,32 +1156,47 @@
         permissions mode of output file
     """
     # local version of file
     FILE = 'leap-seconds.list'
     LOCAL = timescale.utilities.get_data_path(['data',FILE])
     HASH = timescale.utilities.get_hash(LOCAL)
 
-    # try downloading from NIST ftp servers
-    HOST = ['ftp.nist.gov','pub','time',FILE]
+    # try downloading from NIST Boulder ftp servers
+    HOST = ['ftp.boulder.nist.gov','pub','time',FILE]
     try:
         timescale.utilities.check_ftp_connection(HOST[0])
         timescale.utilities.from_ftp(HOST,
             timeout=timeout,
             local=LOCAL,
             hash=HASH,
             verbose=verbose,
             mode=mode)
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
-
-    # try downloading from Internet Engineering Task Force (IETF) mirror
-    REMOTE = ['https://www.ietf.org','timezones','data',FILE]
+    
+    # try downloading from Paris Observatory IERS Centers
+    REMOTE = ['https://hpiers.obspm.fr','iers','bul','bulc','ntp',FILE]
+    try:
+        timescale.utilities.from_http(REMOTE,
+            timeout=timeout,
+            local=LOCAL,
+            hash=HASH,
+            verbose=verbose,
+            mode=mode)
+    except Exception as exc:
+        logging.debug(traceback.format_exc())
+        pass
+    else:
+        return
+    
+    # try downloading from Internet Assigned Numbers Authority (IANA)
+    REMOTE = ['https://data.iana.org','time-zones','data',FILE]
     try:
         timescale.utilities.from_http(REMOTE,
             timeout=timeout,
             local=LOCAL,
             hash=HASH,
             verbose=verbose,
             mode=mode)
@@ -1436,43 +1528,39 @@
     Notes
     -----
     Delta times are the difference between universal time and dynamical time
     """
     # open output daily delta time file
     daily_file = pathlib.Path(daily_file).expanduser().absolute()
     fid = daily_file.open(mode='w', encoding='utf8')
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
     # connect to http host for IERS Bulletin-A files
     HOST = 'https://datacenter.iers.org/availableVersions.php?id=6'
-    bulletin_files,_ = timescale.utilities.iers_list(HOST,
-        timeout=timeout
-    )
+    bulletin_files,_ = timescale.utilities.iers_list(HOST, timeout=timeout)
     # for each Bulletin-A file
     for f in bulletin_files:
         logging.info(f)
-        remote_buffer = timescale.utilities.from_http(f,
-            timeout=timeout
-        )
+        remote_buffer = timescale.utilities.from_http(f, timeout=timeout)
         # read Bulletin-A file from BytesIO object
-        YY, MM, DD, DELTAT = read_iers_bulletin_a(remote_buffer)
+        YY,MM,DD,DELTAT = read_iers_bulletin_a(remote_buffer)
         # print delta time for week to output file
-        for Y, M, D, T in zip(YY, MM, DD, DELTAT):
-            print(f' {Y:4.0f} {M:2.0f} {D:2.0f} {T:7.4f}', file=fid)
+        for Y,M,D,T in zip(YY,MM,DD,DELTAT):
+            print(file_format.format(Y,M,D,T), file=fid)
         # close the bytesIO object
         remote_buffer.close()
     # close the output file
     fid.close()
     # change the permissions mode
     daily_file.chmod(mode)
 
 # PURPOSE: connects to CDDIS Earthdata https server and finds Bulletin-A files
 def cddis_delta_time(
         daily_file: str | pathlib.Path,
         username: str | None = None,
         password: str | None = None,
-        timeout: int | None = 120,
         verbose: bool = False,
         mode: oct = 0o775
     ):
     """
     Connects to the CDDIS Earthdata server to download Bulletin-A files
 
     Reads the IERS Bulletin-A files and calculates the daily delta times
@@ -1485,16 +1573,14 @@
     ----------
     daily_file: str
         output daily delta time file from merged Bulletin-A files
     username: str or NoneType, default None
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
-    timeout: int, default 120
-        timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
 
     Notes
     -----
@@ -1509,49 +1595,41 @@
     # regular expression pattern for finding directories
     R1 = re.compile(r'volume_(.*?)$',re.VERBOSE)
     # regular expression pattern for finding files
     R2 = re.compile(r'iers_bulletina\.(.*?)_(\d+)$',re.VERBOSE)
     # open output daily delta time file
     daily_file = pathlib.Path(daily_file).expanduser().absolute()
     fid = daily_file.open(mode='w', encoding='utf8')
+    file_format = ' {0:4.0f} {1:2.0f} {2:2.0f} {3:7.4f}'
     # for each subdirectory
-    subdirectory, mtimes = timescale.utilities.cddis_list(HOST,
-        build=False,
-        timeout=timeout,
-        pattern=R1
-    )
+    subdirectory, mtimes = timescale.utilities.cddis_list(
+        HOST, build=False, pattern=R1)
     # extract roman numerals from subdirectories
     roman = [R1.findall(s).pop() for s in subdirectory]
     # sort the list of Roman numerals
     subdirectory = [subdirectory[i] for i,j in sorted(enumerate(roman),
         key=lambda i: timescale.utilities.roman_to_int(i[1]))]
     # output file format
     for SUB in subdirectory:
         # find Bulletin-A files in https subdirectory
         HOST.append(SUB)
-        bulletin_files, mtimes = timescale.utilities.cddis_list(HOST,
-            build=False,
-            timeout=timeout,
-            sort=True,
-            pattern=R2
-        )
+        bulletin_files, mtimes = timescale.utilities.cddis_list(
+            HOST, build=False, sort=True, pattern=R2)
         # for each Bulletin-A file
         for f in sorted(bulletin_files):
             logging.info(f)
             # copy remote file contents to BytesIO object
             HOST.append(f)
             remote_buffer = timescale.utilities.from_cddis(HOST,
-                build=False,
-                timeout=timeout
-            )
+                build=False,timeout=20)
             # read Bulletin-A file from BytesIO object
-            YY, MM, DD, DELTAT = read_iers_bulletin_a(remote_buffer)
+            YY,MM,DD,DELTAT = read_iers_bulletin_a(remote_buffer)
             # print delta time for week to output file
-            for Y, M, D, T in zip(YY, MM, DD, DELTAT):
-                print(f' {Y:4.0f} {M:2.0f} {D:2.0f} {T:7.4f}', file=fid)
+            for Y,M,D,T in zip(YY,MM,DD,DELTAT):
+                print(file_format.format(Y,M,D,T),file=fid)
             # close the bytesIO object
             remote_buffer.close()
             # remove the file from the list
             HOST.remove(f)
         # remove the subdirectory from the list
         HOST.remove(SUB)
     # close the output file
@@ -1629,30 +1707,28 @@
         else:
             valid += 1
 
     # calculate components for delta time
     # TAI time is ahead of GPS by 19 seconds
     TAI_GPS = 19.0
     # calculate calendar dates from Modified Julian days
-    Y, M, D, h, m, s = convert_julian(MJD[:valid] + 2400000.5, format='tuple')
+    Y,M,D,h,m,s = convert_julian(MJD[:valid]+2400000.5, format='tuple')
     # calculate GPS Time (seconds since 1980-01-06T00:00:00)
     # by converting the Modified Julian days (days since 1858-11-17T00:00:00)
-    GPS_Time = convert_delta_time(MJD[:valid]*8.64e4,
-        epoch1=_mjd_epoch,
-        epoch2=_gps_epoch,
-        scale=1.0) + \
-        TAI_UTC - TAI_GPS
+    GPS_Time = convert_delta_time(MJD[:valid]*8.64e4, epoch1=_mjd_epoch,
+        epoch2=_gps_epoch, scale=1.0) + TAI_UTC - TAI_GPS
     # number of leap seconds between GPS and UTC
     # this finds the daily correction for weeks with leap seconds
     GPS_UTC = count_leap_seconds(GPS_Time)
     # calculate delta time (TT - UT1) -->
     # (TT-TAI) + (TAI-GPS) + (GPS-UTC) - (UT1-UTC)
     DELTAT = TT_TAI + TAI_GPS + GPS_UTC - UT1_UTC[:valid]
+
     # return dates and delta times
-    return (Y, M, D, DELTAT)
+    return (Y,M,D,DELTAT)
 
 # PURPOSE: connects to servers and downloads latest Bulletin-A file
 def update_bulletin_a(
         timeout: int | None = 20,
         verbose: bool = False,
         mode: oct = 0o775
     ):
@@ -1678,21 +1754,16 @@
     # local version of file
     LOCAL = timescale.utilities.get_data_path(['data','ser7.dat'])
     HASH = timescale.utilities.get_hash(LOCAL)
 
     # try downloading from IERS Rapid Service/Prediction Center (RS/PC)
     REMOTE = ['https://maia.usno.navy.mil','ser7','ser7.dat']
     try:
-        timescale.utilities.from_http(REMOTE,
-            timeout=timeout,
-            local=LOCAL,
-            hash=HASH,
-            verbose=verbose,
-            mode=mode
-        )
+        timescale.utilities.from_http(REMOTE, timeout=timeout, local=LOCAL,
+            hash=HASH, verbose=verbose, mode=mode)
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
 # PURPOSE: connects to servers and downloads delta time files
@@ -1744,16 +1815,15 @@
     HOST = ['http://maia.usno.navy.mil','ser7',FILE]
     try:
         timescale.utilities.from_http(HOST,
             timeout=timeout,
             local=LOCAL,
             hash=HASH,
             verbose=verbose,
-            mode=mode
-        )
+            mode=mode)
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
     # try downloading from NASA Crustal Dynamics Data Information System
@@ -1766,16 +1836,15 @@
         try:
             timescale.utilities.check_ftp_connection(HOST[0])
             timescale.utilities.from_ftp(HOST,
                 timeout=timeout,
                 local=LOCAL,
                 hash=HASH,
                 verbose=verbose,
-                mode=mode
-            )
+                mode=mode)
         except Exception as exc:
             logging.debug(traceback.format_exc())
             pass
         else:
             return
 
     # try downloading from NASA Crustal Dynamics Data Information System
@@ -1785,15 +1854,14 @@
         timescale.utilities.from_cddis(HOST,
             username=username,
             password=password,
             timeout=timeout,
             local=LOCAL,
             hash=HASH,
             verbose=verbose,
-            mode=mode
-        )
+            mode=mode)
     except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
```

### Comparing `timescale-0.0.2/timescale/utilities.py` & `timescale-0.0.3/timescale/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python
 u"""
 utilities.py
-Written by Tyler Sutterley (08/2023)
+Written by Tyler Sutterley (11/2023)
 Download and management utilities for syncing time and auxiliary files
 
 PYTHON DEPENDENCIES:
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 UPDATE HISTORY:
+    Updated 11/2023: updated ssl context to fix deprecation error
     Forked 08/2023: forked from pyTMD file, http and ftp utility functions
     Updated 06/2023: add functions to retrieve and revoke Earthdata tokens
     Updated 05/2023: add reify decorator for evaluation of properties
         make urs a keyword argument in CCDIS list and download functions
         add case for JPL kernel file download where local path is defined
     Updated 04/2023: using pathlib to define and expand paths
         added function to download ephemeride files from JPL SSD server
@@ -601,27 +602,57 @@
             os.utime(local, (local.stat().st_atime, remote_mtime))
         # close the ftp connection
         ftp.close()
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
+def _create_default_ssl_context() -> ssl.SSLContext:
+    """Creates the default SSL context
+    """
+    context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+    _set_ssl_context_options(context)
+    context.options |= ssl.OP_NO_COMPRESSION
+    return context
+
+def _create_ssl_context_no_verify() -> ssl.SSLContext:
+    """Creates an SSL context for unverified connections
+    """
+    context = _create_default_ssl_context()
+    context.check_hostname = False
+    context.verify_mode = ssl.CERT_NONE
+    return context
+
+def _set_ssl_context_options(context: ssl.SSLContext) -> None:
+    """Sets the default options for the SSL context
+    """
+    if sys.version_info >= (3, 10) or ssl.OPENSSL_VERSION_INFO >= (1, 1, 0, 7):
+        context.minimum_version = ssl.TLSVersion.TLSv1_2
+    else:
+        context.options |= ssl.OP_NO_SSLv2
+        context.options |= ssl.OP_NO_SSLv3
+        context.options |= ssl.OP_NO_TLSv1
+        context.options |= ssl.OP_NO_TLSv1_1
+
 # default ssl context
-_default_ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+_default_ssl_context = _create_ssl_context_no_verify()
 
 # PURPOSE: check internet connection
-def check_connection(HOST: str, context=_default_ssl_context):
+def check_connection(
+        HOST: str,
+        context: ssl.SSLContext = _default_ssl_context,
+    ):
     """
     Check internet connection with http host
 
     Parameters
     ----------
     HOST: str
         remote http host
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     """
     # attempt to connect to http host
     try:
         urllib2.urlopen(HOST, timeout=20, context=context)
     except urllib2.HTTPError as exc:
         logging.debug(exc.code)
@@ -632,30 +663,30 @@
     else:
         return True
 
 # PURPOSE: list a directory on an Apache http Server
 def http_list(
         HOST: str | list,
         timeout: int | None = None,
-        context = _default_ssl_context,
+        context: ssl.SSLContext = _default_ssl_context,
         parser = lxml.etree.HTMLParser(),
         format: str = '%Y-%m-%d %H:%M',
         pattern: str = '',
         sort: bool = False
     ):
     """
     List a directory on an Apache http Server
 
     Parameters
     ----------
     HOST: str or list
         remote http host path
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     parser: obj, default lxml.etree.HTMLParser()
         HTML parser for ``lxml``
     format: str, default '%Y-%m-%d %H:%M'
         format for input time string
     pattern: str, default ''
         regular expression pattern for reducing list
@@ -706,15 +737,15 @@
         # return the list of column names and last modified times
         return (colnames, collastmod)
 
 # PURPOSE: download a file from a http host
 def from_http(
         HOST: str | list,
         timeout: int | None = None,
-        context = _default_ssl_context,
+        context: ssl.SSLContext = _default_ssl_context,
         local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         fid = sys.stdout,
         mode: oct = 0o775
     ):
@@ -723,15 +754,15 @@
 
     Parameters
     ----------
     HOST: str or list
         remote http host path split as list
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
@@ -841,15 +872,15 @@
     """
     attempt to build a urllib opener for NASA Earthdata
 
     Parameters
     ----------
     urs: str
         Earthdata login URS 3 host
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     password_manager: bool, default True
         Create password manager context using default realm
     get_ca_certs: bool, default True
         Get list of loaded “certification authority” certificates
     redirect: bool, default True
         Create redirect handler object
@@ -928,15 +959,15 @@
 
     Parameters
     ----------
     username: str or NoneType, default None
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     password_manager: bool, default True
         Create password manager context using default realm
     get_ca_certs: bool, default True
         Get list of loaded “certification authority” certificates
     redirect: bool, default True
         Create redirect handler object
@@ -1356,27 +1387,27 @@
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: list a directory on IERS https Server
 def iers_list(
         HOST: str | list,
         timeout: int | None = None,
-        context = _default_ssl_context,
+        context: ssl.SSLContext = _default_ssl_context,
         parser = lxml.etree.HTMLParser()
     ):
     """
     List a directory on IERS Bulletin-A https server
 
     Parameters
     ----------
     HOST: str or list
         remote http host path
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     parser: obj, default lxml.etree.HTMLParser()
         HTML parser for ``lxml``
 
     Returns
     -------
     colnames: list
@@ -1409,15 +1440,15 @@
         # sort list of column names and last modified times in reverse order
         # return the list of column names and last modified times
         return (colnames[::-1], collastmod[::-1])
 
 def from_jpl_ssd(
         kernel='de440s.bsp',
         timeout: int | None = None,
-        context = _default_ssl_context,
+        context: ssl.SSLContext = _default_ssl_context,
         local: str | pathlib.Path | None = None,
         hash: str = '',
         chunk: int = 16384,
         verbose: bool = False,
         mode: oct = 0o775
     ):
     """
@@ -1428,15 +1459,15 @@
 
     Parameters
     ----------
     kernel: str
         JPL kernel file to download
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+    context: obj, default timescale.utilities._default_ssl_context
         SSL context for ``urllib`` opener object
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
```

### Comparing `timescale-0.0.2/timescale.egg-info/PKG-INFO` & `timescale-0.0.3/timescale.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timescale
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python tools for time and astronomical calculations.
 Home-page: https://github.com/tsutterley/timescale
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: Time,leap seconds,TAI,GPS,UT1,TT
 Classifier: Development Status :: 3 - Alpha
@@ -15,24 +15,30 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: lxml
+Requires-Dist: numpy
+Requires-Dist: python-dateutil
+Requires-Dist: scipy
+Requires-Dist: setuptools_scm
 
 =========
 timescale
 =========
 
 |Language|
 |License|
 |PyPI Version|
 |Anaconda-Server|
 |Documentation Status|
+|zenodo|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/pyTMD?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/github/license/tsutterley/timescale
    :target: https://github.com/tsutterley/timescale/blob/main/LICENSE
 
@@ -41,14 +47,17 @@
 
 .. |Anaconda-Server| image:: https://img.shields.io/conda/vn/conda-forge/timescale
    :target: https://anaconda.org/conda-forge/timescale
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/timescale/badge/?version=latest
    :target: https://timescale.readthedocs.io/en/latest/?badge=latest
 
+.. |zenodo| image:: https://zenodo.org/badge/681330279.svg
+   :target: https://zenodo.org/badge/latestdoi/681330279
+
 Python tools for time and astronomical calculations
 
 Dependencies
 ############
 
 - `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
 - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
```

### Comparing `timescale-0.0.2/timescale.egg-info/SOURCES.txt` & `timescale-0.0.3/timescale.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 timescale/version.py
 timescale.egg-info/PKG-INFO
 timescale.egg-info/SOURCES.txt
 timescale.egg-info/dependency_links.txt
 timescale.egg-info/requires.txt
 timescale.egg-info/top_level.txt
 timescale/data/deltat.data
+timescale/data/finals.all
 timescale/data/historic_deltat.data
 timescale/data/iers_deltat.data
 timescale/data/leap-seconds.list
+timescale/data/mean-pole.tab
 timescale/data/merged_deltat.data
 timescale/data/ser7.dat
 timescale/data/tab5.2e.txt
 timescale/data/tab5.3a.txt
 timescale/data/tab5.3b.txt
```

