# Comparing `tmp/nextcaptcha-python-1.0.1.tar.gz` & `tmp/nextcaptcha_python-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcaptcha-python-1.0.1.tar", last modified: Wed Mar 27 15:47:09 2024, max compression
+gzip compressed data, was "nextcaptcha_python-1.0.4.tar", last modified: Thu Apr 18 02:52:37 2024, max compression
```

## Comparing `nextcaptcha-python-1.0.1.tar` & `nextcaptcha_python-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:47:09.306252 nextcaptcha-python-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-27 15:47:02.000000 nextcaptcha-python-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-27 15:47:09.302252 nextcaptcha-python-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-27 15:47:02.000000 nextcaptcha-python-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:47:09.302252 nextcaptcha-python-1.0.1/nextcaptcha/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-27 15:47:02.000000 nextcaptcha-python-1.0.1/nextcaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-03-27 15:47:02.000000 nextcaptcha-python-1.0.1/nextcaptcha/next.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 15:47:09.302252 nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-27 15:47:09.000000 nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-03-27 15:47:09.000000 nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 15:47:09.000000 nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 15:47:09.000000 nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-27 15:47:09.000000 nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 15:47:09.306252 nextcaptcha-python-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-27 15:47:02.000000 nextcaptcha-python-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/nextcaptcha/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/nextcaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/nextcaptcha/next.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/setup.py
```

### Comparing `nextcaptcha-python-1.0.1/LICENSE` & `nextcaptcha_python-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcaptcha-python-1.0.1/PKG-INFO` & `nextcaptcha_python-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcaptcha-python
-Version: 1.0.1
+Version: 1.0.4
 Summary: NextCaptcha Captcha Solving Service Api Wrapper for Python to solving recaptcha v2, v3,recapthcha moible,hcaptcha,funcaptcha
 Home-page: https://github.com/nextcaptcha/nextcaptcha-python/
 Author: nextcaptcha
 Author-email: support@nextcaptcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nextcaptcha-python-1.0.1/README.md` & `nextcaptcha_python-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nextcaptcha-python-1.0.1/nextcaptcha/next.py` & `nextcaptcha_python-1.0.4/nextcaptcha/next.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.client_key = client_key
         self.solft_id = solft_id
         self.callback_url = callback_url
         self.open_log = open_log
         self.session = requests.session()
 
     def _get_balance(self) -> str:
-        resp = self.session.get(url=self.HOST + "/getBalance", json={"clientKey": self.client_key})
+        resp = self.session.post(url=self.HOST + "/getBalance", json={"clientKey": self.client_key})
         if resp.status_code != 200:
             if self.open_log:
                 logging.error(f"Error: {resp.status_code} {resp.text}")
             return resp.json()
         if self.open_log:
             logging.info(f"Balance: {resp.json().get('balance')}")
         return resp.json().get("balance")
```

### Comparing `nextcaptcha-python-1.0.1/nextcaptcha_python.egg-info/PKG-INFO` & `nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcaptcha-python
-Version: 1.0.1
+Version: 1.0.4
 Summary: NextCaptcha Captcha Solving Service Api Wrapper for Python to solving recaptcha v2, v3,recapthcha moible,hcaptcha,funcaptcha
 Home-page: https://github.com/nextcaptcha/nextcaptcha-python/
 Author: nextcaptcha
 Author-email: support@nextcaptcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nextcaptcha-python-1.0.1/setup.py` & `nextcaptcha_python-1.0.4/setup.py`

 * *Files identical despite different names*

