# Comparing `tmp/minsprojectr-0.0.1.tar.gz` & `tmp/minsprojectr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minsprojectr-0.0.1.tar", last modified: Thu Apr 18 17:41:06 2024, max compression
+gzip compressed data, was "minsprojectr-0.0.2.tar", last modified: Thu Apr 18 18:10:40 2024, max compression
```

## Comparing `minsprojectr-0.0.1.tar` & `minsprojectr-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 17:41:06.808531 minsprojectr-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-18 17:39:53.000000 minsprojectr-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      615 2024-04-18 17:41:06.806531 minsprojectr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      214 2024-04-18 12:56:25.000000 minsprojectr-0.0.1/README.md
--rw-rw-rw-   0        0        0      387 2024-04-18 17:39:14.000000 minsprojectr-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-18 17:41:06.809134 minsprojectr-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-18 17:41:06.745327 minsprojectr-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 17:41:06.762095 minsprojectr-0.0.1/src/minsprojectr/
--rw-rw-rw-   0        0        0        0 2024-04-17 18:06:51.000000 minsprojectr-0.0.1/src/minsprojectr/init.py
--rw-rw-rw-   0        0        0      100 2024-04-17 14:17:28.000000 minsprojectr-0.0.1/src/minsprojectr/operations.py
-drwxrwxrwx   0        0        0        0 2024-04-18 17:41:06.795148 minsprojectr-0.0.1/src/minsprojectr.egg-info/
--rw-rw-rw-   0        0        0      615 2024-04-18 17:41:06.000000 minsprojectr-0.0.1/src/minsprojectr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-18 17:41:06.000000 minsprojectr-0.0.1/src/minsprojectr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 17:41:06.000000 minsprojectr-0.0.1/src/minsprojectr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 17:41:06.000000 minsprojectr-0.0.1/src/minsprojectr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 18:10:40.514495 minsprojectr-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-18 17:39:53.000000 minsprojectr-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      804 2024-04-18 18:10:40.511809 minsprojectr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2024-04-18 18:02:37.000000 minsprojectr-0.0.2/README.md
+-rw-rw-rw-   0        0        0      387 2024-04-18 18:10:14.000000 minsprojectr-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:10:40.514766 minsprojectr-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 18:10:40.464769 minsprojectr-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-18 18:10:40.477746 minsprojectr-0.0.2/src/minsprojectr/
+-rw-rw-rw-   0        0        0        0 2024-04-17 18:06:51.000000 minsprojectr-0.0.2/src/minsprojectr/init.py
+-rw-rw-rw-   0        0        0      100 2024-04-17 14:17:28.000000 minsprojectr-0.0.2/src/minsprojectr/operations.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:10:40.508932 minsprojectr-0.0.2/src/minsprojectr.egg-info/
+-rw-rw-rw-   0        0        0      804 2024-04-18 18:10:40.000000 minsprojectr-0.0.2/src/minsprojectr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-18 18:10:40.000000 minsprojectr-0.0.2/src/minsprojectr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:10:40.000000 minsprojectr-0.0.2/src/minsprojectr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-18 18:10:40.000000 minsprojectr-0.0.2/src/minsprojectr.egg-info/top_level.txt
```

### Comparing `minsprojectr-0.0.1/LICENSE` & `minsprojectr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minsprojectr-0.0.1/PKG-INFO` & `minsprojectr-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: minsprojectr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package for basic mathematical operations
 Author-email: Sai <sai275stw@gamil.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  Package
 
 This is a simple  package. You can use functions defined in this package
 to perform basic additions, subtractions, and multiplications of two numbers
 with add(), sub(), and multiply() respectively. 
+
+usage: ->>
+            from minsprojectr import operations
+        
+            given two integers 'a' and 'b', provided methods are
+            add(a,b), sub(a,b) and multiply(a,b)
```

### Comparing `minsprojectr-0.0.1/src/minsprojectr.egg-info/PKG-INFO` & `minsprojectr-0.0.2/src/minsprojectr.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 Metadata-Version: 2.1
 Name: minsprojectr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package for basic mathematical operations
 Author-email: Sai <sai275stw@gamil.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #  Package
 
 This is a simple  package. You can use functions defined in this package
 to perform basic additions, subtractions, and multiplications of two numbers
 with add(), sub(), and multiply() respectively. 
+
+usage: ->>
+            from minsprojectr import operations
+        
+            given two integers 'a' and 'b', provided methods are
+            add(a,b), sub(a,b) and multiply(a,b)
```

