# Comparing `tmp/mozilla-version-2.2.0.tar.gz` & `tmp/mozilla-version-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-version-2.2.0.tar", last modified: Wed Apr 17 14:23:32 2024, max compression
+gzip compressed data, was "mozilla-version-2.3.0.tar", last modified: Wed Apr 17 16:43:04 2024, max compression
```

## Comparing `mozilla-version-2.2.0.tar` & `mozilla-version-2.3.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.204070 mozilla-version-2.2.0/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/LICENSE
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/MANIFEST.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2024-04-17 14:23:32.203953 mozilla-version-2.2.0/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla-version-2.2.0/README.md
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.200083 mozilla-version-2.2.0/mozilla_version/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      262 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     4961 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     2468 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    28669 2024-04-17 14:22:13.000000 mozilla-version-2.2.0/mozilla_version/gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1988 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     9520 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1335 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/parser.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.202441 mozilla-version-2.2.0/mozilla_version/test/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/__init__.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/test_balrog.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      268 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/test/test_default_imports.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/test_errors.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla-version-2.2.0/mozilla_version/test/test_fenix.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    41476 2024-04-17 14:22:13.000000 mozilla-version-2.2.0/mozilla_version/test/test_gecko.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     3526 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/test/test_maven.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    11948 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/test/test_mobile.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla-version-2.2.0/mozilla_version/test/test_version.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     7929 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/mozilla_version/version.py
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.200849 mozilla-version-2.2.0/mozilla_version.egg-info/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2024-04-17 14:23:31.000000 mozilla-version-2.2.0/mozilla_version.egg-info/PKG-INFO
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      973 2024-04-17 14:23:32.000000 mozilla-version-2.2.0/mozilla_version.egg-info/SOURCES.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-17 14:23:31.000000 mozilla-version-2.2.0/mozilla_version.egg-info/dependency_links.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-17 08:07:18.000000 mozilla-version-2.2.0/mozilla_version.egg-info/not-zip-safe
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2024-04-17 14:23:32.000000 mozilla-version-2.2.0/mozilla_version.egg-info/requires.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2024-04-17 14:23:32.000000 mozilla-version-2.2.0/mozilla_version.egg-info/top_level.txt
-drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 14:23:32.203642 mozilla-version-2.2.0/requirements/
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/requirements/base.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      363 2024-04-17 07:59:45.000000 mozilla-version-2.2.0/requirements/base.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       70 2022-11-25 14:28:49.000000 mozilla-version-2.2.0/requirements/docs.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)    15614 2024-04-17 07:59:45.000000 mozilla-version-2.2.0/requirements/docs.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)      143 2024-04-17 07:59:39.000000 mozilla-version-2.2.0/requirements/test.in
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     8589 2024-04-17 07:59:45.000000 mozilla-version-2.2.0/requirements/test.txt
--rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2024-04-17 14:23:32.204112 mozilla-version-2.2.0/setup.cfg
--rw-r--r--   0 johanlorenzo   (501) staff       (20)     1194 2023-05-23 08:14:29.000000 mozilla-version-2.2.0/setup.py
--rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2024-04-17 14:22:13.000000 mozilla-version-2.2.0/version.txt
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 16:43:04.971125 mozilla-version-2.3.0/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    15922 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/LICENSE
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      139 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/MANIFEST.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2024-04-17 16:43:04.970998 mozilla-version-2.3.0/PKG-INFO
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7491 2022-11-25 16:16:39.000000 mozilla-version-2.3.0/README.md
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 16:43:04.968082 mozilla-version-2.3.0/mozilla_version/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      262 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/__init__.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     4961 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/balrog.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     2468 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/errors.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      199 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/mozilla_version/fenix.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    28030 2024-04-17 16:42:34.000000 mozilla-version-2.3.0/mozilla_version/gecko.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1988 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/maven.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     9478 2024-04-17 16:42:34.000000 mozilla-version-2.3.0/mozilla_version/mobile.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1335 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/parser.py
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 16:43:04.970080 mozilla-version-2.3.0/mozilla_version/test/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       87 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/mozilla_version/test/__init__.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7839 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/mozilla_version/test/test_balrog.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      268 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/test/test_default_imports.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      933 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/mozilla_version/test/test_errors.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      193 2022-07-07 15:15:03.000000 mozilla-version-2.3.0/mozilla_version/test/test_fenix.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    41476 2024-04-17 14:22:13.000000 mozilla-version-2.3.0/mozilla_version/test/test_gecko.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     3526 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/test/test_maven.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    11948 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/mozilla_version/test/test_mobile.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     7441 2022-06-29 08:41:37.000000 mozilla-version-2.3.0/mozilla_version/test/test_version.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    10049 2024-04-17 16:42:34.000000 mozilla-version-2.3.0/mozilla_version/version.py
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 16:43:04.968941 mozilla-version-2.3.0/mozilla_version.egg-info/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      451 2024-04-17 16:43:04.000000 mozilla-version-2.3.0/mozilla_version.egg-info/PKG-INFO
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      973 2024-04-17 16:43:04.000000 mozilla-version-2.3.0/mozilla_version.egg-info/SOURCES.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-17 16:43:04.000000 mozilla-version-2.3.0/mozilla_version.egg-info/dependency_links.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        1 2024-04-17 15:47:57.000000 mozilla-version-2.3.0/mozilla_version.egg-info/not-zip-safe
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2024-04-17 16:43:04.000000 mozilla-version-2.3.0/mozilla_version.egg-info/requires.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       16 2024-04-17 16:43:04.000000 mozilla-version-2.3.0/mozilla_version.egg-info/top_level.txt
+drwxr-xr-x   0 johanlorenzo   (501) staff       (20)        0 2024-04-17 16:43:04.970817 mozilla-version-2.3.0/requirements/
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       12 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/requirements/base.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      363 2024-04-17 07:59:45.000000 mozilla-version-2.3.0/requirements/base.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       70 2022-11-25 14:28:49.000000 mozilla-version-2.3.0/requirements/docs.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)    15614 2024-04-17 07:59:45.000000 mozilla-version-2.3.0/requirements/docs.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)      143 2024-04-17 07:59:39.000000 mozilla-version-2.3.0/requirements/test.in
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     8589 2024-04-17 07:59:45.000000 mozilla-version-2.3.0/requirements/test.txt
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)       38 2024-04-17 16:43:04.971175 mozilla-version-2.3.0/setup.cfg
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)     1194 2023-05-23 08:14:29.000000 mozilla-version-2.3.0/setup.py
+-rw-r--r--   0 johanlorenzo   (501) staff       (20)        6 2024-04-17 16:42:34.000000 mozilla-version-2.3.0/version.txt
```

### Comparing `mozilla-version-2.2.0/LICENSE` & `mozilla-version-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/README.md` & `mozilla-version-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/balrog.py` & `mozilla-version-2.3.0/mozilla_version/balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/errors.py` & `mozilla-version-2.3.0/mozilla_version/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/gecko.py` & `mozilla-version-2.3.0/mozilla_version/gecko.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 import attr
 import re
 
 from mozilla_version.errors import (
     PatternNotMatchedError, TooManyTypesError, NoVersionTypeError
 )
 from mozilla_version.parser import strictly_positive_int_or_none
-from mozilla_version.version import BaseVersion, VersionType
+from mozilla_version.version import BaseVersion, ShipItVersion, VersionType
 
 
 def _find_type(version):
     version_type = None
 
     def ensure_version_type_is_not_already_defined(previous_type, candidate_type):
         if previous_type is not None:
@@ -88,15 +88,15 @@
     if version_type is None:
         raise NoVersionTypeError(str(version))
 
     return version_type
 
 
 @attr.s(frozen=True, eq=False, hash=True)
-class GeckoVersion(BaseVersion):
+class GeckoVersion(ShipItVersion):
     """Class that validates and handles version numbers for Gecko-based products.
 
     You may want to use specific classes like FirefoxVersion. These classes define edge cases
     that were shipped.
 
     Raises:
         PatternNotMatchedError: if the string doesn't match the pattern of a valid version number
@@ -142,46 +142,38 @@
     is_esr = attr.ib(type=bool, default=False)
     old_fourth_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
     release_candidate_number = attr.ib(
         type=int, converter=strictly_positive_int_or_none, default=None
     )
     version_type = attr.ib(init=False, default=attr.Factory(_find_type, takes_self=True))
 
-    def __attrs_post_init__(self):
-        """Ensure attributes are sane all together."""
+    def _get_all_error_messages_for_attributes(self):
+        error_messages = super()._get_all_error_messages_for_attributes()
+
         # General checks
-        error_messages = [
+        error_messages.extend([
             pattern_message
             for condition, pattern_message in ((
                 not self.is_four_digit_scheme and self.old_fourth_number is not None,
                 'The old fourth number can only be defined on Gecko 1.5.x.y or 2.0.x.y',
             ), (
                 self.beta_number is not None and self.patch_number is not None,
                 'Beta number and patch number cannot be both defined',
             ), (
                 self.is_major and self.is_esr,
                 'Version cannot be both a major and an ESR one',
             ), (
-                self.is_major and self.is_stability,
-                'Version cannot be both a major and a stability one',
-            ), (
-                self.is_major and self.is_development,
-                'Version cannot be both a major and a development one',
-            ), (
                 self.is_stability and self.is_esr,
                 'Version cannot be both a stability and an ESR one',
             ), (
-                self.is_stability and self.is_development,
-                'Version cannot be both a stability and a development one',
-            ), (
                 self.is_development and self.is_esr,
                 'Version cannot be both a development and an ESR one',
             ))
             if condition
-        ]
+        ])
 
         # Firefox 5 is the first version to implement the rapid release model, which defines
         # the scheme used so far.
         if self.is_rapid_release_scheme:
             error_messages.extend([
                 pattern_message
                 for condition, pattern_message in ((
@@ -231,16 +223,15 @@
 
             if self.old_fourth_number is not None and self.patch_number != 0:
                 error_messages.append(
                     'The old fourth number cannot be defined if the patch number is not 0 '
                     '(we have never shipped a release that did so)'
                 )
 
-        if error_messages:
-            raise PatternNotMatchedError(self, patterns=error_messages)
+        return error_messages
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Firefox version number."""
         return super().parse(
             version_string, regex_groups=('is_nightly', 'is_aurora_or_devedition', 'is_esr')
         )
@@ -282,52 +273,36 @@
     @property
     def is_major(self):
         """Return `True` if `GeckoVersion` is considered to be a major version.
 
         It's usually the .0 release but some exceptions may occur. ESR are not considered
         major versions.
         """
-        return all((
-            not self.is_development,
-            not self.is_esr,
-            self.minor_number == 0,
-            self.patch_number is None
-        ))
+        return super().is_major and not self.is_esr
 
     @property
     def is_stability(self):
         """Return `True` if `GeckoVersion` is a version that fixed a major one."""
         conditions = [
-            not self.is_development,
-            not self.is_major,
             not self.is_esr,
         ]
         if self.is_four_digit_scheme:
+            # super().is_stability has an incompatible condition. So we must not use it
+            # in this specific case.
             conditions.extend([
+                not self.is_development,
+                not self.is_major,
                 self.patch_number == 0,
                 self.old_fourth_number != 0,
             ])
         else:
-            conditions.append(
-                self.minor_number != 0 or self.patch_number != 0
-            )
+            conditions.append(super().is_stability)
 
         return all(conditions)
 
-    @property
-    def is_development(self):
-        """Return `True` if `GeckoVersion` was known to require further development.
-
-        It's usually a beta or before the rapid release scheme, a release candidate.
-        """
-        return any((
-            self.is_beta,
-            self.is_release_candidate,
-        ))
-
     def __str__(self):
         """Implement string representation.
 
         Computes a new string based on the given attributes.
         """
         string = super().__str__()
 
@@ -640,24 +615,26 @@
 
 
 class DeveditionVersion(GeckoVersion):
     """Class that validates and handles Devedition after it became an equivalent to beta."""
 
     # No edge case were shipped
 
-    def __attrs_post_init__(self):
+    def _get_all_error_messages_for_attributes(self):
         """Ensure attributes are sane all together."""
+        error_messages = super()._get_all_error_messages_for_attributes()
+
         if (
             (not self.is_beta) or
             (self.major_number < 54) or
             (self.major_number == 54 and self.beta_number < 11)
         ):
-            raise PatternNotMatchedError(
-                self, patterns=('Devedition as a product must be a beta >= 54.0b11',)
-            )
+            error_messages.append('Devedition as a product must be a beta >= 54.0b11')
+
+        return error_messages
 
 
 class FennecVersion(_VersionWithEdgeCases):
     """Class that validates and handles Fennec (Firefox for Android) version numbers."""
 
     _RELEASED_EDGE_CASES = ({
         'major_number': 33,
@@ -701,20 +678,22 @@
         if (
             self.major_number == self._LAST_FENNEC_VERSION and
             self.minor_number > 0 and
             self.patch_number is None
         ):
             return
 
+        super().__attrs_post_init__()
+
+    def _get_all_error_messages_for_attributes(self):
+        error_messages = super()._get_all_error_messages_for_attributes()
         if self.major_number > self._LAST_FENNEC_VERSION:
-            raise PatternNotMatchedError(
-                self, patterns=(f'Last Fennec version is {self._LAST_FENNEC_VERSION}',)
-            )
+            error_messages.append(f'Last Fennec version is {self._LAST_FENNEC_VERSION}')
 
-        super().__attrs_post_init__()
+        return error_messages
 
     def _create_bump_kwargs(self, field):
         kwargs = super()._create_bump_kwargs(field)
 
         if (
             field != 'patch_number' and
             kwargs['major_number'] == self._LAST_FENNEC_VERSION and
```

### Comparing `mozilla-version-2.2.0/mozilla_version/maven.py` & `mozilla-version-2.3.0/mozilla_version/maven.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/mobile.py` & `mozilla-version-2.3.0/mozilla_version/mobile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Defines characteristics of a Mobile version at Mozilla."""
 
 import attr
 import re
 
 from mozilla_version.errors import PatternNotMatchedError, TooManyTypesError, NoVersionTypeError
 from mozilla_version.gecko import GeckoVersion
-from mozilla_version.version import BaseVersion, VersionType
+from mozilla_version.version import BaseVersion, ShipItVersion, VersionType
 from mozilla_version.parser import strictly_positive_int_or_none
 
 
 def _find_type(version):
     version_type = None
 
     def ensure_version_type_is_not_already_defined(previous_type, candidate_type):
@@ -33,15 +33,15 @@
     if version_type is None:
         raise NoVersionTypeError(str(version))
 
     return version_type
 
 
 @attr.s(frozen=True, eq=False, hash=True)
-class MobileVersion(BaseVersion):
+class MobileVersion(ShipItVersion):
     """Validate and handle version numbers for mobile products.
 
     This covers applications such as Fenix and Focus for Android.
     """
 
     _VALID_ENOUGH_VERSION_PATTERN = re.compile(r"""
         ^(?P<major_number>\d+)
@@ -70,17 +70,16 @@
     beta_number = attr.ib(type=int, converter=strictly_positive_int_or_none, default=None)
     is_nightly = attr.ib(type=bool, default=False)
     release_candidate_number = attr.ib(
         type=int, converter=strictly_positive_int_or_none, default=None
     )
     version_type = attr.ib(init=False, default=attr.Factory(_find_type, takes_self=True))
 
-    def __attrs_post_init__(self):
-        """Ensure attributes are sane all together."""
-        error_messages = []
+    def _get_all_error_messages_for_attributes(self):
+        error_messages = super()._get_all_error_messages_for_attributes()
 
         if self.is_gecko_pattern:
             error_messages.extend([
                 pattern_message
                 for condition, pattern_message in ((
                     self.beta_number is not None and self.patch_number is not None,
                     'Beta number and patch number cannot be both defined',
@@ -116,16 +115,15 @@
                     'Nightlies are not supported until Mobile v{}'.format(
                         self._FIRST_VERSION_TO_FOLLOW_GECKO_PATTERN
                     ),
                 ))
                 if condition
             ])
 
-        if error_messages:
-            raise PatternNotMatchedError(self, patterns=error_messages)
+        return error_messages
 
     @classmethod
     def parse(cls, version_string):
         """Construct an object representing a valid Firefox version number."""
         mobile_version = super().parse(
             version_string, regex_groups=('is_nightly',)
         )
```

### Comparing `mozilla-version-2.2.0/mozilla_version/parser.py` & `mozilla-version-2.3.0/mozilla_version/parser.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/test/test_balrog.py` & `mozilla-version-2.3.0/mozilla_version/test/test_balrog.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/test/test_errors.py` & `mozilla-version-2.3.0/mozilla_version/test/test_errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/test/test_gecko.py` & `mozilla-version-2.3.0/mozilla_version/test/test_gecko.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/test/test_maven.py` & `mozilla-version-2.3.0/mozilla_version/test/test_maven.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/test/test_mobile.py` & `mozilla-version-2.3.0/mozilla_version/test/test_mobile.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version/test/test_version.py` & `mozilla-version-2.3.0/mozilla_version/test/test_version.py`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/mozilla_version.egg-info/SOURCES.txt` & `mozilla-version-2.3.0/mozilla_version.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/requirements/docs.txt` & `mozilla-version-2.3.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/requirements/test.txt` & `mozilla-version-2.3.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `mozilla-version-2.2.0/setup.py` & `mozilla-version-2.3.0/setup.py`

 * *Files identical despite different names*

