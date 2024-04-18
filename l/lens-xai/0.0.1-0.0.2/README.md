# Comparing `tmp/lens_xai-0.0.1.tar.gz` & `tmp/lens_xai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lens_xai-0.0.1.tar", last modified: Thu Apr 18 10:18:20 2024, max compression
+gzip compressed data, was "lens_xai-0.0.2.tar", last modified: Thu Apr 18 13:27:15 2024, max compression
```

## Comparing `lens_xai-0.0.1.tar` & `lens_xai-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 dwane      (501) staff       (20)        0 2024-04-18 10:18:20.626359 lens_xai-0.0.1/
--rw-r--r--   0 dwane      (501) staff       (20)     7048 2024-04-17 06:14:13.000000 lens_xai-0.0.1/LICENSE
--rw-r--r--   0 dwane      (501) staff       (20)      354 2024-04-18 10:18:20.626169 lens_xai-0.0.1/PKG-INFO
--rw-r--r--   0 dwane      (501) staff       (20)     1831 2024-04-17 06:14:13.000000 lens_xai-0.0.1/README.md
-drwxr-xr-x   0 dwane      (501) staff       (20)        0 2024-04-18 10:18:20.625969 lens_xai-0.0.1/lens_xai.egg-info/
--rw-r--r--   0 dwane      (501) staff       (20)      354 2024-04-18 10:18:20.000000 lens_xai-0.0.1/lens_xai.egg-info/PKG-INFO
--rw-r--r--   0 dwane      (501) staff       (20)      154 2024-04-18 10:18:20.000000 lens_xai-0.0.1/lens_xai.egg-info/SOURCES.txt
--rw-r--r--   0 dwane      (501) staff       (20)        1 2024-04-18 10:18:20.000000 lens_xai-0.0.1/lens_xai.egg-info/dependency_links.txt
--rw-r--r--   0 dwane      (501) staff       (20)        1 2024-04-18 10:18:20.000000 lens_xai-0.0.1/lens_xai.egg-info/top_level.txt
--rw-r--r--   0 dwane      (501) staff       (20)       38 2024-04-18 10:18:20.626394 lens_xai-0.0.1/setup.cfg
--rw-r--r--   0 dwane      (501) staff       (20)      549 2024-04-18 10:17:53.000000 lens_xai-0.0.1/setup.py
+drwxr-xr-x   0 dwane      (501) staff       (20)        0 2024-04-18 13:27:15.344243 lens_xai-0.0.2/
+-rw-r--r--   0 dwane      (501) staff       (20)     7048 2024-04-17 06:14:13.000000 lens_xai-0.0.2/LICENSE
+-rw-r--r--   0 dwane      (501) staff       (20)      337 2024-04-18 13:27:15.344070 lens_xai-0.0.2/PKG-INFO
+-rw-r--r--   0 dwane      (501) staff       (20)     1831 2024-04-17 06:14:13.000000 lens_xai-0.0.2/README.md
+drwxr-xr-x   0 dwane      (501) staff       (20)        0 2024-04-18 13:27:15.343917 lens_xai-0.0.2/lens_xai.egg-info/
+-rw-r--r--   0 dwane      (501) staff       (20)      337 2024-04-18 13:27:15.000000 lens_xai-0.0.2/lens_xai.egg-info/PKG-INFO
+-rw-r--r--   0 dwane      (501) staff       (20)      154 2024-04-18 13:27:15.000000 lens_xai-0.0.2/lens_xai.egg-info/SOURCES.txt
+-rw-r--r--   0 dwane      (501) staff       (20)        1 2024-04-18 13:27:15.000000 lens_xai-0.0.2/lens_xai.egg-info/dependency_links.txt
+-rw-r--r--   0 dwane      (501) staff       (20)        1 2024-04-18 13:27:15.000000 lens_xai-0.0.2/lens_xai.egg-info/top_level.txt
+-rw-r--r--   0 dwane      (501) staff       (20)       38 2024-04-18 13:27:15.344283 lens_xai-0.0.2/setup.cfg
+-rw-r--r--   0 dwane      (501) staff       (20)      532 2024-04-18 13:27:04.000000 lens_xai-0.0.2/setup.py
```

### Comparing `lens_xai-0.0.1/LICENSE` & `lens_xai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lens_xai-0.0.1/README.md` & `lens_xai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lens_xai-0.0.1/setup.py` & `lens_xai-0.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 setup(
 name='lens_xai',
-version='0.0.1',
-author='Dwane van der Sluis',
-author_email='your.email@example.com',
+version='0.0.2',
+author='ucabdv1',
+author_email='ucabdv1@ucl.ac.uk',
 description='A short description of your package',
 packages=find_packages(),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
 'Operating System :: OS Independent',
 ],
```

