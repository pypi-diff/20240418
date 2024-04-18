# Comparing `tmp/submit4dn-4.0.1.tar.gz` & `tmp/submit4dn-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "submit4dn-4.0.1.tar", max compression
+gzip compressed data, was "submit4dn-4.0.2.tar", max compression
```

## Comparing `submit4dn-4.0.1.tar` & `submit4dn-4.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1083 2023-12-07 20:55:25.462065 submit4dn-4.0.1/LICENSE.txt
--rw-r--r--   0        0        0     7905 2023-12-07 20:55:25.462065 submit4dn-4.0.1/README.md
--rw-r--r--   0        0        0      935 2023-12-07 20:55:25.466065 submit4dn-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-07 20:55:25.470065 submit4dn-4.0.1/wranglertools/__init__.py
--rwxr-xr-x   0        0        0    22110 2023-12-07 20:55:25.470065 submit4dn-4.0.1/wranglertools/get_field_info.py
--rwxr-xr-x   0        0        0    71670 2023-12-07 20:55:25.474065 submit4dn-4.0.1/wranglertools/import_data.py
--rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 submit4dn-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-18 19:14:22.106597 submit4dn-4.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     7905 2024-04-18 19:14:22.106597 submit4dn-4.0.2/README.md
+-rw-r--r--   0        0        0      935 2024-04-18 19:14:22.110597 submit4dn-4.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 19:14:22.114597 submit4dn-4.0.2/wranglertools/__init__.py
+-rwxr-xr-x   0        0        0    22110 2024-04-18 19:14:22.118597 submit4dn-4.0.2/wranglertools/get_field_info.py
+-rwxr-xr-x   0        0        0    71618 2024-04-18 19:14:22.118597 submit4dn-4.0.2/wranglertools/import_data.py
+-rw-r--r--   0        0        0     8781 1970-01-01 00:00:00.000000 submit4dn-4.0.2/PKG-INFO
```

### Comparing `submit4dn-4.0.1/LICENSE.txt` & `submit4dn-4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `submit4dn-4.0.1/README.md` & `submit4dn-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `submit4dn-4.0.1/pyproject.toml` & `submit4dn-4.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Submit4DN"
-version = "4.0.1"
+version = "4.0.2"
 description = "Utility package for submitting data to the 4DN Data Portal"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/4dn-dcic/Submit4DN"
 repository = "https://github.com/4dn-dcic/Submit4DN"
 packages = [
```

### Comparing `submit4dn-4.0.1/wranglertools/get_field_info.py` & `submit4dn-4.0.2/wranglertools/get_field_info.py`

 * *Files identical despite different names*

### Comparing `submit4dn-4.0.1/wranglertools/import_data.py` & `submit4dn-4.0.2/wranglertools/import_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -789,28 +789,26 @@
             else:
                 # deal with errors about linked objects not in db - checking for those with
                 # aliases present in the workbook that should be ignored
                 utrl_txt = 'Unable to resolve link:'
                 nf_txt = 'not found'
                 not_found = None
                 alias_bit = None
-                if error_id:
-                    alias_bit = error_id
-                elif utrl_txt in error_description:
+                if utrl_txt in error_description:
                     alias_bit = error_description.replace(utrl_txt, '')
                 elif error_description.endswith(nf_txt):
                     alias_bit = error_description.replace(nf_txt, '').replace("'", '')
                 if alias_bit:
                     not_found = alias_bit.strip()
                 # ignore ones about existing aliases
                 if not_found and not_found in all_aliases:
                     continue
                 error_field = err['name']
-                report.append("{sheet:<30}Field '{er}': {des}"
-                              .format(er=error_field, des=error_description, sheet="ERROR " + sheet.lower()))
+                report.append("{sheet:<30}{eid} Field '{er}': {des}"
+                              .format(er=error_field, des=error_description, eid=error_id, sheet="ERROR " + sheet.lower()))
     # if there is a an access forbidden error
     elif error_dic.get('title') == 'Forbidden':
         error_description = error_dic['description']
         try:
             report.append("{sheet:<30}{eid}: {des}"
                           .format(des=error_description, eid=error_id, sheet="ERROR " + sheet.lower()))
         except Exception:
```

### Comparing `submit4dn-4.0.1/PKG-INFO` & `submit4dn-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: submit4dn
-Version: 4.0.1
+Version: 4.0.2
 Summary: Utility package for submitting data to the 4DN Data Portal
 Home-page: https://github.com/4dn-dcic/Submit4DN
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.0,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

