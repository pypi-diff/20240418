# Comparing `tmp/underhill-0.3.tar.gz` & `tmp/underhill-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "underhill-0.3.tar", last modified: Fri Apr 12 18:08:42 2024, max compression
+gzip compressed data, was "underhill-0.4.tar", last modified: Thu Apr 18 20:27:35 2024, max compression
```

## Comparing `underhill-0.3.tar` & `underhill-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 18:08:42.974041 underhill-0.3/
--rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-12 18:08:42.973918 underhill-0.3/PKG-INFO
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 18:08:42.972413 underhill-0.3/packages/
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 18:08:42.972763 underhill-0.3/packages/underhill/
--rw-r--r--   0 josiah     (501) staff       (20)        0 2024-04-11 21:17:26.000000 underhill-0.3/packages/underhill/__init__.py
--rw-r--r--   0 josiah     (501) staff       (20)     2116 2024-04-12 18:08:42.000000 underhill-0.3/packages/underhill/expedition.py
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 18:08:42.973374 underhill-0.3/packages/underhill.egg-info/
--rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-12 18:08:42.000000 underhill-0.3/packages/underhill.egg-info/PKG-INFO
--rw-r--r--   0 josiah     (501) staff       (20)      305 2024-04-12 18:08:42.000000 underhill-0.3/packages/underhill.egg-info/SOURCES.txt
--rw-r--r--   0 josiah     (501) staff       (20)        1 2024-04-12 18:08:42.000000 underhill-0.3/packages/underhill.egg-info/dependency_links.txt
--rw-r--r--   0 josiah     (501) staff       (20)       36 2024-04-12 18:08:42.000000 underhill-0.3/packages/underhill.egg-info/requires.txt
--rw-r--r--   0 josiah     (501) staff       (20)       10 2024-04-12 18:08:42.000000 underhill-0.3/packages/underhill.egg-info/top_level.txt
--rw-r--r--   0 josiah     (501) staff       (20)       38 2024-04-12 18:08:42.974076 underhill-0.3/setup.cfg
--rw-r--r--   0 josiah     (501) staff       (20)      508 2024-04-12 18:08:42.000000 underhill-0.3/setup.py
-drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-12 18:08:42.973486 underhill-0.3/test/
--rw-r--r--   0 josiah     (501) staff       (20)      346 2024-04-12 00:16:28.000000 underhill-0.3/test/test_expedition.py
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-18 20:27:35.733554 underhill-0.4/
+-rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-18 20:27:35.733437 underhill-0.4/PKG-INFO
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-18 20:27:35.731928 underhill-0.4/packages/
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-18 20:27:35.732277 underhill-0.4/packages/underhill/
+-rw-r--r--   0 josiah     (501) staff       (20)        0 2024-04-11 21:17:26.000000 underhill-0.4/packages/underhill/__init__.py
+-rw-r--r--   0 josiah     (501) staff       (20)     2246 2024-04-18 20:27:35.000000 underhill-0.4/packages/underhill/expedition.py
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-18 20:27:35.732872 underhill-0.4/packages/underhill.egg-info/
+-rw-r--r--   0 josiah     (501) staff       (20)      189 2024-04-18 20:27:35.000000 underhill-0.4/packages/underhill.egg-info/PKG-INFO
+-rw-r--r--   0 josiah     (501) staff       (20)      305 2024-04-18 20:27:35.000000 underhill-0.4/packages/underhill.egg-info/SOURCES.txt
+-rw-r--r--   0 josiah     (501) staff       (20)        1 2024-04-18 20:27:35.000000 underhill-0.4/packages/underhill.egg-info/dependency_links.txt
+-rw-r--r--   0 josiah     (501) staff       (20)       36 2024-04-18 20:27:35.000000 underhill-0.4/packages/underhill.egg-info/requires.txt
+-rw-r--r--   0 josiah     (501) staff       (20)       10 2024-04-18 20:27:35.000000 underhill-0.4/packages/underhill.egg-info/top_level.txt
+-rw-r--r--   0 josiah     (501) staff       (20)       38 2024-04-18 20:27:35.733590 underhill-0.4/setup.cfg
+-rw-r--r--   0 josiah     (501) staff       (20)      508 2024-04-18 20:27:35.000000 underhill-0.4/setup.py
+drwxr-xr-x   0 josiah     (501) staff       (20)        0 2024-04-18 20:27:35.733001 underhill-0.4/test/
+-rw-r--r--   0 josiah     (501) staff       (20)      818 2024-04-12 22:16:17.000000 underhill-0.4/test/test_expedition.py
```

### Comparing `underhill-0.3/packages/underhill/expedition.py` & `underhill-0.4/packages/underhill/expedition.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,19 @@
         response = requests.post(f"http://{self.underhill_host}:{self.pathfinder_port}/embark")
         content = response.json()
         self.port = content.get("port")
         self.expedition_id = content.get("expedition_id")
 
         # prepare session object
         self.session = requests.Session()
-        self.session.headers.update({"user-agent": generate_user_agent()})
+        self.session.headers.update({"user-agent": generate_user_agent(
+            os=["win", "mac", "linux"],
+            navigator=["chrome", "firefox"],
+            device_type=["desktop"]
+        )})
         self.proxy_settings = {
             "http": f"http://{underhill_host}:{self.port}",
             "https": f"http://{underhill_host}:{self.port}"
         }
         self.session.proxies.update(self.proxy_settings)
 
     def __enter__(self):
```

