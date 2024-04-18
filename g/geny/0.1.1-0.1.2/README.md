# Comparing `tmp/geny-0.1.1.tar.gz` & `tmp/geny-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geny-0.1.1.tar", last modified: Thu Jan 18 02:27:05 2024, max compression
+gzip compressed data, was "geny-0.1.2.tar", last modified: Thu Apr 18 01:15:48 2024, max compression
```

## Comparing `geny-0.1.1.tar` & `geny-0.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.801592 geny-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-01-18 02:26:47.000000 geny-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-01-18 02:27:05.801592 geny-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-01-18 02:26:47.000000 geny-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.793593 geny-0.1.1/geny/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-18 02:26:47.000000 geny-0.1.1/geny/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.797592 geny-0.1.1/geny/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-18 02:26:47.000000 geny-0.1.1/geny/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2730 2024-01-18 02:26:47.000000 geny-0.1.1/geny/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.797592 geny-0.1.1/geny/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.797592 geny-0.1.1/geny/commands/destroy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/destroy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/destroy/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/destroy/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/destroy/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.797592 geny-0.1.1/geny/commands/generate/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/generate/dockerfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/generate/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-18 02:26:47.000000 geny-0.1.1/geny/commands/generate/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.797592 geny-0.1.1/geny/core/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.797592 geny-0.1.1/geny/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/decorators/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/decorators/singleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.801592 geny-0.1.1/geny/core/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/filesystem/transformations.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.801592 geny-0.1.1/geny/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/templates/protocols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/templates/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-18 02:26:47.000000 geny-0.1.1/geny/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.801592 geny-0.1.1/geny/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-18 02:26:47.000000 geny-0.1.1/geny/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-01-18 02:26:47.000000 geny-0.1.1/geny/extensions/aliased.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-18 02:26:47.000000 geny-0.1.1/geny/extensions/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-01-18 02:26:47.000000 geny-0.1.1/geny/extensions/discoverable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.801592 geny-0.1.1/geny/template_files/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-18 02:26:47.000000 geny-0.1.1/geny/template_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 02:27:05.801592 geny-0.1.1/geny.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-01-18 02:27:05.000000 geny-0.1.1/geny.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-01-18 02:27:05.000000 geny-0.1.1/geny.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 02:27:05.000000 geny-0.1.1/geny.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-18 02:27:05.000000 geny-0.1.1/geny.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-01-18 02:27:05.000000 geny-0.1.1/geny.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-18 02:27:05.000000 geny-0.1.1/geny.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-01-18 02:26:47.000000 geny-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 02:27:05.801592 geny-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 01:15:34.000000 geny-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-18 01:15:48.962913 geny-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-18 01:15:34.000000 geny-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.954913 geny-0.1.2/geny/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-18 01:15:34.000000 geny-0.1.2/geny/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-18 01:15:34.000000 geny-0.1.2/geny/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-04-18 01:15:34.000000 geny-0.1.2/geny/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/commands/destroy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/destroy/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/commands/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/generate/dockerfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/generate/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-18 01:15:34.000000 geny-0.1.2/geny/commands/generate/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/decorators/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/decorators/singleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.958913 geny-0.1.2/geny/core/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/filesystem/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/templates/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/templates/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 01:15:34.000000 geny-0.1.2/geny/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/aliased.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-18 01:15:34.000000 geny-0.1.2/geny/extensions/discoverable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny/template_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-18 01:15:34.000000 geny-0.1.2/geny/template_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:15:48.962913 geny-0.1.2/geny.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 01:15:48.000000 geny-0.1.2/geny.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-18 01:15:34.000000 geny-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:15:48.962913 geny-0.1.2/setup.cfg
```

### Comparing `geny-0.1.1/LICENSE` & `geny-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/PKG-INFO` & `geny-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geny
-Version: 0.1.1
+Version: 0.1.2
 Summary: An extendable file generator
 Author-email: Leo Neto <leo@ekletik.com>
 Maintainer-email: Leo Neto <leo@ekletik.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Leo
```

### Comparing `geny-0.1.1/README.md` & `geny-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/cli/cli.py` & `geny-0.1.2/geny/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import click
 import logging
 from pathlib import Path
-from geny import VERSION
 from geny.extensions.combined import AliasedAndDiscoverableGroup
 from geny.core.templates.template import TemplateParser
 
 
 @click.command(
     cls=AliasedAndDiscoverableGroup, context_settings=dict(ignore_unknown_options=True)
 )
 @click.option("--debug", is_flag=True, help="Enable debug logs.")
 @click.option("--dry", is_flag=True, help="Do not modify the file system.")
-@click.option("-f", "--force", is_flag=True, help="Override any conflicting files.")
+@click.option("-f", "--force", is_flag=True, envvar="GENY_ENABLE_FORCE", help="Override any conflicting files.")
 @click.option("--verbose", is_flag=True, help="Enable verbosity.")
 @click.option(
     "--templates-dir",
     "-t",
     envvar="GENY_TEMPLATES_DIR",
     help="Template directory.",
     type=click.Path(),
 )
-@click.version_option(version=VERSION)
+@click.version_option(package_name="geny")
 @click.pass_context
 def cli(ctx, debug, dry, force, verbose, templates_dir):
     """
     geny
 
     an extendable file generator.
     """
```

### Comparing `geny-0.1.1/geny/commands/destroy/template.py` & `geny-0.1.2/geny/commands/destroy/template.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/commands/generate/dockerfile.py` & `geny-0.1.2/geny/commands/generate/dockerfile.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/commands/generate/template.py` & `geny-0.1.2/geny/commands/generate/template.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/core/filesystem/directories.py` & `geny-0.1.2/geny/core/filesystem/directories.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/core/filesystem/files.py` & `geny-0.1.2/geny/core/filesystem/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,18 @@
     def create(self, parent: Path = None, after_hooks: list[Callable] = None, **kwargs):
         if after_hooks is None:
             after_hooks = []
 
         path = self.path(parent)
 
         if path.exists():
-            logger.error(f"File already exists: {path}")
-            return
+            if not kwargs.get('GENY_ENABLE_FORCE', False):
+                logger.error(f"File already exists: {path}")
+                return
+            logger.debug(f"Overriding {path}")
 
         contents = self.contents(**kwargs)
 
         logger.info(f"create: {path}")
 
         # NOTE: Handle missing intermediate directories
         if not path.absolute().parent.exists():
```

### Comparing `geny-0.1.1/geny/core/filesystem/finder.py` & `geny-0.1.2/geny/core/filesystem/finder.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/core/filesystem/transformations.py` & `geny-0.1.2/geny/core/filesystem/transformations.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/core/utils.py` & `geny-0.1.2/geny/core/utils.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/extensions/aliased.py` & `geny-0.1.2/geny/extensions/aliased.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/extensions/combined.py` & `geny-0.1.2/geny/extensions/combined.py`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/geny/extensions/discoverable.py` & `geny-0.1.2/geny/extensions/discoverable.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,17 @@
         ns = {}
         fn = os.path.join(COMMANDS_FOLDER, name, "main.py")
 
         try:
             execute_command(fn, ns)
         except FileNotFoundError:
             try:
+                if PLUGINS_FOLDER is None:
+                    return
+
                 pfn = os.path.join(PLUGINS_FOLDER, name, "main.py")
                 execute_command(pfn, ns)
             except FileNotFoundError or TypeError:
                 pass
 
         try:
             return ns[name]
```

### Comparing `geny-0.1.1/geny.egg-info/PKG-INFO` & `geny-0.1.2/geny.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geny
-Version: 0.1.1
+Version: 0.1.2
 Summary: An extendable file generator
 Author-email: Leo Neto <leo@ekletik.com>
 Maintainer-email: Leo Neto <leo@ekletik.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Leo
```

### Comparing `geny-0.1.1/geny.egg-info/SOURCES.txt` & `geny-0.1.2/geny.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geny-0.1.1/pyproject.toml` & `geny-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "geny"
 description = "An extendable file generator"
 authors = [{ name = "Leo Neto", email = "leo@ekletik.com" }]
 maintainers = [{ name = "Leo Neto", email = "leo@ekletik.com" }]
 requires-python = ">=3.6"
 license = { file = "LICENSE" }
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 keywords = [
   "automation",
   "files",
   "generators",
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
```

