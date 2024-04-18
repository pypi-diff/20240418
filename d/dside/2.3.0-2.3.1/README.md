# Comparing `tmp/dside-2.3.0.tar.gz` & `tmp/dside-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dside-2.3.0.tar", last modified: Tue Feb 20 16:50:30 2024, max compression
+gzip compressed data, was "dside-2.3.1.tar", last modified: Thu Apr 18 10:12:31 2024, max compression
```

## Comparing `dside-2.3.0.tar` & `dside-2.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 16:50:30.858709 dside-2.3.0/
--rw-rw-rw-   0        0        0     1091 2022-05-31 11:23:54.000000 dside-2.3.0/LICENSE
--rw-rw-rw-   0        0        0     3450 2024-02-20 16:50:30.857714 dside-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2749 2023-10-15 13:51:17.000000 dside-2.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-20 16:50:30.858709 dside-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1448 2024-02-20 16:49:40.000000 dside-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-20 16:50:30.810490 dside-2.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-02-20 16:50:30.829564 dside-2.3.0/src/dside/
--rw-rw-rw-   0        0        0    85076 2024-02-20 16:48:54.000000 dside-2.3.0/src/dside/DSI.py
--rw-rw-rw-   0        0        0       22 2022-05-31 11:23:54.000000 dside-2.3.0/src/dside/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-20 16:50:30.856714 dside-2.3.0/src/dside.egg-info/
--rw-rw-rw-   0        0        0     3450 2024-02-20 16:50:30.000000 dside-2.3.0/src/dside.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2024-02-20 16:50:30.000000 dside-2.3.0/src/dside.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 16:50:30.000000 dside-2.3.0/src/dside.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-02-20 16:50:30.000000 dside-2.3.0/src/dside.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-20 16:50:30.000000 dside-2.3.0/src/dside.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 10:12:31.094911 dside-2.3.1/
+-rw-rw-rw-   0        0        0     1091 2022-05-31 11:23:54.000000 dside-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3450 2024-04-18 10:12:31.093910 dside-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2749 2023-10-15 13:51:17.000000 dside-2.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 10:12:31.094911 dside-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1448 2024-04-18 10:11:34.000000 dside-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:12:31.044909 dside-2.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 10:12:31.066911 dside-2.3.1/src/dside/
+-rw-rw-rw-   0        0        0    85229 2024-04-18 10:10:45.000000 dside-2.3.1/src/dside/DSI.py
+-rw-rw-rw-   0        0        0       22 2022-05-31 11:23:54.000000 dside-2.3.1/src/dside/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:12:31.091907 dside-2.3.1/src/dside.egg-info/
+-rw-rw-rw-   0        0        0     3450 2024-04-18 10:12:31.000000 dside-2.3.1/src/dside.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2024-04-18 10:12:31.000000 dside-2.3.1/src/dside.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 10:12:31.000000 dside-2.3.1/src/dside.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-18 10:12:31.000000 dside-2.3.1/src/dside.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 10:12:31.000000 dside-2.3.1/src/dside.egg-info/top_level.txt
```

### Comparing `dside-2.3.0/LICENSE` & `dside-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dside-2.3.0/PKG-INFO` & `dside-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dside
-Version: 2.3.0
+Version: 2.3.1
 Summary: Design space identification tool for plotting and analysing design spaces (2D and 3D).
 Home-page: https://github.com/stvsach/dside
 Author: Steven Sachio
 Author-email: stevensachio1506@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dside Version: 2.3.0 Summary: Design space
+Metadata-Version: 2.1 Name: dside Version: 2.3.1 Summary: Design space
 identification tool for plotting and analysing design spaces (2D and 3D). Home-
 page: https://github.com/stvsach/dside Author: Steven Sachio Author-email:
 stevensachio1506@gmail.com License: MIT Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Programming Language :: Python :: 3 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: numpy
```

### Comparing `dside-2.3.0/README.md` & `dside-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dside-2.3.0/setup.py` & `dside-2.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 short_description = 'Design space identification tool for plotting and analysing design'+\
     ' spaces (2D and 3D).'
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name = 'dside',
```

### Comparing `dside-2.3.0/src/dside/DSI.py` & `dside-2.3.1/src/dside/DSI.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,17 @@
     def screen(self, constraints):
         """
         Takes in the DataFrame, data, and dictionary, constraints, 
         giving out the satisfied and violated DataFrame of samples
         constraints: {'output_name1': [lbd1, ubd1], 'output_name2': [lbd1, ubd2], ...}
         """
         import pandas as pd
-        data = self.df
+        if 'SatFlag' in list(self.df.columns):
+            self.df.pop('SatFlag')
+        data = self.df.copy()
         self.constraints = constraints
         sat = data.copy()
         for i in list(constraints.keys()):
             sat = sat[sat[i] >= constraints[i][0]]
             sat = sat[sat[i] <= constraints[i][1]]
         exclude_these = data.index.isin(list(sat.index))
         vio = data[~exclude_these]
@@ -785,30 +787,30 @@
 
         # Calculate design space size and classify regions
         if dim == 3:
             shp = self.classify_regions3D(shp)
             volume = 0
             for v in shp['P'][shp['simplices']]:
                 volume += np.abs(np.dot(v[0] - v[3], np.cross(v[1] - v[3], v[2] - v[3])))/6
-            shp['size'] = volume
+            shp['size'] = self.mm_size_norm(volume, self.normP)
         else:
             shp = self.classify_regions2D(shp)
             P = shp['P']
             simps = shp['simplices']
             v = simps
             a = (P[v][:, 0][:, 0] - P[v][:, 1][:, 0])**2 + \
                 (P[v][:, 0][:, 1] - P[v][:, 1][:, 1])**2
             b = (P[v][:, 1][:, 0] - P[v][:, 2][:, 0])**2 + \
                 (P[v][:, 1][:, 1] - P[v][:, 2][:, 1])**2
             c = (P[v][:, 2][:, 0] - P[v][:, 0][:, 0])**2 + \
                 (P[v][:, 2][:, 1] - P[v][:, 0][:, 1])**2
             a, b, c = np.sqrt([a, b, c])
             s = (a + b + c)*0.5
             area = np.sqrt(s*(s - a)*(s - b)*(s - c)) # area from Heron's formula
-            shp['size'] = np.sum(area)
+            shp['size'] = self.mm_size_norm(np.sum(area), self.normP)
     
         if vpoints.shape[0] == 0:
             self.vindsp = None
             self.report['no_vindsp'] = 0
         else:
             self.vindsp = vio[inside(vpoints, shp)]
             self.report['no_vindsp'] = self.vindsp.shape[0]
```

### Comparing `dside-2.3.0/src/dside.egg-info/PKG-INFO` & `dside-2.3.1/src/dside.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dside
-Version: 2.3.0
+Version: 2.3.1
 Summary: Design space identification tool for plotting and analysing design spaces (2D and 3D).
 Home-page: https://github.com/stvsach/dside
 Author: Steven Sachio
 Author-email: stevensachio1506@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dside Version: 2.3.0 Summary: Design space
+Metadata-Version: 2.1 Name: dside Version: 2.3.1 Summary: Design space
 identification tool for plotting and analysing design spaces (2D and 3D). Home-
 page: https://github.com/stvsach/dside Author: Steven Sachio Author-email:
 stevensachio1506@gmail.com License: MIT Classifier: Development Status :: 2 -
 Pre-Alpha Classifier: Programming Language :: Python :: 3 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Education Requires-Python: >=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: numpy
```

