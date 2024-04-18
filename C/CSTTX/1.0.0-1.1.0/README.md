# Comparing `tmp/CSTTX-1.0.0.tar.gz` & `tmp/CSTTX-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSTTX-1.0.0.tar", last modified: Wed Apr 17 00:41:59 2024, max compression
+gzip compressed data, was "CSTTX-1.1.0.tar", last modified: Thu Apr 18 11:07:08 2024, max compression
```

## Comparing `CSTTX-1.0.0.tar` & `CSTTX-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 00:41:59.712272 CSTTX-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-04-17 00:41:59.707181 CSTTX-1.0.0/CSTTX.egg-info/
--rw-rw-rw-   0        0        0      468 2024-04-17 00:41:59.000000 CSTTX-1.0.0/CSTTX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-04-17 00:41:59.000000 CSTTX-1.0.0/CSTTX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 00:41:59.000000 CSTTX-1.0.0/CSTTX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 00:41:59.000000 CSTTX-1.0.0/CSTTX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 00:41:59.000000 CSTTX-1.0.0/CSTTX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      468 2024-04-17 00:41:59.710202 CSTTX-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        5 2024-04-17 00:38:12.000000 CSTTX-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 00:41:59.712272 CSTTX-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      732 2024-04-17 00:41:54.000000 CSTTX-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 11:07:08.605059 CSTTX-1.1.0/
+drwxrwxrwx   0        0        0        0 2024-04-18 11:07:08.603040 CSTTX-1.1.0/CSTTX.egg-info/
+-rw-rw-rw-   0        0        0      468 2024-04-18 11:07:08.000000 CSTTX-1.1.0/CSTTX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2024-04-18 11:07:08.000000 CSTTX-1.1.0/CSTTX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:07:08.000000 CSTTX-1.1.0/CSTTX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 11:07:08.000000 CSTTX-1.1.0/CSTTX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      468 2024-04-18 11:07:08.604053 CSTTX-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2024-04-17 00:38:12.000000 CSTTX-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 11:07:08.605059 CSTTX-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      716 2024-04-18 11:00:42.000000 CSTTX-1.1.0/setup.py
```

### Comparing `CSTTX-1.0.0/setup.py` & `CSTTX-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='CSTTX',
-  version='1.0.0',
+  version='1.1.0',
   author='RESIST',
   author_email='JONSON@gmail.com',
   description='CRYPTO LIBRARY',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://docs.github.com/',
   packages=find_packages(),
-  install_requires=['requests>=2.25.1'],
+  install_requires=[''],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   keywords='example python',
   project_urls={
```

