# Comparing `tmp/meshtastic2hass-1.0.7.tar.gz` & `tmp/meshtastic2hass-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic2hass-1.0.7.tar", last modified: Mon Apr  1 18:32:08 2024, max compression
+gzip compressed data, was "meshtastic2hass-1.0.8.tar", last modified: Thu Apr 18 12:26:33 2024, max compression
```

## Comparing `meshtastic2hass-1.0.7.tar` & `meshtastic2hass-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:32:08.279971 meshtastic2hass-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:32:08.271971 meshtastic2hass-1.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:32:08.275972 meshtastic2hass-1.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-01 18:32:08.279971 meshtastic2hass-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-01 18:32:08.279971 meshtastic2hass-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:32:08.275972 meshtastic2hass-1.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:32:08.275972 meshtastic2hass-1.0.7/src/meshtastic2hass/
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/src/meshtastic2hass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/src/meshtastic2hass/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/src/meshtastic2hass/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15125 2024-04-01 18:32:01.000000 meshtastic2hass-1.0.7/src/meshtastic2hass/meshtastic2hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:32:08.279971 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-01 18:32:08.000000 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 18:32:08.000000 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:32:08.000000 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:32:08.000000 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-01 18:32:08.000000 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-01 18:32:08.000000 meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:26:33.238634 meshtastic2hass-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:26:33.234634 meshtastic2hass-1.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:26:33.234634 meshtastic2hass-1.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-18 12:26:33.238634 meshtastic2hass-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-18 12:26:33.238634 meshtastic2hass-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:26:33.234634 meshtastic2hass-1.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:26:33.234634 meshtastic2hass-1.0.8/src/meshtastic2hass/
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/src/meshtastic2hass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/src/meshtastic2hass/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/src/meshtastic2hass/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15125 2024-04-18 12:26:20.000000 meshtastic2hass-1.0.8/src/meshtastic2hass/meshtastic2hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:26:33.238634 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-04-18 12:26:33.000000 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-18 12:26:33.000000 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:26:33.000000 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:26:32.000000 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 12:26:33.000000 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 12:26:33.000000 meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/top_level.txt
```

### Comparing `meshtastic2hass-1.0.7/.coveragerc` & `meshtastic2hass-1.0.8/.coveragerc`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/.github/workflows/python-package.yml` & `meshtastic2hass-1.0.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/.github/workflows/python-publish.yml` & `meshtastic2hass-1.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/.gitignore` & `meshtastic2hass-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/LICENSE` & `meshtastic2hass-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/PKG-INFO` & `meshtastic2hass-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic2hass
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python client that connects Meshtastic radios via MQTT to Home Assistant (Hass).
 Home-page: https://github.com/Mictronics/meshtastic2hass
 Author: Michael Wolf
 Author-email: michael@mictronics.de
 License: GPL v3+
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic2hass-1.0.7/README.md` & `meshtastic2hass-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/setup.cfg` & `meshtastic2hass-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/setup.py` & `meshtastic2hass-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/src/meshtastic2hass/__init__.py` & `meshtastic2hass-1.0.8/src/meshtastic2hass/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/src/meshtastic2hass/globals.py` & `meshtastic2hass-1.0.8/src/meshtastic2hass/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/src/meshtastic2hass/meshtastic2hass.py` & `meshtastic2hass-1.0.8/src/meshtastic2hass/meshtastic2hass.py`

 * *Files identical despite different names*

### Comparing `meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/PKG-INFO` & `meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic2hass
-Version: 1.0.7
+Version: 1.0.8
 Summary: A Python client that connects Meshtastic radios via MQTT to Home Assistant (Hass).
 Home-page: https://github.com/Mictronics/meshtastic2hass
 Author: Michael Wolf
 Author-email: michael@mictronics.de
 License: GPL v3+
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic2hass-1.0.7/src/meshtastic2hass.egg-info/SOURCES.txt` & `meshtastic2hass-1.0.8/src/meshtastic2hass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

