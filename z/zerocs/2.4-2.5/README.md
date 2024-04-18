# Comparing `tmp/zerocs-2.4.tar.gz` & `tmp/zerocs-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocs-2.4.tar", last modified: Sun Mar 24 03:06:52 2024, max compression
+gzip compressed data, was "zerocs-2.5.tar", last modified: Thu Apr 18 02:24:32 2024, max compression
```

## Comparing `zerocs-2.4.tar` & `zerocs-2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.156836 zerocs-2.4/
--rw-rw-rw-   0        0        0     1144 2024-03-24 02:59:20.000000 zerocs-2.4/LICENSE
--rw-rw-rw-   0        0        0    10214 2024-03-24 03:06:52.153429 zerocs-2.4/PKG-INFO
--rw-rw-rw-   0        0        0     9559 2024-03-24 02:59:20.000000 zerocs-2.4/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-24 03:06:52.156836 zerocs-2.4/setup.cfg
--rw-rw-rw-   0        0        0      883 2024-03-24 03:06:48.000000 zerocs-2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.115499 zerocs-2.4/zerocs/
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.139475 zerocs-2.4/zerocs/__base__/
--rw-rw-rw-   0        0        0      352 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/__base__/__init__.py
--rw-rw-rw-   0        0        0     1356 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.139475 zerocs-2.4/zerocs/build/
--rw-rw-rw-   0        0        0      609 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/build/__init__.py
--rw-rw-rw-   0        0        0     2954 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/build/build.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.140863 zerocs-2.4/zerocs/common/
--rw-rw-rw-   0        0        0      166 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/common/__init__.py
--rw-rw-rw-   0        0        0      244 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/common/common.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.142403 zerocs-2.4/zerocs/config/
--rw-rw-rw-   0        0        0      473 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/config/__init__.py
--rw-rw-rw-   0        0        0      450 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/config/config.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.143407 zerocs-2.4/zerocs/database/
--rw-rw-rw-   0        0        0     2781 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/database/__init__.py
--rw-rw-rw-   0        0        0     8046 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/database/database.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.145698 zerocs-2.4/zerocs/fork/
--rw-rw-rw-   0        0        0      495 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/fork/__init__.py
--rw-rw-rw-   0        0        0     4740 2024-03-24 03:03:03.000000 zerocs-2.4/zerocs/fork/fork.py
--rw-rw-rw-   0        0        0     1218 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/fork/fork_logger.py
--rw-rw-rw-   0        0        0     1285 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/fork/fork_service.py
--rw-rw-rw-   0        0        0     5178 2024-03-24 03:03:03.000000 zerocs-2.4/zerocs/fork/fork_work.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.147293 zerocs-2.4/zerocs/interface/
--rw-rw-rw-   0        0        0     2209 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/interface/__init__.py
--rw-rw-rw-   0        0        0     3207 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/interface/interface.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.147822 zerocs-2.4/zerocs/logger/
--rw-rw-rw-   0        0        0      938 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/logger/__init__.py
--rw-rw-rw-   0        0        0     2303 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.149179 zerocs-2.4/zerocs/main/
--rw-rw-rw-   0        0        0      332 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/main/__init__.py
--rw-rw-rw-   0        0        0      700 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/main/main.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.150256 zerocs-2.4/zerocs/observer/
--rw-rw-rw-   0        0        0      741 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/observer/__init__.py
--rw-rw-rw-   0        0        0      719 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/observer/observer.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.151337 zerocs-2.4/zerocs/rabbit/
--rw-rw-rw-   0        0        0      686 2024-03-24 03:03:03.000000 zerocs-2.4/zerocs/rabbit/__init__.py
--rw-rw-rw-   0        0        0     1903 2024-03-24 03:03:03.000000 zerocs-2.4/zerocs/rabbit/rabbit.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.152333 zerocs-2.4/zerocs/services/
--rw-rw-rw-   0        0        0      606 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/services/__init__.py
--rw-rw-rw-   0        0        0     1140 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/services/services.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.153429 zerocs-2.4/zerocs/utils/
--rw-rw-rw-   0        0        0     1600 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/utils/__init__.py
--rw-rw-rw-   0        0        0     4164 2024-03-24 03:03:03.000000 zerocs-2.4/zerocs/utils/rpc_proxy.py
--rw-rw-rw-   0        0        0     5934 2024-03-24 03:03:03.000000 zerocs-2.4/zerocs/utils/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.153429 zerocs-2.4/zerocs/verification/
--rw-rw-rw-   0        0        0      232 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/verification/__init__.py
--rw-rw-rw-   0        0        0      451 2024-03-24 02:59:20.000000 zerocs-2.4/zerocs/verification/verification.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:06:52.153429 zerocs-2.4/zerocs.egg-info/
--rw-rw-rw-   0        0        0    10214 2024-03-24 03:06:52.000000 zerocs-2.4/zerocs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1006 2024-03-24 03:06:52.000000 zerocs-2.4/zerocs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 03:06:52.000000 zerocs-2.4/zerocs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-03-24 03:06:52.000000 zerocs-2.4/zerocs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-24 03:06:52.000000 zerocs-2.4/zerocs.egg-info/top_level.txt
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1144 2024-04-18 02:09:46.000000 zerocs-2.5/LICENSE
+-rw-r--r--   0 yanping   (1001) yanping   (1001)     9947 2024-04-18 02:24:32.812584 zerocs-2.5/PKG-INFO
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     9559 2024-04-18 02:09:46.000000 zerocs-2.5/README.rst
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)       38 2024-04-18 02:24:32.812584 zerocs-2.5/setup.cfg
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      883 2024-04-18 02:12:17.000000 zerocs-2.5/setup.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/__base__/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      352 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/__base__/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1356 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/__init__.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/build/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      601 2024-04-18 02:19:19.000000 zerocs-2.5/zerocs/build/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     3122 2024-04-18 02:19:19.000000 zerocs-2.5/zerocs/build/build.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/common/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      166 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/common/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      244 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/common/common.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/config/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      473 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/config/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      450 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/config/config.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/database/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     2781 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/database/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     8046 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/database/database.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/fork/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      495 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/fork/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     4708 2024-04-18 02:19:19.000000 zerocs-2.5/zerocs/fork/fork.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1218 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/fork/fork_logger.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1285 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/fork/fork_service.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     5350 2024-04-18 02:21:35.000000 zerocs-2.5/zerocs/fork/fork_work.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/interface/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     2209 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/interface/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     3207 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/interface/interface.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/logger/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      938 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/logger/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     2303 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/logger/logger.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/main/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      332 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/main/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      700 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/main/main.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/observer/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      741 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/observer/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      719 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/observer/observer.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/rabbit/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      686 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/rabbit/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1903 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/rabbit/rabbit.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/services/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      606 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/services/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1142 2024-04-18 02:19:19.000000 zerocs-2.5/zerocs/services/services.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/utils/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1600 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/utils/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     4164 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/utils/rpc_proxy.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     5934 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/utils/utils.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs/verification/
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      232 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/verification/__init__.py
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)      451 2024-04-18 02:09:46.000000 zerocs-2.5/zerocs/verification/verification.py
+drwxrwxr-x   0 yanping   (1001) yanping   (1001)        0 2024-04-18 02:24:32.812584 zerocs-2.5/zerocs.egg-info/
+-rw-r--r--   0 yanping   (1001) yanping   (1001)     9947 2024-04-18 02:24:32.000000 zerocs-2.5/zerocs.egg-info/PKG-INFO
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)     1006 2024-04-18 02:24:32.000000 zerocs-2.5/zerocs.egg-info/SOURCES.txt
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)        1 2024-04-18 02:24:32.000000 zerocs-2.5/zerocs.egg-info/dependency_links.txt
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)       31 2024-04-18 02:24:32.000000 zerocs-2.5/zerocs.egg-info/requires.txt
+-rw-rw-r--   0 yanping   (1001) yanping   (1001)        7 2024-04-18 02:24:32.000000 zerocs-2.5/zerocs.egg-info/top_level.txt
```

### Comparing `zerocs-2.4/LICENSE` & `zerocs-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/PKG-INFO` & `zerocs-2.5/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: zerocs
-Version: 2.4
-Summary: zerocs
-Home-page: https://gitee.com/ZYPH/zerocs
-Author: YanPing
-Author-email: zyphhxx@foxmail.com
-Maintainer: YanPing
-Maintainer-email: zyphhxx@foxmail.com
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-License-File: LICENSE
-Requires-Dist: nameko
-Requires-Dist: pika
-Requires-Dist: pytz
-Requires-Dist: pymongo
-Requires-Dist: kombu
-
 zerocs Description Document
 ============================
 
 zerocs: zero config service
 +++++++++++++++++++++++++++
 
 1. introduction
@@ -260,8 +237,8 @@
     An unenforceable partial declaration does not constitute a waiver of our
     right to enforce the declaration.
 
 +   This project has the right to make unilateral changes to the terms and attachments of this statement at any time,
     and publish them through message push, webpage announcement, and other means. Once published,
     it will automatically take effect without the need for separate notice;
     If you continue to use this statement after the announcement of changes,
-    it means that you have fully read, understood, and accepted the revised statement.
+    it means that you have fully read, understood, and accepted the revised statement.
```

### Comparing `zerocs-2.4/README.rst` & `zerocs-2.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,244 +1,267 @@
-zerocs Description Document
-============================
-
-zerocs: zero config service
-+++++++++++++++++++++++++++
-
-1. introduction
-
-    1. zerocs is a distributed task framework with extremely simple configuration.
-    Enable users to quickly build distributed task systems with minimal
-    configuration and learning costs
-
-    2. The framework has functions such as service management, work management,
-    and task management, which can meet most usage scenarios
-
-    3. Note: Version 1.9 is not compatible with version 1.3.
-    It is recommended to upgrade to version 1.9 and above
-
-    4. Decentralization starting from version 1.9,
-    no longer distinguishing between master and slave nodes
-
-2. start using
-
-    1. Please install RabbitMQ before use,
-    rabbitmq official website : https://www.rabbitmq.com,
-    It is recommended to use Docker installation during testing::
-
-            docker run -d --hostname my-rabbit --name rabbit \
-            -e RABBITMQ_DEFAULT_USER=user \
-            -e RABBITMQ_DEFAULT_PASS=password \
-            -p 15672:15672 -p 5672:5672 rabbitmq:management
-
-    2. Please install MongoDB before use,
-    Installation steps reference : https://docs.mongoing.com/install-mongodb
-
-    3. To use the framework, it is very simple, just refer to zerocs
-    in the first line of your startup script
-    Please create the corresponding directory and files before starting::
-
-          ├─logs //log directory
-          ├─service_list //Directory of microservice codes
-          │  │─test
-          │  │  ├─test.py
-          │  │  ├─test1.py
-          ├─main.py  //main
-          └─zerocs_test.py //Test Script
-
-    4. main.py ::
-
-        # -*- encoding: utf-8 -*-
-        # Master startup file, please refer to zerocs first
-        # Flask API is not mandatory and can be connected to other management systems
-
-        import os
-        import logging
-        from flask_cors import CORS
-        from flask import Flask, request
-
-        from zerocs import Main, Interface
-        from service_list.test import test, test1
-
-        app = Flask(__name__)
-        CORS(app, supports_credentials=True)
-
-        logging.basicConfig(level=logging.ERROR)
-        script_path = os.path.dirname(os.path.realpath(__file__))
-
-
-        class Master:
-
-            def __init__(self):
-                config = {
-                    "PATH": script_path,
-                    "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
-                    "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
-                }
-                Main.run_master(
-                    configs=config,
-                    services=[test, test1]
-                )
-
-            @staticmethod
-            def get_service_list(query: dict, field: dict, limit: int, page: int) -> dict:
-                count, data = Interface.get_service_list(query, field, limit, page)
-                return {"count": count, "data": data}
-
-            @staticmethod
-            def stop_tasks(task_id: str):
-                Interface.insert_stop_tasks(task_id)
-
-            @staticmethod
-            def remote_call(service_name: str, service_ip: str, method_name: str, **params):
-                rpc_proxy = Interface.remote_call_by_name_and_ip(service_name, service_ip)
-                return rpc_proxy.remote_call(service_name, method_name, **params)
-
-            @staticmethod
-            def send_message(service_name: str, message: dict):
-                if 'task_id' in message:
-                    Interface.send_message(service_name, message)
-
-            @staticmethod
-            def restart_service(service_name: str):
-                Interface.restart_service(service_name)
-
-
-        @app.route("/")
-        def index():
-            data = _main.get_service_list({}, {"_id": 0}, 10, 0)
-            return data
-
-
-        @app.route("/get_service_list")
-        def get_service_list():
-            request_json = request.get_json()
-            query = request_json['query']
-            field = request_json['field']
-            limit = request_json['limit']
-            page = request_json['page']
-
-            data = _main.get_service_list(query, field, limit, page)
-            return data
-
-
-        @app.route("/restart_service")
-        def restart_service():
-            request_json = request.get_json()
-            service_name = request_json['service_name']
-            _main.restart_service(service_name)
-            return {"code": 0}
-
-
-        if __name__ == '__main__':
-            _main = Master()
-            app.run(host='0.0.0.0', port=5002)
-
-    5. test.py ::
-
-        import time
-
-        class RpcFunction:
-            """
-            Class Name Not modifiable, Define RPC functions
-            """
-            service_name = 'test'
-
-            def get_service_name(self, xxx):
-                return {"service_name": self.service_name, "param": xxx}
-
-
-        class WorkFunction:
-            """
-            Class Name Not modifiable, Work Code
-            """
-
-            def __init__(self, task_data):
-                """
-                :param task_data: Task data JSON format
-                """
-                logger = self.__getattribute__('logger')
-                rpc_proxy = self.__getattribute__('rpc_proxy')
-
-                """
-                Call the rpc interface
-
-                data = rpc_proxy.remote_call(service_name, method_name, **params)
-                """
-
-    6. zerocs_test.py ::
-
-        # -*- encoding: utf-8 -*-
-        import os
-
-        from zerocs import Interface
-
-        script_path = os.path.dirname(os.path.realpath(__file__))
-
-        if __name__ == '__main__':
-            config = {
-                "PATH": os.path.join(script_path, 'logs'),
-                "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
-                "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
-            }
-
-            # initialization
-            Interface.init_proxy(config)
-
-            # Stop the task
-            Interface.insert_stop_tasks('1001')
-
-            # Call the RPC interface
-            obj = Interface.remote_call_by_name_and_ip('test', '192.168.0.101')
-            print(obj.remote_call('test' ,'get_service_name', param='1111111111'))
-
-            # Issue task message
-            Interface.send_message('test', {"task_id": "100", "msg": "xxxxxxxxxxxxxxxx"})
-
-
-A distributed task scheduling system was completed in just a few steps
-======================================================================
-
-Disclaimers
-================
-
-
-+   Before using the zerocs framework, please carefully read and fully understand this statement.
-    You can choose not to use the zerocs framework, but once you use the zerocs framework,
-    Your usage behavior is deemed to be recognition and acceptance of the entire content of this statement.
-
-+   You promise to use the zerocs framework in a legal and reasonable manner,
-    Do not use the zerocs board framework to engage in any illegal or malicious behavior that infringes
-    on the legitimate interests of others,
-    We will not apply the zerocs framework to any platform that violates Chinese laws and regulations.
-
-+   Any accident, negligence, contract damage, defamation
-    This project does not assume any legal responsibility for copyright or intellectual property
-    infringement and any losses caused (including but not limited to direct,
-    indirect, incidental or derivative losses).
-
-+   The user clearly and agrees to all the contents listed in the terms of this statement,
-    The potential risks and related consequences of using the zerocs framework will be entirely borne by the user,
-    and this project will not bear any legal responsibility.
-
-+   After reading this disclaimer, any unit or individual should obtain the MIT Open Source License
-    Conduct legitimate publishing, dissemination, and use of the zerocs framework within the permitted scope,
-    If the breach of this disclaimer clause or the violation of laws and regulations results in legal
-    liability (including but not limited to civil compensation and criminal liability),
-    the defaulter shall bear the responsibility on their own.
-
-+   The author owns intellectual property rights (including but not limited to trademark rights, patents, Copyrights,
-    trade secrets, etc.) of zerocs framework, and the above products are protected by relevant laws and regulations
-
-+   No entity or individual shall apply for intellectual property rights related to
-    the zerocs Framework itself without the written authorization of the Author.
-
-+   If any part of this statement is deemed invalid or unenforceable,
-    the remaining parts shall remain in full force and effect.
-    An unenforceable partial declaration does not constitute a waiver of our
-    right to enforce the declaration.
-
-+   This project has the right to make unilateral changes to the terms and attachments of this statement at any time,
-    and publish them through message push, webpage announcement, and other means. Once published,
-    it will automatically take effect without the need for separate notice;
-    If you continue to use this statement after the announcement of changes,
-    it means that you have fully read, understood, and accepted the revised statement.
+Metadata-Version: 2.1
+Name: zerocs
+Version: 2.5
+Summary: zerocs
+Home-page: https://gitee.com/ZYPH/zerocs
+Author: YanPing
+Author-email: zyphhxx@foxmail.com
+Maintainer: YanPing
+Maintainer-email: zyphhxx@foxmail.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+License-File: LICENSE
+Requires-Dist: nameko
+Requires-Dist: pika
+Requires-Dist: pytz
+Requires-Dist: pymongo
+Requires-Dist: kombu
+
+zerocs Description Document
+============================
+
+zerocs: zero config service
++++++++++++++++++++++++++++
+
+1. introduction
+
+    1. zerocs is a distributed task framework with extremely simple configuration.
+    Enable users to quickly build distributed task systems with minimal
+    configuration and learning costs
+
+    2. The framework has functions such as service management, work management,
+    and task management, which can meet most usage scenarios
+
+    3. Note: Version 1.9 is not compatible with version 1.3.
+    It is recommended to upgrade to version 1.9 and above
+
+    4. Decentralization starting from version 1.9,
+    no longer distinguishing between master and slave nodes
+
+2. start using
+
+    1. Please install RabbitMQ before use,
+    rabbitmq official website : https://www.rabbitmq.com,
+    It is recommended to use Docker installation during testing::
+
+            docker run -d --hostname my-rabbit --name rabbit \
+            -e RABBITMQ_DEFAULT_USER=user \
+            -e RABBITMQ_DEFAULT_PASS=password \
+            -p 15672:15672 -p 5672:5672 rabbitmq:management
+
+    2. Please install MongoDB before use,
+    Installation steps reference : https://docs.mongoing.com/install-mongodb
+
+    3. To use the framework, it is very simple, just refer to zerocs
+    in the first line of your startup script
+    Please create the corresponding directory and files before starting::
+
+          ├─logs //log directory
+          ├─service_list //Directory of microservice codes
+          │  │─test
+          │  │  ├─test.py
+          │  │  ├─test1.py
+          ├─main.py  //main
+          └─zerocs_test.py //Test Script
+
+    4. main.py ::
+
+        # -*- encoding: utf-8 -*-
+        # Master startup file, please refer to zerocs first
+        # Flask API is not mandatory and can be connected to other management systems
+
+        import os
+        import logging
+        from flask_cors import CORS
+        from flask import Flask, request
+
+        from zerocs import Main, Interface
+        from service_list.test import test, test1
+
+        app = Flask(__name__)
+        CORS(app, supports_credentials=True)
+
+        logging.basicConfig(level=logging.ERROR)
+        script_path = os.path.dirname(os.path.realpath(__file__))
+
+
+        class Master:
+
+            def __init__(self):
+                config = {
+                    "PATH": script_path,
+                    "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
+                    "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
+                }
+                Main.run_master(
+                    configs=config,
+                    services=[test, test1]
+                )
+
+            @staticmethod
+            def get_service_list(query: dict, field: dict, limit: int, page: int) -> dict:
+                count, data = Interface.get_service_list(query, field, limit, page)
+                return {"count": count, "data": data}
+
+            @staticmethod
+            def stop_tasks(task_id: str):
+                Interface.insert_stop_tasks(task_id)
+
+            @staticmethod
+            def remote_call(service_name: str, service_ip: str, method_name: str, **params):
+                rpc_proxy = Interface.remote_call_by_name_and_ip(service_name, service_ip)
+                return rpc_proxy.remote_call(service_name, method_name, **params)
+
+            @staticmethod
+            def send_message(service_name: str, message: dict):
+                if 'task_id' in message:
+                    Interface.send_message(service_name, message)
+
+            @staticmethod
+            def restart_service(service_name: str):
+                Interface.restart_service(service_name)
+
+
+        @app.route("/")
+        def index():
+            data = _main.get_service_list({}, {"_id": 0}, 10, 0)
+            return data
+
+
+        @app.route("/get_service_list")
+        def get_service_list():
+            request_json = request.get_json()
+            query = request_json['query']
+            field = request_json['field']
+            limit = request_json['limit']
+            page = request_json['page']
+
+            data = _main.get_service_list(query, field, limit, page)
+            return data
+
+
+        @app.route("/restart_service")
+        def restart_service():
+            request_json = request.get_json()
+            service_name = request_json['service_name']
+            _main.restart_service(service_name)
+            return {"code": 0}
+
+
+        if __name__ == '__main__':
+            _main = Master()
+            app.run(host='0.0.0.0', port=5002)
+
+    5. test.py ::
+
+        import time
+
+        class RpcFunction:
+            """
+            Class Name Not modifiable, Define RPC functions
+            """
+            service_name = 'test'
+
+            def get_service_name(self, xxx):
+                return {"service_name": self.service_name, "param": xxx}
+
+
+        class WorkFunction:
+            """
+            Class Name Not modifiable, Work Code
+            """
+
+            def __init__(self, task_data):
+                """
+                :param task_data: Task data JSON format
+                """
+                logger = self.__getattribute__('logger')
+                rpc_proxy = self.__getattribute__('rpc_proxy')
+
+                """
+                Call the rpc interface
+
+                data = rpc_proxy.remote_call(service_name, method_name, **params)
+                """
+
+    6. zerocs_test.py ::
+
+        # -*- encoding: utf-8 -*-
+        import os
+
+        from zerocs import Interface
+
+        script_path = os.path.dirname(os.path.realpath(__file__))
+
+        if __name__ == '__main__':
+            config = {
+                "PATH": os.path.join(script_path, 'logs'),
+                "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
+                "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
+            }
+
+            # initialization
+            Interface.init_proxy(config)
+
+            # Stop the task
+            Interface.insert_stop_tasks('1001')
+
+            # Call the RPC interface
+            obj = Interface.remote_call_by_name_and_ip('test', '192.168.0.101')
+            print(obj.remote_call('test' ,'get_service_name', param='1111111111'))
+
+            # Issue task message
+            Interface.send_message('test', {"task_id": "100", "msg": "xxxxxxxxxxxxxxxx"})
+
+
+A distributed task scheduling system was completed in just a few steps
+======================================================================
+
+Disclaimers
+================
+
+
++   Before using the zerocs framework, please carefully read and fully understand this statement.
+    You can choose not to use the zerocs framework, but once you use the zerocs framework,
+    Your usage behavior is deemed to be recognition and acceptance of the entire content of this statement.
+
++   You promise to use the zerocs framework in a legal and reasonable manner,
+    Do not use the zerocs board framework to engage in any illegal or malicious behavior that infringes
+    on the legitimate interests of others,
+    We will not apply the zerocs framework to any platform that violates Chinese laws and regulations.
+
++   Any accident, negligence, contract damage, defamation
+    This project does not assume any legal responsibility for copyright or intellectual property
+    infringement and any losses caused (including but not limited to direct,
+    indirect, incidental or derivative losses).
+
++   The user clearly and agrees to all the contents listed in the terms of this statement,
+    The potential risks and related consequences of using the zerocs framework will be entirely borne by the user,
+    and this project will not bear any legal responsibility.
+
++   After reading this disclaimer, any unit or individual should obtain the MIT Open Source License
+    Conduct legitimate publishing, dissemination, and use of the zerocs framework within the permitted scope,
+    If the breach of this disclaimer clause or the violation of laws and regulations results in legal
+    liability (including but not limited to civil compensation and criminal liability),
+    the defaulter shall bear the responsibility on their own.
+
++   The author owns intellectual property rights (including but not limited to trademark rights, patents, Copyrights,
+    trade secrets, etc.) of zerocs framework, and the above products are protected by relevant laws and regulations
+
++   No entity or individual shall apply for intellectual property rights related to
+    the zerocs Framework itself without the written authorization of the Author.
+
++   If any part of this statement is deemed invalid or unenforceable,
+    the remaining parts shall remain in full force and effect.
+    An unenforceable partial declaration does not constitute a waiver of our
+    right to enforce the declaration.
+
++   This project has the right to make unilateral changes to the terms and attachments of this statement at any time,
+    and publish them through message push, webpage announcement, and other means. Once published,
+    it will automatically take effect without the need for separate notice;
+    If you continue to use this statement after the announcement of changes,
+    it means that you have fully read, understood, and accepted the revised statement.
```

### Comparing `zerocs-2.4/setup.py` & `zerocs-2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='zerocs',
-    version='2.4',
+    version='2.5',
     description="zerocs",
     long_description=open('README.rst', encoding='utf-8').read(),
     # long_description_content_type='text/plain',
     include_package_data=True,
     author='YanPing',
     author_email='zyphhxx@foxmail.com',
     maintainer='YanPing',
```

### Comparing `zerocs-2.4/zerocs/__init__.py` & `zerocs-2.5/zerocs/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/build/__init__.py` & `zerocs-2.5/zerocs/build/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     @staticmethod
     def gen_service_id(name: str) -> str:
         """
         gen service id
         """
 
     @staticmethod
-    def build(func: object, rabbitmq_config: str) -> object:
+    def build(func: object, config: dict) -> object:
         """
         build
         """
 
 
 class WorkBuild(BaseSetattr):
```

### Comparing `zerocs-2.4/zerocs/build/build.py` & `zerocs-2.5/zerocs/build/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- encoding: utf-8 -*-
 import inspect
 import logging
+import os
 
 from nameko.rpc import rpc
 from zerocs.utils import Utils
 from zerocs.rabbit import RabbitMq
-from zerocs.logger import AsynchronousLog
+from zerocs.logger import AsynchronousLog, Logger
 
 from zerocs.build import ServiceBuild, WorkBuild
 
 
 class DefaultFunc:
     logger = None
     service_id = None
@@ -34,15 +35,15 @@
 
     @staticmethod
     def gen_service_id(name):
         _ip = Utils.get_ipaddr()
         return Utils.get_service_id(name, _ip)
 
     @staticmethod
-    def build(func: object, rabbitmq_config: str) -> object:
+    def build(func: object, config: dict) -> object:
         _apis = {}
         build = Build(DefaultFunc)
 
         for _name in func.__dict__:
             if _name.startswith('__') is False:
                 _value = func.__dict__.get(_name)
                 if type(_value) in [type(lambda: None)]:
@@ -62,21 +63,24 @@
 
                 build.setattr(_name, func.__dict__.get(_name))
 
         name = func.__dict__.get('service_name')
         if name is None:
             logging.warning('service_name is None')
 
-        service_ip = Utils.get_ipaddr()
-        RabbitMq.rabbitmq_init(rabbitmq_config)
+        Logger.logs_path = os.path.join(config.get('PATH'), 'logs')
+        build.setattr('logger', Logger.logger(name))
+
+        # RabbitMq.rabbitmq_init(config.get('RABBITMQ_CONFIG'))
+        # build.setattr('logger', AsynchronousLog.init_asynchronous_log(name, service_ip))
 
+        service_ip = Utils.get_ipaddr()
         build.setattr('apis', _apis)
-        build.setattr('logger', AsynchronousLog.init_asynchronous_log(name, service_ip))
         build.setattr('service_ip', service_ip)
-        build.setattr('rabbitmq_config', rabbitmq_config)
+        build.setattr('rabbitmq_config', config.get('RABBITMQ_CONFIG'))
         build.setattr('service_id', ServiceBuild.gen_service_id(name))
         build.setattr('name', ServiceBuild.gen_service_id(name))
 
         return build.build
 
 
 @WorkBuild
```

### Comparing `zerocs-2.4/zerocs/database/__init__.py` & `zerocs-2.5/zerocs/database/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/database/database.py` & `zerocs-2.5/zerocs/database/database.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/fork/fork.py` & `zerocs-2.5/zerocs/fork/fork.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             subprocess.Popen(cmd, stdin=subprocess.PIPE, stderr=subprocess.PIPE, stdout=subprocess.PIPE, shell=True)
         else:
             subprocess.Popen(cmd, stdin=subprocess.PIPE, stderr=subprocess.PIPE, stdout=subprocess.PIPE, shell=True)
 
     @staticmethod
     def fork_service(service_list: list, config: dict) -> None:
         for service in service_list:
-            func = ServiceBuild.build(func=service.RpcFunction, rabbitmq_config=config.get('RABBITMQ_CONFIG'))
+            func = ServiceBuild.build(func=service.RpcFunction, config=config)
             _python = Utils.get_python_path()
             _script = os.path.join(current_directory, 'fork_service.py')
 
             _apis = func.__dict__.get('apis')
             _service_id = func.__dict__.get('service_id')
             _service_ip = func.__dict__.get('service_ip')
             _service_name = func.__dict__.get('service_name')
```

### Comparing `zerocs-2.4/zerocs/fork/fork_logger.py` & `zerocs-2.5/zerocs/fork/fork_logger.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/fork/fork_service.py` & `zerocs-2.5/zerocs/fork/fork_service.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/fork/fork_work.py` & `zerocs-2.5/zerocs/fork/fork_work.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from argparse import ArgumentParser
 
 from zerocs.config import Config
 from zerocs.build import WorkBuild
 from zerocs.rabbit import RabbitMq
 from zerocs.database import MongoDB
 from zerocs.observer import ObserverBase
-from zerocs.logger import AsynchronousLog
+from zerocs.logger import AsynchronousLog, Logger
 from zerocs.utils import ZeroProxy, Utils
 
 max_cpu_count = multiprocessing.cpu_count() - 3
 
 
 class MultiProcessWork:
 
@@ -26,21 +26,26 @@
         self.work_ip = work_ip
         self.function = function
         self.work_name = work_name
 
         MongoDB.init(config.get('MONGODB_CONFIG'))
         RabbitMq.rabbitmq_init(config.get('RABBITMQ_CONFIG'))
 
+        Logger.logs_path = os.path.join(self.config.get('PATH'), 'logs')
+
         self.rpc_config = {"AMQP_URI": self.config.get('RABBITMQ_CONFIG')}
-        self.logger = AsynchronousLog.init_asynchronous_log(self.work_name, self.work_ip)
+        self.logger = Logger.logger(self.work_name)
 
     def run_task_func_win(self, function, task_data, run_id):
         sys.path.insert(0, self.config.get('PATH'))
         RabbitMq.rabbitmq_init(self.config.get('RABBITMQ_CONFIG'))
-        logger = AsynchronousLog.init_asynchronous_log(self.work_name, self.work_ip)
+        # logger = AsynchronousLog.init_asynchronous_log(self.work_name, self.work_ip)
+
+        Logger.logs_path = os.path.join(self.config.get('PATH'), 'logs')
+        logger = Logger.logger(self.work_name)
 
         setattr(function, 'logger', logger)
         setattr(function, 'work_ip', self.work_ip)
         setattr(function, 'work_name', self.work_name)
         setattr(function, 'rpc_proxy', ZeroProxy.init_rpc_proxy(self.rpc_config))
 
         try:
```

### Comparing `zerocs-2.4/zerocs/interface/__init__.py` & `zerocs-2.5/zerocs/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/interface/interface.py` & `zerocs-2.5/zerocs/interface/interface.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/logger/__init__.py` & `zerocs-2.5/zerocs/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/logger/logger.py` & `zerocs-2.5/zerocs/logger/logger.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/main/main.py` & `zerocs-2.5/zerocs/main/main.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/observer/__init__.py` & `zerocs-2.5/zerocs/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/observer/observer.py` & `zerocs-2.5/zerocs/observer/observer.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/rabbit/__init__.py` & `zerocs-2.5/zerocs/rabbit/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/rabbit/rabbit.py` & `zerocs-2.5/zerocs/rabbit/rabbit.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/services/__init__.py` & `zerocs-2.5/zerocs/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/services/services.py` & `zerocs-2.5/zerocs/services/services.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 
         Fork.fork_service(_temporary, Config.get_configs())
         Fork.fork_work(_temporary, Config.get_configs())
 
     @staticmethod
     def update(subject: object) -> None:
         config = subject.get_configs()
-        Fork.fork_logger(config)
+        # Fork.fork_logger(config)
         Fork.fork_service(ServiceRegistration.ServiceList, config)
         Fork.fork_work(ServiceRegistration.ServiceList, config)
```

### Comparing `zerocs-2.4/zerocs/utils/__init__.py` & `zerocs-2.5/zerocs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/utils/rpc_proxy.py` & `zerocs-2.5/zerocs/utils/rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs/utils/utils.py` & `zerocs-2.5/zerocs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `zerocs-2.4/zerocs.egg-info/PKG-INFO` & `zerocs-2.5/zerocs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-Metadata-Version: 2.1
-Name: zerocs
-Version: 2.4
-Summary: zerocs
-Home-page: https://gitee.com/ZYPH/zerocs
-Author: YanPing
-Author-email: zyphhxx@foxmail.com
-Maintainer: YanPing
-Maintainer-email: zyphhxx@foxmail.com
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-License-File: LICENSE
-Requires-Dist: nameko
-Requires-Dist: pika
-Requires-Dist: pytz
-Requires-Dist: pymongo
-Requires-Dist: kombu
-
-zerocs Description Document
-============================
-
-zerocs: zero config service
-+++++++++++++++++++++++++++
-
-1. introduction
-
-    1. zerocs is a distributed task framework with extremely simple configuration.
-    Enable users to quickly build distributed task systems with minimal
-    configuration and learning costs
-
-    2. The framework has functions such as service management, work management,
-    and task management, which can meet most usage scenarios
-
-    3. Note: Version 1.9 is not compatible with version 1.3.
-    It is recommended to upgrade to version 1.9 and above
-
-    4. Decentralization starting from version 1.9,
-    no longer distinguishing between master and slave nodes
-
-2. start using
-
-    1. Please install RabbitMQ before use,
-    rabbitmq official website : https://www.rabbitmq.com,
-    It is recommended to use Docker installation during testing::
-
-            docker run -d --hostname my-rabbit --name rabbit \
-            -e RABBITMQ_DEFAULT_USER=user \
-            -e RABBITMQ_DEFAULT_PASS=password \
-            -p 15672:15672 -p 5672:5672 rabbitmq:management
-
-    2. Please install MongoDB before use,
-    Installation steps reference : https://docs.mongoing.com/install-mongodb
-
-    3. To use the framework, it is very simple, just refer to zerocs
-    in the first line of your startup script
-    Please create the corresponding directory and files before starting::
-
-          ├─logs //log directory
-          ├─service_list //Directory of microservice codes
-          │  │─test
-          │  │  ├─test.py
-          │  │  ├─test1.py
-          ├─main.py  //main
-          └─zerocs_test.py //Test Script
-
-    4. main.py ::
-
-        # -*- encoding: utf-8 -*-
-        # Master startup file, please refer to zerocs first
-        # Flask API is not mandatory and can be connected to other management systems
-
-        import os
-        import logging
-        from flask_cors import CORS
-        from flask import Flask, request
-
-        from zerocs import Main, Interface
-        from service_list.test import test, test1
-
-        app = Flask(__name__)
-        CORS(app, supports_credentials=True)
-
-        logging.basicConfig(level=logging.ERROR)
-        script_path = os.path.dirname(os.path.realpath(__file__))
-
-
-        class Master:
-
-            def __init__(self):
-                config = {
-                    "PATH": script_path,
-                    "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
-                    "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
-                }
-                Main.run_master(
-                    configs=config,
-                    services=[test, test1]
-                )
-
-            @staticmethod
-            def get_service_list(query: dict, field: dict, limit: int, page: int) -> dict:
-                count, data = Interface.get_service_list(query, field, limit, page)
-                return {"count": count, "data": data}
-
-            @staticmethod
-            def stop_tasks(task_id: str):
-                Interface.insert_stop_tasks(task_id)
-
-            @staticmethod
-            def remote_call(service_name: str, service_ip: str, method_name: str, **params):
-                rpc_proxy = Interface.remote_call_by_name_and_ip(service_name, service_ip)
-                return rpc_proxy.remote_call(service_name, method_name, **params)
-
-            @staticmethod
-            def send_message(service_name: str, message: dict):
-                if 'task_id' in message:
-                    Interface.send_message(service_name, message)
-
-            @staticmethod
-            def restart_service(service_name: str):
-                Interface.restart_service(service_name)
-
-
-        @app.route("/")
-        def index():
-            data = _main.get_service_list({}, {"_id": 0}, 10, 0)
-            return data
-
-
-        @app.route("/get_service_list")
-        def get_service_list():
-            request_json = request.get_json()
-            query = request_json['query']
-            field = request_json['field']
-            limit = request_json['limit']
-            page = request_json['page']
-
-            data = _main.get_service_list(query, field, limit, page)
-            return data
-
-
-        @app.route("/restart_service")
-        def restart_service():
-            request_json = request.get_json()
-            service_name = request_json['service_name']
-            _main.restart_service(service_name)
-            return {"code": 0}
-
-
-        if __name__ == '__main__':
-            _main = Master()
-            app.run(host='0.0.0.0', port=5002)
-
-    5. test.py ::
-
-        import time
-
-        class RpcFunction:
-            """
-            Class Name Not modifiable, Define RPC functions
-            """
-            service_name = 'test'
-
-            def get_service_name(self, xxx):
-                return {"service_name": self.service_name, "param": xxx}
-
-
-        class WorkFunction:
-            """
-            Class Name Not modifiable, Work Code
-            """
-
-            def __init__(self, task_data):
-                """
-                :param task_data: Task data JSON format
-                """
-                logger = self.__getattribute__('logger')
-                rpc_proxy = self.__getattribute__('rpc_proxy')
-
-                """
-                Call the rpc interface
-
-                data = rpc_proxy.remote_call(service_name, method_name, **params)
-                """
-
-    6. zerocs_test.py ::
-
-        # -*- encoding: utf-8 -*-
-        import os
-
-        from zerocs import Interface
-
-        script_path = os.path.dirname(os.path.realpath(__file__))
-
-        if __name__ == '__main__':
-            config = {
-                "PATH": os.path.join(script_path, 'logs'),
-                "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
-                "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
-            }
-
-            # initialization
-            Interface.init_proxy(config)
-
-            # Stop the task
-            Interface.insert_stop_tasks('1001')
-
-            # Call the RPC interface
-            obj = Interface.remote_call_by_name_and_ip('test', '192.168.0.101')
-            print(obj.remote_call('test' ,'get_service_name', param='1111111111'))
-
-            # Issue task message
-            Interface.send_message('test', {"task_id": "100", "msg": "xxxxxxxxxxxxxxxx"})
-
-
-A distributed task scheduling system was completed in just a few steps
-======================================================================
-
-Disclaimers
-================
-
-
-+   Before using the zerocs framework, please carefully read and fully understand this statement.
-    You can choose not to use the zerocs framework, but once you use the zerocs framework,
-    Your usage behavior is deemed to be recognition and acceptance of the entire content of this statement.
-
-+   You promise to use the zerocs framework in a legal and reasonable manner,
-    Do not use the zerocs board framework to engage in any illegal or malicious behavior that infringes
-    on the legitimate interests of others,
-    We will not apply the zerocs framework to any platform that violates Chinese laws and regulations.
-
-+   Any accident, negligence, contract damage, defamation
-    This project does not assume any legal responsibility for copyright or intellectual property
-    infringement and any losses caused (including but not limited to direct,
-    indirect, incidental or derivative losses).
-
-+   The user clearly and agrees to all the contents listed in the terms of this statement,
-    The potential risks and related consequences of using the zerocs framework will be entirely borne by the user,
-    and this project will not bear any legal responsibility.
-
-+   After reading this disclaimer, any unit or individual should obtain the MIT Open Source License
-    Conduct legitimate publishing, dissemination, and use of the zerocs framework within the permitted scope,
-    If the breach of this disclaimer clause or the violation of laws and regulations results in legal
-    liability (including but not limited to civil compensation and criminal liability),
-    the defaulter shall bear the responsibility on their own.
-
-+   The author owns intellectual property rights (including but not limited to trademark rights, patents, Copyrights,
-    trade secrets, etc.) of zerocs framework, and the above products are protected by relevant laws and regulations
-
-+   No entity or individual shall apply for intellectual property rights related to
-    the zerocs Framework itself without the written authorization of the Author.
-
-+   If any part of this statement is deemed invalid or unenforceable,
-    the remaining parts shall remain in full force and effect.
-    An unenforceable partial declaration does not constitute a waiver of our
-    right to enforce the declaration.
-
-+   This project has the right to make unilateral changes to the terms and attachments of this statement at any time,
-    and publish them through message push, webpage announcement, and other means. Once published,
-    it will automatically take effect without the need for separate notice;
-    If you continue to use this statement after the announcement of changes,
-    it means that you have fully read, understood, and accepted the revised statement.
+Metadata-Version: 2.1
+Name: zerocs
+Version: 2.5
+Summary: zerocs
+Home-page: https://gitee.com/ZYPH/zerocs
+Author: YanPing
+Author-email: zyphhxx@foxmail.com
+Maintainer: YanPing
+Maintainer-email: zyphhxx@foxmail.com
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+License-File: LICENSE
+Requires-Dist: nameko
+Requires-Dist: pika
+Requires-Dist: pytz
+Requires-Dist: pymongo
+Requires-Dist: kombu
+
+zerocs Description Document
+============================
+
+zerocs: zero config service
++++++++++++++++++++++++++++
+
+1. introduction
+
+    1. zerocs is a distributed task framework with extremely simple configuration.
+    Enable users to quickly build distributed task systems with minimal
+    configuration and learning costs
+
+    2. The framework has functions such as service management, work management,
+    and task management, which can meet most usage scenarios
+
+    3. Note: Version 1.9 is not compatible with version 1.3.
+    It is recommended to upgrade to version 1.9 and above
+
+    4. Decentralization starting from version 1.9,
+    no longer distinguishing between master and slave nodes
+
+2. start using
+
+    1. Please install RabbitMQ before use,
+    rabbitmq official website : https://www.rabbitmq.com,
+    It is recommended to use Docker installation during testing::
+
+            docker run -d --hostname my-rabbit --name rabbit \
+            -e RABBITMQ_DEFAULT_USER=user \
+            -e RABBITMQ_DEFAULT_PASS=password \
+            -p 15672:15672 -p 5672:5672 rabbitmq:management
+
+    2. Please install MongoDB before use,
+    Installation steps reference : https://docs.mongoing.com/install-mongodb
+
+    3. To use the framework, it is very simple, just refer to zerocs
+    in the first line of your startup script
+    Please create the corresponding directory and files before starting::
+
+          ├─logs //log directory
+          ├─service_list //Directory of microservice codes
+          │  │─test
+          │  │  ├─test.py
+          │  │  ├─test1.py
+          ├─main.py  //main
+          └─zerocs_test.py //Test Script
+
+    4. main.py ::
+
+        # -*- encoding: utf-8 -*-
+        # Master startup file, please refer to zerocs first
+        # Flask API is not mandatory and can be connected to other management systems
+
+        import os
+        import logging
+        from flask_cors import CORS
+        from flask import Flask, request
+
+        from zerocs import Main, Interface
+        from service_list.test import test, test1
+
+        app = Flask(__name__)
+        CORS(app, supports_credentials=True)
+
+        logging.basicConfig(level=logging.ERROR)
+        script_path = os.path.dirname(os.path.realpath(__file__))
+
+
+        class Master:
+
+            def __init__(self):
+                config = {
+                    "PATH": script_path,
+                    "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
+                    "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
+                }
+                Main.run_master(
+                    configs=config,
+                    services=[test, test1]
+                )
+
+            @staticmethod
+            def get_service_list(query: dict, field: dict, limit: int, page: int) -> dict:
+                count, data = Interface.get_service_list(query, field, limit, page)
+                return {"count": count, "data": data}
+
+            @staticmethod
+            def stop_tasks(task_id: str):
+                Interface.insert_stop_tasks(task_id)
+
+            @staticmethod
+            def remote_call(service_name: str, service_ip: str, method_name: str, **params):
+                rpc_proxy = Interface.remote_call_by_name_and_ip(service_name, service_ip)
+                return rpc_proxy.remote_call(service_name, method_name, **params)
+
+            @staticmethod
+            def send_message(service_name: str, message: dict):
+                if 'task_id' in message:
+                    Interface.send_message(service_name, message)
+
+            @staticmethod
+            def restart_service(service_name: str):
+                Interface.restart_service(service_name)
+
+
+        @app.route("/")
+        def index():
+            data = _main.get_service_list({}, {"_id": 0}, 10, 0)
+            return data
+
+
+        @app.route("/get_service_list")
+        def get_service_list():
+            request_json = request.get_json()
+            query = request_json['query']
+            field = request_json['field']
+            limit = request_json['limit']
+            page = request_json['page']
+
+            data = _main.get_service_list(query, field, limit, page)
+            return data
+
+
+        @app.route("/restart_service")
+        def restart_service():
+            request_json = request.get_json()
+            service_name = request_json['service_name']
+            _main.restart_service(service_name)
+            return {"code": 0}
+
+
+        if __name__ == '__main__':
+            _main = Master()
+            app.run(host='0.0.0.0', port=5002)
+
+    5. test.py ::
+
+        import time
+
+        class RpcFunction:
+            """
+            Class Name Not modifiable, Define RPC functions
+            """
+            service_name = 'test'
+
+            def get_service_name(self, xxx):
+                return {"service_name": self.service_name, "param": xxx}
+
+
+        class WorkFunction:
+            """
+            Class Name Not modifiable, Work Code
+            """
+
+            def __init__(self, task_data):
+                """
+                :param task_data: Task data JSON format
+                """
+                logger = self.__getattribute__('logger')
+                rpc_proxy = self.__getattribute__('rpc_proxy')
+
+                """
+                Call the rpc interface
+
+                data = rpc_proxy.remote_call(service_name, method_name, **params)
+                """
+
+    6. zerocs_test.py ::
+
+        # -*- encoding: utf-8 -*-
+        import os
+
+        from zerocs import Interface
+
+        script_path = os.path.dirname(os.path.realpath(__file__))
+
+        if __name__ == '__main__':
+            config = {
+                "PATH": os.path.join(script_path, 'logs'),
+                "RABBITMQ_CONFIG": "amqp://admin:Rabbit*ads12@127.0.0.1:5672",
+                "MONGODB_CONFIG": "mongodb://admin:123456@127.0.0.1:27017"
+            }
+
+            # initialization
+            Interface.init_proxy(config)
+
+            # Stop the task
+            Interface.insert_stop_tasks('1001')
+
+            # Call the RPC interface
+            obj = Interface.remote_call_by_name_and_ip('test', '192.168.0.101')
+            print(obj.remote_call('test' ,'get_service_name', param='1111111111'))
+
+            # Issue task message
+            Interface.send_message('test', {"task_id": "100", "msg": "xxxxxxxxxxxxxxxx"})
+
+
+A distributed task scheduling system was completed in just a few steps
+======================================================================
+
+Disclaimers
+================
+
+
++   Before using the zerocs framework, please carefully read and fully understand this statement.
+    You can choose not to use the zerocs framework, but once you use the zerocs framework,
+    Your usage behavior is deemed to be recognition and acceptance of the entire content of this statement.
+
++   You promise to use the zerocs framework in a legal and reasonable manner,
+    Do not use the zerocs board framework to engage in any illegal or malicious behavior that infringes
+    on the legitimate interests of others,
+    We will not apply the zerocs framework to any platform that violates Chinese laws and regulations.
+
++   Any accident, negligence, contract damage, defamation
+    This project does not assume any legal responsibility for copyright or intellectual property
+    infringement and any losses caused (including but not limited to direct,
+    indirect, incidental or derivative losses).
+
++   The user clearly and agrees to all the contents listed in the terms of this statement,
+    The potential risks and related consequences of using the zerocs framework will be entirely borne by the user,
+    and this project will not bear any legal responsibility.
+
++   After reading this disclaimer, any unit or individual should obtain the MIT Open Source License
+    Conduct legitimate publishing, dissemination, and use of the zerocs framework within the permitted scope,
+    If the breach of this disclaimer clause or the violation of laws and regulations results in legal
+    liability (including but not limited to civil compensation and criminal liability),
+    the defaulter shall bear the responsibility on their own.
+
++   The author owns intellectual property rights (including but not limited to trademark rights, patents, Copyrights,
+    trade secrets, etc.) of zerocs framework, and the above products are protected by relevant laws and regulations
+
++   No entity or individual shall apply for intellectual property rights related to
+    the zerocs Framework itself without the written authorization of the Author.
+
++   If any part of this statement is deemed invalid or unenforceable,
+    the remaining parts shall remain in full force and effect.
+    An unenforceable partial declaration does not constitute a waiver of our
+    right to enforce the declaration.
+
++   This project has the right to make unilateral changes to the terms and attachments of this statement at any time,
+    and publish them through message push, webpage announcement, and other means. Once published,
+    it will automatically take effect without the need for separate notice;
+    If you continue to use this statement after the announcement of changes,
+    it means that you have fully read, understood, and accepted the revised statement.
```

### Comparing `zerocs-2.4/zerocs.egg-info/SOURCES.txt` & `zerocs-2.5/zerocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

