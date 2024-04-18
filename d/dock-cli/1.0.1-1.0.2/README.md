# Comparing `tmp/dock_cli-1.0.1.tar.gz` & `tmp/dock_cli-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dock_cli-1.0.1.tar", last modified: Mon Apr 15 16:21:10 2024, max compression
+gzip compressed data, was "dock_cli-1.0.2.tar", last modified: Wed Apr 17 15:58:53 2024, max compression
```

## Comparing `dock_cli-1.0.1.tar` & `dock_cli-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:21:10.398607 dock_cli-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-15 16:20:59.000000 dock_cli-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-15 16:21:10.398607 dock_cli-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-15 16:20:59.000000 dock_cli-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:21:10.398607 dock_cli-1.0.1/dock_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:21:10.398607 dock_cli-1.0.1/dock_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/cli/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:21:10.398607 dock_cli-1.0.1/dock_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/utils/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-15 16:20:59.000000 dock_cli-1.0.1/dock_cli/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:21:10.398607 dock_cli-1.0.1/dock_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-15 16:21:10.000000 dock_cli-1.0.1/dock_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 16:21:10.000000 dock_cli-1.0.1/dock_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:21:10.000000 dock_cli-1.0.1/dock_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-15 16:21:10.000000 dock_cli-1.0.1/dock_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 16:21:10.000000 dock_cli-1.0.1/dock_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 16:21:10.000000 dock_cli-1.0.1/dock_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:21:10.402607 dock_cli-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-15 16:20:59.000000 dock_cli-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:53.443574 dock_cli-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-17 15:58:38.000000 dock_cli-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-17 15:58:53.443574 dock_cli-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-17 15:58:38.000000 dock_cli-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:53.439574 dock_cli-1.0.2/dock_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:53.439574 dock_cli-1.0.2/dock_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/cli/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:53.439574 dock_cli-1.0.2/dock_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/utils/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-17 15:58:38.000000 dock_cli-1.0.2/dock_cli/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 15:58:53.439574 dock_cli-1.0.2/dock_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-17 15:58:53.000000 dock_cli-1.0.2/dock_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-17 15:58:53.000000 dock_cli-1.0.2/dock_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 15:58:53.000000 dock_cli-1.0.2/dock_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 15:58:53.000000 dock_cli-1.0.2/dock_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 15:58:53.000000 dock_cli-1.0.2/dock_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 15:58:53.000000 dock_cli-1.0.2/dock_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 15:58:53.443574 dock_cli-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-17 15:58:38.000000 dock_cli-1.0.2/setup.py
```

### Comparing `dock_cli-1.0.1/LICENSE` & `dock_cli-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/PKG-INFO` & `dock_cli-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock_cli-1.0.1/README.md` & `dock_cli-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/cli/chart.py` & `dock_cli-1.0.2/dock_cli/cli/chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,25 +69,28 @@
 @config_cli.command(name='view',
                     help="View current charts' configuration")
 @click.pass_obj
 def config_view(obj):
     sections = obj.helper.get_charts()
     if not sections:
         logging.getLogger(__name__).warning('No charts found.')
-    for section in obj.helper.get_charts():
+    for section in sections:
         utils.print_chart_config(obj.config, section)
 
 @config_cli.command(name='set',
                     help='Add or update an chart section in the configuration')
 @click.pass_obj
 @click.argument('section', required=True, type=click.Path(exists=True, file_okay=False),
                 callback=cb.transform_to_section)
-def config_set(obj, section):
+@click.option('--registry', required=False, type=str,
+              help='Name of the registry for this section.')
+def config_set(obj, section, registry):
     if obj.config.has_section(section) is False:
         obj.config.add_section(section)
+    utils.set_config_option(obj.config, section, Chart.REGISTRY, registry)
     utils.set_config_option(obj.config, section, Chart.TYPE, SectionType.CHART)
     obj.helper.validate_section(section)
     utils.print_chart_config(obj.config, section)
     utils.update_config(obj.config, obj.config_file)
 
 @config_cli.command(name='set-registry',
                     help='Set default registry for all charts in the configuration')
```

### Comparing `dock_cli-1.0.1/dock_cli/cli/image.py` & `dock_cli-1.0.2/dock_cli/cli/image.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/main.py` & `dock_cli-1.0.2/dock_cli/main.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/utils/callback.py` & `dock_cli-1.0.2/dock_cli/utils/callback.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/utils/commands.py` & `dock_cli-1.0.2/dock_cli/utils/commands.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/utils/helpers.py` & `dock_cli-1.0.2/dock_cli/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/utils/schema.py` & `dock_cli-1.0.2/dock_cli/utils/schema.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli/utils/utils.py` & `dock_cli-1.0.2/dock_cli/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dock_cli-1.0.1/dock_cli.egg-info/PKG-INFO` & `dock_cli-1.0.2/dock_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dock-cli
-Version: 1.0.1
+Version: 1.0.2
 Summary: CLI for manage container applications
 Author: Posen
 Author-email: posen2101024@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `dock_cli-1.0.1/setup.py` & `dock_cli-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='dock-cli',
-    version='1.0.1',
+    version='1.0.2',
     author='Posen',
     author_email='posen2101024@gmail.com',
     description='CLI for manage container applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
```

