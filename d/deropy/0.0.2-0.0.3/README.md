# Comparing `tmp/deropy-0.0.2.tar.gz` & `tmp/deropy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.0.2.tar", last modified: Wed Apr 10 14:47:19 2024, max compression
+gzip compressed data, was "deropy-0.0.3.tar", last modified: Thu Apr 18 14:45:57 2024, max compression
```

## Comparing `deropy-0.0.2.tar` & `deropy-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.126374 deropy-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 14:47:19.126374 deropy-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-10 14:47:12.000000 deropy-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.122374 deropy-0.0.2/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.126374 deropy-0.0.2/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-10 14:47:12.000000 deropy-0.0.2/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 14:47:19.126374 deropy-0.0.2/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 14:47:19.000000 deropy-0.0.2/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 14:47:19.126374 deropy-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-10 14:47:12.000000 deropy-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:57.351847 deropy-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-18 14:45:57.351847 deropy-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-18 14:45:53.000000 deropy-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:57.347847 deropy-0.0.3/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:57.351847 deropy-0.0.3/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9499 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-18 14:45:53.000000 deropy-0.0.3/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:45:57.351847 deropy-0.0.3/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-18 14:45:57.000000 deropy-0.0.3/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-18 14:45:57.000000 deropy-0.0.3/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:45:57.000000 deropy-0.0.3/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 14:45:57.000000 deropy-0.0.3/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-18 14:45:57.000000 deropy-0.0.3/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 14:45:57.000000 deropy-0.0.3/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:45:57.351847 deropy-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-18 14:45:53.000000 deropy-0.0.3/setup.py
```

### Comparing `deropy-0.0.2/PKG-INFO` & `deropy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of tool to help of DERO smart contract development
-Home-page: https://github.com/lcances/deropy
+Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: click==8.0.4
 Requires-Dist: requests==2.27.1
 Requires-Dist: coloredlogs==15.0.1
```

### Comparing `deropy-0.0.2/README.md` & `deropy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.0.2/deropy/commands/deploy.py` & `deropy-0.0.3/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.0.2/deropy/commands/generate.py` & `deropy-0.0.3/deropy/commands/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import click
 import json
 import os
 
 @click.command('generate')
-@click.option('-f', '--file', type=click.Path(), help='Create a file with the given name')
+@click.argument('file', type=click.Path())
 @click.option('-s', '--scid', type=str, help='The SCID of the smart contract', default='')
 def generate(file, scid):
     _generate_class(file, scid)
     _generate_tests(file)
 
 # def generate_tests(functions):
 #     file_content = _read_bas(file)
```

### Comparing `deropy-0.0.2/deropy.egg-info/PKG-INFO` & `deropy-0.0.3/deropy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A set of tool to help of DERO smart contract development
-Home-page: https://github.com/lcances/deropy
+Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: click==8.0.4
 Requires-Dist: requests==2.27.1
 Requires-Dist: coloredlogs==15.0.1
```

### Comparing `deropy-0.0.2/setup.py` & `deropy-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.0.2',
-    url='https://github.com/lcances/deropy',
+    version=os.getenv('DEROPY_VERSION') or '0.0.3',
+    url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'click==8.0.4',
```

