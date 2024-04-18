# Comparing `tmp/robotframework-xlibrary-11.0.0.tar.gz` & `tmp/robotframework-xlibrary-11.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\robotframework-xlibrary-11.0.0.tar", last modified: Wed Apr 17 07:36:25 2024, max compression
+gzip compressed data, was "dist\robotframework-xlibrary-11.0.1.tar", last modified: Wed Apr 17 10:25:38 2024, max compression
```

## Comparing `robotframework-xlibrary-11.0.0.tar` & `robotframework-xlibrary-11.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/
--rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.0/LICENSE
--rw-rw-rw-   0        0        0     1588 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-11.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-04-17 07:35:37.000000 robotframework-xlibrary-11.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/XLibrary/
--rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.0/src/XLibrary/__init__.py
--rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.0/src/XLibrary/main.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/
--rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/__init__.py
--rw-rw-rw-   0        0        0     4248 2024-04-11 04:31:16.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/module1.py
--rw-rw-rw-   0        0        0     5643 2024-04-17 07:20:47.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/
--rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/__init__.py
--rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/module1.py
--rw-rw-rw-   0        0        0      261 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/module2.py
-drwxrwxrwx   0        0        0        0 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/
--rw-rw-rw-   0        0        0     1588 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-17 07:36:25.000000 robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/
+-rw-rw-rw-   0        0        0        0 2024-03-13 03:39:44.000000 robotframework-xlibrary-11.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1588 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-03-18 09:46:55.000000 robotframework-xlibrary-11.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      783 2024-04-17 10:19:07.000000 robotframework-xlibrary-11.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/XLibrary/
+-rw-rw-rw-   0        0        0     1114 2024-04-17 07:26:57.000000 robotframework-xlibrary-11.0.1/src/XLibrary/__init__.py
+-rw-rw-rw-   0        0        0      235 2024-03-18 09:34:26.000000 robotframework-xlibrary-11.0.1/src/XLibrary/main.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule1/
+-rw-rw-rw-   0        0        0      108 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule1/__init__.py
+-rw-rw-rw-   0        0        0     1601 2024-04-17 10:17:57.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule1/module1.py
+-rw-rw-rw-   0        0        0     5479 2024-04-17 10:24:52.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule1/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule2/
+-rw-rw-rw-   0        0        0      114 2024-03-18 09:34:30.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule2/__init__.py
+-rw-rw-rw-   0        0        0     1774 2024-04-13 12:59:03.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule2/module1.py
+-rw-rw-rw-   0        0        0      261 2024-04-17 10:18:54.000000 robotframework-xlibrary-11.0.1/src/XLibrary/submodule2/module2.py
+drwxrwxrwx   0        0        0        0 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/
+-rw-rw-rw-   0        0        0     1588 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-17 10:25:38.000000 robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/top_level.txt
```

### Comparing `robotframework-xlibrary-11.0.0/PKG-INFO` & `robotframework-xlibrary-11.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.0
+Version: 11.0.1
 Summary: Test Custom Library robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.0/README.md` & `robotframework-xlibrary-11.0.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.0/setup.py` & `robotframework-xlibrary-11.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="robotframework-xlibrary",
-    version="11.0.0",
+    version="11.0.1",
     author="Tassana Khrueawan",
     author_email="tassana.khr@gmail.com",
     description="Test Custom Library robotframework-xlibrary",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Khrx1999/robotframework-xlibrary.git",
     package_dir={'': 'src'},
```

### Comparing `robotframework-xlibrary-11.0.0/src/XLibrary/__init__.py` & `robotframework-xlibrary-11.0.1/src/XLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.0/src/XLibrary/submodule1/module2.py` & `robotframework-xlibrary-11.0.1/src/XLibrary/submodule1/module2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pymongo
 import logging
 
 class XDrint:
     def CDCDCD(self):
         print("Hello, world! เทสภาษาไทย222")
 
-    @keyword("Connect Mongodb With URL")
+    @keyword("XConnect Mongodb With URL")
     def connect_to_mongodb_with_uri(self, dbURI, timeout=10):
         """
         ***|    Description     |***
         | *`Connect Mongodb With URL`* | เป็น Keyword ไว้เชื่อมต่อกับ MongoDB โดยใช้ URI โดยเฉพาะ |
 
         
         ***|    Example     |***
@@ -34,79 +34,95 @@
         except pymongo.errors.ServerSelectionTimeoutError as e:
             logging.error("| Fail: การเชื่อมต่อ MongoDB ล้มเหลว เนื่องจาก TimeOut | %s |" % str(e))
             raise Exception("การเชื่อมต่อ MongoDB ล้มเหลว เนื่องจาก TimeOut")
         except Exception as e:
             logging.error("| Fail: การเชื่อมต่อ MongoDB ล้มเหลว | %s |" % str(e))
             raise Exception("การเชื่อมต่อ MongoDB ล้มเหลว: " + str(e))
     
-    @keyword("Query MongoDB")
+    @keyword("XQuery MongoDB")
     def query_mongodb(self, database_name, collection_name, query):
         """
         ***|    Description     |***
         |   *`Query MongoDB`*   |   เป็น Keyword สำหรับ Query ข้อมูลใน Collection จะได้ทั้งก้อนออกมา |
 
         
         ***|    Example     |***
         | *`${result}`* | *`Query MongoDB`* | *`database_name`* | *`collection_name`* | *`Command Query`* | 
         | *`Log`* | *`${result}`* |
 
 
         ***|    Parameters     |***
             - **`database_name`**  Database NAME.
             - **`collection_name`**  Collection NAME.
-	    - **`query`**  คำสั่ง Query.
+	        - **`query`**  คำสั่ง Query.
 
 
         *`Create By Tassana Khrueawan`*
         """
         collection = self._dbconnection[database_name][collection_name]
         query_dict = ast.literal_eval(query)
         result = collection.find(query_dict)
         return list(result)
       
     
-    @keyword("Query Dynamic Characteristic Value")
-    def query_dynamic_characteristic_value(self, result_list, key='None', characteristic_name=None):
+    @keyword("XQuery Dynamic Value")
+    def query_dynamic_value(self, result, field='None', value='None', expect=None):
         """
-        ***คำอธิบาย Description***
-        |   Query Dynamic Characteristic Value   |   Keyword สำหรับ Query ข้อมูลใน key ที่กำหนดและได้ Value ของลักษณะที่ต้องการ |
+        ***|    Description     |***
+        |   *`XQuery Dynamic Value`*   |   เป็น Keyword สำหรับ Query ข้อมูลใน Collection แบบเจาะลงไป |
+
+        
+        ***|    Example     |***
+        | *`${arpu_value}`* | *`XQuery Dynamic Value`* | *`result`* | *`productCharacteristic`* | *`name`* | *`arpu`* |
+        | *`Log`* | *`${arpu_value}`* |
+
+        
+        ***|    Parameters     |***
+            - **`result`**  ยังไม่ได้ใส่รายละเอียด
+            - **`field`**   ยังไม่ได้ใส่รายละเอียด
+            - **`value`**   ยังไม่ได้ใส่รายละเอียด
+	        - **`expect`**  ยังไม่ได้ใส่รายละเอียด
+
 
-        ***ตัวอย่างการใช้งาน Example***
-        | ${value} =  Query Dynamic Characteristic Value  ${result}  key  characteristic_name |
-        | key คือชื่อของ field ที่มีลักษณะสินค้า เช่น productCharacteristic |
-        | characteristic_name เช่น number, ratingType, arpu หรือเป็น None ถ้าต้องการทั้ง object |
-        | Log  ${value} |
-        """
-        for item in result_list:
-            if key in item and isinstance(item[key], list):
-                if characteristic_name:
-                    for char in item[key]:
-                        if char.get('name') == characteristic_name:
+        *`Create By Tassana Khrueawan`*
+        """
+        for item in result:
+            if field in item and isinstance(item[field], list):
+                if expect:
+                    for char in item[field]:
+                        if char.get(value) == expect:
                             return char.get('value')
                 else:
-                    return item[key]
-        return None  
+                    return item[field]
+        return None
 
-    @keyword("Query Specific Field Value")
-    def query_specific_field_value(self, document, field_name=None):
+    @keyword("XQuery Specific Value")
+    def query_specific_value(self, result, field_name=None):
         """
-        ***คำอธิบาย Description***
-        |   Query Specific Field Value   |   Keyword สำหรับ Query ข้อมูลจาก field ที่กำหนดใน document |
+        ***|    Description     |***
+        |   XQuery Specific Value   |   Keyword สำหรับ Query ข้อมูลใน Collection แบบไม่เจาะลงไป |
+
+        
+        ***|    Example     |***
+        | *`${name}`* | *`XQuery Specific Value`* | *`result`* | *`name`* |
+        | *`Log`* | *`${name}`* |
+
 
-        ***ตัวอย่างการใช้งาน Example***
-        | ${value} = Query Specific Field Value ${document} field_name |
-        | field_name เป็นชื่อของ field ที่ต้องการค่า เช่น name, status, productCharacteristic เป็นต้น |
-        | หากไม่ระบุ field_name จะ return ทั้ง document |
-        | Log ${value} |
+        ***|    Parameters     |***
+            - **`result`**  ยังไม่ได้ใส่รายละเอียด
+            - **`field_name`**   ยังไม่ได้ใส่รายละเอียด
+
+
+        *`Create By Tassana Khrueawan`*
         """
-        # Return the whole document if no field_name is provided
         if not field_name:
-            return document
-        
-        # If field_name is provided, navigate through the document to find the value
-        value = document.get(field_name, None)
+            return result
 
-        # If field_name refers to a list of dictionaries, we may need to handle it differently
-        if isinstance(value, list) and all(isinstance(item, dict) for item in value):
-            return [item.get('value', None) for item in value if 'value' in item]
+        results = []
+        if isinstance(result, list):
+            for doc in result:
+                if isinstance(doc, dict) and field_name in doc:
+                    results.append(doc[field_name])
+        else:
+            results = result.get(field_name, None)
 
-        return value
+        return results
```

### Comparing `robotframework-xlibrary-11.0.0/src/XLibrary/submodule2/module1.py` & `robotframework-xlibrary-11.0.1/src/XLibrary/submodule2/module1.py`

 * *Files identical despite different names*

### Comparing `robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/PKG-INFO` & `robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-xlibrary
-Version: 11.0.0
+Version: 11.0.1
 Summary: Test Custom Library robotframework-xlibrary
 Home-page: https://github.com/Khrx1999/robotframework-xlibrary.git
 Author: Tassana Khrueawan
 Author-email: tassana.khr@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotframework-xlibrary-11.0.0/src/robotframework_xlibrary.egg-info/SOURCES.txt` & `robotframework-xlibrary-11.0.1/src/robotframework_xlibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

