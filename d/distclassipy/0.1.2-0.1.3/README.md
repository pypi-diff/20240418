# Comparing `tmp/distclassipy-0.1.2.tar.gz` & `tmp/distclassipy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distclassipy-0.1.2.tar", last modified: Tue Mar 12 18:58:02 2024, max compression
+gzip compressed data, was "distclassipy-0.1.3.tar", last modified: Thu Apr 18 06:41:29 2024, max compression
```

## Comparing `distclassipy-0.1.2.tar` & `distclassipy-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:58:02.070539 distclassipy-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-12 18:57:54.000000 distclassipy-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    45032 2024-03-12 18:58:02.070539 distclassipy-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-12 18:57:54.000000 distclassipy-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:58:02.070539 distclassipy-0.1.2/distclassipy/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-12 18:57:54.000000 distclassipy-0.1.2/distclassipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17633 2024-03-12 18:57:54.000000 distclassipy-0.1.2/distclassipy/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    49403 2024-03-12 18:57:54.000000 distclassipy-0.1.2/distclassipy/distances.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-03-12 18:57:54.000000 distclassipy-0.1.2/distclassipy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:58:02.070539 distclassipy-0.1.2/distclassipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45032 2024-03-12 18:58:02.000000 distclassipy-0.1.2/distclassipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-12 18:58:02.000000 distclassipy-0.1.2/distclassipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 18:58:02.000000 distclassipy-0.1.2/distclassipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 18:58:02.000000 distclassipy-0.1.2/distclassipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-12 18:58:02.000000 distclassipy-0.1.2/distclassipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-12 18:57:54.000000 distclassipy-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 18:58:02.070539 distclassipy-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 18:57:54.000000 distclassipy-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 18:58:02.070539 distclassipy-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-03-12 18:57:54.000000 distclassipy-0.1.2/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-03-12 18:57:54.000000 distclassipy-0.1.2/tests/test_distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.139538 distclassipy-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 06:41:23.000000 distclassipy-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    46355 2024-04-18 06:41:29.139538 distclassipy-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-18 06:41:23.000000 distclassipy-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.135538 distclassipy-0.1.3/distclassipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 06:41:23.000000 distclassipy-0.1.3/distclassipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18143 2024-04-18 06:41:23.000000 distclassipy-0.1.3/distclassipy/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49563 2024-04-18 06:41:23.000000 distclassipy-0.1.3/distclassipy/distances.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.139538 distclassipy-0.1.3/distclassipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    46355 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 06:41:29.000000 distclassipy-0.1.3/distclassipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 06:41:23.000000 distclassipy-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:41:29.139538 distclassipy-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-18 06:41:23.000000 distclassipy-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:41:29.139538 distclassipy-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-18 06:41:23.000000 distclassipy-0.1.3/tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-18 06:41:23.000000 distclassipy-0.1.3/tests/test_distances.py
```

### Comparing `distclassipy-0.1.2/LICENSE` & `distclassipy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `distclassipy-0.1.2/PKG-INFO` & `distclassipy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distclassipy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for a distance-based classifier which can use several different distance metrics.
 Author-email: Siddharth Chaini <sidchaini@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/sidchaini/DistClassiPy
-Project-URL: Documenation, https://sidchaini.github.io/DistClassiPy/
+Project-URL: Documentation, https://sidchaini.github.io/DistClassiPy/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -708,14 +708,17 @@
 
 [![PyPI](https://img.shields.io/pypi/v/distclassipy?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/distclassipy/)
 [![Installs](https://img.shields.io/pypi/dm/distclassipy.svg?label=PyPI%20downloads)](https://pypi.org/project/distclassipy/)
 [![Codecov](https://codecov.io/gh/sidchaini/distclassipy/branch/main/graph/badge.svg)](https://codecov.io/gh/sidchaini/distclassipy)
 [![License - GPL-3](https://img.shields.io/pypi/l/distclassipy.svg)](https://github.com/sidchaini/distclassipy/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+[![arXiv](https://img.shields.io/badge/arXiv-astro--ph%2F2403.12120-red)](https://arxiv.org/abs/2403.12120) 
+[![ascl:2403.002](https://img.shields.io/badge/ascl-2403.002-blue.svg?colorB=262255)](https://ascl.net/2403.002)
+
 <!-- [![Paper](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.1038/s41586-020-2649-2) -->
 
 A python package for a distance-based classifier which can use several different distance metrics.
 
 ## Installation
 To install DistClassiPy, run the following command:
@@ -739,55 +742,55 @@
 )
 clf = dcpy.DistanceMetricClassifier(metric="canberra")
 clf.fit(X, y)
 print(clf.predict([[0, 0, 0, 0]]))
 ```
 
 ## Features
-- Multiple distance metrics support
-- Easy integration with existing data processing pipelines
-- Efficient and scalable for large datasets
+- **Distance Metric-Based Classification**: Utilizes a variety of distance metrics for classification.
+- **Customizable for Scientific Goals**: Allows fine-tuning based on scientific objectives by selecting appropriate distance metrics and features, enhancing both computational efficiency and model performance.
+- **Interpretable Results**: Offers improved interpretability of classification outcomes by directly using distance metrics and feature importance, making it ideal for scientific applications.
+- **Efficient and Scalable**: Demonstrates lower computational requirements compared to traditional methods like Random Forests, making it suitable for large datasets
+- **Open Source and Accessible**: Available as an open-source Python package on PyPI, encouraging broad application in astronomy and beyond
 
 ## Documentation
 
 For more detailed information about the package and its functionalities, please refer to the [official documentation](https://sidchaini.github.io/DistClassiPy/).
 
 ## Contributing
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to open an [issue](https://github.com/sidchaini/DistClassiPy/issues) or submit a [pull request](https://github.com/sidchaini/DistClassiPy/pulls).
 
 ## License
 DistClassiPy is released under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html). See the LICENSE file for more details.
 
 ## Citation
 
 If you use DistClassiPy in your research or project, please consider citing the paper:
-> Light Curve Classification with DistClassiPy: a new distance-based classifier (submitted to A&C)
-
+> Chaini, S., Mahabal, A., Kembhavi, A., & Bianco, F. B. (2024). Light Curve Classification with DistClassiPy: a new distance-based classifier. arXiv. https://doi.org/10.48550/arXiv.2403.12120
 
-<!--
 ### Bibtex
 
 
 ```bibtex
-@ARTICLE{Chaini2024,
-       author = {{Chaini}, S. and {Mahabal}, A. and {Kembhavi}, A. and {Bianco}, F.~B.},
-        title = "{Light Curve Classification with DistClassiPy: a new distance-based classifier}",
-      journal = {Submitted to A&C},
-    %  keywords = {},
-         year = 2024,
-      %   month = ,
-      %  volume = {},
-      %     eid = {},
-      %   pages = {},
-      %     doi = {},
-      %  adsurl = {},
-      % adsnote = {}
+@ARTICLE{chaini2024light,
+       author = {{Chaini}, Siddharth and {Mahabal}, Ashish and {Kembhavi}, Ajit and {Bianco}, Federica B.},
+       title = "{Light Curve Classification with DistClassiPy: a new distance-based classifier}",
+       journal = {arXiv e-prints},
+       keywords = {Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Solar and Stellar Astrophysics, Computer Science - Machine Learning},
+       year = 2024,
+       month = mar,
+       eid = {arXiv:2403.12120},
+       pages = {arXiv:2403.12120},
+       archivePrefix = {arXiv},
+       eprint = {2403.12120},
+       primaryClass = {astro-ph.IM},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2024arXiv240312120C},
+       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
--->
   
 
 <!-- You can also find citation information in the [CITATION.cff](https://github.com/sidchaini/DistClassiPy/CITATION.cff) file. -->
 
 
 ## Authors
 Siddharth Chaini, Ashish Mahabal, Ajit Kembhavi and Federica B. Bianco.
```

### Comparing `distclassipy-0.1.2/README.md` & `distclassipy-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 [![PyPI](https://img.shields.io/pypi/v/distclassipy?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/distclassipy/)
 [![Installs](https://img.shields.io/pypi/dm/distclassipy.svg?label=PyPI%20downloads)](https://pypi.org/project/distclassipy/)
 [![Codecov](https://codecov.io/gh/sidchaini/distclassipy/branch/main/graph/badge.svg)](https://codecov.io/gh/sidchaini/distclassipy)
 [![License - GPL-3](https://img.shields.io/pypi/l/distclassipy.svg)](https://github.com/sidchaini/distclassipy/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+[![arXiv](https://img.shields.io/badge/arXiv-astro--ph%2F2403.12120-red)](https://arxiv.org/abs/2403.12120) 
+[![ascl:2403.002](https://img.shields.io/badge/ascl-2403.002-blue.svg?colorB=262255)](https://ascl.net/2403.002)
+
 <!-- [![Paper](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.1038/s41586-020-2649-2) -->
 
 A python package for a distance-based classifier which can use several different distance metrics.
 
 ## Installation
 To install DistClassiPy, run the following command:
@@ -39,55 +42,55 @@
 )
 clf = dcpy.DistanceMetricClassifier(metric="canberra")
 clf.fit(X, y)
 print(clf.predict([[0, 0, 0, 0]]))
 ```
 
 ## Features
-- Multiple distance metrics support
-- Easy integration with existing data processing pipelines
-- Efficient and scalable for large datasets
+- **Distance Metric-Based Classification**: Utilizes a variety of distance metrics for classification.
+- **Customizable for Scientific Goals**: Allows fine-tuning based on scientific objectives by selecting appropriate distance metrics and features, enhancing both computational efficiency and model performance.
+- **Interpretable Results**: Offers improved interpretability of classification outcomes by directly using distance metrics and feature importance, making it ideal for scientific applications.
+- **Efficient and Scalable**: Demonstrates lower computational requirements compared to traditional methods like Random Forests, making it suitable for large datasets
+- **Open Source and Accessible**: Available as an open-source Python package on PyPI, encouraging broad application in astronomy and beyond
 
 ## Documentation
 
 For more detailed information about the package and its functionalities, please refer to the [official documentation](https://sidchaini.github.io/DistClassiPy/).
 
 ## Contributing
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to open an [issue](https://github.com/sidchaini/DistClassiPy/issues) or submit a [pull request](https://github.com/sidchaini/DistClassiPy/pulls).
 
 ## License
 DistClassiPy is released under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html). See the LICENSE file for more details.
 
 ## Citation
 
 If you use DistClassiPy in your research or project, please consider citing the paper:
-> Light Curve Classification with DistClassiPy: a new distance-based classifier (submitted to A&C)
-
+> Chaini, S., Mahabal, A., Kembhavi, A., & Bianco, F. B. (2024). Light Curve Classification with DistClassiPy: a new distance-based classifier. arXiv. https://doi.org/10.48550/arXiv.2403.12120
 
-<!--
 ### Bibtex
 
 
 ```bibtex
-@ARTICLE{Chaini2024,
-       author = {{Chaini}, S. and {Mahabal}, A. and {Kembhavi}, A. and {Bianco}, F.~B.},
-        title = "{Light Curve Classification with DistClassiPy: a new distance-based classifier}",
-      journal = {Submitted to A&C},
-    %  keywords = {},
-         year = 2024,
-      %   month = ,
-      %  volume = {},
-      %     eid = {},
-      %   pages = {},
-      %     doi = {},
-      %  adsurl = {},
-      % adsnote = {}
+@ARTICLE{chaini2024light,
+       author = {{Chaini}, Siddharth and {Mahabal}, Ashish and {Kembhavi}, Ajit and {Bianco}, Federica B.},
+       title = "{Light Curve Classification with DistClassiPy: a new distance-based classifier}",
+       journal = {arXiv e-prints},
+       keywords = {Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Solar and Stellar Astrophysics, Computer Science - Machine Learning},
+       year = 2024,
+       month = mar,
+       eid = {arXiv:2403.12120},
+       pages = {arXiv:2403.12120},
+       archivePrefix = {arXiv},
+       eprint = {2403.12120},
+       primaryClass = {astro-ph.IM},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2024arXiv240312120C},
+       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
--->
   
 
 <!-- You can also find citation information in the [CITATION.cff](https://github.com/sidchaini/DistClassiPy/CITATION.cff) file. -->
 
 
 ## Authors
 Siddharth Chaini, Ashish Mahabal, Ajit Kembhavi and Federica B. Bianco.
```

### Comparing `distclassipy-0.1.2/distclassipy/__init__.py` & `distclassipy-0.1.3/distclassipy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 
 from .classifier import (
     DistanceMetricClassifier,
 )  # Importing the DistanceMetricClassifier from the classifier module
 from .distances import (
     Distance,
 )  # Importing the Distance class from the distances module
-from .version import __version__
+
+__version__ = "0.1.3"
```

### Comparing `distclassipy-0.1.2/distclassipy/classifier.py` & `distclassipy-0.1.3/distclassipy/classifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+A module which contains the DistanceMetricClassifier introduced by Chaini et al. (2024) in "Light Curve Classification with DistClassiPy: a new distance-based classifier".
+"""
+
 import numpy as np
 import pandas as pd
 import scipy
 from .distances import Distance
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.utils.validation import check_X_y, check_array, check_is_fitted
 from sklearn.utils.multiclass import unique_labels
@@ -90,45 +94,54 @@
         self.metric = metric
         self.scale = scale
         self.central_stat = central_stat
         self.dispersion_stat = dispersion_stat
         self.calculate_kde = calculate_kde
         self.calculate_1d_dist = calculate_1d_dist
 
-        # Hardcoded source packages to check for distance metrics.
-        self.metric_sources_ = {
-            "scipy.spatial.distance": scipy.spatial.distance,
-            "distances.Distance": Distance(),
-        }
-
     def set_metric_fn_(self):
         """
         Set the metric function based on the provided metric.
 
         If the metric is a string, the function will look for a corresponding function in scipy.spatial.distance or distances.Distance. If the metric is a function, it will be used directly.
         """
 
+        # Hardcoded source packages to check for distance metrics.
+        metric_sources_ = {
+            "scipy.spatial.distance": scipy.spatial.distance,
+            "distances.Distance": Distance(),
+        }
+
         if callable(self.metric):
             self.metric_fn_ = self.metric
             self.metric_arg_ = self.metric
 
         elif isinstance(self.metric, str):
             metric_str_lowercase = self.metric.lower()
             metric_found = False
-            for package_str, source in self.metric_sources_.items():
+            for package_str, source in metric_sources_.items():
+
+                # Don't use scipy for jaccard as their implementation only works with booleans - use custom jaccard instead
+                if (
+                    package_str == "scipy.spatial.distance"
+                    and metric_str_lowercase == "jaccard"
+                ):
+                    continue
+
                 if hasattr(source, metric_str_lowercase):
                     self.metric_fn_ = getattr(source, metric_str_lowercase)
                     metric_found = True
-                    if package_str == "scipy.spatial.distance":
-                        # Use the string as an argument if it belongs to scipy as it is optimized
-                        self.metric_arg_ = self.metric
-                    else:
-                        self.metric_arg_ = self.metric_fn_
-                    break
 
+                    # Use the string as an argument if it belongs to scipy as it is optimized
+                    self.metric_arg_ = (
+                        self.metric
+                        if package_str == "scipy.spatial.distance"
+                        else self.metric_fn_
+                    )
+                    break
             if not metric_found:
                 raise ValueError(
                     f"{self.metric} metric not found. Please pass a string of the name of a metric in scipy.spatial.distance or distances.Distance, or pass a metric function directly. For a list of available metrics, see: https://sidchaini.github.io/DistClassiPy/distances.html or https://docs.scipy.org/doc/scipy/reference/spatial.distance.html"
                 )
 
     def fit(self, X: np.array, y: np.array, feat_labels: list[str] = None):
         """
@@ -354,17 +367,15 @@
                     ).ravel()
                     if self.scale and self.dispersion_stat == "std":
                         sum_1d_dists = sum_1d_dists + dists / self.df_std_.loc[cl, feat]
                     elif self.scale and self.dispersion_stat == "std":
                         sum_1d_dists = sum_1d_dists + dists / self.df_iqr_.loc[cl, feat]
                     else:
                         sum_1d_dists = sum_1d_dists + dists
-                confs = 1 / sum_1d_dists
-                # Add epsilon later
-                # confs = 1 / (sum_1d_dists + np.finfo(float).eps)
+                confs = 1 / np.clip(sum_1d_dists, a_min=np.finfo(float).eps, a_max=None)
                 conf_cl.append(confs)
             conf_cl = np.array(conf_cl)
             self.conf_cl_ = conf_cl
 
         self.analyis_ = True
 
         return y_pred
@@ -384,15 +395,17 @@
         if not hasattr(self, "analyis_"):
             raise ValueError(
                 "Use predict_and_analyse() instead of predict() for confidence calculation."
             )
 
         # Calculate confidence for each prediction
         if method == "distance_inverse":
-            self.confidence_df_ = 1 / self.centroid_dist_df_
+            self.confidence_df_ = 1 / np.clip(
+                self.centroid_dist_df_, a_min=np.finfo(float).eps, a_max=None
+            )
             self.confidence_df_.columns = [
                 x.replace("_dist", "_conf") for x in self.confidence_df_.columns
             ]
 
         elif method == "1d_distance_inverse":
             if not self.calculate_1d_dist:
                 raise ValueError(
```

### Comparing `distclassipy-0.1.2/distclassipy/distances.py` & `distclassipy-0.1.3/distclassipy/distances.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         5. Harmonic mean distance
         6. Fidelity
         7. Minimimum Symmetric Chi Squared
         8. Probabilistic Symmetric Chi Squared
 
     In addition, the following code was added to all functions for array conversion:
         u,v = np.asarray(u), np.asarray(v)
+-----
 """
 
 import numpy as np
 
 
 class Distance:
 
@@ -85,41 +86,41 @@
                vol. 1(4), pp. 300-307.
         """
         u, v = np.asarray(u), np.asarray(v)
         uvmult = u * v
         with np.errstate(divide="ignore", invalid="ignore"):
             return np.sum(np.where(uvmult != 0, ((u - v) ** 2 * (u + v)) / uvmult, 0))
 
-    def bhattacharyya(self, u, v):
-        """
-        Calculate the Bhattacharyya distance between two vectors.
-
-        Returns a distance value between 0 and 1.
-
-        Parameters
-        ----------
-        - u, v: Input vectors between which the distance is to be calculated.
+    # def bhattacharyya(self, u, v):
+    #     """
+    #     Calculate the Bhattacharyya distance between two vectors.
 
-        Returns
-        -------
-        - The Bhattacharyya distance between the two vectors.
+    #     Returns a distance value between 0 and 1.
 
-        References
-        ----------
-            1. Bhattacharyya A (1947) On a measure of divergence between two
-               statistical populations defined by probability distributions,
-               Bull. Calcutta Math. Soc., 35, 99–109.
-            2. Sung-Hyuk C. (2007) Comprehensive Survey on Distance/Similarity
-               Measures between Probability Density Functions. International
-               Journal of Mathematical Models and Methods in Applied Sciences.
-               1(4), 300-307.
-            3. https://en.wikipedia.org/wiki/Bhattacharyya_distance
-        """
-        u, v = np.asarray(u), np.asarray(v)
-        return -np.log(np.sum(np.sqrt(u * v)))
+    #     Parameters
+    #     ----------
+    #     - u, v: Input vectors between which the distance is to be calculated.
+
+    #     Returns
+    #     -------
+    #     - The Bhattacharyya distance between the two vectors.
+
+    #     References
+    #     ----------
+    #         1. Bhattacharyya A (1947) On a measure of divergence between two
+    #            statistical populations defined by probability distributions,
+    #            Bull. Calcutta Math. Soc., 35, 99–109.
+    #         2. Sung-Hyuk C. (2007) Comprehensive Survey on Distance/Similarity
+    #            Measures between Probability Density Functions. International
+    #            Journal of Mathematical Models and Methods in Applied Sciences.
+    #            1(4), 300-307.
+    #         3. https://en.wikipedia.org/wiki/Bhattacharyya_distance
+    #     """
+    #     u, v = np.asarray(u), np.asarray(v)
+    #     return -np.log(np.sum(np.sqrt(u * v)))
 
     def braycurtis(self, u, v):
         """
         Calculate the Bray-Curtis distance between two vectors.
 
         The Bray-Curtis distance is a measure of dissimilarity between two non-negative vectors,
         often used in ecology to measure the compositional dissimilarity between two sites based on counts
@@ -393,34 +394,34 @@
                Measures between Probability Density Functions. International
                Journal of Mathematical Models and Methods in Applied Sciences.
                1(4), 300-307.
         """
         u, v = np.asarray(u), np.asarray(v)
         return np.linalg.norm(u - v)
 
-    def fidelity(self, u, v):
-        """
-        Calculate the fidelity distance between two vectors.
+    # def fidelity(self, u, v):
+    #     """
+    #     Calculate the fidelity distance between two vectors.
 
-        The fidelity distance measures the similarity between two probability distributions.
+    #     The fidelity distance measures the similarity between two probability distributions.
 
-        Parameters
-        ----------
-        - u, v: Input vectors between which the distance is to be calculated.
+    #     Parameters
+    #     ----------
+    #     - u, v: Input vectors between which the distance is to be calculated.
 
-        Returns
-        -------
-        - The fidelity distance between the two vectors.
+    #     Returns
+    #     -------
+    #     - The fidelity distance between the two vectors.
 
-        Notes
-        -----
-            Added by SC.
-        """
-        u, v = np.asarray(u), np.asarray(v)
-        return 1 - (np.sum(np.sqrt(u * v)))
+    #     Notes
+    #     -----
+    #         Added by SC.
+    #     """
+    #     u, v = np.asarray(u), np.asarray(v)
+    #     return 1 - (np.sum(np.sqrt(u * v)))
 
     def google(self, u, v):
         """
         Calculate the Normalized Google Distance (NGD) between two vectors.
 
         NGD is a measure of similarity derived from the number of hits returned by the Google search engine for a given set of keywords.
 
@@ -511,34 +512,34 @@
               Measures between Probability Density Functions. International
               Journal of Mathematical Models and Methods in Applied Sciences.
               1(4), 300-307.
         """
         u, v = np.asarray(u), np.asarray(v)
         return np.sqrt(2 * np.sum((np.sqrt(u) - np.sqrt(v)) ** 2))
 
-    def inner(self, u, v):
-        """
-        Calculate the inner product distance between two vectors.
+    # def inner(self, u, v):
+    #     """
+    #     Calculate the inner product distance between two vectors.
 
-        The inner product distance is a measure of similarity between two vectors, based on their inner product.
+    #     The inner product distance is a measure of similarity between two vectors, based on their inner product.
 
-        Parameters
-        ----------
-        - u, v: Input vectors between which the distance is to be calculated.
+    #     Parameters
+    #     ----------
+    #     - u, v: Input vectors between which the distance is to be calculated.
 
-        Returns
-        -------
-        - The inner product distance between the two vectors.
+    #     Returns
+    #     -------
+    #     - The inner product distance between the two vectors.
 
-        Notes
-        -----
-            Added by SC.
-        """
-        u, v = np.asarray(u), np.asarray(v)
-        return 1 - np.dot(u, v)
+    #     Notes
+    #     -----
+    #         Added by SC.
+    #     """
+    #     u, v = np.asarray(u), np.asarray(v)
+    #     return 1 - np.dot(u, v)
 
     def jaccard(self, u, v):
         """
         Calculate the Jaccard distance between two vectors.
 
         The Jaccard distance measures dissimilarity between sample sets.
 
@@ -1028,40 +1029,40 @@
                Journal of Mathematical Models and Methods in Applied Sciences.
                1(4), 300-307.
         """
         u, v = np.asarray(u), np.asarray(v)
         with np.errstate(divide="ignore", invalid="ignore"):
             return np.sum(np.where(u != 0, (u - v) ** 2 / u, 0))
 
-    def nonintersection(self, u, v):
-        """
-        Calculate the Nonintersection distance between two vectors.
-
-        Parameters
-        ----------
-        - u, v: Input vectors between which the distance is to be calculated.
-
-        Returns
-        -------
-        - The Nonintersection distance between the two vectors.
-
-        References
-        ----------
-            1. Sung-Hyuk C. (2007) Comprehensive Survey on Distance/Similarity
-               Measures between Probability Density Functions. International
-               Journal of Mathematical Models and Methods in Applied Sciences.
-               1(4), 300-307.
+    # def nonintersection(self, u, v):
+    #     """
+    #     Calculate the Nonintersection distance between two vectors.
 
-        Notes
-        -----
-            When used for comparing two probability density functions (pdfs),
-            Nonintersection distance equals half of Cityblock distance.
-        """
-        u, v = np.asarray(u), np.asarray(v)
-        return 1 - np.sum(np.minimum(u, v))
+    #     Parameters
+    #     ----------
+    #     - u, v: Input vectors between which the distance is to be calculated.
+
+    #     Returns
+    #     -------
+    #     - The Nonintersection distance between the two vectors.
+
+    #     References
+    #     ----------
+    #         1. Sung-Hyuk C. (2007) Comprehensive Survey on Distance/Similarity
+    #            Measures between Probability Density Functions. International
+    #            Journal of Mathematical Models and Methods in Applied Sciences.
+    #            1(4), 300-307.
+
+    #     Notes
+    #     -----
+    #         When used for comparing two probability density functions (pdfs),
+    #         Nonintersection distance equals half of Cityblock distance.
+    #     """
+    #     u, v = np.asarray(u), np.asarray(v)
+    #     return 1 - np.sum(np.minimum(u, v))
 
     def pearson_chisq(self, u, v):
         """
         Calculate the Pearson chi-square divergence between two vectors.
 
         Parameters
         ----------
```

### Comparing `distclassipy-0.1.2/distclassipy.egg-info/PKG-INFO` & `distclassipy-0.1.3/distclassipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distclassipy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package for a distance-based classifier which can use several different distance metrics.
 Author-email: Siddharth Chaini <sidchaini@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -675,15 +675,15 @@
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Repository, https://github.com/sidchaini/DistClassiPy
-Project-URL: Documenation, https://sidchaini.github.io/DistClassiPy/
+Project-URL: Documentation, https://sidchaini.github.io/DistClassiPy/
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -708,14 +708,17 @@
 
 [![PyPI](https://img.shields.io/pypi/v/distclassipy?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/distclassipy/)
 [![Installs](https://img.shields.io/pypi/dm/distclassipy.svg?label=PyPI%20downloads)](https://pypi.org/project/distclassipy/)
 [![Codecov](https://codecov.io/gh/sidchaini/distclassipy/branch/main/graph/badge.svg)](https://codecov.io/gh/sidchaini/distclassipy)
 [![License - GPL-3](https://img.shields.io/pypi/l/distclassipy.svg)](https://github.com/sidchaini/distclassipy/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
+[![arXiv](https://img.shields.io/badge/arXiv-astro--ph%2F2403.12120-red)](https://arxiv.org/abs/2403.12120) 
+[![ascl:2403.002](https://img.shields.io/badge/ascl-2403.002-blue.svg?colorB=262255)](https://ascl.net/2403.002)
+
 <!-- [![Paper](https://img.shields.io/badge/DOI-10.1038%2Fs41586--020--2649--2-blue)](
 https://doi.org/10.1038/s41586-020-2649-2) -->
 
 A python package for a distance-based classifier which can use several different distance metrics.
 
 ## Installation
 To install DistClassiPy, run the following command:
@@ -739,55 +742,55 @@
 )
 clf = dcpy.DistanceMetricClassifier(metric="canberra")
 clf.fit(X, y)
 print(clf.predict([[0, 0, 0, 0]]))
 ```
 
 ## Features
-- Multiple distance metrics support
-- Easy integration with existing data processing pipelines
-- Efficient and scalable for large datasets
+- **Distance Metric-Based Classification**: Utilizes a variety of distance metrics for classification.
+- **Customizable for Scientific Goals**: Allows fine-tuning based on scientific objectives by selecting appropriate distance metrics and features, enhancing both computational efficiency and model performance.
+- **Interpretable Results**: Offers improved interpretability of classification outcomes by directly using distance metrics and feature importance, making it ideal for scientific applications.
+- **Efficient and Scalable**: Demonstrates lower computational requirements compared to traditional methods like Random Forests, making it suitable for large datasets
+- **Open Source and Accessible**: Available as an open-source Python package on PyPI, encouraging broad application in astronomy and beyond
 
 ## Documentation
 
 For more detailed information about the package and its functionalities, please refer to the [official documentation](https://sidchaini.github.io/DistClassiPy/).
 
 ## Contributing
 Contributions are welcome! If you have suggestions for improvements or bug fixes, please feel free to open an [issue](https://github.com/sidchaini/DistClassiPy/issues) or submit a [pull request](https://github.com/sidchaini/DistClassiPy/pulls).
 
 ## License
 DistClassiPy is released under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.en.html). See the LICENSE file for more details.
 
 ## Citation
 
 If you use DistClassiPy in your research or project, please consider citing the paper:
-> Light Curve Classification with DistClassiPy: a new distance-based classifier (submitted to A&C)
-
+> Chaini, S., Mahabal, A., Kembhavi, A., & Bianco, F. B. (2024). Light Curve Classification with DistClassiPy: a new distance-based classifier. arXiv. https://doi.org/10.48550/arXiv.2403.12120
 
-<!--
 ### Bibtex
 
 
 ```bibtex
-@ARTICLE{Chaini2024,
-       author = {{Chaini}, S. and {Mahabal}, A. and {Kembhavi}, A. and {Bianco}, F.~B.},
-        title = "{Light Curve Classification with DistClassiPy: a new distance-based classifier}",
-      journal = {Submitted to A&C},
-    %  keywords = {},
-         year = 2024,
-      %   month = ,
-      %  volume = {},
-      %     eid = {},
-      %   pages = {},
-      %     doi = {},
-      %  adsurl = {},
-      % adsnote = {}
+@ARTICLE{chaini2024light,
+       author = {{Chaini}, Siddharth and {Mahabal}, Ashish and {Kembhavi}, Ajit and {Bianco}, Federica B.},
+       title = "{Light Curve Classification with DistClassiPy: a new distance-based classifier}",
+       journal = {arXiv e-prints},
+       keywords = {Astrophysics - Instrumentation and Methods for Astrophysics, Astrophysics - Solar and Stellar Astrophysics, Computer Science - Machine Learning},
+       year = 2024,
+       month = mar,
+       eid = {arXiv:2403.12120},
+       pages = {arXiv:2403.12120},
+       archivePrefix = {arXiv},
+       eprint = {2403.12120},
+       primaryClass = {astro-ph.IM},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2024arXiv240312120C},
+       adsnote = {Provided by the SAO/NASA Astrophysics Data System}
 }
 ```
--->
   
 
 <!-- You can also find citation information in the [CITATION.cff](https://github.com/sidchaini/DistClassiPy/CITATION.cff) file. -->
 
 
 ## Authors
 Siddharth Chaini, Ashish Mahabal, Ajit Kembhavi and Federica B. Bianco.
```

### Comparing `distclassipy-0.1.2/pyproject.toml` & `distclassipy-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "distclassipy"
-version = "0.1.2"
+dynamic = ["version"]
 description = "A python package for a distance-based classifier which can use several different distance metrics."
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 authors = [{name = "Siddharth Chaini", email = "sidchaini@gmail.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -25,10 +25,13 @@
 dependencies = [
     "joblib>=1.3.2",
     "numpy>=1.26.3",
     "pandas>=2.2.0",
     "scikit-learn>=1.4.0"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "distclassipy.__version__"}
+
 [project.urls]
 Repository = "https://github.com/sidchaini/DistClassiPy"
-Documenation = "https://sidchaini.github.io/DistClassiPy/"
+Documentation = "https://sidchaini.github.io/DistClassiPy/"
```

### Comparing `distclassipy-0.1.2/tests/test_classifier.py` & `distclassipy-0.1.3/tests/test_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import pytest
 import numpy as np
 from distclassipy.classifier import DistanceMetricClassifier
+from sklearn.utils.estimator_checks import check_estimator
 
 
 # Test initialization of the classifier with specific parameters
 def test_init():
     clf = DistanceMetricClassifier(metric="euclidean", scale=True)
     assert clf.metric == "euclidean"
     assert clf.scale is True
 
 
-# Fix later
-# # Test classifier estimator compatibility with scikit-learn
-# def test_estimator_compatibility():
-#     from sklearn.utils.estimator_checks import check_estimator
-
-#     check_estimator(DistanceMetricClassifier())
+def test_sklearn_compatibility():
+    check_estimator(DistanceMetricClassifier())
 
 
 # Test fitting the classifier to a dataset
 def test_fit():
     X = np.array([[1, 2], [3, 4], [5, 6]])  # Sample feature set
     y = np.array([0, 1, 0])  # Sample target values
     clf = DistanceMetricClassifier()
@@ -101,15 +98,15 @@
         clf.fit(X, y)
 
 
 # Test setting central statistical method to median
 def test_central_stat_median():
     X = np.array([[1, 2], [3, 4], [5, 6]])  # Sample feature set
     y = np.array([0, 1, 0])  # Sample target values
-    clf = DistanceMetricClassifier(central_stat="median")
+    clf = DistanceMetricClassifier(central_stat="median", dispersion_stat="iqr")
     clf.fit(X, y)
     assert clf.central_stat == "median"
 
 
 # Test setting central statistical method to mean
 def test_central_stat_mean():
     X = np.array([[1, 2], [3, 4], [5, 6]])  # Sample feature set
```

