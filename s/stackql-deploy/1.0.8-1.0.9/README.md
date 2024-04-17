# Comparing `tmp/stackql_deploy-1.0.8.tar.gz` & `tmp/stackql_deploy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackql_deploy-1.0.8.tar", last modified: Wed Apr 17 00:38:34 2024, max compression
+gzip compressed data, was "stackql_deploy-1.0.9.tar", last modified: Wed Apr 17 01:12:59 2024, max compression
```

## Comparing `stackql_deploy-1.0.8.tar` & `stackql_deploy-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:38:34.900972 stackql_deploy-1.0.8/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.8/LICENSE
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 00:38:34.883778 stackql_deploy-1.0.8/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.8/README.rst
--rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 00:38:34.903352 stackql_deploy-1.0.8/setup.cfg
--rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-17 00:38:09.000000 stackql_deploy-1.0.8/setup.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:38:34.193268 stackql_deploy-1.0.8/stackql_deploy/
--rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-17 00:38:09.000000 stackql_deploy-1.0.8/stackql_deploy/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5315 2024-04-17 00:37:50.000000 stackql_deploy-1.0.8/stackql_deploy/cli.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:38:34.575383 stackql_deploy-1.0.8/stackql_deploy/cmd/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.8/stackql_deploy/cmd/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     6291 2024-04-16 23:16:19.000000 stackql_deploy-1.0.8/stackql_deploy/cmd/build.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.0.8/stackql_deploy/cmd/teardown.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.0.8/stackql_deploy/cmd/test.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:38:34.814013 stackql_deploy-1.0.8/stackql_deploy/lib/
--rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.8/stackql_deploy/lib/__init__.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.8/stackql_deploy/lib/bootstrap.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.8/stackql_deploy/lib/config.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.8/stackql_deploy/lib/templating.py
--rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.8/stackql_deploy/lib/utils.py
-drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 00:38:34.863298 stackql_deploy-1.0.8/stackql_deploy.egg-info/
--rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 00:38:33.000000 stackql_deploy-1.0.8/stackql_deploy.egg-info/PKG-INFO
--rwxrwxrwx   0 javen     (1000) javen     (1000)      576 2024-04-17 00:38:33.000000 stackql_deploy-1.0.8/stackql_deploy.egg-info/SOURCES.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 00:38:33.000000 stackql_deploy-1.0.8/stackql_deploy.egg-info/dependency_links.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-17 00:38:33.000000 stackql_deploy-1.0.8/stackql_deploy.egg-info/entry_points.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-17 00:38:33.000000 stackql_deploy-1.0.8/stackql_deploy.egg-info/requires.txt
--rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-17 00:38:33.000000 stackql_deploy-1.0.8/stackql_deploy.egg-info/top_level.txt
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:59.084573 stackql_deploy-1.0.9/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1071 2024-03-15 01:52:38.000000 stackql_deploy-1.0.9/LICENSE
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 01:12:59.054865 stackql_deploy-1.0.9/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8214 2024-04-16 23:03:24.000000 stackql_deploy-1.0.9/README.rst
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       38 2024-04-17 01:12:59.087598 stackql_deploy-1.0.9/setup.cfg
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     1300 2024-04-17 00:53:56.000000 stackql_deploy-1.0.9/setup.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:56.725468 stackql_deploy-1.0.9/stackql_deploy/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       23 2024-04-17 00:53:56.000000 stackql_deploy-1.0.9/stackql_deploy/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5607 2024-04-17 01:12:14.000000 stackql_deploy-1.0.9/stackql_deploy/cli.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:58.404766 stackql_deploy-1.0.9/stackql_deploy/cmd/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     6291 2024-04-16 23:16:19.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/build.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3433 2024-04-16 23:17:44.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/teardown.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2542 2024-04-16 23:17:44.000000 stackql_deploy-1.0.9/stackql_deploy/cmd/test.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:58.906858 stackql_deploy-1.0.9/stackql_deploy/lib/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-16 23:31:31.000000 stackql_deploy-1.0.9/stackql_deploy/lib/__init__.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      333 2024-04-12 03:18:07.000000 stackql_deploy-1.0.9/stackql_deploy/lib/bootstrap.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     3647 2024-04-16 02:40:32.000000 stackql_deploy-1.0.9/stackql_deploy/lib/config.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     2782 2024-04-16 03:47:18.000000 stackql_deploy-1.0.9/stackql_deploy/lib/templating.py
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     5279 2024-04-16 03:46:51.000000 stackql_deploy-1.0.9/stackql_deploy/lib/utils.py
+drwxrwxrwx   0 javen     (1000) javen     (1000)        0 2024-04-17 01:12:59.006557 stackql_deploy-1.0.9/stackql_deploy.egg-info/
+-rwxrwxrwx   0 javen     (1000) javen     (1000)     8892 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/PKG-INFO
+-rwxrwxrwx   0 javen     (1000) javen     (1000)      576 2024-04-17 01:12:56.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)        1 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       58 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/entry_points.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       37 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/requires.txt
+-rwxrwxrwx   0 javen     (1000) javen     (1000)       15 2024-04-17 01:12:55.000000 stackql_deploy-1.0.9/stackql_deploy.egg-info/top_level.txt
```

### Comparing `stackql_deploy-1.0.8/LICENSE` & `stackql_deploy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/PKG-INFO` & `stackql_deploy-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.8
+Version: 1.0.9
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.0.8/README.rst` & `stackql_deploy-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/setup.py` & `stackql_deploy-1.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='stackql-deploy',
-    version='1.0.8',
+    version='1.0.9',
     description='Model driven resource provisioning and deployment framework using StackQL.',
     long_description=readme,
     author='Jeffrey Aven',
     author_email='javen@stackql.io',
     url='https://github.com/stackql/stackql-deploy',
     license='MIT',
     packages=find_packages(),
```

### Comparing `stackql_deploy-1.0.8/stackql_deploy/cli.py` & `stackql_deploy-1.0.9/stackql_deploy/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,35 +91,40 @@
     if os.path.exists(base_path):
         raise click.ClickException(f"directory '{stack_name}' already exists.")
     
     directories = ['stackql_docs', 'stackql_resources', 'stackql_tests']
     for directory in directories:
         os.makedirs(os.path.join(base_path, directory), exist_ok=True)
     
-    # Correctly set the path for templates
-    template_base_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'templates')
+    template_base_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'templates')
     env = Environment(loader=FileSystemLoader(template_base_path))
-    
+
+    logger.debug("template base path:", template_base_path)
+
     template_files = {
         'stackql_manifest.yml.template': 'stackql_manifest.yml',
         'stackql_docs/resource1.md.template': os.path.join('stackql_docs', 'resource1.md'),
         'stackql_resources/resource1.iql.template': os.path.join('stackql_resources', 'resource1.iql'),
         'stackql_tests/resource1.iql.template': os.path.join('stackql_tests', 'resource1.iql')
     }
     
     for template_name, output_name in template_files.items():
+        logger.debug("template name:", template_name)
+        logger.debug("template output name:", output_name)
         template = env.get_template(template_name)
         rendered_content = template.render(stack_name=stack_name)
         with open(os.path.join(base_path, output_name), 'w') as f:
             f.write(rendered_content)
 
 @click.command()
 @click.argument('stack_name')
-def init(stack_name):
+@click.option('--log-level', default='INFO', help='Set the logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL)')
+def init(stack_name, log_level):
     """Initialize a new stackql-deploy project structure."""
+    setup_logger("init", locals())
     create_project_structure(stack_name)
     click.echo(f"project {stack_name} initialized successfully.")
 
 @click.group()
 def cli():
     pass
```

### Comparing `stackql_deploy-1.0.8/stackql_deploy/cmd/build.py` & `stackql_deploy-1.0.9/stackql_deploy/cmd/build.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/stackql_deploy/cmd/teardown.py` & `stackql_deploy-1.0.9/stackql_deploy/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/stackql_deploy/cmd/test.py` & `stackql_deploy-1.0.9/stackql_deploy/cmd/test.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/stackql_deploy/lib/config.py` & `stackql_deploy-1.0.9/stackql_deploy/lib/config.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/stackql_deploy/lib/templating.py` & `stackql_deploy-1.0.9/stackql_deploy/lib/templating.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/stackql_deploy/lib/utils.py` & `stackql_deploy-1.0.9/stackql_deploy/lib/utils.py`

 * *Files identical despite different names*

### Comparing `stackql_deploy-1.0.8/stackql_deploy.egg-info/PKG-INFO` & `stackql_deploy-1.0.9/stackql_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackql-deploy
-Version: 1.0.8
+Version: 1.0.9
 Summary: Model driven resource provisioning and deployment framework using StackQL.
 Home-page: https://github.com/stackql/stackql-deploy
 Author: Jeffrey Aven
 Author-email: javen@stackql.io
 License: MIT
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `stackql_deploy-1.0.8/stackql_deploy.egg-info/SOURCES.txt` & `stackql_deploy-1.0.9/stackql_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

