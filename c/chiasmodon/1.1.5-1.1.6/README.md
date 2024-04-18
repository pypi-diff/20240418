# Comparing `tmp/chiasmodon-1.1.5.tar.gz` & `tmp/chiasmodon-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiasmodon-1.1.5.tar", last modified: Thu Apr 18 02:58:42 2024, max compression
+gzip compressed data, was "chiasmodon-1.1.6.tar", last modified: Thu Apr 18 03:07:36 2024, max compression
```

## Comparing `chiasmodon-1.1.5.tar` & `chiasmodon-1.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.5/LICENSE.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/PKG-INFO
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13130 2024-04-17 23:12:00.000000 chiasmodon-1.1.5/README.md
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/chiasmodon.egg-info/
--rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/PKG-INFO
--rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/SOURCES.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/dependency_links.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/requires.txt
--rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 02:58:42.000000 chiasmodon-1.1.5/chiasmodon.egg-info/top_level.txt
-drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/cli/
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    20524 2024-04-18 02:57:01.000000 chiasmodon-1.1.5/cli/chiasmodon_cli.py
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 02:58:28.000000 chiasmodon-1.1.5/pychiasmodon.py
--rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 02:58:42.070534 chiasmodon-1.1.5/setup.cfg
--rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 02:58:26.000000 chiasmodon-1.1.5/setup.py
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1053 2024-04-16 18:26:16.000000 chiasmodon-1.1.6/LICENSE.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/PKG-INFO
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    13130 2024-04-17 23:12:00.000000 chiasmodon-1.1.6/README.md
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/chiasmodon.egg-info/
+-rw-r--r--   0 mhm       (1000) mhm       (1000)    13688 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/PKG-INFO
+-rw-r--r--   0 mhm       (1000) mhm       (1000)      237 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/SOURCES.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/dependency_links.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       27 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/requires.txt
+-rw-r--r--   0 mhm       (1000) mhm       (1000)        1 2024-04-18 03:07:36.000000 chiasmodon-1.1.6/chiasmodon.egg-info/top_level.txt
+drwxr-xr-x   0 mhm       (1000) mhm       (1000)        0 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/cli/
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    21184 2024-04-18 03:07:32.000000 chiasmodon-1.1.6/cli/chiasmodon_cli.py
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)    18598 2024-04-18 03:07:30.000000 chiasmodon-1.1.6/pychiasmodon.py
+-rw-r--r--   0 mhm       (1000) mhm       (1000)       38 2024-04-18 03:07:36.700509 chiasmodon-1.1.6/setup.cfg
+-rwxr-xr-x   0 mhm       (1000) mhm       (1000)     1253 2024-04-18 03:07:35.000000 chiasmodon-1.1.6/setup.py
```

### Comparing `chiasmodon-1.1.5/LICENSE.txt` & `chiasmodon-1.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.5/PKG-INFO` & `chiasmodon-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.5
+Version: 1.1.6
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.5/README.md` & `chiasmodon-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `chiasmodon-1.1.5/chiasmodon.egg-info/PKG-INFO` & `chiasmodon-1.1.6/chiasmodon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiasmodon
-Version: 1.1.5
+Version: 1.1.6
 Summary: Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..
 Home-page: https://github.com/chiasmod0n/chiasmodon
 Author: chiasmod0n
 License: UNKNOWN
 Keywords: intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `chiasmodon-1.1.5/cli/chiasmodon_cli.py` & `chiasmodon-1.1.6/cli/chiasmodon_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,91 +140,92 @@
 
         output['related'] = [i.save_format() for i in related]
 
         if related:
             ULIT.wFile((self.output_folder / 'related.txt'), '\n'.join(output['related'])) 
             print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'related.txt')}{T.RESET}\n"
 
-        self.print(f"\nFind client creds in {T.GREEN+'*.'+domain+T.RESET}")
-        client_creds:list[Result] = self.search(
-            method='domain',
-            query=domain,
-            country=self.options.country,
-            view_type='cred',
-            sort=True ,
-            timeout=self.options.timeout,
-            only_domain_emails=False,
-            all=True,
-            limit=1000000,
-            callback_view_result=self.scan_callback,
-            yaspin=yaspin
-        )
-        output['client-creds'] =[i.save_format() for i in client_creds]
-
-        if client_creds:
-            ULIT.wFile((self.output_folder / 'client-creds.txt'), '\n'.join([':'.join(i) for i in output['client-creds']]))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-creds.txt')}{T.RESET}\n"
-            
-            for i in client_creds:
-                output['client-usernames'].append(i.username) if i.username and not i.email  and '/' not in i.username and  i.username not in output['client-usernames']  else None
-                output['client-passwords'].append(i.password) if i.password and i.password not in output['client-passwords'] else None
-                output['client-emails'].append(i.email) if i.email  and i.email not in output['client-emails'] else None
-                output['subdomains'].append(i.domain) if i.domain and i.domain not in output['subdomains'] and i.domain != domain else None
-                output['urls'].append(i.url) if i.url and i.url not in output['urls'] else None
-                output['endpoints'].append(i.urlEndpoint) if i.urlEndpoint and i.urlEndpoint not in output['endpoints'] else None
-                output['ports'].append(i.urlPort) if i.urlPort and i.urlPort not in output['ports'] else None
+        if self.options.scan_clients.lower() == 'yes':
+            self.print(f"\nFind client creds in {T.GREEN+'*.'+domain+T.RESET}")
+            client_creds:list[Result] = self.search(
+                method='domain',
+                query=domain,
+                country=self.options.country,
+                view_type='cred',
+                sort=True ,
+                timeout=self.options.timeout,
+                only_domain_emails=False,
+                all=True,
+                limit=1000000,
+                callback_view_result=self.scan_callback,
+                yaspin=yaspin
+            )
+            output['client-creds'] =[i.save_format() for i in client_creds]
+        
+            if client_creds:
+                ULIT.wFile((self.output_folder / 'client-creds.txt'), '\n'.join([':'.join(i) for i in output['client-creds']]))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-creds.txt')}{T.RESET}\n"
                 
-            ULIT.wFile((self.output_folder / 'client-usernames.txt'), '\n'.join(output['client-usernames']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-usernames.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'client-emails.txt'), '\n'.join(output['client-emails']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-emails.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'client-passwords.txt'), '\n'.join(output['client-passwords']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-passwords.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'endpoints.txt'), '\n'.join(output['endpoints']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'endpoints.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'ports.txt'), '\n'.join([f"{i}" for i in output['ports']]))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'ports.txt')}{T.RESET}\n"
-
-            ULIT.wFile((self.output_folder / 'subdomains.txt'), '\n'.join(output['subdomains']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'subdomains.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'urls.txt'), '\n'.join([f"{i}" for i in output['urls']]))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'urls.txt')}{T.RESET}\n"
-
-
-        self.print(f"\nFind employees creds for {T.GREEN+domain+T.RESET}")
-        employe_creds = self.search(
-            method='domain',
-            query=domain,
-            country=self.options.country,
-            view_type='cred',
-            sort=True ,
-            timeout=self.options.timeout,
-            only_domain_emails=True,
-            all=False,
-            limit=1000000,
-            callback_view_result=self.scan_callback,
-            yaspin=yaspin
-        )
-        output['employe-creds'] =[i.save_format() for i in employe_creds]
+                for i in client_creds:
+                    output['client-usernames'].append(i.username) if i.username and not i.email  and '/' not in i.username and  i.username not in output['client-usernames']  else None
+                    output['client-passwords'].append(i.password) if i.password and i.password not in output['client-passwords'] else None
+                    output['client-emails'].append(i.email) if i.email  and i.email not in output['client-emails'] else None
+                    output['subdomains'].append(i.domain) if i.domain and i.domain not in output['subdomains'] and i.domain != domain else None
+                    output['urls'].append(i.url) if i.url and i.url not in output['urls'] else None
+                    output['endpoints'].append(i.urlEndpoint) if i.urlEndpoint and i.urlEndpoint not in output['endpoints'] else None
+                    output['ports'].append(i.urlPort) if i.urlPort and i.urlPort not in output['ports'] else None
+                    
+                ULIT.wFile((self.output_folder / 'client-usernames.txt'), '\n'.join(output['client-usernames']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-usernames.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'client-emails.txt'), '\n'.join(output['client-emails']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-emails.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'client-passwords.txt'), '\n'.join(output['client-passwords']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'client-passwords.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'endpoints.txt'), '\n'.join(output['endpoints']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'endpoints.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'ports.txt'), '\n'.join([f"{i}" for i in output['ports']]))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'ports.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'subdomains.txt'), '\n'.join(output['subdomains']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'subdomains.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'urls.txt'), '\n'.join([f"{i}" for i in output['urls']]))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'urls.txt')}{T.RESET}\n"
+
+
+        if self.options.scan_employees.lower() == 'yes':
+            self.print(f"\nFind employees creds for {T.GREEN+domain+T.RESET}")
+            employe_creds = self.search(
+                method='domain',
+                query=domain,
+                country=self.options.country,
+                view_type='cred',
+                sort=True ,
+                timeout=self.options.timeout,
+                only_domain_emails=True,
+                all=False,
+                limit=1000000,
+                callback_view_result=self.scan_callback,
+                yaspin=yaspin
+            )
+            output['employe-creds'] =[i.save_format() for i in employe_creds]
 
-        if employe_creds:
-            ULIT.wFile((self.output_folder / 'employe-creds.txt'), '\n'.join([':'.join(i) for i in output['employe-creds']]))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-creds.txt')}{T.RESET}\n"
-            for i in employe_creds:
-                output['employe-usernames'].append(i.username) if i.username and not i.email and '/' not in i.username and i.username not in output['employe-usernames']  else None
-                output['employe-passwords'].append(i.password) if i.password and i.password not in output['employe-passwords'] else None
-                output['employe-emails'].append(i.email) if i.email  and i.email not in output['employe-emails'] else None
-                
-            ULIT.wFile((self.output_folder / 'employe-usernames.txt'), '\n'.join(output['employe-usernames']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-usernames.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'employe-emails.txt'), '\n'.join(output['employe-emails']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-emails.txt')}{T.RESET}\n"
-            ULIT.wFile((self.output_folder / 'employe-passwords.txt'), '\n'.join(output['employe-passwords']))
-            print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-passwords.txt')}{T.RESET}\n"
-        
+            if employe_creds:
+                ULIT.wFile((self.output_folder / 'employe-creds.txt'), '\n'.join([':'.join(i) for i in output['employe-creds']]))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-creds.txt')}{T.RESET}\n"
+                for i in employe_creds:
+                    output['employe-usernames'].append(i.username) if i.username and not i.email and '/' not in i.username and i.username not in output['employe-usernames']  else None
+                    output['employe-passwords'].append(i.password) if i.password and i.password not in output['employe-passwords'] else None
+                    output['employe-emails'].append(i.email) if i.email  and i.email not in output['employe-emails'] else None
+                    
+                ULIT.wFile((self.output_folder / 'employe-usernames.txt'), '\n'.join(output['employe-usernames']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-usernames.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'employe-emails.txt'), '\n'.join(output['employe-emails']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-emails.txt')}{T.RESET}\n"
+                ULIT.wFile((self.output_folder / 'employe-passwords.txt'), '\n'.join(output['employe-passwords']))
+                print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'employe-passwords.txt')}{T.RESET}\n"
+            
         ULIT.wJsonToFile((self.output_folder / 'scan.json'), output)
         print_output += f"\t{T.MAGENTA}-{T.RESET} {T.BLUE}{(self.output_folder / 'scan.json')}{T.RESET}"
 
         self.print(print_output)
         
 class CLI(Chiasmodon):
     def __init__(self, options:argparse.Namespace) -> None:
@@ -377,14 +378,16 @@
     parser.add_argument('-c','--cidr',          help='Search by CIDR.',type=str)
     parser.add_argument('-n','--asn',          help='Search by ASN.',type=str)
     parser.add_argument('-e','--email',         help='Search by email, only pro, only pro account.',type=str)
     parser.add_argument('-u','--username',      help='Search by username, only pro account.',type=str)
     parser.add_argument('-p','--password',      help='Search by password, only pro account.',type=str)
     parser.add_argument('-ep','--endpoint',     help='Search by url endpoint.',type=str)    
     parser.add_argument('-s','--scan',          help='scan the company domain (Related company, Client creds, Empolye creds, Company ASNs, Company Apps).',action='store_true', default=False)
+    parser.add_argument('-sc','--scan-clients', help='Run clients scan, default is yes, Ex: -sc no',type=str, default='yes')
+    parser.add_argument('-se','--scan-employees',help='Run employees scan, default is yes, Ex: -se no',type=str, default='yes')
     #parser.add_argument('-fs','--full-scan',    help='',action='store_true', default=False) # "soon" 
     parser.add_argument('-C','--country',       help='sort result by country code default is all', type=str, default='all')
     parser.add_argument('-A','--all',           help='view all result using "like",this option work only with (-d or --domain),default is False', action='store_true', default=False)
     parser.add_argument('-de','--domain-emails',help='only result for company "root" domain, this option work only with (-d or --domain), default is False',action='store_true', default=False)
     parser.add_argument('-r','--related',       help='Get related company domains,this option work only with (-d or --domain), default False',action='store_true', default=False)
     parser.add_argument('-o','--output',        help='filename to save the result', type=str,)
     parser.add_argument('-vt','--view-type',    help='type view the result default is "cred".', choices=VIEW_TYPE_LIST, type=str, default='cred')
```

### Comparing `chiasmodon-1.1.5/pychiasmodon.py` & `chiasmodon-1.1.6/pychiasmodon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import time
 import requests
 import tldextract
 from yaspin import Spinner 
 
-VERSION = "1.1.5"
+VERSION = "1.1.6"
 _API_URL = 'https://chiasmodon.com/v2/api/beta'
 _API_HEADERS = {'user-agent':'cli/python'}
 _VIEW_TYPE = {
     'cred':['domain', 'email', 'cidr', 'app', 'asn', 'username','password',  'endpoint',],
     'url':['domain', 'email', 'cidr', 'asn', 'username','password', 'endpoint',],
     'subdomain':['domain'],
     'email':['domain', 'cidr', 'asn', 'app' ,'endpoint', 'phone', 'password'],
```

### Comparing `chiasmodon-1.1.5/setup.py` & `chiasmodon-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='chiasmodon',
-      version='1.1.5',
+      version='1.1.6',
       description='Chiasmodon is an OSINT (Open Source Intelligence) tool designed to assist in the process of gathering information about a target domain. Its primary functionality revolves around searching for domain-related data, including domain emails, domain credentials (usernames and passwords), CIDRs (Classless Inter-Domain Routing), ASNs (Autonomous System Numbers), and subdomains..',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='chiasmod0n',
       keywords='intelligence osint credentials emails asn cidr bugbounty subdomains information-gathering intelligence-analysis reconnaissance attack-surface subdomain-enumeration reconnaissance-framework bugbounty-tool email-enumeration chiasmodon',
       url='https://github.com/chiasmod0n/chiasmodon',
       packages=['.'],
```

