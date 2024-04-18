# Comparing `tmp/cloudformation-cli-python-plugin-2.1.8.tar.gz` & `tmp/cloudformation-cli-python-plugin-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cloudformation-cli-python-plugin-2.1.8.tar", last modified: Thu Apr 20 17:22:48 2023, max compression
+gzip compressed data, was "cloudformation-cli-python-plugin-2.1.9.tar", last modified: Thu Apr 18 17:41:21 2024, max compression
```

## Comparing `cloudformation-cli-python-plugin-2.1.8.tar` & `cloudformation-cli-python-plugin-2.1.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/
--rw-r--r--   0 izoran   (22393816) amazon     (100)    10142 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/LICENSE
--rw-r--r--   0 izoran   (22393816) amazon     (100)      143 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/MANIFEST.in
--rw-r--r--   0 izoran   (22393816) amazon     (100)     4925 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/PKG-INFO
--rw-r--r--   0 izoran   (22393816) amazon     (100)     3075 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/README.md
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/
--rw-r--r--   0 izoran   (22393816) amazon     (100)     4925 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO
--rw-r--r--   0 izoran   (22393816) amazon     (100)      984 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 izoran   (22393816) amazon     (100)        1 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 izoran   (22393816) amazon     (100)      476 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/entry_points.txt
--rw-r--r--   0 izoran   (22393816) amazon     (100)       52 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/requires.txt
--rw-r--r--   0 izoran   (22393816) amazon     (100)        5 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/top_level.txt
--rw-r--r--   0 izoran   (22393816) amazon     (100)        1 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/zip-safe
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/
--rw-r--r--   0 izoran   (22393816) amazon     (100)      101 2023-04-20 16:20:40.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/__init__.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)    16576 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/codegen.py
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/
--rw-r--r--   0 izoran   (22393816) amazon     (100)     1759 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/Python.gitignore
--rw-r--r--   0 izoran   (22393816) amazon     (100)        0 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/__init__.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)     1417 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/parser.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)     1681 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/resolver.py
-drwxr-xr-x   0 izoran   (22393816) amazon     (100)        0 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/
--rw-r--r--   0 izoran   (22393816) amazon     (100)     1806 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/README.md
--rw-r--r--   0 izoran   (22393816) amazon     (100)     3618 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/handlers.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)     3384 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_handlers.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)     2337 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_models.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)     2544 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/models.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)       30 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/requirements.txt
--rw-r--r--   0 izoran   (22393816) amazon     (100)     2232 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/target_model.py
--rw-r--r--   0 izoran   (22393816) amazon     (100)      738 2023-04-20 17:22:48.000000 cloudformation-cli-python-plugin-2.1.8/setup.cfg
--rw-r--r--   0 izoran   (22393816) amazon     (100)     2750 2023-04-20 15:40:14.000000 cloudformation-cli-python-plugin-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.961019 cloudformation-cli-python-plugin-2.1.9/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:41:21.000000 cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.961019 cloudformation-cli-python-plugin-2.1.9/python/rpdk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16782 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/data/Python.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/hook_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/hook_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/target_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 17:41:21.965019 cloudformation-cli-python-plugin-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-18 17:41:13.000000 cloudformation-cli-python-plugin-2.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cloudformation-cli-python-plugin-2.1.8/LICENSE` & `cloudformation-cli-python-plugin-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/PKG-INFO` & `cloudformation-cli-python-plugin-2.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,130 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli-python-plugin
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python 3.6 and 3.7 language support for the CloudFormation CLI
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
-Description: # AWS CloudFormation Resource Provider Python Plugin
-        
-        The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
-        
-        This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
-        
-        ## AWS CloudFormation Resource Provider Python Plugin
-        
-        The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
-        
-        This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
-        
-        [![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
-        
-        ## Community
-        
-        Join us on Discord! Connect & interact with CloudFormation developers &
-        experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
-        Guard and more:
-        
-        [![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
-        
-        Installation
-        ------------
-        
-        ```bash
-        pip install cloudformation-cli-python-plugin
-        ```
-        
-        Howto
-        -----
-        
-        ```
-        $ cfn init
-        Initializing new project
-        What's the name of your resource type?
-        (Organization::Service::Resource)
-        >> Foo::Bar::Baz
-        Select a language for code generation:
-        [1] java
-        [2] csharp
-        [3] python36
-        [4] python37
-        (enter an integer):
-        >> 4
-        Use docker for platform-independent packaging (Y/n)?
-        This is highly recommended unless you are experienced
-        with cross-platform Python packaging.
-        >> y
-        Initialized a new project in <>
-        $ cfn submit --dry-run
-        $ cat <<EOT > test.json
-        {
-          "credentials": {
-            "accessKeyId": "",
-            "secretAccessKey": "",
-            "sessionToken": ""
-          },
-          "action": "CREATE",
-          "request": {
-            "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
-            "desiredResourceState": {
-              "Title": "This_Is_The_Title_For_My_Example",
-              "TestCode": "NOT_STARTED"
-            },
-            "previousResourceState": null,
-            "logicalResourceIdentifier": null
-          },
-          "callbackContext": null
-        }
-        EOT
-        $ sam local invoke TestEntrypoint --event test.json
-        ```
-        
-        Development
-        -----------
-        
-        For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
-        
-        ```
-        python3 -m venv env
-        source env/bin/activate
-        pip install -e . -e src/ \
-          -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
-        pre-commit install
-        ```
-        
-        Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
-        
-        ```
-        # run all hooks on all files, mirrors what the CI runs
-        pre-commit run --all-files
-        # run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
-        pre-commit run pytest-local
-        ```
-        
-        License
-        -------
-        
-        This library is licensed under the Apache 2.0 License.
-        
 Keywords: Amazon Web Services AWS CloudFormation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AWS CloudFormation Resource Provider Python Plugin
+
+The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
+
+This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
+
+## AWS CloudFormation Resource Provider Python Plugin
+
+The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
+
+This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
+
+[![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
+
+## Community
+
+Join us on Discord! Connect & interact with CloudFormation developers &
+experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
+Guard and more:
+
+[![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
+
+Installation
+------------
+
+```bash
+pip install cloudformation-cli-python-plugin
+```
+
+Howto
+-----
+
+```
+$ cfn init
+Initializing new project
+What's the name of your resource type?
+(Organization::Service::Resource)
+>> Foo::Bar::Baz
+Select a language for code generation:
+[1] java
+[2] csharp
+[3] python38
+[4] python39
+[5] python310
+[6] python311
+[7] python312
+(enter an integer):
+>> 4
+Use docker for platform-independent packaging (Y/n)?
+This is highly recommended unless you are experienced
+with cross-platform Python packaging.
+>> y
+Initialized a new project in <>
+$ cfn submit --dry-run
+$ cat <<EOT > test.json
+{
+  "credentials": {
+    "accessKeyId": "",
+    "secretAccessKey": "",
+    "sessionToken": ""
+  },
+  "action": "CREATE",
+  "request": {
+    "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
+    "desiredResourceState": {
+      "Title": "This_Is_The_Title_For_My_Example",
+      "TestCode": "NOT_STARTED"
+    },
+    "previousResourceState": null,
+    "logicalResourceIdentifier": null
+  },
+  "callbackContext": null
+}
+EOT
+$ sam local invoke TestEntrypoint --event test.json
+```
+
+Development
+-----------
+
+For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
+
+```
+python3 -m venv env
+source env/bin/activate
+pip install -e . -e src/ \
+  -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
+pre-commit install
+```
+
+Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
+
+```
+# run all hooks on all files, mirrors what the CI runs
+pre-commit run --all-files
+# run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
+pre-commit run pytest-local
+```
+
+License
+-------
+
+This library is licensed under the Apache 2.0 License.
```

### Comparing `cloudformation-cli-python-plugin-2.1.8/README.md` & `cloudformation-cli-python-plugin-2.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,16 +35,19 @@
 Initializing new project
 What's the name of your resource type?
 (Organization::Service::Resource)
 >> Foo::Bar::Baz
 Select a language for code generation:
 [1] java
 [2] csharp
-[3] python36
-[4] python37
+[3] python38
+[4] python39
+[5] python310
+[6] python311
+[7] python312
 (enter an integer):
 >> 4
 Use docker for platform-independent packaging (Y/n)?
 This is highly recommended unless you are experienced
 with cross-platform Python packaging.
 >> y
 Initialized a new project in <>
```

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO` & `cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,124 +1,130 @@
 Metadata-Version: 2.1
 Name: cloudformation-cli-python-plugin
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python 3.6 and 3.7 language support for the CloudFormation CLI
 Home-page: https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
-Description: # AWS CloudFormation Resource Provider Python Plugin
-        
-        The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
-        
-        This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
-        
-        ## AWS CloudFormation Resource Provider Python Plugin
-        
-        The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
-        
-        This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
-        
-        [![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
-        
-        ## Community
-        
-        Join us on Discord! Connect & interact with CloudFormation developers &
-        experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
-        Guard and more:
-        
-        [![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
-        
-        Installation
-        ------------
-        
-        ```bash
-        pip install cloudformation-cli-python-plugin
-        ```
-        
-        Howto
-        -----
-        
-        ```
-        $ cfn init
-        Initializing new project
-        What's the name of your resource type?
-        (Organization::Service::Resource)
-        >> Foo::Bar::Baz
-        Select a language for code generation:
-        [1] java
-        [2] csharp
-        [3] python36
-        [4] python37
-        (enter an integer):
-        >> 4
-        Use docker for platform-independent packaging (Y/n)?
-        This is highly recommended unless you are experienced
-        with cross-platform Python packaging.
-        >> y
-        Initialized a new project in <>
-        $ cfn submit --dry-run
-        $ cat <<EOT > test.json
-        {
-          "credentials": {
-            "accessKeyId": "",
-            "secretAccessKey": "",
-            "sessionToken": ""
-          },
-          "action": "CREATE",
-          "request": {
-            "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
-            "desiredResourceState": {
-              "Title": "This_Is_The_Title_For_My_Example",
-              "TestCode": "NOT_STARTED"
-            },
-            "previousResourceState": null,
-            "logicalResourceIdentifier": null
-          },
-          "callbackContext": null
-        }
-        EOT
-        $ sam local invoke TestEntrypoint --event test.json
-        ```
-        
-        Development
-        -----------
-        
-        For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
-        
-        ```
-        python3 -m venv env
-        source env/bin/activate
-        pip install -e . -e src/ \
-          -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
-        pre-commit install
-        ```
-        
-        Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
-        
-        ```
-        # run all hooks on all files, mirrors what the CI runs
-        pre-commit run --all-files
-        # run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
-        pre-commit run pytest-local
-        ```
-        
-        License
-        -------
-        
-        This library is licensed under the Apache 2.0 License.
-        
 Keywords: Amazon Web Services AWS CloudFormation
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AWS CloudFormation Resource Provider Python Plugin
+
+The CloudFormation CLI (cfn) allows you to author your own resource providers that can be used by CloudFormation.
+
+This plugin library helps to provide Python runtime bindings for the execution of your providers by CloudFormation.
+
+## AWS CloudFormation Resource Provider Python Plugin
+
+The CloudFormation Resource Provider Development Kit (RPDK) allows you to author your own resource providers that can be used by CloudFormation.
+
+This plugin library helps to provide runtime bindings for the execution of your providers by CloudFormation.
+
+[![Build Status](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin.svg?branch=master)](https://travis-ci.com/aws-cloudformation/cloudformation-cli-python-plugin)
+
+## Community
+
+Join us on Discord! Connect & interact with CloudFormation developers &
+experts, find channels to discuss and get help for our CLIs, cfn-lint, CloudFormation registry, StackSets,
+Guard and more:
+
+[![Join our Discord](https://discordapp.com/api/guilds/981586120448020580/widget.png?style=banner3)](https://discord.gg/9zpd7TTRwq)
+
+Installation
+------------
+
+```bash
+pip install cloudformation-cli-python-plugin
+```
+
+Howto
+-----
+
+```
+$ cfn init
+Initializing new project
+What's the name of your resource type?
+(Organization::Service::Resource)
+>> Foo::Bar::Baz
+Select a language for code generation:
+[1] java
+[2] csharp
+[3] python38
+[4] python39
+[5] python310
+[6] python311
+[7] python312
+(enter an integer):
+>> 4
+Use docker for platform-independent packaging (Y/n)?
+This is highly recommended unless you are experienced
+with cross-platform Python packaging.
+>> y
+Initialized a new project in <>
+$ cfn submit --dry-run
+$ cat <<EOT > test.json
+{
+  "credentials": {
+    "accessKeyId": "",
+    "secretAccessKey": "",
+    "sessionToken": ""
+  },
+  "action": "CREATE",
+  "request": {
+    "clientRequestToken": "ecba020e-b2e6-4742-a7d0-8a06ae7c4b2b",
+    "desiredResourceState": {
+      "Title": "This_Is_The_Title_For_My_Example",
+      "TestCode": "NOT_STARTED"
+    },
+    "previousResourceState": null,
+    "logicalResourceIdentifier": null
+  },
+  "callbackContext": null
+}
+EOT
+$ sam local invoke TestEntrypoint --event test.json
+```
+
+Development
+-----------
+
+For changes to the plugin, a Python virtual environment is recommended. The development requirements can be sourced from the core repository:
+
+```
+python3 -m venv env
+source env/bin/activate
+pip install -e . -e src/ \
+  -r https://raw.githubusercontent.com/aws-cloudformation/aws-cloudformation-rpdk/master/requirements.txt
+pre-commit install
+```
+
+Linting and running unit tests is done via [pre-commit](https://pre-commit.com/), and so is performed automatically on commit. The continuous integration also runs these checks. Manual options are available so you don't have to commit):
+
+```
+# run all hooks on all files, mirrors what the CI runs
+pre-commit run --all-files
+# run unit tests only. can also be used for other hooks, e.g. black, flake8, pylint-local
+pre-commit run pytest-local
+```
+
+License
+-------
+
+This library is licensed under the Apache 2.0 License.
```

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt` & `cloudformation-cli-python-plugin-2.1.9/python/cloudformation_cli_python_plugin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/codegen.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,23 +35,23 @@
     pass
 
 
 def validate_no(value):
     return value.lower() not in ("n", "no")
 
 
-class Python36LanguagePlugin(LanguagePlugin):
+class _PythonLanguagePlugin(LanguagePlugin):
     MODULE_NAME = __name__
-    NAME = "python36"
-    RUNTIME = "python3.6"
+    NAME = ""
+    RUNTIME = ""
     HOOK_ENTRY_POINT = "{}.handlers.hook"
     RESOURCE_ENTRY_POINT = "{}.handlers.resource"
     TEST_ENTRY_POINT = "{}.handlers.test_entrypoint"
     CODE_URI = "build/"
-    DOCKER_TAG = 3.6
+    DOCKER_TAG = ""
 
     def __init__(self):
         self.env = self._setup_jinja_env(
             trim_blocks=True, lstrip_blocks=True, keep_trailing_newline=True
         )
         self.env.filters["translate_type"] = translate_type
         self.env.filters["contains_model"] = contains_model
@@ -233,17 +233,16 @@
             target_schema = target_info["Schema"]
             target_namespace = [
                 s.lower() for s in target_type_name.split("::")
             ]  # AWS::SQS::Queue -> awssqsqueue
             target_name = "".join(
                 [s.capitalize() for s in target_namespace]
             )  # awssqsqueue -> AwsSqsQueue
-            target_model_file = "{}.py".format(
-                "_".join(target_namespace)
-            )  # awssqsqueue -> aws_sqs_queue.py
+            target_model_file = f'{"_".join(target_namespace)}.py'
+            # awssqsqueue -> aws_sqs_queue.py
 
             models = resolve_models(target_schema, target_name)
 
             # TODO: Remove once tagging is fully supported
             if models.get(target_name, {}).get("Tags"):  # pragma: no cover
                 models[target_name]["Tags"] = ResolvedType(
                     ContainerType.PRIMITIVE, UNDEFINED
@@ -366,15 +365,15 @@
             )
 
         docker_client = docker.from_env()
         try:
             logs = docker_client.containers.run(
                 image=image,
                 command=command,
-                auto_remove=True,
+                remove=True,
                 volumes=volumes,
                 stream=True,
                 entrypoint="",
                 user=localuser,
                 platform="linux/amd64",
             )
         except RequestsConnectionError as e:
@@ -421,23 +420,35 @@
         except (FileNotFoundError, CalledProcessError) as e:
             raise DownstreamError("pip build failed") from e
 
         LOG.debug("--- pip stdout:\n%s", completed_proc.stdout)
         LOG.debug("--- pip stderr:\n%s", completed_proc.stderr)
 
 
-class Python37LanguagePlugin(Python36LanguagePlugin):
-    NAME = "python37"
-    RUNTIME = "python3.7"
-    DOCKER_TAG = 3.7
-
-
-class Python38LanguagePlugin(Python36LanguagePlugin):
+class Python38LanguagePlugin(_PythonLanguagePlugin):
     NAME = "python38"
     RUNTIME = "python3.8"
     DOCKER_TAG = 3.8
 
 
-class Python39LanguagePlugin(Python36LanguagePlugin):
+class Python39LanguagePlugin(_PythonLanguagePlugin):
     NAME = "python39"
     RUNTIME = "python3.9"
     DOCKER_TAG = 3.9
+
+
+class Python310LanguagePlugin(_PythonLanguagePlugin):
+    NAME = "python310"
+    RUNTIME = "python3.10"
+    DOCKER_TAG = 3.10
+
+
+class Python311LanguagePlugin(_PythonLanguagePlugin):
+    NAME = "python311"
+    RUNTIME = "python3.11"
+    DOCKER_TAG = 3.11
+
+
+class Python312LanguagePlugin(_PythonLanguagePlugin):
+    NAME = "python312"
+    RUNTIME = "python3.12"
+    DOCKER_TAG = 3.12
```

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/data/Python.gitignore` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/data/Python.gitignore`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/parser.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 def setup_subparser(subparsers, parents, python_version, python_version_number):
     parser = subparsers.add_parser(
         python_version,
         description=(
-            "This sub command generates IDE and build files for Python "
-            "{}".format(python_version_number)
+            "This sub command generates IDE and build files for "
+            f"Python {python_version_number}"
         ),
         parents=parents,
     )
     parser.set_defaults(language=python_version)
 
     group = parser.add_mutually_exclusive_group()
 
@@ -26,21 +26,25 @@
         help="""Generally not recommended unless you are experienced
             with cross-platform Python packaging""",
     )
 
     return parser
 
 
-def setup_subparser_python36(subparsers, parents):
-    return setup_subparser(subparsers, parents, "python36", "3.6")
-
-
-def setup_subparser_python37(subparsers, parents):
-    return setup_subparser(subparsers, parents, "python37", "3.7")
-
-
 def setup_subparser_python38(subparsers, parents):
     return setup_subparser(subparsers, parents, "python38", "3.8")
 
 
 def setup_subparser_python39(subparsers, parents):
     return setup_subparser(subparsers, parents, "python39", "3.9")
+
+
+def setup_subparser_python310(subparsers, parents):
+    return setup_subparser(subparsers, parents, "python310", "3.10")
+
+
+def setup_subparser_python311(subparsers, parents):
+    return setup_subparser(subparsers, parents, "python311", "3.11")
+
+
+def setup_subparser_python312(subparsers, parents):
+    return setup_subparser(subparsers, parents, "python312", "3.12")
```

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/resolver.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/resolver.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/README.md` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/README.md`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/handlers.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/handlers.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_handlers.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/hook_handlers.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/hook_models.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/hook_models.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/models.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/models.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/python/rpdk/python/templates/target_model.py` & `cloudformation-cli-python-plugin-2.1.9/python/rpdk/python/templates/target_model.py`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/setup.cfg` & `cloudformation-cli-python-plugin-2.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cloudformation-cli-python-plugin-2.1.8/setup.py` & `cloudformation-cli-python-plugin-2.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,39 +32,47 @@
     url="https://github.com/aws-cloudformation/aws-cloudformation-rpdk-python-plugin/",
     # https://packaging.python.org/guides/packaging-namespace-packages/
     packages=["rpdk.python"],
     package_dir={"": "python"},
     # package_data -> use MANIFEST.in instead
     include_package_data=True,
     zip_safe=True,
-    python_requires=">=3.6",
-    install_requires=["cloudformation-cli>=0.2.26", "types-dataclasses>=0.1.5"],
+    python_requires=">=3.8",
+    install_requires=[
+        "cloudformation-cli>=0.2.26",
+        "types-dataclasses>=0.1.5",
+    ],
     entry_points={
         "rpdk.v1.languages": [
+            "python312 = rpdk.python.codegen:Python312LanguagePlugin",
+            "python311 = rpdk.python.codegen:Python311LanguagePlugin",
+            "python310 = rpdk.python.codegen:Python310LanguagePlugin",
             "python39 = rpdk.python.codegen:Python39LanguagePlugin",
             "python38 = rpdk.python.codegen:Python38LanguagePlugin",
-            "python37 = rpdk.python.codegen:Python37LanguagePlugin",
-            "python36 = rpdk.python.codegen:Python36LanguagePlugin",
         ],
         "rpdk.v1.parsers": [
+            "python312 = rpdk.python.parser:setup_subparser_python312",
+            "python311 = rpdk.python.parser:setup_subparser_python311",
+            "python310 = rpdk.python.parser:setup_subparser_python310",
             "python39 = rpdk.python.parser:setup_subparser_python39",
             "python38 = rpdk.python.parser:setup_subparser_python38",
-            "python37 = rpdk.python.parser:setup_subparser_python37",
-            "python36 = rpdk.python.parser:setup_subparser_python36",
         ],
     },
     license="Apache License 2.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Topic :: Software Development :: Build Tools",
         "Topic :: Software Development :: Code Generators",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     keywords="Amazon Web Services AWS CloudFormation",
 )
```

