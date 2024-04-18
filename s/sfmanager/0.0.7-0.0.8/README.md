# Comparing `tmp/sfmanager-0.0.7.tar.gz` & `tmp/sfmanager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sfmanager-0.0.7.tar", last modified: Thu Apr 18 07:19:48 2024, max compression
+gzip compressed data, was "sfmanager-0.0.8.tar", last modified: Thu Apr 18 08:07:23 2024, max compression
```

## Comparing `sfmanager-0.0.7.tar` & `sfmanager-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 07:19:48.574015 sfmanager-0.0.7/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 07:19:48.574015 sfmanager-0.0.7/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.7/README.md
--rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 07:19:48.574015 sfmanager-0.0.7/setup.cfg
--rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 07:19:24.000000 sfmanager-0.0.7/setup.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 07:19:48.570015 sfmanager-0.0.7/sfmanager/
--rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.7/sfmanager/__init__.py
--rw-rw-r--   0 grand     (1000) grand     (1000)     1416 2024-04-18 07:19:11.000000 sfmanager-0.0.7/sfmanager/app.py
-drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 07:19:48.574015 sfmanager-0.0.7/sfmanager.egg-info/
--rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 07:19:48.000000 sfmanager-0.0.7/sfmanager.egg-info/PKG-INFO
--rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 07:19:48.000000 sfmanager-0.0.7/sfmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 07:19:48.000000 sfmanager-0.0.7/sfmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 07:19:48.000000 sfmanager-0.0.7/sfmanager.egg-info/requires.txt
--rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 07:19:48.000000 sfmanager-0.0.7/sfmanager.egg-info/top_level.txt
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 08:07:23.400433 sfmanager-0.0.8/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 08:07:23.400433 sfmanager-0.0.8/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      365 2024-04-18 05:45:03.000000 sfmanager-0.0.8/README.md
+-rw-rw-r--   0 grand     (1000) grand     (1000)       38 2024-04-18 08:07:23.400433 sfmanager-0.0.8/setup.cfg
+-rw-rw-r--   0 grand     (1000) grand     (1000)      800 2024-04-18 08:07:19.000000 sfmanager-0.0.8/setup.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 08:07:23.396435 sfmanager-0.0.8/sfmanager/
+-rw-rw-r--   0 grand     (1000) grand     (1000)       73 2024-04-18 06:32:48.000000 sfmanager-0.0.8/sfmanager/__init__.py
+-rw-rw-r--   0 grand     (1000) grand     (1000)     1623 2024-04-18 08:06:12.000000 sfmanager-0.0.8/sfmanager/app.py
+drwxrwxr-x   0 grand     (1000) grand     (1000)        0 2024-04-18 08:07:23.396435 sfmanager-0.0.8/sfmanager.egg-info/
+-rw-rw-r--   0 grand     (1000) grand     (1000)      882 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 grand     (1000) grand     (1000)      231 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)        1 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       17 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/requires.txt
+-rw-rw-r--   0 grand     (1000) grand     (1000)       10 2024-04-18 08:07:23.000000 sfmanager-0.0.8/sfmanager.egg-info/top_level.txt
```

### Comparing `sfmanager-0.0.7/PKG-INFO` & `sfmanager-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
 Keywords: tensor
```

### Comparing `sfmanager-0.0.7/setup.py` & `sfmanager-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='sfmanager',
-    version='0.0.7',
+    version='0.0.8',
     author='GrandTheBest',
     author_email='grandinfo-cm@gmail.com',
     description='Super filemanager for python',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://t.me/grand_studios',
     packages=find_packages(),
```

### Comparing `sfmanager-0.0.7/sfmanager/app.py` & `sfmanager-0.0.8/sfmanager/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,53 +10,53 @@
 		if self.level >= 1:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					raw = f.readline()
 				return raw
 			except FileNotFoundError:
 				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 1")
 
 	def readlines(self):
 		if self.level >= 1:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					raw = f.readlines()
 				return raw
 			except FileNotFoundError:
 				print("Something went wrong...")
+		else:
+			print(f"Low access level! {self.level}, but need 1")
 	def set(self, text):
-		if self.level >= 2:
+		if self.level >= 3:
 			try:
 				with open(f"{self.filename}", "w") as f:
 					f.write(text)
 					return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
-				return 0
 		else:
-			return 0
+			print(f"Low access level! {self.level}, but need 3")
 	def add(self, text):
 		if self.level >= 2:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					old = f.read()
 				with open(f"{self.filename}", "w") as f:
 					f.write(old + " " + text)
 					return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
-				return 0
 		else:
-			return 0
+			print(f"Low access level! {self.level}, but need 2")
 	def replace(self, target, text):
-		if self.level >= 2:
+		if self.level >= 3:
 			try:
 				with open(f"{self.filename}", "r") as f:
 					data = f.read().replace(target, text)
 				with open(f"{self.filename}", "w") as f:
 					f.write(data)
-					return 1
 			except FileNotFoundError:
 				print("Something went wrong...")
-				return 0
 		else:
-			return 0
+			print(f"Low access level! {self.level}, but need 3")
```

### Comparing `sfmanager-0.0.7/sfmanager.egg-info/PKG-INFO` & `sfmanager-0.0.8/sfmanager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfmanager
-Version: 0.0.7
+Version: 0.0.8
 Summary: Super filemanager for python
 Home-page: https://t.me/grand_studios
 Author: GrandTheBest
 Author-email: grandinfo-cm@gmail.com
 License: UNKNOWN
 Project-URL: GitHub, https://github.com/grandescobar/sfmanager
 Keywords: tensor
```

