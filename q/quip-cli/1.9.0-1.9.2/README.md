# Comparing `tmp/quip-cli-1.9.0.tar.gz` & `tmp/quip-cli-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quip-cli-1.9.0.tar", last modified: Mon Apr 15 22:08:12 2024, max compression
+gzip compressed data, was "quip-cli-1.9.2.tar", last modified: Thu Apr 18 17:29:18 2024, max compression
```

## Comparing `quip-cli-1.9.0.tar` & `quip-cli-1.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-15 22:08:12.881988 quip-cli-1.9.0/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27949 2024-04-15 22:08:12.881753 quip-cli-1.9.0/PKG-INFO
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27549 2023-08-18 17:30:20.000000 quip-cli-1.9.0/README.md
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.9.0/pyproject.toml
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-15 22:08:12.878738 quip-cli-1.9.0/quip/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2277 2024-04-15 21:16:21.000000 quip-cli-1.9.0/quip/__init__.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.9.0/quip/external.py
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5307 2023-08-21 16:56:55.000000 quip-cli-1.9.0/quip/fact.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    22972 2024-04-15 21:45:23.000000 quip-cli-1.9.0/quip/field_builder.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    74251 2023-08-21 18:36:06.000000 quip-cli-1.9.0/quip/quip.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.9.0/quip/version_builder.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-15 22:08:12.881311 quip-cli-1.9.0/quip_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27949 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      333 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2024-04-15 22:08:12.000000 quip-cli-1.9.0/quip_cli.egg-info/top_level.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-15 22:08:12.882028 quip-cli-1.9.0/setup.cfg
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.9.0/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-18 17:29:18.822640 quip-cli-1.9.2/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29453 2024-04-18 17:29:18.822402 quip-cli-1.9.2/PKG-INFO
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29053 2024-04-16 13:47:26.000000 quip-cli-1.9.2/README.md
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.9.2/pyproject.toml
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-18 17:29:18.819697 quip-cli-1.9.2/quip/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2277 2024-04-18 17:29:08.000000 quip-cli-1.9.2/quip/__init__.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.9.2/quip/external.py
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     5307 2023-08-21 16:56:55.000000 quip-cli-1.9.2/quip/fact.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    25603 2024-04-18 17:15:32.000000 quip-cli-1.9.2/quip/field_builder.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    74410 2024-04-16 14:28:06.000000 quip-cli-1.9.2/quip/quip.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.9.2/quip/version_builder.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2024-04-18 17:29:18.822041 quip-cli-1.9.2/quip_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    29453 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      333 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2024-04-18 17:29:18.000000 quip-cli-1.9.2/quip_cli.egg-info/top_level.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2024-04-18 17:29:18.822687 quip-cli-1.9.2/setup.cfg
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.9.2/setup.py
```

### Comparing `quip-cli-1.9.0/PKG-INFO` & `quip-cli-1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.9.0
+Version: 1.9.2
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -505,14 +505,18 @@
 template_type: Extension
 agent_type: Any
 description: AWS M2 - Mainframe Modernization
 extension: aws-m2
 min_release: 7.0.0.0
 var_prefix: ext
 sys_id: fb7fc3a05eac4d57a74fe1b1342b3938
+common_script: false
+always_cancel: true
+send_environment: Launch, Dynamic Choice
+send_variables: Local
 fields:
 
 - action: Choice
   hint: Select the action you want to run
   start: true
   field_mapping: Choice Field 1
   items:
@@ -522,21 +526,24 @@
   - sync-start-batch
 
 - credentials: Credential
   hint: Put Access key to Runtime User and Secret Key to Password fields
   label: AWS Credentials
   end: true
   field_mapping: Credential Field 1
+  allow_variable: true
+  span: 2
 
 - end_point: Text
   hint: This field is optional. If you don't put the value it will be generated by
     using the region value.
   start: true
   default: https://m2.us-east-1.amazonaws.com
   field_mapping: Text Field 4
+  regex: http.*
 
 - application: Choice
   hint: Application will be retrieved from AWS automatically
   span: 2
   dynamic: true
   field_mapping: Choice Field 2
   items: []
@@ -564,28 +571,44 @@
   values:
   - task_name
   - template: Value
   - variable_1: Value 1
   - variable_2: Value 2
 
 ```
+Fields of Universal Template definitions:
+* name: Name of the template
+* template_type: Type of the template. Extension | Script
+* agent_type: Agent Type of the template. Any | Linux | Windows
+* description: Description of the template
+* extension: Name of the extension. This name should be same as the value in extension.yml file
+* min_release: Min release of the extension. Change this value based on the api level of extension.yml file. Example: 7.0.0.0
+* var_prefix: Prefix of the extension. There is a length limit. Keep it less than 32 chars. Example: ext
+* sys_id: Uniq ID of the template. Example: fb7fc3a05eac4d57a74fe1b1342b3938
+* common_script: Only for script type templates. true|false
+* script_ext_windows: The extension of the script on Windows: py | uapy | bat
+* always_cancel: Cancel on Force Finish. true|false
+* send_environment: To send environment variables to template: Launch [, Dynamic Choice][, Dynamic Command] | All | Yes|No | true|false
+* send_variables: To send the variables to the template: Local | Yes|No | True|false
 
 Format of the child elements are like this.
 
 * First value will be the name of the field and the value of that element will be the type of the field.
 * Field Types can be one of these items
     * Text
     * Large Text (aliases: large, largetext, textarea, text area)
     * Integer
     * Boolean (aliases: bool, check, checkbox, check box)
     * Choice (aliases: items, select, option, options, list)
     * Credential (aliases: creds, cred, credentials)
     * Script
     * Array (aliases: grid)
     * Float
+    * Sap Connection 
+    * Database Connection
 * Other Fields:
     * label: By default field name will be converted as a label but if you want to overwrite that value you can use that field
     * hint: The hint message of the field
     * field_mapping: This is the mapping for the database fields. If this value is missing, quip will automatically assign the next available field. It is safe to not provide this value for new extension/template. The assigned values will be automatically added to the file.
     * default: If there is a default value, you can use that field. 
     * required: If the field is required, you can use that field. Default: false
     * start: If you want the field to be in the left side of the row, set value to true. Default: false
@@ -596,14 +619,16 @@
     * restriction: If the field has restrictions like output only, set the value to "Output Only". Default: No Restriction
     * name_title: This field is only for Array types. This field is the label of the first field.
     * value_title: This field is only for Array types. This field is the label of the second field.
     * titles: (alias: headers) This field is another representation of the name_title and value_title fields. You can set the name and value field title in a comma seperated string. For example: `titles: Field Name, Field Value`
     * values: Default values of an Array field.
     * allow_multiple: This field is only for Choice types. To allow selecting multiple values, set value to true. Default: false
     * allow_empty: This field is only for Choice types. To allow not selecting any value, set value to true. Default: false
+    * allow_variable: This field is only for credential. To allow adding variable option for credentials, set value to true. Default: false
+    * regex: This field is only for text fields. It will add validation with regular expression to text fields.
     * length: Sets the max lenght of the field.
     * max: Sets the maximum allowed number for that field.
     * min: Set the minimum allowed number for that field.
     
     ### items
     This field is required for Choice type. This field will include the items of the choice field. Items can be a simple string without a space and it will be used as the name of the item and label will be generated from the names. If you want to give a specific label, in this case set it like this. `- use_ssl: Use SSL`
```

### Comparing `quip-cli-1.9.0/README.md` & `quip-cli-1.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -493,14 +493,18 @@
 template_type: Extension
 agent_type: Any
 description: AWS M2 - Mainframe Modernization
 extension: aws-m2
 min_release: 7.0.0.0
 var_prefix: ext
 sys_id: fb7fc3a05eac4d57a74fe1b1342b3938
+common_script: false
+always_cancel: true
+send_environment: Launch, Dynamic Choice
+send_variables: Local
 fields:
 
 - action: Choice
   hint: Select the action you want to run
   start: true
   field_mapping: Choice Field 1
   items:
@@ -510,21 +514,24 @@
   - sync-start-batch
 
 - credentials: Credential
   hint: Put Access key to Runtime User and Secret Key to Password fields
   label: AWS Credentials
   end: true
   field_mapping: Credential Field 1
+  allow_variable: true
+  span: 2
 
 - end_point: Text
   hint: This field is optional. If you don't put the value it will be generated by
     using the region value.
   start: true
   default: https://m2.us-east-1.amazonaws.com
   field_mapping: Text Field 4
+  regex: http.*
 
 - application: Choice
   hint: Application will be retrieved from AWS automatically
   span: 2
   dynamic: true
   field_mapping: Choice Field 2
   items: []
@@ -552,28 +559,44 @@
   values:
   - task_name
   - template: Value
   - variable_1: Value 1
   - variable_2: Value 2
 
 ```
+Fields of Universal Template definitions:
+* name: Name of the template
+* template_type: Type of the template. Extension | Script
+* agent_type: Agent Type of the template. Any | Linux | Windows
+* description: Description of the template
+* extension: Name of the extension. This name should be same as the value in extension.yml file
+* min_release: Min release of the extension. Change this value based on the api level of extension.yml file. Example: 7.0.0.0
+* var_prefix: Prefix of the extension. There is a length limit. Keep it less than 32 chars. Example: ext
+* sys_id: Uniq ID of the template. Example: fb7fc3a05eac4d57a74fe1b1342b3938
+* common_script: Only for script type templates. true|false
+* script_ext_windows: The extension of the script on Windows: py | uapy | bat
+* always_cancel: Cancel on Force Finish. true|false
+* send_environment: To send environment variables to template: Launch [, Dynamic Choice][, Dynamic Command] | All | Yes|No | true|false
+* send_variables: To send the variables to the template: Local | Yes|No | True|false
 
 Format of the child elements are like this.
 
 * First value will be the name of the field and the value of that element will be the type of the field.
 * Field Types can be one of these items
     * Text
     * Large Text (aliases: large, largetext, textarea, text area)
     * Integer
     * Boolean (aliases: bool, check, checkbox, check box)
     * Choice (aliases: items, select, option, options, list)
     * Credential (aliases: creds, cred, credentials)
     * Script
     * Array (aliases: grid)
     * Float
+    * Sap Connection 
+    * Database Connection
 * Other Fields:
     * label: By default field name will be converted as a label but if you want to overwrite that value you can use that field
     * hint: The hint message of the field
     * field_mapping: This is the mapping for the database fields. If this value is missing, quip will automatically assign the next available field. It is safe to not provide this value for new extension/template. The assigned values will be automatically added to the file.
     * default: If there is a default value, you can use that field. 
     * required: If the field is required, you can use that field. Default: false
     * start: If you want the field to be in the left side of the row, set value to true. Default: false
@@ -584,14 +607,16 @@
     * restriction: If the field has restrictions like output only, set the value to "Output Only". Default: No Restriction
     * name_title: This field is only for Array types. This field is the label of the first field.
     * value_title: This field is only for Array types. This field is the label of the second field.
     * titles: (alias: headers) This field is another representation of the name_title and value_title fields. You can set the name and value field title in a comma seperated string. For example: `titles: Field Name, Field Value`
     * values: Default values of an Array field.
     * allow_multiple: This field is only for Choice types. To allow selecting multiple values, set value to true. Default: false
     * allow_empty: This field is only for Choice types. To allow not selecting any value, set value to true. Default: false
+    * allow_variable: This field is only for credential. To allow adding variable option for credentials, set value to true. Default: false
+    * regex: This field is only for text fields. It will add validation with regular expression to text fields.
     * length: Sets the max lenght of the field.
     * max: Sets the maximum allowed number for that field.
     * min: Set the minimum allowed number for that field.
     
     ### items
     This field is required for Choice type. This field will include the items of the choice field. Items can be a simple string without a space and it will be used as the name of the item and label will be generated from the names. If you want to give a specific label, in this case set it like this. `- use_ssl: Use SSL`
```

### Comparing `quip-cli-1.9.0/quip/__init__.py` & `quip-cli-1.9.2/quip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from colorama import Fore, Style, init
 
 init()
 
-__version__ = "1.9.0"
+__version__ = "1.9.2"
 
 def cprint(text, color, end='\n', style='Normal'):
     if len(str(text).strip()) == 0: return
     fore = getattr(Fore, color.upper())
     style = getattr(Style, style.upper())
     print('{0}{1}{2}{3}'.format(fore, style, text, Style.RESET_ALL), end=end)
```

### Comparing `quip-cli-1.9.0/quip/external.py` & `quip-cli-1.9.2/quip/external.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.0/quip/fact.py` & `quip-cli-1.9.2/quip/fact.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.0/quip/field_builder.py` & `quip-cli-1.9.2/quip/field_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import uuid
 import copy
 
-def prepare_fields(fields, code):
+def prepare_fields(fields, code, code_type="simple"):
     numbers = {}
     available_fields = { 
         "Text": list(range(1, 21)),
         "Large Text": list(range(1, 5)),
         "Integer": list(range(1, 11)),
         "Boolean": list(range(1, 16)),
         "Choice": list(range(1, 16)),
@@ -35,15 +35,15 @@
 
     for field in fields:  # set field_mapping for the ones that doesn't have yet.
         name = list(field.keys())[0]
         type = list(field.values())[0]
         type = get_type_name(type)
         if code:
             if field.get("restriction", "") != "Output Only":
-                print_code_samples("field", name, type)
+                print_code_samples("field", name, type, format=code_type)
         _field_mapping = field.get("field_mapping", None)
         if _field_mapping is None:
             field_mapping[name] = f"{type} Field {available_fields[type].pop(0)}"
     if not code: 
         print(field_mapping)
 
     for field in fields:
@@ -65,15 +65,17 @@
         elif type == "Script":
             _dict = create_script_field(name, field_mapping[name], sequence)
         elif type == "Boolean":
             _dict = create_boolean_field(name, field_mapping[name], sequence)
         elif type == "Choice":
             if code:
                 if field.get("dynamic", False):
-                    print_code_samples("dynamic_choice", name)
+                    print_code_samples("dynamic_choice", name, format=code_type)
+                else:
+                    print_code_samples("choice", name, items=field.get("items", []), format=code_type)
             _dict = create_choice_field(name, field_mapping[name], sequence, field.get("items", []))
         elif type == "Array":
             if "titles" in field:
                 name_title, value_title = field["titles"].split(",")
             elif "headers" in field:
                 name_title, value_title = field["headers"].split(",")
             else:
@@ -108,17 +110,17 @@
     set_if_not_equal(result, "minReleaseLevel", conf.get("min_release", None), None)
     set_if_not_equal(result, "variablePrefix", conf.get("var_prefix", None), None)
     set_if_not_equal(result, "sysId", conf.get("sys_id", None), None)
     set_if_not_equal(result, "scriptTypeWindows", conf.get("script_ext_windows", None), None)
     set_if_not_equal(result, "useCommonScript", conf.get("common_script", None), None)
     set_if_not_equal(result, "alwaysCancelOnFinish", conf.get("always_cancel", None), None)
     set_if_not_equal(result, "sendEnvironment", conf.get("send_environment", "Launch"), "Launch")
-    if str(result["sendEnvironment"]).lower() in ["all", "yes", "true"]:
+    if str(result.get("sendEnvironment", "")).lower() in ["all", "yes", "true"]:
         result["sendEnvironment"] = "Launch, Dynamic Choice, Dynamic Command"
-    elif str(result["sendEnvironment"]).lower() in ["", "no", "false"]:
+    elif result.get("sendEnvironment", "").lower() in ["", "no", "false"]:
         result["sendEnvironment"] = "Launch"
     set_if_not_equal(result, "sendVariables", conf.get("send_variables", None), None)
     if str(result.get("sendVariables", "")).lower() in ["local", "yes", "true"]:
         result["sendVariables"] = "Local"
     elif str(result.get("sendVariables", "")).lower() in ["", "no", "false"]:
         result["sendVariables"] = None
 
@@ -282,114 +284,114 @@
 
     return dict
 
 def dump_fields(fields_json):
     fields = []
     reverse_field_mapping = {}
     for field_json in fields_json:
-        reverse_field_mapping[field_json["fieldMapping"]] = field_json["name"]
+        reverse_field_mapping[field_json.get("fieldMapping", None)] = field_json.get("name", None)
 
     for field_json in fields_json:
         field = {}
-        if field_json["fieldMapping"].startswith("Large Text"):
-            field[field_json["name"]] = "Large Text"
+        if field_json.get("fieldMapping", None).startswith("Large Text"):
+            field[field_json.get("name", None)] = "Large Text"
         else:
-            field[field_json["name"]] = field_json["fieldType"]
-        set_if_not_equal(field, "label", field_json["label"], labelize(field_json["name"]))
-        set_if_not_equal(field, "hint", field_json["hint"], None)
-        set_if_not_equal(field, "field_mapping", field_json["fieldMapping"], None)
-        set_if_not_equal(field, "default", field_json["fieldValue"], None)
-        set_if_not_equal(field, "required", field_json["required"], False)
-        set_if_not_equal(field, "start", field_json["formStartRow"], False)
-        set_if_not_equal(field, "end", field_json["formEndRow"], False)
-        set_if_not_equal(field, "span", field_json["formColumnSpan"], 1)
-        set_if_not_equal(field, "text_type", field_json["textType"], "Plain")
-        set_if_not_equal(field, "dynamic", field_json["choiceDynamic"], False)
-        set_if_not_equal(field, "restriction", field_json["fieldRestriction"], "No Restriction")
-        set_if_not_equal(field, "name_title", field_json["arrayNameTitle"], None)
-        set_if_not_equal(field, "value_title", field_json["arrayValueTitle"], None)
-        set_if_not_equal(field, "allow_multiple", field_json["choiceAllowMultiple"], False)
-        set_if_not_equal(field, "allow_empty", field_json["choiceAllowEmpty"], False)
-        set_if_not_equal(field, "length", field_json["fieldLength"], None)
-        set_if_not_equal(field, "max", field_json["intFieldMax"], None)
-        set_if_not_equal(field, "min", field_json["intFieldMin"], None)
+            field[field_json.get("name", None)] = field_json.get("fieldType", None)
+        set_if_not_equal(field, "label", field_json.get("label", None), labelize(field_json.get("name", None)))
+        set_if_not_equal(field, "hint", field_json.get("hint", None), None)
+        set_if_not_equal(field, "field_mapping", field_json.get("fieldMapping", None), None)
+        set_if_not_equal(field, "default", field_json.get("fieldValue", None), None)
+        set_if_not_equal(field, "required", field_json.get("required", None), False)
+        set_if_not_equal(field, "start", field_json.get("formStartRow", None), False)
+        set_if_not_equal(field, "end", field_json.get("formEndRow", None), False)
+        set_if_not_equal(field, "span", field_json.get("formColumnSpan", None), 1)
+        set_if_not_equal(field, "text_type", field_json.get("textType", None), "Plain")
+        set_if_not_equal(field, "dynamic", field_json.get("choiceDynamic", None), False)
+        set_if_not_equal(field, "restriction", field_json.get("fieldRestriction", None), "No Restriction")
+        set_if_not_equal(field, "name_title", field_json.get("arrayNameTitle", None), None)
+        set_if_not_equal(field, "value_title", field_json.get("arrayValueTitle", None), None)
+        set_if_not_equal(field, "allow_multiple", field_json.get("choiceAllowMultiple", None), False)
+        set_if_not_equal(field, "allow_empty", field_json.get("choiceAllowEmpty", None), False)
+        set_if_not_equal(field, "length", field_json.get("fieldLength", None), None)
+        set_if_not_equal(field, "max", field_json.get("intFieldMax", None), None)
+        set_if_not_equal(field, "min", field_json.get("intFieldMin", None), None)
 
-        if field_json["fieldType"] == "Text":
-            set_if_not_equal(field, "regex", field_json["fieldRegex"], None)
+        if field_json.get("fieldType", None) == "Text":
+            set_if_not_equal(field, "regex", field_json.get("fieldRegex", None), None)
 
-        if field_json["fieldType"] == "Credential":
-            set_if_not_equal(field, "allow_variable", field_json["allowVariable"], False)
+        if field_json.get("fieldType", None) == "Credential":
+            set_if_not_equal(field, "allow_variable", field_json.get("allowVariable", None), False)
 
-        if field_json["fieldType"] == "Array":
+        if field_json.get("fieldType", None) == "Array":
             field["values"] = []
-            for choice in field_json["arrayFieldValue"]:
+            for choice in field_json.get("arrayFieldValue", None):
                 if len(choice.get('value')) > 0:
                     field["values"].append({f"{choice.get('name')}": f"{choice.get('value')}"})
                 else:
                     field["values"].append(choice.get('name'))
         
-        if field_json["fieldType"] == "Choice":
+        if field_json.get("fieldType", None) == "Choice":
             field["items"] = []
-            for choice in field_json["choices"]:
+            for choice in field_json.get("choices", None):
                 if choice.get('fieldValueLabel') != labelize(choice.get('fieldValue')) and choice.get("useFieldValueForLabel") == False:
                     field["items"].append({f"{choice.get('fieldValue')}": f"{choice.get('fieldValueLabel')}"})     
                 elif choice.get("useFieldValueForLabel"):
                     field["items"].append({f"{choice.get('fieldValue')}": f"{choice.get('fieldValue')}"})
                 else:
                     field["items"].append(choice.get('fieldValue'))
 
-            if len(field_json["choiceFields"]) > 0:
+            if len(field_json.get("choiceFields", None)) > 0:
                 field["dependencies"] = []
-                for choice_field in field_json["choiceFields"]:
+                for choice_field in field_json.get("choiceFields", None):
                     if choice_field is None:
                         continue
                     field["dependencies"].append(reverse_field_mapping[choice_field])
 
-        if field_json["showIfField"] is not None:
+        if field_json.get("showIfField", None) is not None:
             field["show_if"] = {}
             show_if = field["show_if"]
-            show_if[reverse_field_mapping[field_json["showIfField"]]] = field_json["showIfFieldValue"]
-            set_if_not_equal(show_if, "no_space", field_json["noSpaceIfHidden"], True)
-            set_if_not_equal(show_if, "required", field_json["requireIfVisible"], False)
-            set_if_not_equal(show_if, "preserve_value", field_json["preserveValueIfHidden"], False)
+            show_if[reverse_field_mapping[field_json.get("showIfField", None)]] = field_json.get("showIfFieldValue", None)
+            set_if_not_equal(show_if, "no_space", field_json.get("noSpaceIfHidden", None), True)
+            set_if_not_equal(show_if, "required", field_json.get("requireIfVisible", None), False)
+            set_if_not_equal(show_if, "preserve_value", field_json.get("preserveValueIfHidden", None), False)
         
-        if field_json["requireIfField"] is not None:
+        if field_json.get("requireIfField", None) is not None:
             field["require_if"] = {}
             require_if = field["require_if"]
-            require_if[reverse_field_mapping[field_json["requireIfField"]]] = field_json["requireIfFieldValue"]
+            require_if[reverse_field_mapping[field_json.get("requireIfField", None)]] = field_json.get("requireIfFieldValue", None)
         
         raw_items = {}
-        set_if_not_equal(raw_items, "booleanNoValue", field_json["booleanNoValue"], None)
-        set_if_not_equal(raw_items, "booleanValueType", field_json["booleanValueType"], "true/false")
-        set_if_not_equal(raw_items, "booleanYesValue", field_json["booleanYesValue"], None)
-        set_if_not_equal(raw_items, "choiceSortOption", field_json["choiceSortOption"], "Sequence")
-        set_if_not_equal(raw_items, "defaultListView", field_json["defaultListView"], False)
-        set_if_not_equal(raw_items, "preserveOutputOnRerun", field_json["preserveOutputOnRerun"], False)
+        set_if_not_equal(raw_items, "booleanNoValue", field_json.get("booleanNoValue", None), None)
+        set_if_not_equal(raw_items, "booleanValueType", field_json.get("booleanValueType", None), "true/false")
+        set_if_not_equal(raw_items, "booleanYesValue", field_json.get("booleanYesValue", None), None)
+        set_if_not_equal(raw_items, "choiceSortOption", field_json.get("choiceSortOption", None), "Sequence")
+        set_if_not_equal(raw_items, "defaultListView", field_json.get("defaultListView", None), False)
+        set_if_not_equal(raw_items, "preserveOutputOnRerun", field_json.get("preserveOutputOnRerun", None), False)
         if len(raw_items) > 0:
             field["raw"] = raw_items
         fields.append(field)
     
     return fields
 
 
 def dump_template_fields(_json):
     result = {}
-    set_if_not_equal(result, "name", _json["name"], None)
-    set_if_not_equal(result, "template_type", _json["templateType"], None)
-    set_if_not_equal(result, "agent_type", _json["agentType"], None)
-    set_if_not_equal(result, "extension", _json["extension"], None)
-    set_if_not_equal(result, "min_release", _json["minReleaseLevel"], None)
-    set_if_not_equal(result, "var_prefix", _json["variablePrefix"], None)
-    set_if_not_equal(result, "sys_id", _json["sysId"], None)
-    set_if_not_equal(result, "script_ext_windows", _json["scriptTypeWindows"], None)
-    set_if_not_equal(result, "common_script", _json["useCommonScript"], None)
-    set_if_not_equal(result, "always_cancel", _json["alwaysCancelOnFinish"], None)
-    set_if_not_equal(result, "send_environment", _json["sendEnvironment"], None)
-    set_if_not_equal(result, "send_variables", _json["sendVariables"], None)
-    result["description"] = "" if _json["description"] is None else _json["description"]  # always show description
+    set_if_not_equal(result, "name", _json.get("name", None), None)
+    set_if_not_equal(result, "template_type", _json.get("templateType", None), None)
+    set_if_not_equal(result, "agent_type", _json.get("agentType", None), None)
+    set_if_not_equal(result, "extension", _json.get("extension", None), None)
+    set_if_not_equal(result, "min_release", _json.get("minReleaseLevel", None), None)
+    set_if_not_equal(result, "var_prefix", _json.get("variablePrefix", None), None)
+    set_if_not_equal(result, "sys_id", _json.get("sysId", None), None)
+    set_if_not_equal(result, "script_ext_windows", _json.get("scriptTypeWindows", None), None)
+    set_if_not_equal(result, "common_script", _json.get("useCommonScript", None), None)
+    set_if_not_equal(result, "always_cancel", _json.get("alwaysCancelOnFinish", None), None)
+    set_if_not_equal(result, "send_environment", _json.get("sendEnvironment", None), None)
+    set_if_not_equal(result, "send_variables", _json.get("sendVariables", None), None)
+    result["description"] = "" if _json.get("description", None) is None else _json.get("description", None)  # always show description
     return result
 
 def dump_events(events_json):
     events = []
     if events_json is None:
         return events
 
@@ -450,34 +452,70 @@
         return value 
     
     try:
         return value.strip()
     except:
         return value
 
-def print_code_samples(code_type, name, type=None):
+def print_code_samples(code_type, name, type=None, items=None, format="simple"):
     if code_type == "field":
-        if type == "Credential":
-            line = ('self.{name} = {{ "user": fields.get("{name}.user", None), "password": fields.get("{name}.password", None) }}'.format(name=name))
-        elif type == "Choice":
-            line = ("""self.{name} = fields.get("{name}", [None])[0]""".format(name=name))
-        elif type == "Boolean":
-            line = ("""self.{name} = fields.get("{name}", False)""".format(name=name))
-        else:
-            line = ("""self.{name} = fields.get("{name}", None)""".format(name=name))
+        if format == "simple":
+            if type == "Credential":
+                line = ('self.{name} = {{ "user": fields.get("{name}.user", None), "password": fields.get("{name}.password", None) }}'.format(name=name))
+            elif type == "Choice":
+                line = ("""self.{name} = get_first_element(fields.get("{name}", []), default=None)""".format(name=name))
+            elif type == "Boolean":
+                line = ("""self.{name} = fields.get("{name}", False)""".format(name=name))
+            else:
+                line = ("""self.{name} = fields.get("{name}", None)""".format(name=name))
+        elif format == "common":
+            if type == "Credential":
+                line = ('{name}: fields.Credential'.format(name=name))
+            elif type == "Choice":
+                if code_type == "dynamic_choice":
+                    line = '{name} : fields.DynamicChoice'.format(name=name)
+                else:
+                    line = ('{name}: {type}'.format(name=name, type=name.capitalize()))
+            elif type == "Boolean":
+                line = ('{name}: bool'.format(name=name))
+            elif type == "Text":
+                line = ('{name}: str'.format(name=name))
+            elif type == "Large Text":
+                line = ('{name}: str'.format(name=name))
+            elif type == "Integer":
+                line = ('{name}: int'.format(name=name))
+            elif type == "Array":
+                line = ('{name}: list'.format(name=name))
+            elif type == "Float":
+                line = ('{name}: float'.format(name=name))
+            elif type == "Sap Connection":
+                line = ('{name}: fields.SapConnection'.format(name=name))
+            elif type == "Database Connection":
+                line = ('{name}: fields.DatabaseConnection'.format(name=name))
+            else:
+                line = ('{name}: {type}'.format(name=name, type=type.lower()))
         print(line)
     if code_type == "dynamic_choice":
         print(f"@dynamic_choice_command(\"{name}\")")
         print(f"def get_{name}(self, fields):")
         print("    _fields = []")
         print("""    return ExtensionResult(
     rc = 0,
     message = "Available Fields: '{}'".format(_fields),
     values = _fields
     )""")
+    
+    if code_type == "choice":
+        print(f"\nclass {name.capitalize()}(Enum)")
+        if items is not None:
+            for item in items:
+                if isinstance(item, dict):
+                    print(f"    {list(item.keys())[0].upper()} = \"{list(item.keys())[0]}\"")
+                else:
+                    print(f"    {item.upper()} = \"{item}\"")
 
 FIELD_TEMPLATE = {
             "arrayFieldValue" : [ ],
             "arrayNameTitle" : None,
             "arrayValueTitle" : None,
             "booleanNoValue" : None,
             "booleanValueType" : "true/false",
```

### Comparing `quip-cli-1.9.0/quip/quip.py` & `quip-cli-1.9.2/quip/quip.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,17 +310,19 @@
         self._version_files = self.uip_global_config.get("version_files", None)
         self.default_template = self._global_conf_defaults.get("template", "ue-task")
         self.project_prefix = self._global_conf_defaults.get("project_prefix", None)
         self.project_name = self.format_ext_name(project_name)
         self.extension_name = self.project_folder_name = self.format_project_folder_name(project_name.lower(), self.args.template, self.project_prefix)
         self.template_name = self.titleize(project_name)
         self.use_keyring = self._global_conf_defaults.get("use_keyring", True)
+        self.code_type = self._global_conf_defaults.get("code_type", "simple")
         logging.debug(f"Project Name: {self.project_name}")
         logging.debug(f"Template Name: {self.template_name}")
         logging.debug(f"Folder Name: {self.project_folder_name}")
+        logging.debug(f"Code Type: {self.code_type}")
 
     def new_template(self):
         logging.info(f"creating new template {self.template_name}")
         if os.path.exists(self.project_folder_name):
             logging.error("Folder already exists")
             sys.exit(1)
 
@@ -691,15 +693,15 @@
         if os.path.exists(fields_path):
             with open(fields_path) as f:
                 conf = yaml.safe_load(f)
                 template_dict = fb.prepare_template_fields(conf)
                 new_fields = conf.get("fields", [])
                 
                 logging.debug("FIELDS: ", new_fields)
-                fields_dict = fb.prepare_fields(new_fields, code)
+                fields_dict = fb.prepare_fields(new_fields, code, code_type=self.code_type)
                 template_dict["fields"] = fields_dict
 
                 new_events = conf.get("events", [])
                 logging.debug("EVENTS: ", new_events)
                 events_dict = fb.prepare_event_fields(new_events)
                 template_dict["events"] = events_dict
```

### Comparing `quip-cli-1.9.0/quip/version_builder.py` & `quip-cli-1.9.2/quip/version_builder.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.9.0/quip_cli.egg-info/PKG-INFO` & `quip-cli-1.9.2/quip_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.9.0
+Version: 1.9.2
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -505,14 +505,18 @@
 template_type: Extension
 agent_type: Any
 description: AWS M2 - Mainframe Modernization
 extension: aws-m2
 min_release: 7.0.0.0
 var_prefix: ext
 sys_id: fb7fc3a05eac4d57a74fe1b1342b3938
+common_script: false
+always_cancel: true
+send_environment: Launch, Dynamic Choice
+send_variables: Local
 fields:
 
 - action: Choice
   hint: Select the action you want to run
   start: true
   field_mapping: Choice Field 1
   items:
@@ -522,21 +526,24 @@
   - sync-start-batch
 
 - credentials: Credential
   hint: Put Access key to Runtime User and Secret Key to Password fields
   label: AWS Credentials
   end: true
   field_mapping: Credential Field 1
+  allow_variable: true
+  span: 2
 
 - end_point: Text
   hint: This field is optional. If you don't put the value it will be generated by
     using the region value.
   start: true
   default: https://m2.us-east-1.amazonaws.com
   field_mapping: Text Field 4
+  regex: http.*
 
 - application: Choice
   hint: Application will be retrieved from AWS automatically
   span: 2
   dynamic: true
   field_mapping: Choice Field 2
   items: []
@@ -564,28 +571,44 @@
   values:
   - task_name
   - template: Value
   - variable_1: Value 1
   - variable_2: Value 2
 
 ```
+Fields of Universal Template definitions:
+* name: Name of the template
+* template_type: Type of the template. Extension | Script
+* agent_type: Agent Type of the template. Any | Linux | Windows
+* description: Description of the template
+* extension: Name of the extension. This name should be same as the value in extension.yml file
+* min_release: Min release of the extension. Change this value based on the api level of extension.yml file. Example: 7.0.0.0
+* var_prefix: Prefix of the extension. There is a length limit. Keep it less than 32 chars. Example: ext
+* sys_id: Uniq ID of the template. Example: fb7fc3a05eac4d57a74fe1b1342b3938
+* common_script: Only for script type templates. true|false
+* script_ext_windows: The extension of the script on Windows: py | uapy | bat
+* always_cancel: Cancel on Force Finish. true|false
+* send_environment: To send environment variables to template: Launch [, Dynamic Choice][, Dynamic Command] | All | Yes|No | true|false
+* send_variables: To send the variables to the template: Local | Yes|No | True|false
 
 Format of the child elements are like this.
 
 * First value will be the name of the field and the value of that element will be the type of the field.
 * Field Types can be one of these items
     * Text
     * Large Text (aliases: large, largetext, textarea, text area)
     * Integer
     * Boolean (aliases: bool, check, checkbox, check box)
     * Choice (aliases: items, select, option, options, list)
     * Credential (aliases: creds, cred, credentials)
     * Script
     * Array (aliases: grid)
     * Float
+    * Sap Connection 
+    * Database Connection
 * Other Fields:
     * label: By default field name will be converted as a label but if you want to overwrite that value you can use that field
     * hint: The hint message of the field
     * field_mapping: This is the mapping for the database fields. If this value is missing, quip will automatically assign the next available field. It is safe to not provide this value for new extension/template. The assigned values will be automatically added to the file.
     * default: If there is a default value, you can use that field. 
     * required: If the field is required, you can use that field. Default: false
     * start: If you want the field to be in the left side of the row, set value to true. Default: false
@@ -596,14 +619,16 @@
     * restriction: If the field has restrictions like output only, set the value to "Output Only". Default: No Restriction
     * name_title: This field is only for Array types. This field is the label of the first field.
     * value_title: This field is only for Array types. This field is the label of the second field.
     * titles: (alias: headers) This field is another representation of the name_title and value_title fields. You can set the name and value field title in a comma seperated string. For example: `titles: Field Name, Field Value`
     * values: Default values of an Array field.
     * allow_multiple: This field is only for Choice types. To allow selecting multiple values, set value to true. Default: false
     * allow_empty: This field is only for Choice types. To allow not selecting any value, set value to true. Default: false
+    * allow_variable: This field is only for credential. To allow adding variable option for credentials, set value to true. Default: false
+    * regex: This field is only for text fields. It will add validation with regular expression to text fields.
     * length: Sets the max lenght of the field.
     * max: Sets the maximum allowed number for that field.
     * min: Set the minimum allowed number for that field.
     
     ### items
     This field is required for Choice type. This field will include the items of the choice field. Items can be a simple string without a space and it will be used as the name of the item and label will be generated from the names. If you want to give a specific label, in this case set it like this. `- use_ssl: Use SSL`
```

### Comparing `quip-cli-1.9.0/setup.py` & `quip-cli-1.9.2/setup.py`

 * *Files identical despite different names*

