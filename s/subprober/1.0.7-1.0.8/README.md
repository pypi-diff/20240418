# Comparing `tmp/subprober-1.0.7.tar.gz` & `tmp/subprober-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprober-1.0.7.tar", last modified: Mon Feb 19 16:39:47 2024, max compression
+gzip compressed data, was "subprober-1.0.8.tar", last modified: Thu Apr 18 17:30:54 2024, max compression
```

## Comparing `subprober-1.0.7.tar` & `subprober-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:47.073562 subprober-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-19 16:39:39.000000 subprober-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-19 16:39:47.073562 subprober-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-02-19 16:39:39.000000 subprober-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:39:47.073562 subprober-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-19 16:39:39.000000 subprober-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:47.073562 subprober-1.0.7/subprober/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:39.000000 subprober-1.0.7/subprober/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:47.073562 subprober-1.0.7/subprober/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:39.000000 subprober-1.0.7/subprober/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-19 16:39:39.000000 subprober-1.0.7/subprober/modules/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:47.073562 subprober-1.0.7/subprober/modules/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:39.000000 subprober-1.0.7/subprober/modules/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-02-19 16:39:39.000000 subprober-1.0.7/subprober/modules/lib/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-19 16:39:39.000000 subprober-1.0.7/subprober/subprober.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:39:47.073562 subprober-1.0.7/subprober.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-19 16:39:47.000000 subprober-1.0.7/subprober.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-19 16:39:47.000000 subprober-1.0.7/subprober.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:39:47.000000 subprober-1.0.7/subprober.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-19 16:39:47.000000 subprober-1.0.7/subprober.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-19 16:39:47.000000 subprober-1.0.7/subprober.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 16:39:47.000000 subprober-1.0.7/subprober.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.447594 subprober-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 17:30:45.000000 subprober-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-18 17:30:54.447594 subprober-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-04-18 17:30:45.000000 subprober-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:30:54.447594 subprober-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-18 17:30:45.000000 subprober-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/banner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/banner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/banner/banner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14698 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/core/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/core/probes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/core/probes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/core/probes/probes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/core/screenshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/core/screenshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/core/screenshot/screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/extender/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/extender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/extender/extender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.443594 subprober-1.0.8/subprober/modules/help/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/help/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/help/help.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.447594 subprober-1.0.8/subprober/modules/update/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.447594 subprober-1.0.8/subprober/modules/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/verify/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.447594 subprober-1.0.8/subprober/modules/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/modules/version/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-18 17:30:45.000000 subprober-1.0.8/subprober/subprober.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:30:54.447594 subprober-1.0.8/subprober.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-18 17:30:54.000000 subprober-1.0.8/subprober.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-18 17:30:54.000000 subprober-1.0.8/subprober.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:30:54.000000 subprober-1.0.8/subprober.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-18 17:30:54.000000 subprober-1.0.8/subprober.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-18 17:30:54.000000 subprober-1.0.8/subprober.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 17:30:54.000000 subprober-1.0.8/subprober.egg-info/top_level.txt
```

### Comparing `subprober-1.0.7/LICENSE` & `subprober-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `subprober-1.0.7/README.md` & `subprober-1.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,48 @@
-# Subprober v1.0.7 - A Fast Multi-Purpose Http Probing Tool for Penetration Testing
+# Subprober v1.0.8 - A Fast Multi-Purpose Http Probing Tool for Penetration Testing
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/sanjai-AK47/Subprober) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/sanjai-AK47/Subprober) [![GitHub license](https://img.shields.io/github/license/sanjai-AK47/Subprober)](https://github.com/sanjai-AK47/Subprober/blob/main/LICENSE) [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/d-sanjai-kumar-109a7227b/)
 
 ### Overview
 
 Subprober  is a powerful and efficient tool designed for penetration testers and security professionals. This release introduces several enhancements, bug fixes, and new features to elevate your subdomain probing experience. Subprober facilitates fast and reliable information extraction, making it an invaluable asset for penetration testing workflows.
 
-### Features in V1.0.7:
-- Subprober is capable to handle high loads
-- accuracy and concurrency are improved
-- add extra configuration in probing saving outputs
-- added new command `-dhp` `--disable-http-probe` to only probe https protocol
-- improved subprober's memory allocations
-- added deduplication that remove duplicated urls and etc..
+### Features in V1.0.8:
+- **New Probing configurations**
+
+    - **-ip**   : **finds the ips of urls**
+    - **-cn**   : **find the cname of urls**
+    - **-maxr** : **maximum redirection for url**
+    - **-ra**   : **enable random agent to probe with random agent**
+    - **-X**    : **custom method for urls to probe**
+    - **-H**    : **set custom header for urls to probe**
+    - **-sc**   : **removed default to show response code and this flag to improve the subprober I/O**
+    
+- **Improved Concurrency**
+
+    - **Subprober concurrency and accuracy are improved with asynchoronous libraries** `aiohttp`, `arsenic`, `aiodns` **which make subprober to asynchornously probe
+        urls**
+        
+- **Headless**
+
+    - **-ss**   : **enable to probe and take screenshots for urls (required: chormedriver, geckodriver to be installed)**
+    - **-st**   : **set a timeout value for urls to take screenshots**
+    - **-bt**   : **select your browser type to take screenshots**
+    
+- **IO Support**:
+
+    - **Subprober now support stdout when using `-nc` flag which make subprober output to be piped and extend your automated workflows**
+    - **Now Subprober automatically detect the stdin are connected or not and quits**
+    - **Improved Subprober is now capable to handle high load urls and probe for it and tested with 4m+ urls**
+
+### Speed and Loads:
+Subprober is really concurrent in probing and taking screenshots asynchornously and speed may differ depends on your network
+subprober can be used even in your  less sources `aws` VPS server without causing any high load to your system but only when probing
+but not when taking screenshots, ip, cnames and Subprober can handle high load of urls and subprober tested with 2m+ urls and probed
+without any problem, users can also try more urls than tested
 
 ### Installation and Updates
 
 ##### Method 1:
 
 ```bash
 pip install git+https://github.com/sanjai-AK47/Subprober.git
@@ -29,122 +55,97 @@
 git clone https://github.com/sanjai-AK47/SubProber.git
 cd Subprober
 pip install .
 subprober -h
 ```
 
 
-
-### Recommended Concurrencies:
-
-**Info:** Subprober is improved with higher concurrency and accuracy for probings and recommend the users to use the concurrencies less which is efficient and accurate for probing
-  - 30-50   : this range of concurrency can be given when probing for more than 50K+ Subdomains, ips, domains etc..
-  - 50-80   : this range of concurrency can be given when probing for more than 100K+ Subdomains, ips, domains etc..
-  - 100-120 : this range of concurrency can be given when probing for more than 150K+ Subdomains, ips, domains etc..
-
-Note higher concurrency values may results in inaccurate results because subprober builded with higher concurrency and more accurate than other probing tool with following mentioned concurrency values
-
 ### Usage
 
 ```yaml
 subprober -h      
  
 
    _____       __    ____             __             
   / ___/__  __/ /_  / __ \_________  / /_  ___  _____
   \__ \/ / / / __ \/ /_/ / ___/ __ \/ __ \/ _ \/ ___/
  ___/ / /_/ / /_/ / ____/ /  / /_/ / /_/ /  __/ /    
 /____/\__,_/_.___/_/   /_/   \____/_.___/\___/_/     
                                                          
                 
                 
-                    Author : D.Sanjai Kumar @CyberRevoltSecurities
-
-                                                                         
-                                                  
+                    @RevoltSecurities
 
           
 Subprober - An essential HTTP multi-purpose Probing Tool for Penetration testers
 
 [Description] :
 
-    Subprober is a high-performance tool designed for probing and  extract vital information efficiently.
+    Subprober is a high-performance tool designed for probing and extract vital information efficiently.
 
 [Options]:
 
-
     [INPUT]:
 
-        -f,   --filename              Specify the filename containing a list of subdomains for targeted probing. 
-                                      This flag is used to find and analyze status codes and other pertinent details.
-                                      
-        -u,   --url                   Specify a target URL for direct probing. This flag allows for the extraction of 
-                                      status codes and other valuable information.
-                                      
-        stdin                         Subprober supports stdin input by using cat or echo command with subprober using pipe `|`
+        -f,    --filename              specify the filename containing a list of urls for probing.                                       
+        -u,    --url                   specify a target URL for direct probing
+        stdin/stdout                   subprober supports both stdin/stdout and enable -nc to pipe the output of subprober
                                       
     [PROBES-CONFIG]:
 
-
-        -tl,  --title                 Retrieve and display the title of subdomains.
- 
-        -sv,  --server                Identify and display the server information associated with subdomains.
-
-        -wc,  --word-count            Retrieve and display the content length of subdomains.
-        
-        -l ,  --location              Display the redirected location of the response.
-
-        -apt, --application-type      Determine and display the application type of subdomains.
-
-        -p,   --path                  Specify a path for probe and get results ex:: -p admin.php
-    
-        -px,  --proxy                 Specify a proxy to send the requests through your proxy or BurpSuite ex: 127.0.0.1:8080
+        -sc,   --status-code           display the response status code
+        -tl,   --title                 retrieve and display the titles
+        -sv,   --server                identify and display the server name
+        -wc,   --word-count            retrieve and display the content length
+        -l ,   --location              display the redirected location of the response.
+        -apt,  --application-type      determine and display the application type.
+        -p,    --path                  specify a path for probe and get results ex: -p admin.php
+        -px,   --proxy                 specify a proxy to send the requests through your proxy or BurpSuite (ex: http://127.0.0.1:8080)
+        -gw,   --grep-word             enable The grep word flag will be usefull when grepping partiuclar status codes
+        -ar,   --allow-redirect        enabling these flag will make Subprober to follow the redirection and ger results
+        -dhp,  --disable-http-probe    disables the subprober from probing to http protocols and only for https when no protocol is specified
+        -X  ,  --method                request methods to probe and get response
+        -H  ,  --header                add a custom headers for probing and -H can be used multiple times to pass multiple header values (ex: -H application/json -H X-Forwarded-Host: 127.0.0.1)
+        -ra ,  --random-agent          enable Random User-Agent to use for probing (default: subprober/Alpha)
+        -ip ,  --ip                    find ip address for the host
+        -cn ,  --cname                 find cname for the host
+        -maxr, --max-redirection       set a max value to follow redirection (default: 10)
     
-        -gw,  --grep-word             Enable The grep word flag will be usefull when grepping partiuclar codes like for 200: OK ---> cat subprober-results.txt | grep OK 
-                                      This will show the results with 200-299 range codes
-                                                                  
-        -ar,  --allow-redirect        Enabling these flag will make Subprober to follow the redirection and ger results
-        
-        -dhp. --disable-http-probe    Disables the subprober from probing to http protocols and only for https when no protocol is specified
-        
-    [MATCHERS]:
+    [HEADLESS-Mode]:
 
-        -ex,  --exclude               Exclude specific response status code(s) from the analysis.
+        -ss,   --screenshot            enable to take screenshot of the page using headless browsers with asynchronous performance
+        -st,   --screenshot-timeout    eet a timeout values for taking screenshosts  
+        -br,   --browser-type          select a browser for taking screenshots and browser available: chrome, firefox (default: chrome)
+                                       and requires chrome driver, gecko driver to be installed
+    [MATCHERS]:
 
-        -mc,  --match                 Specify specific response status code(s) to include in the analysis.
+        -ex,   --exclude               exclude specific response status code(s) from the analysis.
+        -mc,   --match                 specify specific response status code(s) to include in the analysis.
                                       
     [OUTPUT]:
     
-        -o,   --output                Define the output filename to store the results of the probing operation.
-        
-        -das, ---disable-auto-save    Disable the autosave of the results when no output file is specified 
+        -o,    --output                define the output filename to store the results of the probing operation.
+        -das,  ---disable-auto-save    disable the autosave of the results when no output file is specified.
+        -oD,   --output-directory      define a folder name to save  screenshot outputs.
 
     [Rate-Limits]:
 
-                      
-        -c,   --concurrency           Set the concurrency level for multiple processes. Default is 50.
-        
-        -to,  --timeout               Set a custom timeout value for sending requests.
-
+        -c,    --concurrency           set the concurrency level for subprober (default 50)
+        -to,   --timeout               set a custom timeout value for sending requests.
         
     [UPDATES]:
-
-
-        -up,  --update                Update Subprober to the latest version (pip required to be installed)
-
+        -up,   --update                update Subprober to the latest version (pip required to be installed)
+        -sup,  --show-updates          shows the current version subprober updates 
     [DEBUG]:
 
-                      
-        -h,   --help                  Show this help message for you and exit!
-        
-        -s,   --silent                Enable silent mode to suppress the display of Subprober banner and version information.
-
-        -v,   --verbose               Enable verbose mode to display error results on the console.
+        -h,    --help                  show this help message for you and exit!
+        -s,    --silent                enable silent mode to suppress the display of Subprober banner and version information.
+        -v,    --verbose               enable verbose mode to display error results on the console.
+        -nc,   --no-color              enabling the --no-color will display the output without any CLI colors
 
-        -nc,  --no-color              Enabling the --no-color will display the output without any CLI colors
 ```
 
 #### Basic Usage
 
 ```bash
 subprober -f subdomains.txt -o output.txt -tl -wc -sv  -apt -wc -ex 500 -v -o output.txt -c 20
 ```
```

