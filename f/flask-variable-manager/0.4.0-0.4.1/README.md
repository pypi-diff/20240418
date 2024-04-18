# Comparing `tmp/flask_variable_manager-0.4.0.tar.gz` & `tmp/flask_variable_manager-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_variable_manager-0.4.0.tar", last modified: Wed Apr 17 08:00:36 2024, max compression
+gzip compressed data, was "flask_variable_manager-0.4.1.tar", last modified: Thu Apr 18 13:08:20 2024, max compression
```

## Comparing `flask_variable_manager-0.4.0.tar` & `flask_variable_manager-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.838660 flask_variable_manager-0.4.0/flask_variable_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/flask_variable_manager/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/extension/variable_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/flask_variable_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/flask_variable_manager/tests/test_vm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-17 08:00:36.000000 flask_variable_manager-0.4.0/flask_variable_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-17 08:00:32.000000 flask_variable_manager-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 08:00:36.842660 flask_variable_manager-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:20.423416 flask_variable_manager-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-18 13:08:20.423416 flask_variable_manager-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:20.419415 flask_variable_manager-0.4.1/flask_variable_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/flask_variable_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:20.419415 flask_variable_manager-0.4.1/flask_variable_manager/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/flask_variable_manager/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/flask_variable_manager/extension/variable_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:20.423416 flask_variable_manager-0.4.1/flask_variable_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/flask_variable_manager/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/flask_variable_manager/tests/test_vm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:08:20.423416 flask_variable_manager-0.4.1/flask_variable_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-18 13:08:20.000000 flask_variable_manager-0.4.1/flask_variable_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-18 13:08:20.000000 flask_variable_manager-0.4.1/flask_variable_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:08:20.000000 flask_variable_manager-0.4.1/flask_variable_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 13:08:20.000000 flask_variable_manager-0.4.1/flask_variable_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 13:08:20.000000 flask_variable_manager-0.4.1/flask_variable_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-18 13:08:13.000000 flask_variable_manager-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:08:20.423416 flask_variable_manager-0.4.1/setup.cfg
```

### Comparing `flask_variable_manager-0.4.0/LICENSE` & `flask_variable_manager-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_variable_manager-0.4.0/PKG-INFO` & `flask_variable_manager-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask_variable_manager-0.4.0/README.md` & `flask_variable_manager-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `flask_variable_manager-0.4.0/flask_variable_manager/extension/variable_manager.py` & `flask_variable_manager-0.4.1/flask_variable_manager/extension/variable_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from flask import g, jsonify, request, render_template_string
 
 
 def define_routes(app):
     @app.route('/vm/render', methods=['POST'])
     def render_template():
         """
+        vm/render: Render a string as a Jinja2 template
         ---
         tags:
           - Rendering
         summary: Render a string as a Jinja2 template
         description: This endpoint allows you to render a string as a Jinja2 template.
         parameters:
           - in: formData
@@ -29,14 +30,15 @@
         rendered_template = render_template_string(template_string, _local=g.local, system=g.system)
 
         return rendered_template
 
     @app.route('/vm/var', methods=['POST'])
     def set_variable():
         """
+        /vm/var: Set a user-defined variable
         ---
         tags:
           - Variables
         summary: Set a user-defined variable
         description: This endpoint allows you to set a user-defined variable.
         parameters:
           - in: formData
@@ -58,14 +60,15 @@
 
         g.local[key] = value
         return jsonify({'message': 'The variable has been set successfully.'})
 
     @app.route('/vm/vars', methods=['POST'])
     def set_variables():
         """
+        /vm/vars: Set multiple user-defined variables
         ---
         tags:
           - Variables
         summary: Set multiple user-defined variables
         description: This endpoint allows you to set multiple user-defined variables.
         parameters:
           - in: body
@@ -85,14 +88,15 @@
             g.local[key] = value
 
         return jsonify({'message': 'The variables have been set successfully.'})
 
     @app.route('/vm/var', methods=['GET'])
     def get_variables():
         """
+        /vm/var: Get all user-defined variables
         ---
         tags:
           - Variables
         summary: Get all user-defined variables
         description: This endpoint allows you to get all user-defined variables.
         responses:
           200:
@@ -105,14 +109,15 @@
                   description: The user-defined variables.
         """
         return jsonify(g.local.to_dict())
 
     @app.route('/vm/vars', methods=['DELETE'])
     def clear_variables():
         """
+        /vm/vars: Clear all user-defined variables
         ---
         tags:
           - Variables
         summary: Clear all user-defined variables
         description: This endpoint allows you to clear all user-defined variables.
         responses:
           200:
@@ -120,14 +125,15 @@
         """
         g.local.to_dict().clear()
         return jsonify({'message': 'All user-defined variables have been cleared.'})
 
     @app.route('/vm/var/<key>', methods=['DELETE'])
     def clear_variable(key):
         """
+        /vm/var/{key}: Clear a user-defined variable
         ---
         tags:
           - Variables
         summary: Clear a user-defined variable
         description: This endpoint allows you to clear a user-defined variable.
         parameters:
           - in: path
@@ -144,14 +150,15 @@
             return jsonify({'message': 'The variable has been cleared successfully.'})
         except KeyError:
             return jsonify({'message': 'The variable does not exist.'}), 404
 
     @app.route('/py/runner', methods=['POST'])
     def run_python_code():
         """
+        /py/runner: Run Python code and return the result
         ---
         tags:
           - Python
         summary: Run Python code and return the result
         description: This endpoint allows you to run Python code and return the result.
         parameters:
           - in: body
@@ -180,14 +187,15 @@
         for key in unwanted_keys:
             del local_vars[key]
         return jsonify({'result': str(result)})
 
     @app.route('/py/install', methods=['POST'])
     def install_python_package():
         """
+        /py/install: Install a Python package
         ---
         tags:
           - Python
         summary: Install a Python package
         description: This endpoint allows you to install a Python package.
         parameters:
           - in: formData
@@ -204,14 +212,15 @@
         for package_name in package_name.split('\n'):
             subprocess.run(['pip', 'install', package_name])
         return jsonify({'message': 'The package has been installed successfully.'})
 
     @app.route('/py/uninstall', methods=['POST'])
     def uninstall_python_package():
         """
+        /py/uninstall: Uninstall a Python package
         ---
         tags:
           - Python
         summary: Uninstall a Python package
         description: This endpoint allows you to uninstall a Python package.
         parameters:
           - in: formData
@@ -228,14 +237,15 @@
         for package_name in package_name.split('\n'):
             subprocess.run(['pip', 'uninstall', '-y', package_name])
         return jsonify({'message': 'The package has been uninstalled successfully.'})
 
     @app.route('/py/packages', methods=['GET'])
     def get_python_packages():
         """
+        /py/packages: Get all installed Python packages
         ---
         tags:
           - Python
         summary: Get all installed Python packages
         description: This endpoint allows you to get all installed Python packages.
         responses:
           200:
```

### Comparing `flask_variable_manager-0.4.0/flask_variable_manager/tests/test_vm.py` & `flask_variable_manager-0.4.1/flask_variable_manager/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `flask_variable_manager-0.4.0/flask_variable_manager.egg-info/PKG-INFO` & `flask_variable_manager-0.4.1/flask_variable_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-variable-manager
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create a variable manager in flask, enter values in python, and use values on the jinja template.
 Author-email: minwook-shin <minwook0106@gmail.com>
 Project-URL: Homepage, https://github.com/minwook-shin/flask-variable-manager
 Project-URL: Bug Tracker, https://github.com/minwook-shin/flask-variable-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `flask_variable_manager-0.4.0/pyproject.toml` & `flask_variable_manager-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 include-package-data = false
 
 [tool.setuptools.packages.find]
 include = ['flask_variable_manager*']
 
 [project]
 name = "flask-variable-manager"
-version = "0.4.0"
+version = "0.4.1"
 description = "Create a variable manager in flask, enter values in python, and use values on the jinja template."
 authors = [
     { name = "minwook-shin", email = "minwook0106@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

