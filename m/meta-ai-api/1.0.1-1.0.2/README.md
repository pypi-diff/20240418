# Comparing `tmp/meta_ai_api-1.0.1.tar.gz` & `tmp/meta_ai_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meta_ai_api-1.0.1.tar", last modified: Thu Apr 18 21:22:47 2024, max compression
+gzip compressed data, was "meta_ai_api-1.0.2.tar", last modified: Thu Apr 18 21:28:25 2024, max compression
```

## Comparing `meta_ai_api-1.0.1.tar` & `meta_ai_api-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.585205 meta_ai_api-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/src/meta_ai_api/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/src/meta_ai_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-18 21:22:43.000000 meta_ai_api-1.0.1/src/meta_ai_api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:22:47.589206 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:22:47.000000 meta_ai_api-1.0.1/src/meta_ai_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.888744 meta_ai_api-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/src/meta_ai_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/src/meta_ai_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-18 21:28:21.000000 meta_ai_api-1.0.2/src/meta_ai_api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 21:28:25.892744 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 21:28:25.000000 meta_ai_api-1.0.2/src/meta_ai_api.egg-info/top_level.txt
```

### Comparing `meta_ai_api-1.0.1/setup.py` & `meta_ai_api-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `meta_ai_api-1.0.1/src/meta_ai_api/main.py` & `meta_ai_api-1.0.2/src/meta_ai_api/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,8 +72,8 @@
         ]["content"]:
             text += content["text"] + "\n"
         return text
 
 
 if __name__ == "__main__":
     meta = MetaAI()
-    print(meta.prompt("What was the match results for PSG vs Barca on April 16th"))
+    print(meta.prompt("Whats the weather in San Francisco today?"))
```

