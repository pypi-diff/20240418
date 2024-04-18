# Comparing `tmp/ResourceBundle-2.1.0.tar.gz` & `tmp/resourcebundle-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ResourceBundle-2.1.0.tar", last modified: Sun May 14 20:17:03 2023, max compression
+gzip compressed data, was "resourcebundle-2.2.0.tar", last modified: Thu Apr 18 01:45:36 2024, max compression
```

## Comparing `ResourceBundle-2.1.0.tar` & `resourcebundle-2.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:17:03.897961 ResourceBundle-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-14 20:17:03.897961 ResourceBundle-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:17:03.893961 ResourceBundle-2.1.0/ResourceBundle/
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/ResourceBundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/ResourceBundle/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 20:17:03.893961 ResourceBundle-2.1.0/ResourceBundle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-14 20:17:03.000000 ResourceBundle-2.1.0/ResourceBundle.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 20:17:03.897961 ResourceBundle-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-14 20:16:52.000000 ResourceBundle-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:45:36.309221 resourcebundle-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 01:45:31.000000 resourcebundle-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-18 01:45:36.305221 resourcebundle-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-04-18 01:45:31.000000 resourcebundle-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:45:36.305221 resourcebundle-2.2.0/ResourceBundle/
+-rw-r--r--   0 runner    (1001) docker     (127)    11083 2024-04-18 01:45:31.000000 resourcebundle-2.2.0/ResourceBundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-18 01:45:31.000000 resourcebundle-2.2.0/ResourceBundle/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 01:45:36.305221 resourcebundle-2.2.0/ResourceBundle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-18 01:45:36.000000 resourcebundle-2.2.0/ResourceBundle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 01:45:36.000000 resourcebundle-2.2.0/ResourceBundle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 01:45:36.000000 resourcebundle-2.2.0/ResourceBundle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 01:45:36.000000 resourcebundle-2.2.0/ResourceBundle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 01:45:36.000000 resourcebundle-2.2.0/ResourceBundle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 01:45:31.000000 resourcebundle-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 01:45:36.309221 resourcebundle-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-18 01:45:31.000000 resourcebundle-2.2.0/setup.py
```

### Comparing `ResourceBundle-2.1.0/LICENSE` & `resourcebundle-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ResourceBundle-2.1.0/PKG-INFO` & `resourcebundle-2.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 Metadata-Version: 2.1
 Name: ResourceBundle
-Version: 2.1.0
-Summary: ResourceBundle is a module that manages internationalization of string resources
-Home-page: https://felix-zenk.github.io/projects/ResourceBundle
+Version: 2.2.0
+Summary: ResourceBundle is a module that manages internationalization of string resources.
+Home-page: https://github.com/felix-zenk/ResourceBundle
 Author: Felix Zenk
-Author-email: felix.zenk@web.de
-Project-URL: Bug Reports, https://github.com/felix-zenk/ResourceBundle/issues
-Project-URL: Source, https://github.com/felix-zenk/ResourceBundle
+Author-email: Felix Zenk <felix.zenk@web.de>
+License: MIT
+Project-URL: Homepage, https://github.com/felix-zenk/ResourceBundle
+Project-URL: Documentation, https://github.com/felix-zenk/ResourceBundle
+Project-URL: Repository, https://github.com/felix-zenk/ResourceBundle
+Project-URL: Issues, https://github.com/felix-zenk/ResourceBundle/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib_metadata; python_version < "3.8"
 
 # ResourceBundle
 
 [![PyPI-Versions](https://img.shields.io/pypi/pyversions/ResourceBundle)](https://pypi.org/project/ResourceBundle)
 [![PyPI version](https://badge.fury.io/py/ResourceBundle.svg)](https://pypi.org/project/ResourceBundle)
-[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
+[![Build package](https://github.com/felix-zenk/ResourceBundle/actions/workflows/build.yaml/badge.svg)](https://github.com/felix-zenk/ResourceBundle/actions/workflows/build.yaml)
+[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/ResourceBundle/blob/main/LICENSE)
 
+ResourceBundle is a package that manages internationalization / localization (i18n / l10n) of string resources.
+It is inspired by Java's ResourceBundle and accepts the same format as a Java ``PropertyResourceBundle``.
 
-ResourceBundle is a module that manages internationalization of string resources.
-It is inspired by javas ResourceBundle and accepts the same format as a java PropertyResourceBundle.
-
-> **Note:** ResourceBundle is not the python way of doing internationalization.
+> **Note:** ResourceBundle is not the pythonic way of internationalization / localization.
 > This package is only intended to be used if you *absolutely have* to work with ResourceBundle files
-> or need a quick working way when porting from java.
+> or need a quick working way when porting from Java.
 >
 > For information on how to do internationalization in python,
 > see the [official documentation](https://docs.python.org/3/library/gettext.html).
-> You can use the `ResourceBundle.Converter.to_gettext()` method to convert your ResourceBundle files to gettext po files.
+> You can use the [`ResourceBundle.Converter.to_gettext()`](#gettext)
+> method to convert your ResourceBundle files to gettext `po` files.
 
 ---
 ### Installation
 
 The ResourceBundle module can be downloaded from [PyPI](https://pypi.org/project/ResourceBundle):
 
 ```bash
-# linux / macOS
+# Linux / macOS
 $  python3 -m pip install ResourceBundle
 
-# windows
+# Windows
 >  py -m pip install ResourceBundle
 ```
 
 ### Usage
 
-Assuming you come from java, you are probably familiar with the ResourceBundle file format.
-If not,you can read about it
+Assuming you come from Java, you are probably familiar with the ResourceBundle file format.
+If not, you can read about it
 [here](https://docs.oracle.com/en/java/javase/20/docs/api/java.base/java/util/PropertyResourceBundle.html).
 
 Get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
 
 ```python
 import ResourceBundle
 
@@ -73,20 +81,21 @@
 until a matching key was found.
 If the key is not present in any of its parents a ``ResourceBundle.exceptions.NotInResourceBundleError`` will be raised.
 
 ---
 
 ### gettext
 
-The ResourceBundle module can convert ResourceBundle files to gettext pot / po files.
-This can be done by using the ``ResourceBundle.Converter.to_gettext()`` function.
+The ResourceBundle module can convert ResourceBundle files to gettext `pot` / `po` files.
+This can be done by using the ``ResourceBundle.Converter.to_gettext()`` method.
 
 ```python
 from ResourceBundle import Converter
 
 # convert all .properties files in the current directory to .po files
 Converter.to_gettext(".", ".")
 ```
 
-Note however that this step is obsolete if you are using gettext properly
-as this will include automatically extracting strings from your source code.
+Note however that this step is obsolete if you are using ``gettext`` properly
+as this will include automatically extracting strings from your source code with the help of a library like
+[Babel](https://babel.pocoo.org/en/latest/) with its [pybabel](https://babel.pocoo.org/en/latest/cmdline.html) tool.
 The function is only intended as a head start to keep existing translations.
```

### Comparing `ResourceBundle-2.1.0/ResourceBundle/__init__.py` & `resourcebundle-2.2.0/ResourceBundle/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
-Module containing the implementation of the ResourceBundle
+Module containing the implementation of the ResourceBundle.
 """
-from __future__ import annotations
-
 import codecs
 import re
+
 from datetime import datetime
 from os import PathLike, listdir
 from pathlib import Path
-from typing import Sequence, KeysView
+from typing import Sequence, KeysView, Optional
 
 from .exceptions import NotInResourceBundleError, MalformedResourceBundleError
 
-__version_info__ = (2, 1, 0)
-__version__ = ".".join(map(str, __version_info__))
-
 
 class _Parser(object):
     """
     A parser for the .properties file format.
     """
     @staticmethod
     def parse(file_path: Path) -> dict[str, str]:
@@ -64,22 +60,24 @@
                     new_line_no, new_value = next(enumerator)
                     value += new_value.strip().strip("\\")
             elif "=" in line:
                 key, *value = line.split("=")
                 key = key.strip()
                 value = '='.join(value).strip()
             else:
-                raise MalformedResourceBundleError(f"Malformed file: '{file_path}' (line {line_no})")
+                raise MalformedResourceBundleError("Malformed file: '%s' (line %d)" % (file_path, line_no))
 
             if '\\' in value:  # may contain escaped chars
                 value = decode(value)
             if key not in mapping.keys():
                 mapping[key] = value
             else:
-                raise MalformedResourceBundleError(f"Duplicate key '{key}' in file '{file_path}' on line {line_no}")
+                raise MalformedResourceBundleError(
+                    "Duplicate key '%s' in file '%s' on line %d" % (key, file_path, line_no)
+                )
         return mapping
 
 
 class ResourceBundle(object):
     """
     A ResourceBundle manages internationalization of string resources
     """
@@ -99,43 +97,43 @@
             separated by underscores.
             The format for a locale therefore is 'language_script_country_variant'
             like 'en_Latn_US_WINDOWS' or parts of it like 'en_US'
         :param str | PathLike | None path:
             The path to the ResourceBundle .properties files
             (default: current working directory)
         """
-        self._name: str = bundle_name
-        self._locale: str | None = bundle_locale
-        self._path: Path = self._ensure_path(path)
-        self._parent: ResourceBundle | None = self._get_parent_bundle()
-        self._mapping: dict[str, str] = self._map()
+        self._name = bundle_name  # type: str
+        self._locale = bundle_locale  # type: Optional[str]
+        self._path = self._ensure_path(path)  # type: Path
+        self._parent = self._get_parent_bundle()  # type: Optional[ResourceBundle]
+        self._mapping = self._map()  # type: dict[str, str]
         # Save self in cache
         self.__cached_bundles[self.name] = self
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} {self.name}>"
+        return "<%s %s>" % (self.__class__.__name__, self.name)
 
     def __str__(self) -> str:
         return self.name
 
     @property
     def name(self) -> str:
         """
         Get the full name of the ResourceBundle
         """
-        return f"{self._name}" if self._locale is None else f"{self._name}_{self._locale}"
+        return self._name if self._locale is None else "%s_%s" % (self._name, self._locale)
 
     @property
-    def parent(self) -> ResourceBundle:
+    def parent(self) -> "ResourceBundle":
         """
         Get the ResourceBundles parent ResourceBundle
         """
         return self._parent
 
-    def _get_parent_bundle(self) -> ResourceBundle | None:
+    def _get_parent_bundle(self) -> Optional["ResourceBundle"]:
         # This is the root bundle
         if self._locale is None:
             return None
 
         # Cut one part off of the locale
         *parts, _ = self._locale.split("_")
         # If nothing is left set the locale to None else to the shortened locale
@@ -144,36 +142,36 @@
         if self.__cached_bundles.get(parent_locale) is not None:
             return self.__cached_bundles.get(parent_locale)
         # Not cached, start building chain
         return ResourceBundle(self._name, parent_locale, path=self._path)
 
     def _map(self) -> dict[str, str]:
         try:
-            return _Parser.parse(self._path / f"{self.name}.properties")
+            return _Parser.parse(self._path / ("%s.properties" % self.name))
         except FileNotFoundError:
             return dict()
 
     @staticmethod
     def _ensure_path(path: str | PathLike | None) -> Path:
         if isinstance(path, PathLike):
             return Path(path.__fspath__())
         if isinstance(path, str):
             return Path(path)
         if path is None:
             return Path()
-        raise TypeError(f"Path must be of type str or PathLike, not {type(path)}")
+        raise TypeError("Path must be of type str or PathLike, not %s" % type(path))
 
     def __getitem__(self, item) -> str:
         return self.get(item)
 
     def keys(self) -> KeysView[str, str]:
         """
         Return all keys present in this specific ResourceBundle
         """
-        return self._mapping.keys()
+        return self._mapping.keys()  # type: ignore
 
     def get(self, item: str, __default: str = None) -> str:
         """
         Get the value of ``item`` from this or a parent ResourceBundle
 
         :param str item: The key to look up
         :param str __default: A default value that is returned if the key can't be found anywhere
@@ -228,15 +226,29 @@
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\\n"
 "Language-Team: LANGUAGE <LL@li.org>\\n"
 "MIME-Version: 1.0\\n"
 "Content-Type: text/plain; charset=UTF-8\\n"
 "Content-Transfer-Encoding: 8bit\\n"
 "Generated-By: ResourceBundle {version}\\n"
 
-''' # from pygettext.py
+'''  # from pygettext.py
+
+
+def get_package_version() -> str:
+    import sys
+    if (3, 8) < sys.version_info:
+        from importlib_metadata import version
+        from importlib_metadata import PackageNotFoundError
+    else:
+        from importlib.metadata import version
+        from importlib.metadata import PackageNotFoundError
+    try:
+        return version("ResourceBundle")
+    except PackageNotFoundError:
+        return "unknown"
 
 
 class Converter:
     @staticmethod
     def to_gettext(src_path: str | PathLike, dst_path: str | PathLike) -> None:
         """
         Convert ResourceBundle files to a gettext folder structure.
@@ -254,23 +266,23 @@
         resource_bundle_files = [filename for filename in listdir(src_path) if filename.endswith(".properties")]
         if len(resource_bundle_files) == 0:
             raise ValueError("No .properties files found in the src_path.")
 
         for filename in resource_bundle_files:
             if '_' not in filename:
                 bundle_name, locale = (src_path / filename).stem, None
-                dst_file_path = dst_path / f"{bundle_name}_restored_default_values.po"
+                dst_file_path = dst_path / ("%s_restored_default_values.po" % bundle_name)
             else:
                 bundle_name, locale = (src_path / filename).stem.split("_", 1)
-                dst_file_path = dst_path / locale / "LC_MESSAGES" / f"{bundle_name}.po"
+                dst_file_path = dst_path / locale / "LC_MESSAGES" / ("%s.po" % bundle_name)
 
             dst_file_path.parent.mkdir(parents=True, exist_ok=True)
             with open(dst_file_path, mode="w") as dst_fd:
-                dst_fd.write(_pot_header.format(time=datetime.now().strftime("%Y-%m-%d %H:%M%z"), version=__version__))
+                dst_fd.write(_pot_header.format(time=datetime.now().strftime("%Y-%m-%d %H:%M%z"), version=get_package_version()))  # noqa: E501
                 for key, value in dict(get_bundle(bundle_name, locale, path=src_path)).items():
-                    dst_fd.write(f'msgid "{key}"\nmsgstr "{value.strip()}"\n\n')
+                    dst_fd.write('msgid "%s"\nmsgstr "{value.strip()}"\n\n' % key)
                     msg_ids.add(key)
 
         with open(dst_path / "base.pot", mode="w") as f:
-            f.write(_pot_header.format(time=datetime.now().strftime("%Y-%m-%d %H:%M%z"), version=__version__))
+            f.write(_pot_header.format(time=datetime.now().strftime("%Y-%m-%d %H:%M%z"), version=get_package_version()))
             for msg_id in sorted(msg_ids):
-                f.write(f'msgid "{msg_id}"\nmsgstr ""\n\n')
+                f.write('msgid "%s"\nmsgstr ""\n\n' % msg_id)
```

### Comparing `ResourceBundle-2.1.0/ResourceBundle/exceptions.py` & `resourcebundle-2.2.0/ResourceBundle/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+"""
+Module that contains all exceptions that are part of the ResourceBundle package.
+"""
+
+
 class ResourceBundleError(LookupError):
-    pass
+    """Base class for all exceptions in the ResourceBundle module."""
 
 
 class MalformedResourceBundleError(ResourceBundleError):
-    """
-    Error that indicates that a ResourceBundle is malformed.
-    """
+    """Error that indicates that a ResourceBundle is malformed."""
 
 
 class NotInResourceBundleError(ResourceBundleError):
+    """Error that is raised when a key could not be found in a ResourceBundle."""
 
-    def __init__(self, bundle_name: str, key: str):
-        """
-        Error that is raised when a key could not be found in a ResourceBundle.
+    def __init__(self, bundle_name: str, key: str) -> None:
+        """Initialize a new NotInResourceBundleError.
 
         :param str bundle_name: The name of the ResourceBundle
         :param str key: The key that could not be found
         """
-        super(NotInResourceBundleError, self).__init__(f"Can't find key {key} in bundle {bundle_name}!")
+        super(NotInResourceBundleError, self).__init__("Can't find key %s in bundle %s!" % (key, bundle_name))
```

### Comparing `ResourceBundle-2.1.0/ResourceBundle.egg-info/PKG-INFO` & `resourcebundle-2.2.0/ResourceBundle.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 Metadata-Version: 2.1
 Name: ResourceBundle
-Version: 2.1.0
-Summary: ResourceBundle is a module that manages internationalization of string resources
-Home-page: https://felix-zenk.github.io/projects/ResourceBundle
+Version: 2.2.0
+Summary: ResourceBundle is a module that manages internationalization of string resources.
+Home-page: https://github.com/felix-zenk/ResourceBundle
 Author: Felix Zenk
-Author-email: felix.zenk@web.de
-Project-URL: Bug Reports, https://github.com/felix-zenk/ResourceBundle/issues
-Project-URL: Source, https://github.com/felix-zenk/ResourceBundle
+Author-email: Felix Zenk <felix.zenk@web.de>
+License: MIT
+Project-URL: Homepage, https://github.com/felix-zenk/ResourceBundle
+Project-URL: Documentation, https://github.com/felix-zenk/ResourceBundle
+Project-URL: Repository, https://github.com/felix-zenk/ResourceBundle
+Project-URL: Issues, https://github.com/felix-zenk/ResourceBundle/issues
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: importlib_metadata; python_version < "3.8"
 
 # ResourceBundle
 
 [![PyPI-Versions](https://img.shields.io/pypi/pyversions/ResourceBundle)](https://pypi.org/project/ResourceBundle)
 [![PyPI version](https://badge.fury.io/py/ResourceBundle.svg)](https://pypi.org/project/ResourceBundle)
-[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/onboardapis/blob/main/LICENSE)
+[![Build package](https://github.com/felix-zenk/ResourceBundle/actions/workflows/build.yaml/badge.svg)](https://github.com/felix-zenk/ResourceBundle/actions/workflows/build.yaml)
+[![License](https://img.shields.io/github/license/felix-zenk/onboardapis)](https://github.com/felix-zenk/ResourceBundle/blob/main/LICENSE)
 
+ResourceBundle is a package that manages internationalization / localization (i18n / l10n) of string resources.
+It is inspired by Java's ResourceBundle and accepts the same format as a Java ``PropertyResourceBundle``.
 
-ResourceBundle is a module that manages internationalization of string resources.
-It is inspired by javas ResourceBundle and accepts the same format as a java PropertyResourceBundle.
-
-> **Note:** ResourceBundle is not the python way of doing internationalization.
+> **Note:** ResourceBundle is not the pythonic way of internationalization / localization.
 > This package is only intended to be used if you *absolutely have* to work with ResourceBundle files
-> or need a quick working way when porting from java.
+> or need a quick working way when porting from Java.
 >
 > For information on how to do internationalization in python,
 > see the [official documentation](https://docs.python.org/3/library/gettext.html).
-> You can use the `ResourceBundle.Converter.to_gettext()` method to convert your ResourceBundle files to gettext po files.
+> You can use the [`ResourceBundle.Converter.to_gettext()`](#gettext)
+> method to convert your ResourceBundle files to gettext `po` files.
 
 ---
 ### Installation
 
 The ResourceBundle module can be downloaded from [PyPI](https://pypi.org/project/ResourceBundle):
 
 ```bash
-# linux / macOS
+# Linux / macOS
 $  python3 -m pip install ResourceBundle
 
-# windows
+# Windows
 >  py -m pip install ResourceBundle
 ```
 
 ### Usage
 
-Assuming you come from java, you are probably familiar with the ResourceBundle file format.
-If not,you can read about it
+Assuming you come from Java, you are probably familiar with the ResourceBundle file format.
+If not, you can read about it
 [here](https://docs.oracle.com/en/java/javase/20/docs/api/java.base/java/util/PropertyResourceBundle.html).
 
 Get a ResourceBundle instance is by using ``ResourceBundle.get_bundle(name, locale)``.
 
 ```python
 import ResourceBundle
 
@@ -73,20 +81,21 @@
 until a matching key was found.
 If the key is not present in any of its parents a ``ResourceBundle.exceptions.NotInResourceBundleError`` will be raised.
 
 ---
 
 ### gettext
 
-The ResourceBundle module can convert ResourceBundle files to gettext pot / po files.
-This can be done by using the ``ResourceBundle.Converter.to_gettext()`` function.
+The ResourceBundle module can convert ResourceBundle files to gettext `pot` / `po` files.
+This can be done by using the ``ResourceBundle.Converter.to_gettext()`` method.
 
 ```python
 from ResourceBundle import Converter
 
 # convert all .properties files in the current directory to .po files
 Converter.to_gettext(".", ".")
 ```
 
-Note however that this step is obsolete if you are using gettext properly
-as this will include automatically extracting strings from your source code.
+Note however that this step is obsolete if you are using ``gettext`` properly
+as this will include automatically extracting strings from your source code with the help of a library like
+[Babel](https://babel.pocoo.org/en/latest/) with its [pybabel](https://babel.pocoo.org/en/latest/cmdline.html) tool.
 The function is only intended as a head start to keep existing translations.
```

### Comparing `ResourceBundle-2.1.0/setup.py` & `resourcebundle-2.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 import setuptools
-from ResourceBundle import __version__
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
-homepage = "https://felix-zenk.github.io/projects/ResourceBundle"
-source = "https://github.com/felix-zenk/ResourceBundle"
+
+with open('pyproject.toml', mode='r', encoding='utf-8') as f:
+    version = f.read().split('version = ')[1].split('\n')[0].strip().replace('"', '')
 
 
 setuptools.setup(
     name="ResourceBundle",
-    version=__version__,
+    version=version,
     author='Felix Zenk',
     author_email='felix.zenk@web.de',
-    description="ResourceBundle is a module that manages internationalization of string resources",
+    description="ResourceBundle is a module that manages internationalization of string resources.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url=homepage,
+    url="https://github.com/felix-zenk/ResourceBundle",
     project_urls={
-        "Bug Reports": f"{source}/issues",
-        "Source": source
+        "Issues": "https://github.com/felix-zenk/ResourceBundle/issues",
+        "Repository": "https://github.com/felix-zenk/ResourceBundle",
+        "Documentation": "https://github.com/felix-zenk/ResourceBundle",
     },
-    packages=setuptools.find_packages(".", exclude=["tests", "tests.*"]),
+    packages=setuptools.find_packages(".", include=["ResourceBundle*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
+        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13',
         'Topic :: Utilities',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent"
     ],
-    python_requires='>=3.6'
+    python_requires='>=3.5'
 )
```

