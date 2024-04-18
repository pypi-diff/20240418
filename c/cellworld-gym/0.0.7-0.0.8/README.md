# Comparing `tmp/cellworld_gym-0.0.7.tar.gz` & `tmp/cellworld_gym-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellworld_gym-0.0.7.tar", last modified: Wed Apr 17 20:14:27 2024, max compression
+gzip compressed data, was "cellworld_gym-0.0.8.tar", last modified: Wed Apr 17 20:15:02 2024, max compression
```

## Comparing `cellworld_gym-0.0.7.tar` & `cellworld_gym-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 20:14:27.382044 cellworld_gym-0.0.7/
--rw-rw-rw-   0        0        0       35 2024-04-17 20:14:26.000000 cellworld_gym-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      415 2024-04-17 20:14:27.381055 cellworld_gym-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       40 2024-04-17 20:14:26.000000 cellworld_gym-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 20:14:27.363934 cellworld_gym-0.0.7/cellworld_gym/
--rw-rw-rw-   0        0        0       40 2024-04-17 20:14:26.000000 cellworld_gym-0.0.7/cellworld_gym/README.md
--rw-rw-rw-   0        0        0       52 2024-04-17 14:49:47.000000 cellworld_gym-0.0.7/cellworld_gym/__init__.py
--rw-rw-rw-   0        0        0     5839 2024-04-17 20:14:13.000000 cellworld_gym-0.0.7/cellworld_gym/bot_evade.py
--rw-rw-rw-   0        0        0     1636 2024-04-17 20:14:26.000000 cellworld_gym-0.0.7/cellworld_gym/license.txt
--rw-rw-rw-   0        0        0      192 2024-04-17 20:14:26.000000 cellworld_gym-0.0.7/cellworld_gym/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 20:14:27.380036 cellworld_gym-0.0.7/cellworld_gym.egg-info/
--rw-rw-rw-   0        0        0      415 2024-04-17 20:14:27.000000 cellworld_gym-0.0.7/cellworld_gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-04-17 20:14:27.000000 cellworld_gym-0.0.7/cellworld_gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 20:14:27.000000 cellworld_gym-0.0.7/cellworld_gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-17 20:14:27.000000 cellworld_gym-0.0.7/cellworld_gym.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-04-17 20:14:27.000000 cellworld_gym-0.0.7/cellworld_gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-17 20:14:27.000000 cellworld_gym-0.0.7/cellworld_gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 20:14:27.382044 cellworld_gym-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      605 2024-04-17 20:14:26.000000 cellworld_gym-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 20:15:02.656877 cellworld_gym-0.0.8/
+-rw-rw-rw-   0        0        0       35 2024-04-17 20:15:01.000000 cellworld_gym-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      415 2024-04-17 20:15:02.654878 cellworld_gym-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2024-04-17 20:15:01.000000 cellworld_gym-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-17 20:15:02.639805 cellworld_gym-0.0.8/cellworld_gym/
+-rw-rw-rw-   0        0        0       40 2024-04-17 20:15:01.000000 cellworld_gym-0.0.8/cellworld_gym/README.md
+-rw-rw-rw-   0        0        0       52 2024-04-17 14:49:47.000000 cellworld_gym-0.0.8/cellworld_gym/__init__.py
+-rw-rw-rw-   0        0        0     5839 2024-04-17 20:14:13.000000 cellworld_gym-0.0.8/cellworld_gym/bot_evade.py
+-rw-rw-rw-   0        0        0     1636 2024-04-17 20:15:01.000000 cellworld_gym-0.0.8/cellworld_gym/license.txt
+-rw-rw-rw-   0        0        0      192 2024-04-17 20:15:01.000000 cellworld_gym-0.0.8/cellworld_gym/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 20:15:02.653888 cellworld_gym-0.0.8/cellworld_gym.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-04-17 20:15:02.000000 cellworld_gym-0.0.8/cellworld_gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-04-17 20:15:02.000000 cellworld_gym-0.0.8/cellworld_gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 20:15:02.000000 cellworld_gym-0.0.8/cellworld_gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-17 20:15:02.000000 cellworld_gym-0.0.8/cellworld_gym.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-04-17 20:15:02.000000 cellworld_gym-0.0.8/cellworld_gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-17 20:15:02.000000 cellworld_gym-0.0.8/cellworld_gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 20:15:02.656877 cellworld_gym-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      605 2024-04-17 20:15:01.000000 cellworld_gym-0.0.8/setup.py
```

### Comparing `cellworld_gym-0.0.7/cellworld_gym/bot_evade.py` & `cellworld_gym-0.0.8/cellworld_gym/bot_evade.py`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.7/cellworld_gym/license.txt` & `cellworld_gym-0.0.8/cellworld_gym/license.txt`

 * *Files identical despite different names*

### Comparing `cellworld_gym-0.0.7/setup.py` & `cellworld_gym-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,9 +7,9 @@
       author_email='germanespinosa@gmail.com',
       long_description=open('./cellworld_gym/README.md').read(),
       long_description_content_type='text/markdown',
       packages=['cellworld_gym'],
       install_requires=['cellworld_game', 'gym'],
       license='MIT',
       include_package_data=True,
-      version='0.0.7',
+      version='0.0.8',
       zip_safe=False)
```

