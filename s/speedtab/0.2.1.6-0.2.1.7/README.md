# Comparing `tmp/speedtab-0.2.1.6.tar.gz` & `tmp/speedtab-0.2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speedtab-0.2.1.6.tar", max compression
+gzip compressed data, was "speedtab-0.2.1.7.tar", max compression
```

## Comparing `speedtab-0.2.1.6.tar` & `speedtab-0.2.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      567 2024-04-16 07:50:48.088234 speedtab-0.2.1.6/pyproject.toml
--rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.6/speedtab/__init__.py
--rw-r--r--   0        0        0    86804 2024-04-16 07:50:34.216380 speedtab-0.2.1.6/speedtab/client.py
--rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.6/speedtab/enums.py
--rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.6/speedtab/formats.py
--rw-r--r--   0        0        0      783 2024-04-16 07:50:57.741227 speedtab-0.2.1.6/setup.py
--rw-r--r--   0        0        0      808 2024-04-16 07:50:57.741227 speedtab-0.2.1.6/PKG-INFO
+-rw-r--r--   0        0        0      567 2024-04-18 12:03:05.895234 speedtab-0.2.1.7/pyproject.toml
+-rw-r--r--   0        0        0      382 2023-12-14 09:13:27.273500 speedtab-0.2.1.7/speedtab/__init__.py
+-rw-r--r--   0        0        0    86935 2024-04-18 12:02:53.687448 speedtab-0.2.1.7/speedtab/client.py
+-rw-r--r--   0        0        0     7739 2023-12-14 09:47:11.439768 speedtab-0.2.1.7/speedtab/enums.py
+-rw-r--r--   0        0        0     1824 2023-12-14 09:47:11.343768 speedtab-0.2.1.7/speedtab/formats.py
+-rw-r--r--   0        0        0      783 2024-04-18 12:03:13.567006 speedtab-0.2.1.7/setup.py
+-rw-r--r--   0        0        0      808 2024-04-18 12:03:13.567006 speedtab-0.2.1.7/PKG-INFO
```

### Comparing `speedtab-0.2.1.6/pyproject.toml` & `speedtab-0.2.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "speedtab"
-version = "0.2.1.6"
+version = "0.2.1.7"
 description = "Convenient wrapper for working with Google Spreadsheets"
 authors = ["Bogdan Gergel <bogger147@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/BoggerSancho/SpeedTab-beta"
 repository = "https://github.com/BoggerSancho/SpeedTab-beta"
 
 [tool.poetry.dependencies]
```

### Comparing `speedtab-0.2.1.6/speedtab/client.py` & `speedtab-0.2.1.7/speedtab/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,15 +350,15 @@
                         'requests': batch_update_list
                     }}).execute()
 
             if batch_update_data_list:
                 self.connect_v4.spreadsheets().values().batchUpdate(**{
                     'spreadsheetId': self.spreadsheet_id,
                     'body': {
-                        'valueInputOption': 'RAW',
+                        'valueInputOption': 'USER_ENTERED',
                         'data': batch_update_data_list,
                     }}).execute()
         if batch_update_chart_list:
             self.connect_v4.spreadsheets().batchUpdate(**{
                 'spreadsheetId': self.spreadsheet_id,
                 'body': {
                     'requests': batch_update_chart_list
@@ -1036,25 +1036,27 @@
                 .get(spreadsheetId=self.base.spreadsheet_id,
                      ranges=[self.data_cell],
                      includeGridData=True
                      )
                 .execute()['sheets'][0]['data'][0].get('rowData', [])
                 )
 
-    def read_dataframe(self, header_lines: int = 0):
+    def read_dataframe(self, header_lines: int = 1):
         """Takes a cell range as an input, reads cell values and turns them in a pandas DataFrame.
 
         :param header_lines: A range must have a header. The method supports multi-index header rows (not columns!), defaults to 0.
         :return: A pandas DataFrame object.
         """
         rows = self.read_values()
-        if header_lines is None:
+        if header_lines is None or header_lines == 0:
             return pd.DataFrame(data=rows, columns=None)
+        elif header_lines == 1:
+            return pd.DataFrame(data=rows[header_lines:], columns=rows[0])
         else:
-            return pd.DataFrame(data=rows[header_lines + 1:], columns=rows[0:header_lines + 1])
+            return pd.DataFrame(data=rows[header_lines:], columns=rows[0:header_lines])
 
     def read_values(self, formated_values: bool = True):
         """Takes a cell range as an input, and returns a list of lists (per row in the selected range).
         By default, inner lists will contain values in a string format as it preserves the formatting. For instance,
         if the column number is in the dollar format, it will return "$49.09" instead of a float 49.09. To get the
         actual values set formatted_values to False.
```

### Comparing `speedtab-0.2.1.6/speedtab/enums.py` & `speedtab-0.2.1.7/speedtab/enums.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.6/speedtab/formats.py` & `speedtab-0.2.1.7/speedtab/formats.py`

 * *Files identical despite different names*

### Comparing `speedtab-0.2.1.6/setup.py` & `speedtab-0.2.1.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['google-api-python-client>=2.58.0,<3.0.0',
  'google-auth-httplib2>=0.1.0,<0.2.0',
  'google-auth-oauthlib>=0.5.2,<0.6.0']
 
 setup_kwargs = {
     'name': 'speedtab',
-    'version': '0.2.1.6',
+    'version': '0.2.1.7',
     'description': 'Convenient wrapper for working with Google Spreadsheets',
     'long_description': None,
     'author': 'Bogdan Gergel',
     'author_email': 'bogger147@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/BoggerSancho/SpeedTab-beta',
```

### Comparing `speedtab-0.2.1.6/PKG-INFO` & `speedtab-0.2.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speedtab
-Version: 0.2.1.6
+Version: 0.2.1.7
 Summary: Convenient wrapper for working with Google Spreadsheets
 Home-page: https://github.com/BoggerSancho/SpeedTab-beta
 License: MIT
 Author: Bogdan Gergel
 Author-email: bogger147@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

