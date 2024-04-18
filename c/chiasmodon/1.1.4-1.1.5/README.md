# Comparing `tmp/chiasmodon-1.1.4.tar.gz` & `tmp/chiasmodon-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.4.tar", last modified: Thu Apr 18 02:57:37 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.5.tar", last modified: Thu Apr 18 02:58:42 2024, max compression
```

## Comparing `chiasmodon-1.1.4.tar` & `chiasmodon-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:57:37.130539 chiasmodon-1.1.4/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.4/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 02:57:37.130539 chiasmodon-1.1.4/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13130 2024-04-17 23:12:00.000000 chiasmodon-1.1.4/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:57:37.130539 chiasmodon-1.1.4/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 02:57:37.000000 chiasmodon-1.1.4/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 02:57:37.000000 chiasmodon-1.1.4/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 02:57:37.000000 chiasmodon-1.1.4/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 02:57:37.000000 chiasmodon-1.1.4/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 02:57:37.000000 chiasmodon-1.1.4/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:57:37.130539 chiasmodon-1.1.4/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    20524 2024-04-18 02:57:01.000000 chiasmodon-1.1.4/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 02:57:14.000000 chiasmodon-1.1.4/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 02:57:37.130539 chiasmodon-1.1.4/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1279 2024-04-18 02:57:21.000000 chiasmodon-1.1.4/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.5/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13130 2024-04-17 23:12:00.000000 chiasmodon-1.1.5/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    20524 2024-04-18 02:57:01.000000 chiasmodon-1.1.5/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 02:58:28.000000 chiasmodon-1.1.5/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 02:58:26.000000 chiasmodon-1.1.5/setup.py
```

### Comparing `chiasmodon-1.1.4/LICENSE.txt` & `chiasmodon-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.4/PKG-INFO` & `chiasmodon-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.4
+Version: 1.1.5
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.4/README.md` & `chiasmodon-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.4/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.5/chiasmodon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.4
+Version: 1.1.5
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.4/cli/chiasmodon_cli.py` & `chiasmodon-1.1.5/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.4/pychiasmodon.py` & `chiasmodon-1.1.5/pychiasmodon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner 
 
-VERSION = "1.1.4"
+VERSION = "1.1.5"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
     'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
     'subdomain':['domain'],
     'email':['domain', 'cidr', 'asn', 'app' ,'endpoint', 'phone', 'password'],
```

### Comparing `chiasmodon-1.1.4/setup.py` & `chiasmodon-1.1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.4',
+      version='1.1.5',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
-      scripts=['cli/chiasmodon_cli.py', 'cli/chiasmodon_scan.py'],
+      scripts=['cli/chiasmodon_cli.py'],
       install_requires=['requests', 'yaspin', 'tldextract']
      )
```

