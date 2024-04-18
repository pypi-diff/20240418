# Comparing `tmp/chiasmodon-1.1.2.tar.gz` & `tmp/chiasmodon-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.2.tar", last modified: Wed Apr 17 20:07:34 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.3.tar", last modified: Wed Apr 17 20:08:54 2024, max compression
```

## Comparing `chiasmodon-1.1.2.tar` & `chiasmodon-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:07:34.930047 chiasmodon-1.1.2/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.2/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:07:34.930047 chiasmodon-1.1.2/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13135 2024-04-17 20:02:40.000000 chiasmodon-1.1.2/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:07:34.930047 chiasmodon-1.1.2/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13693 2024-04-17 20:07:34.000000 chiasmodon-1.1.2/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 20:07:34.000000 chiasmodon-1.1.2/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:07:34.000000 chiasmodon-1.1.2/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 20:07:34.000000 chiasmodon-1.1.2/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:07:34.000000 chiasmodon-1.1.2/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:07:34.930047 chiasmodon-1.1.2/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11258 2024-04-17 20:07:11.000000 chiasmodon-1.1.2/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19301 2024-04-17 20:07:23.000000 chiasmodon-1.1.2/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 20:07:34.930047 chiasmodon-1.1.2/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 20:07:26.000000 chiasmodon-1.1.2/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:08:54.910041 chiasmodon-1.1.3/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.3/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-17 20:08:54.910041 chiasmodon-1.1.3/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13130 2024-04-17 20:08:42.000000 chiasmodon-1.1.3/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:08:54.910041 chiasmodon-1.1.3/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-17 20:08:54.000000 chiasmodon-1.1.3/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-17 20:08:54.000000 chiasmodon-1.1.3/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:08:54.000000 chiasmodon-1.1.3/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-17 20:08:54.000000 chiasmodon-1.1.3/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-17 20:08:54.000000 chiasmodon-1.1.3/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-17 20:08:54.910041 chiasmodon-1.1.3/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    11258 2024-04-17 20:07:11.000000 chiasmodon-1.1.3/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    19301 2024-04-17 20:08:49.000000 chiasmodon-1.1.3/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-17 20:08:54.910041 chiasmodon-1.1.3/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-17 20:08:51.000000 chiasmodon-1.1.3/setup.py
```

### Comparing `chiasmodon-1.1.2/LICENSE.txt` & `chiasmodon-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.2/PKG-INFO` & `chiasmodon-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.2
+Version: 1.1.3
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -82,16 +82,16 @@
   -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
                         type view the result default is "cred".
   -o OUTPUT, --output OUTPUT
                         filename to save the result
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
-  -A, --all             view all result using "like",this option work only with (-d or --domain , -a or --app),default is False
-  -de, --domain-emails  only result for company domain, this option work only with -d or --domain, default is False
+  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
+  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
   -T TIMEOUT, --timeout TIMEOUT
                         request timeout default is 60.
   -L LIMIT, --limit LIMIT
                         limit results default is 10000.
   -v, --version         version.
 
 Examples:
```

### Comparing `chiasmodon-1.1.2/README.md` & `chiasmodon-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
   -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
                         type view the result default is "cred".
   -o OUTPUT, --output OUTPUT
                         filename to save the result
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
-  -A, --all             view all result using "like",this option work only with (-d or --domain , -a or --app),default is False
-  -de, --domain-emails  only result for company domain, this option work only with -d or --domain, default is False
+  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
+  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
   -T TIMEOUT, --timeout TIMEOUT
                         request timeout default is 60.
   -L LIMIT, --limit LIMIT
                         limit results default is 10000.
   -v, --version         version.
 
 Examples:
```

### Comparing `chiasmodon-1.1.2/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.3/chiasmodon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.2
+Version: 1.1.3
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -82,16 +82,16 @@
   -vt {cred,url,subdomain,email,password,username,app,endpoint,port}, --view-type {cred,url,subdomain,email,password,username,app,endpoint,port}
                         type view the result default is "cred".
   -o OUTPUT, --output OUTPUT
                         filename to save the result
   -ot {text,json,csv}, --output-type {text,json,csv}
                         output format default is "text".
   --init INIT           set the api token.
-  -A, --all             view all result using "like",this option work only with (-d or --domain , -a or --app),default is False
-  -de, --domain-emails  only result for company domain, this option work only with -d or --domain, default is False
+  -A, --all             view all result using "like",this option work only with (-d or --domain),default is False
+  -de, --domain-emails  only result for company "root" domain, this option work only with (-d or --domain), default is False
   -T TIMEOUT, --timeout TIMEOUT
                         request timeout default is 60.
   -L LIMIT, --limit LIMIT
                         limit results default is 10000.
   -v, --version         version.
 
 Examples:
```

### Comparing `chiasmodon-1.1.2/cli/chiasmodon_cli.py` & `chiasmodon-1.1.3/cli/chiasmodon_cli.py`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.2/pychiasmodon.py` & `chiasmodon-1.1.3/pychiasmodon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner
 
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 
 class Chiasmodon:
     API_URL         = 'https://chiasmodon.com/v2/api/beta'
     API_HEADERS     = {'user-agent':'cli/python'}
     VIEW_TYPE = {
         'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
         'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
```

### Comparing `chiasmodon-1.1.2/setup.py` & `chiasmodon-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.2',
+      version='1.1.3',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

