# Comparing `tmp/lingress-2.0.2.tar.gz` & `tmp/lingress-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lingress-2.0.2.tar", last modified: Thu Mar 21 09:35:27 2024, max compression
+gzip compressed data, was "lingress-2.1.0.tar", last modified: Thu Apr 18 08:34:29 2024, max compression
```

## Comparing `lingress-2.0.2.tar` & `lingress-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-03-21 09:35:27.305726 lingress-2.0.2/
--rw-r--r--   0 aeiwz      (501) staff       (20)     1066 2024-02-28 15:01:52.000000 lingress-2.0.2/LICENSE
--rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-03-21 09:35:27.305577 lingress-2.0.2/PKG-INFO
--rw-r--r--   0 aeiwz      (501) staff       (20)     2220 2024-02-28 15:12:10.000000 lingress-2.0.2/README.rst
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-03-21 09:35:27.300262 lingress-2.0.2/lingress/
--rw-r--r--   0 aeiwz      (501) staff       (20)      147 2024-03-21 08:35:13.000000 lingress-2.0.2/lingress/__init__.py
--rw-r--r--   0 aeiwz      (501) staff       (20)    42165 2024-03-21 09:34:09.000000 lingress-2.0.2/lingress/lingress.py
-drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-03-21 09:35:27.304033 lingress-2.0.2/lingress.egg-info/
--rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-03-21 09:35:27.000000 lingress-2.0.2/lingress.egg-info/PKG-INFO
--rw-r--r--   0 aeiwz      (501) staff       (20)      238 2024-03-21 09:35:27.000000 lingress-2.0.2/lingress.egg-info/SOURCES.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)        1 2024-03-21 09:35:27.000000 lingress-2.0.2/lingress.egg-info/dependency_links.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)       90 2024-03-21 09:35:27.000000 lingress-2.0.2/lingress.egg-info/requires.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)        9 2024-03-21 09:35:27.000000 lingress-2.0.2/lingress.egg-info/top_level.txt
--rw-r--r--   0 aeiwz      (501) staff       (20)       80 2024-03-21 09:35:27.306436 lingress-2.0.2/setup.cfg
--rw-r--r--   0 aeiwz      (501) staff       (20)     1378 2024-03-21 09:34:26.000000 lingress-2.0.2/setup.py
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-18 08:34:29.611485 lingress-2.1.0/
+-rw-r--r--   0 aeiwz      (501) staff       (20)     1066 2024-02-28 15:01:52.000000 lingress-2.1.0/LICENSE
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-18 08:34:29.611422 lingress-2.1.0/PKG-INFO
+-rw-r--r--   0 aeiwz      (501) staff       (20)     2220 2024-02-28 15:12:10.000000 lingress-2.1.0/README.rst
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-18 08:34:29.609952 lingress-2.1.0/lingress/
+-rw-r--r--   0 aeiwz      (501) staff       (20)      118 2024-04-18 07:54:20.000000 lingress-2.1.0/lingress/__init__.py
+-rw-r--r--   0 aeiwz      (501) staff       (20)    42166 2024-03-29 03:04:47.000000 lingress-2.1.0/lingress/lingress.py
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3083 2024-04-18 07:55:24.000000 lingress-2.1.0/lingress/utility.py
+drwxr-xr-x   0 aeiwz      (501) staff       (20)        0 2024-04-18 08:34:29.611088 lingress-2.1.0/lingress.egg-info/
+-rw-r--r--   0 aeiwz      (501) staff       (20)     3165 2024-04-18 08:34:29.000000 lingress-2.1.0/lingress.egg-info/PKG-INFO
+-rw-r--r--   0 aeiwz      (501) staff       (20)      258 2024-04-18 08:34:29.000000 lingress-2.1.0/lingress.egg-info/SOURCES.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)        1 2024-04-18 08:34:29.000000 lingress-2.1.0/lingress.egg-info/dependency_links.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)       90 2024-04-18 08:34:29.000000 lingress-2.1.0/lingress.egg-info/requires.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)        9 2024-04-18 08:34:29.000000 lingress-2.1.0/lingress.egg-info/top_level.txt
+-rw-r--r--   0 aeiwz      (501) staff       (20)       80 2024-04-18 08:34:29.611704 lingress-2.1.0/setup.cfg
+-rw-r--r--   0 aeiwz      (501) staff       (20)     1378 2024-04-18 07:56:29.000000 lingress-2.1.0/setup.py
```

### Comparing `lingress-2.0.2/LICENSE` & `lingress-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lingress-2.0.2/PKG-INFO` & `lingress-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lingress
-Version: 2.0.2
+Version: 2.1.0
 Summary: Metabolomics data analysis with univariate (linear regression) and visualization tools.
 Home-page: https://github.com/aeiwz/lingress.git
-Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.0.2.tar.gz
+Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.1.0.tar.gz
 Author: aeiwz
 Author-email: theerayut_aeiw_123@hotmail.com
 License: MIT
 Keywords: Omics,Chemometrics,Visualization,Data Analysis,Univariate,Linear Regression
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lingress-2.0.2/README.rst` & `lingress-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `lingress-2.0.2/lingress/lingress.py` & `lingress-2.1.0/lingress/lingress.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1074,8 +1074,8 @@
         #background color
         fig.update_layout({
             'plot_bgcolor': 'rgba(0, 0, 0, 0)',
             'paper_bgcolor': 'rgba(0, 0, 0, 0)',
         })
         self.fig = fig
         
-        return fig
+        return fig
```

### Comparing `lingress-2.0.2/lingress.egg-info/PKG-INFO` & `lingress-2.1.0/lingress.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lingress
-Version: 2.0.2
+Version: 2.1.0
 Summary: Metabolomics data analysis with univariate (linear regression) and visualization tools.
 Home-page: https://github.com/aeiwz/lingress.git
-Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.0.2.tar.gz
+Download-URL: https://github.com/aeiwz/lingress/archive/refs/tags/v2.1.0.tar.gz
 Author: aeiwz
 Author-email: theerayut_aeiw_123@hotmail.com
 License: MIT
 Keywords: Omics,Chemometrics,Visualization,Data Analysis,Univariate,Linear Regression
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `lingress-2.0.2/setup.py` & `lingress-2.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'lingress',      
   packages = ['lingress'], 
-  version = '2.0.2',  
+  version = '2.1.0',  
   license='MIT', 
   description = 'Metabolomics data analysis with univariate (linear regression) and visualization tools.',
   long_description=DESCRIPTION,
   author = 'aeiwz',                 
   author_email = 'theerayut_aeiw_123@hotmail.com',     
   url = 'https://github.com/aeiwz/lingress.git',  
-  download_url = 'https://github.com/aeiwz/lingress/archive/refs/tags/v2.0.2.tar.gz',  
+  download_url = 'https://github.com/aeiwz/lingress/archive/refs/tags/v2.1.0.tar.gz',  
   keywords = ['Omics', 'Chemometrics', 'Visualization', 'Data Analysis', 'Univariate', 'Linear Regression'],
   install_requires=[            
           'scikit-learn',
           'pandas',
           'numpy',
           'matplotlib',
           'seaborn',
```

