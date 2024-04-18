# Comparing `tmp/grateful_logging-0.0.8.tar.gz` & `tmp/grateful_logging-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grateful_logging-0.0.8.tar", last modified: Sat Feb  3 04:57:28 2024, max compression
+gzip compressed data, was "grateful_logging-0.0.9.tar", last modified: Sat Feb  3 09:17:42 2024, max compression
```

## Comparing `grateful_logging-0.0.8.tar` & `grateful_logging-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.715349 grateful_logging-0.0.8/grateful_logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/grateful_logging/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/assets/config-example.json
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/grateful_logging/formatter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/formatter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/formatter/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/grateful_logging/handler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/handler/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/grateful_logging/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/grateful_logging/parser/json_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/grateful_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-03 04:57:28.000000 grateful_logging-0.0.8/grateful_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-03 04:57:28.000000 grateful_logging-0.0.8/grateful_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 04:57:28.000000 grateful_logging-0.0.8/grateful_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-03 04:57:28.000000 grateful_logging-0.0.8/grateful_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 04:57:28.719349 grateful_logging-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-03 04:57:13.000000 grateful_logging-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.576924 grateful_logging-0.0.9/grateful_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/grateful_logging/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/assets/config-example.json
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/grateful_logging/formatter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/formatter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/formatter/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/grateful_logging/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/handler/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/grateful_logging/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/grateful_logging/parser/json_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/grateful_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-03 09:17:42.000000 grateful_logging-0.0.9/grateful_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-03 09:17:42.000000 grateful_logging-0.0.9/grateful_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-03 09:17:42.000000 grateful_logging-0.0.9/grateful_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-03 09:17:42.000000 grateful_logging-0.0.9/grateful_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-03 09:17:42.580924 grateful_logging-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-03 09:17:27.000000 grateful_logging-0.0.9/setup.py
```

### Comparing `grateful_logging-0.0.8/LICENSE` & `grateful_logging-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grateful_logging-0.0.8/README.md` & `grateful_logging-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `grateful_logging-0.0.8/grateful_logging/assets/config-example.json` & `grateful_logging-0.0.9/grateful_logging/assets/config-example.json`

 * *Files 10% similar despite different names*

```diff
@@ -20,84 +20,88 @@
 00000130: 6454 2548 3a25 4d3a 2553 257a 220a 2020  dT%H:%M:%S%z".  
 00000140: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
 00000150: 2022 6a73 6f6e 223a 207b 0a20 2020 2020   "json": {.     
 00000160: 2020 2020 2020 2022 2829 223a 2022 6772         "()": "gr
 00000170: 6174 6566 756c 5f6c 6f67 6769 6e67 2e66  ateful_logging.f
 00000180: 6f72 6d61 7474 6572 2e6a 736f 6e2e 4a53  ormatter.json.JS
 00000190: 4f4e 466f 726d 6174 7465 7222 2c0a 2020  ONFormatter",.  
-000001a0: 2020 2020 2020 2020 2020 2266 6d74 5f6b            "fmt_k
-000001b0: 6579 7322 3a20 7b0a 2020 2020 2020 2020  eys": {.        
-000001c0: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
-000001d0: 2022 6c65 7665 6c6e 616d 6522 2c0a 2020   "levelname",.  
-000001e0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-000001f0: 6573 7361 6765 223a 2022 6d65 7373 6167  essage": "messag
-00000200: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00000210: 2020 2020 2274 696d 6573 7461 6d70 223a      "timestamp":
-00000220: 2022 7469 6d65 7374 616d 7022 2c0a 2020   "timestamp",.  
-00000230: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00000240: 6f67 6765 7222 3a20 226e 616d 6522 2c0a  ogger": "name",.
-00000250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000260: 226d 6f64 756c 6522 3a20 226d 6f64 756c  "module": "modul
-00000270: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00000280: 2020 2020 2266 756e 6374 696f 6e22 3a20      "function": 
-00000290: 2266 756e 634e 616d 6522 2c0a 2020 2020  "funcName",.    
-000002a0: 2020 2020 2020 2020 2020 2020 226c 696e              "lin
-000002b0: 6522 3a20 226c 696e 656e 6f22 2c0a 2020  e": "lineno",.  
-000002c0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000002d0: 6872 6561 645f 6e61 6d65 223a 2022 7468  hread_name": "th
-000002e0: 7265 6164 4e61 6d65 220a 2020 2020 2020  readName".      
-000002f0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00000300: 7d0a 2020 2020 7d2c 0a20 2020 2022 6861  }.    },.    "ha
-00000310: 6e64 6c65 7273 223a 207b 0a20 2020 2020  ndlers": {.     
-00000320: 2020 2022 6166 696c 6522 3a20 7b0a 2020     "afile": {.  
-00000330: 2020 2020 2020 2020 2020 2263 6c61 7373            "class
-00000340: 223a 2022 6c6f 6767 696e 672e 6861 6e64  ": "logging.hand
-00000350: 6c65 7273 2e52 6f74 6174 696e 6746 696c  lers.RotatingFil
-00000360: 6548 616e 646c 6572 222c 0a20 2020 2020  eHandler",.     
-00000370: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
-00000380: 2244 4542 5547 222c 0a20 2020 2020 2020  "DEBUG",.       
-00000390: 2020 2020 2022 666f 726d 6174 7465 7222       "formatter"
-000003a0: 3a20 226a 736f 6e22 2c0a 2020 2020 2020  : "json",.      
-000003b0: 2020 2020 2020 2266 696c 656e 616d 6522        "filename"
-000003c0: 3a20 226c 6f67 732e 6c6f 672e 6a73 6f6e  : "logs.log.json
-000003d0: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-000003e0: 226d 6178 4279 7465 7322 3a20 3130 3030  "maxBytes": 1000
-000003f0: 302c 0a20 2020 2020 2020 2020 2020 2022  0,.            "
-00000400: 6261 636b 7570 436f 756e 7422 3a20 330a  backupCount": 3.
-00000410: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00000420: 2020 2022 6173 7464 6f75 7422 3a20 7b0a     "astdout": {.
-00000430: 2020 2020 2020 2020 2020 2020 2263 6c61              "cla
-00000440: 7373 223a 2022 6c6f 6767 696e 672e 5374  ss": "logging.St
-00000450: 7265 616d 4861 6e64 6c65 7222 2c0a 2020  reamHandler",.  
-00000460: 2020 2020 2020 2020 2020 226c 6576 656c            "level
-00000470: 223a 2022 5741 524e 494e 4722 2c0a 2020  ": "WARNING",.  
-00000480: 2020 2020 2020 2020 2020 2266 6f72 6d61            "forma
-00000490: 7474 6572 223a 2022 7369 6d70 6c65 222c  tter": "simple",
-000004a0: 0a20 2020 2020 2020 2020 2020 2022 7374  .            "st
-000004b0: 7265 616d 223a 2022 6578 743a 2f2f 7379  ream": "ext://sy
-000004c0: 732e 7374 646f 7574 220a 2020 2020 2020  s.stdout".      
-000004d0: 2020 7d2c 0a20 2020 2020 2020 2022 7175    },.        "qu
-000004e0: 6575 655f 6861 6e64 6c65 7222 3a20 7b0a  eue_handler": {.
-000004f0: 2020 2020 2020 2020 2020 2020 2228 2922              "()"
-00000500: 3a20 2267 7261 7465 6675 6c5f 6c6f 6767  : "grateful_logg
-00000510: 696e 672e 6861 6e64 6c65 722e 7175 6575  ing.handler.queu
-00000520: 652e 5175 6575 6548 616e 646c 6572 222c  e.QueueHandler",
-00000530: 0a20 2020 2020 2020 2020 2020 2022 6861  .            "ha
-00000540: 6e64 6c65 7273 223a 205b 0a20 2020 2020  ndlers": [.     
-00000550: 2020 2020 2020 2020 2020 2022 6166 696c             "afil
-00000560: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
-00000570: 2020 2020 2261 7374 646f 7574 220a 2020      "astdout".  
-00000580: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00000590: 2020 2020 2020 2020 2022 7265 7370 6563           "respec
-000005a0: 745f 6861 6e64 6c65 725f 6c65 7665 6c22  t_handler_level"
-000005b0: 3a20 7472 7565 0a20 2020 2020 2020 207d  : true.        }
-000005c0: 0a20 2020 207d 2c0a 2020 2020 226c 6f67  .    },.    "log
-000005d0: 6765 7273 223a 207b 0a20 2020 2020 2020  gers": {.       
-000005e0: 2022 726f 6f74 223a 207b 0a20 2020 2020   "root": {.     
-000005f0: 2020 2020 2020 2022 6c65 7665 6c22 3a20         "level": 
-00000600: 2244 4542 5547 222c 0a20 2020 2020 2020  "DEBUG",.       
-00000610: 2020 2020 2022 6861 6e64 6c65 7273 223a       "handlers":
-00000620: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00000630: 2020 2022 7175 6575 655f 6861 6e64 6c65     "queue_handle
-00000640: 7222 0a20 2020 2020 2020 2020 2020 205d  r".            ]
-00000650: 0a20 2020 2020 2020 207d 0a20 2020 207d  .        }.    }
-00000660: 0a7d 0a                                  .}.
+000001a0: 2020 2020 2020 2020 2020 2269 6e63 6c75            "inclu
+000001b0: 6465 5f6b 6579 7322 3a20 7b0a 2020 2020  de_keys": {.    
+000001c0: 2020 2020 2020 2020 2020 2020 226c 6576              "lev
+000001d0: 656c 223a 2022 6c65 7665 6c6e 616d 6522  el": "levelname"
+000001e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000001f0: 2020 226d 6573 7361 6765 223a 2022 6d65    "message": "me
+00000200: 7373 6167 6522 2c0a 2020 2020 2020 2020  ssage",.        
+00000210: 2020 2020 2020 2020 2274 696d 6573 7461          "timesta
+00000220: 6d70 223a 2022 7469 6d65 7374 616d 7022  mp": "timestamp"
+00000230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000240: 2020 226c 6f67 6765 7222 3a20 226e 616d    "logger": "nam
+00000250: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00000260: 2020 2020 226d 6f64 756c 6522 3a20 226d      "module": "m
+00000270: 6f64 756c 6522 2c0a 2020 2020 2020 2020  odule",.        
+00000280: 2020 2020 2020 2020 2266 756e 6374 696f          "functio
+00000290: 6e22 3a20 2266 756e 634e 616d 6522 2c0a  n": "funcName",.
+000002a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002b0: 226c 696e 6522 3a20 226c 696e 656e 6f22  "line": "lineno"
+000002c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000002d0: 2020 2274 6872 6561 645f 6e61 6d65 223a    "thread_name":
+000002e0: 2022 7468 7265 6164 4e61 6d65 220a 2020   "threadName".  
+000002f0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00000300: 2020 2020 2020 2020 2022 616c 7761 7973           "always
+00000310: 5f6b 6579 7322 3a20 5b0a 2020 2020 2020  _keys": [.      
+00000320: 2020 2020 2020 2020 2020 226d 6573 7361            "messa
+00000330: 6765 222c 0a20 2020 2020 2020 2020 2020  ge",.           
+00000340: 205d 0a20 2020 2020 2020 207d 0a20 2020   ].        }.   
+00000350: 207d 2c0a 2020 2020 2268 616e 646c 6572   },.    "handler
+00000360: 7322 3a20 7b0a 2020 2020 2020 2020 2261  s": {.        "a
+00000370: 6669 6c65 223a 207b 0a20 2020 2020 2020  file": {.       
+00000380: 2020 2020 2022 636c 6173 7322 3a20 226c       "class": "l
+00000390: 6f67 6769 6e67 2e68 616e 646c 6572 732e  ogging.handlers.
+000003a0: 526f 7461 7469 6e67 4669 6c65 4861 6e64  RotatingFileHand
+000003b0: 6c65 7222 2c0a 2020 2020 2020 2020 2020  ler",.          
+000003c0: 2020 226c 6576 656c 223a 2022 4445 4255    "level": "DEBU
+000003d0: 4722 2c0a 2020 2020 2020 2020 2020 2020  G",.            
+000003e0: 2266 6f72 6d61 7474 6572 223a 2022 6a73  "formatter": "js
+000003f0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
+00000400: 2022 6669 6c65 6e61 6d65 223a 2022 6c6f   "filename": "lo
+00000410: 6773 2e6c 6f67 2e6a 736f 6e6c 222c 0a20  gs.log.jsonl",. 
+00000420: 2020 2020 2020 2020 2020 2022 6d61 7842             "maxB
+00000430: 7974 6573 223a 2031 3030 3030 2c0a 2020  ytes": 10000,.  
+00000440: 2020 2020 2020 2020 2020 2262 6163 6b75            "backu
+00000450: 7043 6f75 6e74 223a 2033 0a20 2020 2020  pCount": 3.     
+00000460: 2020 207d 2c0a 2020 2020 2020 2020 2261     },.        "a
+00000470: 7374 646f 7574 223a 207b 0a20 2020 2020  stdout": {.     
+00000480: 2020 2020 2020 2022 636c 6173 7322 3a20         "class": 
+00000490: 226c 6f67 6769 6e67 2e53 7472 6561 6d48  "logging.StreamH
+000004a0: 616e 646c 6572 222c 0a20 2020 2020 2020  andler",.       
+000004b0: 2020 2020 2022 6c65 7665 6c22 3a20 2257       "level": "W
+000004c0: 4152 4e49 4e47 222c 0a20 2020 2020 2020  ARNING",.       
+000004d0: 2020 2020 2022 666f 726d 6174 7465 7222       "formatter"
+000004e0: 3a20 2273 696d 706c 6522 2c0a 2020 2020  : "simple",.    
+000004f0: 2020 2020 2020 2020 2273 7472 6561 6d22          "stream"
+00000500: 3a20 2265 7874 3a2f 2f73 7973 2e73 7464  : "ext://sys.std
+00000510: 6f75 7422 0a20 2020 2020 2020 207d 2c0a  out".        },.
+00000520: 2020 2020 2020 2020 2271 7565 7565 5f68          "queue_h
+00000530: 616e 646c 6572 223a 207b 0a20 2020 2020  andler": {.     
+00000540: 2020 2020 2020 2022 2829 223a 2022 6772         "()": "gr
+00000550: 6174 6566 756c 5f6c 6f67 6769 6e67 2e68  ateful_logging.h
+00000560: 616e 646c 6572 2e71 7565 7565 2e51 7565  andler.queue.Que
+00000570: 7565 4861 6e64 6c65 7222 2c0a 2020 2020  ueHandler",.    
+00000580: 2020 2020 2020 2020 2268 616e 646c 6572          "handler
+00000590: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
+000005a0: 2020 2020 2020 2261 6669 6c65 222c 0a20        "afile",. 
+000005b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000005c0: 6173 7464 6f75 7422 0a20 2020 2020 2020  astdout".       
+000005d0: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+000005e0: 2020 2020 2272 6573 7065 6374 5f68 616e      "respect_han
+000005f0: 646c 6572 5f6c 6576 656c 223a 2074 7275  dler_level": tru
+00000600: 650a 2020 2020 2020 2020 7d0a 2020 2020  e.        }.    
+00000610: 7d2c 0a20 2020 2022 6c6f 6767 6572 7322  },.    "loggers"
+00000620: 3a20 7b0a 2020 2020 2020 2020 2272 6f6f  : {.        "roo
+00000630: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
+00000640: 2020 226c 6576 656c 223a 2022 4445 4255    "level": "DEBU
+00000650: 4722 2c0a 2020 2020 2020 2020 2020 2020  G",.            
+00000660: 2268 616e 646c 6572 7322 3a20 5b0a 2020  "handlers": [.  
+00000670: 2020 2020 2020 2020 2020 2020 2020 2271                "q
+00000680: 7565 7565 5f68 616e 646c 6572 220a 2020  ueue_handler".  
+00000690: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+000006a0: 2020 2020 7d0a 2020 2020 7d0a 7d0a           }.    }.}.
```

### Comparing `grateful_logging-0.0.8/grateful_logging/cli.py` & `grateful_logging-0.0.9/grateful_logging/cli.py`

 * *Files identical despite different names*

### Comparing `grateful_logging-0.0.8/grateful_logging/configure.py` & `grateful_logging-0.0.9/grateful_logging/configure.py`

 * *Files identical despite different names*

### Comparing `grateful_logging-0.0.8/grateful_logging/handler/queue.py` & `grateful_logging-0.0.9/grateful_logging/handler/queue.py`

 * *Files identical despite different names*

### Comparing `grateful_logging-0.0.8/grateful_logging.egg-info/SOURCES.txt` & `grateful_logging-0.0.9/grateful_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grateful_logging-0.0.8/setup.py` & `grateful_logging-0.0.9/setup.py`

 * *Files identical despite different names*

