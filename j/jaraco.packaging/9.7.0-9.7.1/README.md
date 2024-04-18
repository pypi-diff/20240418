# Comparing `tmp/jaraco_packaging-9.7.0.tar.gz` & `tmp/jaraco_packaging-9.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco_packaging-9.7.0.tar", last modified: Wed Apr 17 02:58:44 2024, max compression
+gzip compressed data, was "jaraco_packaging-9.7.1.tar", last modified: Wed Apr 17 21:32:54 2024, max compression
```

## Comparing `jaraco_packaging-9.7.0.tar` & `jaraco_packaging-9.7.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.811431 jaraco_packaging-9.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.811431 jaraco_packaging-9.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.811431 jaraco_packaging-9.7.0/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/jaraco/packaging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/make-tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/jaraco/packaging/sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 02:58:44.815431 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 02:58:44.000000 jaraco_packaging-9.7.0/jaraco.packaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 02:58:44.819431 jaraco_packaging-9.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 02:58:29.000000 jaraco_packaging-9.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.929577 jaraco_packaging-9.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.925577 jaraco_packaging-9.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.925577 jaraco_packaging-9.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 21:32:54.929577 jaraco_packaging-9.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.925577 jaraco_packaging-9.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.921577 jaraco_packaging-9.7.1/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.929577 jaraco_packaging-9.7.1/jaraco/packaging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/jaraco/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/jaraco/packaging/make-tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/jaraco/packaging/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/jaraco/packaging/sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 21:32:54.929577 jaraco_packaging-9.7.1/jaraco.packaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 21:32:54.000000 jaraco_packaging-9.7.1/jaraco.packaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-17 21:32:54.000000 jaraco_packaging-9.7.1/jaraco.packaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 21:32:54.000000 jaraco_packaging-9.7.1/jaraco.packaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-17 21:32:54.000000 jaraco_packaging-9.7.1/jaraco.packaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 21:32:54.000000 jaraco_packaging-9.7.1/jaraco.packaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 21:32:54.929577 jaraco_packaging-9.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-17 21:32:37.000000 jaraco_packaging-9.7.1/tox.ini
```

### Comparing `jaraco_packaging-9.7.0/.github/workflows/main.yml` & `jaraco_packaging-9.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/LICENSE` & `jaraco_packaging-9.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/NEWS.rst` & `jaraco_packaging-9.7.1/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v9.7.1
+======
+
+Bugfixes
+--------
+
+- In extract_author, expand the logic to support multiple authors in pyproject.toml form.
+
+
 v9.7.0
 ======
 
 Features
 --------
 
 - Configure Sphinx earlier in 'config-inited', allowing other etxensions to rely on the produced values. (#16)
```

### Comparing `jaraco_packaging-9.7.0/PKG-INFO` & `jaraco_packaging-9.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.7.0
+Version: 9.7.1
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco_packaging-9.7.0/README.rst` & `jaraco_packaging-9.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/docs/conf.py` & `jaraco_packaging-9.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/jaraco/packaging/make-tree.py` & `jaraco_packaging-9.7.1/jaraco/packaging/make-tree.py`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/jaraco/packaging/sphinx.py` & `jaraco_packaging-9.7.1/jaraco/packaging/sphinx.py`

 * *Files 21% similar despite different names*

```diff
@@ -131,16 +131,41 @@
     lookup = dict(url.split(', ') for url in project_urls)
     return lookup.get('Source') or lookup.get('Homepage')
 
 
 def extract_author(meta):
     """
     Given project metadata, figure out who the author is.
+
+    The metadata is so irregular, just make some inferences and refine.
+
+    This form comes from a setup.cfg file or setup.py.
+
+    >>> meta = {'Author': 'Jason R. Coombs'}
+    >>> extract_author(meta)
+    'Jason R. Coombs'
+    >>> meta = {'Author': 'Foo Bar, Bing Baz'}
+    >>> extract_author(meta)
+    'Foo Bar, Bing Baz'
+
+    This form comes from pyproject.toml converted from the above config.
+
+    >>> meta = {'Author-email': '"Jason R. Coombs" <jaraco@contoso.com>', 'Author': None}
+    >>> extract_author(meta)
+    'Jason R. Coombs'
+    >>> meta = {'Author-email': 'Foo Bar <foo@bar.name>, Bing Baz <bing@baz.name>', 'Author': None}
+    >>> extract_author(meta)
+    'Foo Bar, Bing Baz'
     """
-    return meta['Author'] or re.search(r'"(.+)"', meta['Author-email']).group(1)
+    return meta['Author'] or ', '.join(
+        match.group('name')
+        for match in re.finditer(
+            r'["]?(?P<name>\w[\w\s.]*?)["]?\s+<\w+@[\w.]+>', meta['Author-email']
+        )
+    )
 
 
 def configure_substitutions(app, config):
     epilogs = config.rst_epilog, f'.. |project| replace:: {config.project}'
     config.rst_epilog = '\n'.join(filter(None, epilogs))
```

### Comparing `jaraco_packaging-9.7.0/jaraco.packaging.egg-info/PKG-INFO` & `jaraco_packaging-9.7.1/jaraco.packaging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.packaging
-Version: 9.7.0
+Version: 9.7.1
 Summary: tools to supplement packaging Python releases
 Home-page: https://github.com/jaraco/jaraco.packaging
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco_packaging-9.7.0/jaraco.packaging.egg-info/SOURCES.txt` & `jaraco_packaging-9.7.1/jaraco.packaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/pytest.ini` & `jaraco_packaging-9.7.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/setup.cfg` & `jaraco_packaging-9.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jaraco_packaging-9.7.0/tox.ini` & `jaraco_packaging-9.7.1/tox.ini`

 * *Files identical despite different names*

