# Comparing `tmp/pyproject_metadata-0.8.0rc1.tar.gz` & `tmp/pyproject_metadata-0.8.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_metadata-0.8.0rc1.tar", last modified: Sun Apr 14 04:17:49 2024, max compression
+gzip compressed data, was "pyproject_metadata-0.8.0rc2.tar", last modified: Wed Apr 17 04:45:38 2024, max compression
```

## Comparing `pyproject_metadata-0.8.0rc1.tar` & `pyproject_metadata-0.8.0rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2198 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/CHANGELOG.rst
--rw-r--r--   0        0        0     1113 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/LICENSE
--rw-r--r--   0        0        0     1782 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/README.md
-lrwxr-xr-x   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/docs/changelog.rst -> ../CHANGELOG.rst
--rw-r--r--   0        0        0     2299 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/docs/conf.py
--rw-r--r--   0        0        0      846 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/docs/index.rst
--rw-r--r--   0        0        0     2528 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/pyproject.toml
--rw-r--r--   0        0        0    20762 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/pyproject_metadata/py.typed
--rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/__init__.py
--rw-r--r--   0        0        0      724 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/dynamic-description/dynamic_description.py
--rw-r--r--   0        0        0       90 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/dynamic-description/pyproject.toml
--rw-r--r--   0        0        0       17 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/README.md
--rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/full_metadata.py
--rw-r--r--   0        0        0     1204 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/pyproject.toml
--rw-r--r--   0        0        0       19 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/LICENSE
--rw-r--r--   0        0        0       17 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/README.rst
--rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/full_metadata2.py
--rw-r--r--   0        0        0     1196 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/pyproject.toml
--rw-r--r--   0        0        0       12 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/unknown-readme-type/README.just-made-this-up-now
--rw-r--r--   0        0        0       97 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/unknown-readme-type/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/packages/unknown-readme-type/unknown_readme_type.py
--rw-r--r--   0        0        0     5899 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/test_rfc822.py
--rw-r--r--   0        0        0    26273 2024-04-14 04:17:49.000000 pyproject_metadata-0.8.0rc1/tests/test_standard_metadata.py
--rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 pyproject_metadata-0.8.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2236 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/CHANGELOG.rst
+-rw-r--r--   0        0        0     1113 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/LICENSE
+-rw-r--r--   0        0        0     1782 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/README.md
+lrwxr-xr-x   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/docs/changelog.rst -> ../CHANGELOG.rst
+-rw-r--r--   0        0        0     2299 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/docs/conf.py
+-rw-r--r--   0        0        0      846 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/docs/index.rst
+-rw-r--r--   0        0        0     2528 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    20885 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/pyproject_metadata/py.typed
+-rw-r--r--   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/__init__.py
+-rw-r--r--   0        0        0      724 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/dynamic-description/dynamic_description.py
+-rw-r--r--   0        0        0       90 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/dynamic-description/pyproject.toml
+-rw-r--r--   0        0        0       17 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata/full_metadata.py
+-rw-r--r--   0        0        0     1204 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata/pyproject.toml
+-rw-r--r--   0        0        0       19 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata2/LICENSE
+-rw-r--r--   0        0        0       17 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata2/README.rst
+-rw-r--r--   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata2/full_metadata2.py
+-rw-r--r--   0        0        0     1196 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/full-metadata2/pyproject.toml
+-rw-r--r--   0        0        0       12 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/unknown-readme-type/README.just-made-this-up-now
+-rw-r--r--   0        0        0       97 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/unknown-readme-type/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/packages/unknown-readme-type/unknown_readme_type.py
+-rw-r--r--   0        0        0     5899 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/test_rfc822.py
+-rw-r--r--   0        0        0    26007 2024-04-17 04:45:38.000000 pyproject_metadata-0.8.0rc2/tests/test_standard_metadata.py
+-rw-r--r--   0        0        0     3003 1970-01-01 00:00:00.000000 pyproject_metadata-0.8.0rc2/PKG-INFO
```

### Comparing `pyproject_metadata-0.8.0rc1/CHANGELOG.rst` & `pyproject_metadata-0.8.0rc2/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 +++++++++
 Changelog
 +++++++++
 
 0.8.0
 =====
 
-- Support specifying the `metadata_version` as 2.1, 2.2, or 2.3
+- Support specifying the ``metadata_version`` as 2.1, 2.2, or 2.3
 - Always normalize extras following PEP 685
 - Preserve the user-specified name style in the metadata. ``.canonical_name`` added to get the normalized name
 - Require "version" in the dynamic table if unset (following PEP 621)
 - Support extras using markers containing "or"
 - Support empty extras
 - Using ``.as_rfc822()`` no longer modifies the metadata object
 - Fix email-author listing for names containing commas
-- Validate the description is one line
 - Separate core metadata keywords with commas, following the (modified) spec
 - An error message reported ``project.license`` instead of ``project.readme``
 - Produce slightly cleaner tracebacks
+  Fix a typo in an exception message
+- Subclasses now type check correctly
 - The build backend is now ``flit-core``
 
 
 0.7.1 (30-01-2023)
 ==================
 
 - Relax ``pypa/packaging`` dependency
```

### Comparing `pyproject_metadata-0.8.0rc1/LICENSE` & `pyproject_metadata-0.8.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/README.md` & `pyproject_metadata-0.8.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/docs/conf.py` & `pyproject_metadata-0.8.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/docs/index.rst` & `pyproject_metadata-0.8.0rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/pyproject.toml` & `pyproject_metadata-0.8.0rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/pyproject_metadata/__init__.py` & `pyproject_metadata-0.8.0rc2/pyproject_metadata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,31 +5,37 @@
 import collections
 import copy
 import dataclasses
 import email.utils
 import os
 import os.path
 import pathlib
+import sys
 import typing
 
 
 if typing.TYPE_CHECKING:
     from collections.abc import Mapping
     from typing import Any
 
     from packaging.requirements import Requirement
 
+    if sys.version_info < (3, 11):
+        from typing_extensions import Self
+    else:
+        from typing import Self
+
 import packaging.markers
 import packaging.requirements
 import packaging.specifiers
 import packaging.utils
 import packaging.version
 
 
-__version__ = '0.8.0rc1'
+__version__ = '0.8.0rc2'
 
 KNOWN_METADATA_VERSIONS = {'2.1', '2.2', '2.3'}
 
 
 class ConfigurationError(Exception):
     '''Error in the backend metadata.'''
     def __init__(self, msg: str, *, key: str | None = None):
@@ -200,30 +206,30 @@
 
     @classmethod
     def from_pyproject(
         cls,
         data: Mapping[str, Any],
         project_dir: str | os.PathLike[str] = os.path.curdir,
         metadata_version: str | None = None,
-    ) -> StandardMetadata:
+    ) -> Self:
         fetcher = DataFetcher(data)
         project_dir = pathlib.Path(project_dir)
 
         if 'project' not in fetcher:
             msg = 'Section "project" missing in pyproject.toml'
             raise ConfigurationError(msg)
 
         dynamic = fetcher.get_list('project.dynamic')
         if 'name' in dynamic:
             msg = 'Unsupported field "name" in "project.dynamic"'
             raise ConfigurationError(msg)
 
         for field in dynamic:
             if field in data['project']:
-                msg = f'Field "project.{field}" declared as dynamic in but is defined'
+                msg = f'Field "project.{field}" declared as dynamic in "project.dynamic" but is defined'
                 raise ConfigurationError(msg)
 
         name = fetcher.get_str('project.name')
         if not name:
             msg = 'Field "project.name" missing'
             raise ConfigurationError(msg)
 
@@ -231,19 +237,18 @@
         requires_python_string = fetcher.get_str('project.requires-python')
         version = packaging.version.Version(version_string) if version_string else None
 
         if version is None and 'version' not in dynamic:
             msg = 'Field "project.version" missing and "version" not specified in "project.dynamic"'
             raise ConfigurationError(msg)
 
-        # Description can't be multiline
+        # Description fills Summary, which cannot be multiline
+        # However, throwing an error isn't backward compatible,
+        # so leave it up to the users for now.
         description = fetcher.get_str('project.description')
-        if description and '\n' in description:
-            msg = 'The description must be a single line'
-            raise ConfigurationError(msg)
 
         if metadata_version and metadata_version not in KNOWN_METADATA_VERSIONS:
             msg = f'The metadata_version must be one of {KNOWN_METADATA_VERSIONS} or None (default)'
             raise ConfigurationError(msg)
 
         return cls(
             name,
```

### Comparing `pyproject_metadata-0.8.0rc1/tests/conftest.py` & `pyproject_metadata-0.8.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/tests/packages/full-metadata/pyproject.toml` & `pyproject_metadata-0.8.0rc2/tests/packages/full-metadata/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/tests/packages/full-metadata2/pyproject.toml` & `pyproject_metadata-0.8.0rc2/tests/packages/full-metadata2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/tests/test_rfc822.py` & `pyproject_metadata-0.8.0rc2/tests/test_rfc822.py`

 * *Files identical despite different names*

### Comparing `pyproject_metadata-0.8.0rc1/tests/test_standard_metadata.py` & `pyproject_metadata-0.8.0rc2/tests/test_standard_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,24 +228,14 @@
                 [project]
                 name = 'test'
                 version = '0.1.0'
                 description = true
             '''),
             ('Field "project.description" has an invalid type, expecting a string (got "True")'),
         ),
-        (
-            textwrap.dedent('''
-                [project]
-                name = 'test'
-                version = '0.1.0'
-                description = """Multiple
-                lines."""
-            '''),
-            ('The description must be a single line'),
-        ),
         # dependencies
         (
             textwrap.dedent('''
                 [project]
                 name = 'test'
                 version = '0.1.0'
                 dependencies = 'some string!'
@@ -763,15 +753,15 @@
     with pytest.raises(pyproject_metadata.ConfigurationError, match='Missing version field'):
         metadata.as_rfc822()
 
 
 def test_stically_defined_dynamic_field():
     with pytest.raises(
         pyproject_metadata.ConfigurationError,
-        match='Field "project.version" declared as dynamic in but is defined',
+        match='Field "project.version" declared as dynamic in "project.dynamic" but is defined',
     ):
         pyproject_metadata.StandardMetadata.from_pyproject({
             'project': {
                 'name': 'example',
                 'version': '1.2.3',
                 'dynamic': [
                     'version',
```

### Comparing `pyproject_metadata-0.8.0rc1/PKG-INFO` & `pyproject_metadata-0.8.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-metadata
-Version: 0.8.0rc1
+Version: 0.8.0rc2
 Summary: PEP 621 metadata parsing
 Author-email: Filipe Laíns <lains@riseup.net>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

