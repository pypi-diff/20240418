# Comparing `tmp/mailwizz-python-sdk-1.0.2.tar.gz` & `tmp/mailwizz_python_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailwizz-python-sdk-1.0.2.tar", last modified: Tue Mar 19 10:31:20 2024, max compression
+gzip compressed data, was "mailwizz_python_sdk-1.0.3.tar", last modified: Thu Apr 18 07:44:26 2024, max compression
```

## Comparing `mailwizz-python-sdk-1.0.2.tar` & `mailwizz_python_sdk-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:31:20.622455 mailwizz-python-sdk-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-19 10:31:20.622455 mailwizz-python-sdk-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:31:20.622455 mailwizz-python-sdk-1.0.2/mailwizz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:31:20.622455 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/campaign_bounces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/campaigns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/campaigns_tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/countries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/customers.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/list_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/list_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/list_subscribers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/endpoint/transactional_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/mailwizz/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 10:31:20.622455 mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-19 10:31:20.000000 mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-19 10:31:20.000000 mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 10:31:20.000000 mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-19 10:31:20.000000 mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 10:31:20.000000 mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 10:31:20.622455 mailwizz-python-sdk-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-19 10:31:10.000000 mailwizz-python-sdk-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:26.535685 mailwizz_python_sdk-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-18 07:44:26.535685 mailwizz_python_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:26.531685 mailwizz_python_sdk-1.0.3/mailwizz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:26.535685 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/campaign_bounces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/campaigns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/campaigns_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/countries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/customers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/list_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/list_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/list_subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/endpoint/transactional_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/mailwizz/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 07:44:26.535685 mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-18 07:44:26.000000 mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-18 07:44:26.000000 mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 07:44:26.000000 mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 07:44:26.000000 mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 07:44:26.000000 mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 07:44:26.535685 mailwizz_python_sdk-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-18 07:44:22.000000 mailwizz_python_sdk-1.0.3/setup.py
```

### Comparing `mailwizz-python-sdk-1.0.2/LICENSE` & `mailwizz_python_sdk-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/PKG-INFO` & `mailwizz_python_sdk-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailwizz-python-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: This repository contains the Python SDK for MailWizz EMA.
 Home-page: https://www.mailwizz.com
 Author: twisted1919
 Author-email: support@mailwizz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mailwizz-python-sdk-1.0.2/README.md` & `mailwizz_python_sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/base.py` & `mailwizz_python_sdk-1.0.3/mailwizz/base.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/client.py` & `mailwizz_python_sdk-1.0.3/mailwizz/client.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/config.py` & `mailwizz_python_sdk-1.0.3/mailwizz/config.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/campaign_bounces.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/campaign_bounces.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/campaigns.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/campaigns.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/campaigns_tracking.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/campaigns_tracking.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/countries.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/countries.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/customers.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/customers.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/list_fields.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/list_fields.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/list_segments.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/list_segments.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,7 +22,55 @@
             'params_get': {
                 'page': page,
                 'per_page': per_page
             }
         })
 
         return client.request()
+
+    def get_segment(self, list_uid: str, segment_uid: str):
+        """
+        Get segments from a certain mail list
+        :param list_uid:
+        :param segment_uid:
+        :return:
+        """
+
+        client = Client({
+            'method': Client.METHOD_GET,
+            'url': self.config.get_api_url(
+                'lists/{list_uid}/segments/{segment_uid}'.format(
+                    list_uid=list_uid,
+                    segment_uid=segment_uid
+                )
+            ),
+            'params_get': {}
+        })
+
+        return client.request()
+
+    def get_subscribers(self, list_uid: str, segment_uid: str, page=1, per_page=10):
+        """
+        Get subscribers from a certain mail list segment
+        :param list_uid:
+        :param segment_uid:
+        :param page:
+        :param per_page:
+        :return:
+        """
+
+        client = Client({
+            'method': Client.METHOD_GET,
+            'url': self.config.get_api_url(
+                'lists/{list_uid}/segments/{segment_uid}/subscribers'.format(
+                    list_uid=list_uid,
+                    segment_uid=segment_uid
+                )
+            ),
+            'params_get': {
+                'page': page,
+                'per_page': per_page
+            }
+        })
+
+        return client.request()
+
```

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/list_subscribers.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/list_subscribers.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/lists.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/lists.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/templates.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/templates.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/endpoint/transactional_emails.py` & `mailwizz_python_sdk-1.0.3/mailwizz/endpoint/transactional_emails.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz/request.py` & `mailwizz_python_sdk-1.0.3/mailwizz/request.py`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/PKG-INFO` & `mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailwizz-python-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: This repository contains the Python SDK for MailWizz EMA.
 Home-page: https://www.mailwizz.com
 Author: twisted1919
 Author-email: support@mailwizz.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mailwizz-python-sdk-1.0.2/mailwizz_python_sdk.egg-info/SOURCES.txt` & `mailwizz_python_sdk-1.0.3/mailwizz_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mailwizz-python-sdk-1.0.2/setup.py` & `mailwizz_python_sdk-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='mailwizz-python-sdk',
-    version='1.0.2',
+    version='1.0.3',
     packages=setuptools.find_packages(),
     url='https://www.mailwizz.com',
     license='MIT',
     author='twisted1919',
     author_email='support@mailwizz.com',
     description='This repository contains the Python SDK for MailWizz EMA.',
     long_description=long_description,
```

