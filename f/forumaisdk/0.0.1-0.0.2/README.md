# Comparing `tmp/forumaisdk-0.0.1.tar.gz` & `tmp/forumaisdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forumaisdk-0.0.1.tar", last modified: Fri Apr 12 14:51:59 2024, max compression
+gzip compressed data, was "forumaisdk-0.0.2.tar", last modified: Thu Apr 18 16:51:06 2024, max compression
```

## Comparing `forumaisdk-0.0.1.tar` & `forumaisdk-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:51:59.763480 forumaisdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:51:59.759480 forumaisdk-0.0.1/ModelMarketSDK/
--rw-r--r--   0 runner    (1001) docker     (127)   579187 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/ModelMarketSDK/LLMMarket.json
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/ModelMarketSDK/ModelMarket.py
--rw-r--r--   0 runner    (1001) docker     (127)   196960 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/ModelMarketSDK/USDC.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/ModelMarketSDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 14:51:59.763480 forumaisdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:51:59.763480 forumaisdk-0.0.1/forumaisdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-12 14:51:59.000000 forumaisdk-0.0.1/forumaisdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-12 14:51:59.000000 forumaisdk-0.0.1/forumaisdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:51:59.000000 forumaisdk-0.0.1/forumaisdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 14:51:59.000000 forumaisdk-0.0.1/forumaisdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 14:51:59.000000 forumaisdk-0.0.1/forumaisdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-12 14:51:48.000000 forumaisdk-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:51:59.763480 forumaisdk-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/ModelMarketSDK/
+-rw-r--r--   0 runner    (1001) docker     (127)   579187 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/LLMMarket.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/ModelMarket.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196960 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/USDC.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/ModelMarketSDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/forumaisdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 16:51:06.000000 forumaisdk-0.0.2/forumaisdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 16:50:58.000000 forumaisdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 16:51:06.645172 forumaisdk-0.0.2/setup.cfg
```

### Comparing `forumaisdk-0.0.1/LICENSE` & `forumaisdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forumaisdk-0.0.1/ModelMarketSDK/LLMMarket.json` & `forumaisdk-0.0.2/ModelMarketSDK/LLMMarket.json`

 * *Files identical despite different names*

### Comparing `forumaisdk-0.0.1/ModelMarketSDK/ModelMarket.py` & `forumaisdk-0.0.2/ModelMarketSDK/ModelMarket.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,24 @@
         self.web3 = Web3(Web3.HTTPProvider(self.rpc))
         script_dir = os.path.dirname(__file__)  # Get the script's directory
         file_path = os.path.join(script_dir, "LLMMarket.json")
         f = open(file_path)
         data = json.load(f)
         f.close()
         abi = data["abi"]
-        self.llm_market = self.web3.eth.contract(address="0x54cc0Ea21A53ddaAbF774d1882702897BCe7Cd05", abi=abi)
+        self.llm_market = self.web3.eth.contract(address="0x4D26F6e4bb4dd9BC5f9E9Cb8714fFf324B57Dae9", abi=abi)
         self.private_key = private_key
         self.public_key = public_key
         script_dir = os.path.dirname(__file__)  # Get the script's directory
         file_path = os.path.join(script_dir, "USDC.json")
         f = open(file_path)
         data = json.load(f)
         f.close()
         abi = data["abi"]
-        self.usdc = self.web3.eth.contract(address="0x15BA0717d7B1E627b8740Bb5589709afC6A99359", abi=abi)
+        self.usdc = self.web3.eth.contract(address="0xFab79D18EcC2076369FD7e7391d5F8C1A98beb3c", abi=abi)
         print("Initialized!")
 
     # returns all the nodes
     def get_hosts(self):
         return self.llm_market.functions.getHosts().call()
 
     # checks if a node is currently paused
```

### Comparing `forumaisdk-0.0.1/ModelMarketSDK/USDC.json` & `forumaisdk-0.0.2/ModelMarketSDK/USDC.json`

 * *Files identical despite different names*

### Comparing `forumaisdk-0.0.1/PKG-INFO` & `forumaisdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forumaisdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: ForumAI Python SDK
 Author-email: ForumAISDK <forumai@github.com>
 Project-URL: Homepage, https://github.com/0xAresDev/ForumAISDK
 Project-URL: Issues, https://github.com/0xAresDev/ForumAISDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forumaisdk-0.0.1/forumaisdk.egg-info/PKG-INFO` & `forumaisdk-0.0.2/forumaisdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forumaisdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: ForumAI Python SDK
 Author-email: ForumAISDK <forumai@github.com>
 Project-URL: Homepage, https://github.com/0xAresDev/ForumAISDK
 Project-URL: Issues, https://github.com/0xAresDev/ForumAISDK/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `forumaisdk-0.0.1/pyproject.toml` & `forumaisdk-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Include the ABI files
 [tool.setuptools.package-data]
 ModelMarketSDK = ["*.json"]
 
 [project]
 name = "forumaisdk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="ForumAISDK", email="forumai@github.com" },
 ]
 description = "ForumAI Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

