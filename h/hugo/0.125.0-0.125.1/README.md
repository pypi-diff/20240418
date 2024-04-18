# Comparing `tmp/hugo-0.125.0.tar.gz` & `tmp/hugo-0.125.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugo-0.125.0.tar", last modified: Tue Apr 16 17:06:13 2024, max compression
+gzip compressed data, was "hugo-0.125.1.tar", last modified: Thu Apr 18 10:54:37 2024, max compression
```

## Comparing `hugo-0.125.0.tar` & `hugo-0.125.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:06:13.769637 hugo-0.125.0/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-16 17:06:06.000000 hugo-0.125.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-16 17:06:06.000000 hugo-0.125.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-16 17:06:06.000000 hugo-0.125.0/LICENSE-hugo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-16 17:06:06.000000 hugo-0.125.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-16 17:06:13.769637 hugo-0.125.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19810 2024-04-16 17:06:06.000000 hugo-0.125.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-16 17:06:06.000000 hugo-0.125.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:06:13.769637 hugo-0.125.0/hugo/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-16 17:06:06.000000 hugo-0.125.0/hugo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:06:13.769637 hugo-0.125.0/hugo/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 17:06:06.000000 hugo-0.125.0/hugo/binaries/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-16 17:06:06.000000 hugo-0.125.0/hugo/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-16 17:06:06.000000 hugo-0.125.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-16 17:06:13.773637 hugo-0.125.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-16 17:06:06.000000 hugo-0.125.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:54:37.450910 hugo-0.125.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-18 10:54:33.000000 hugo-0.125.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-18 10:54:33.000000 hugo-0.125.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-18 10:54:33.000000 hugo-0.125.1/LICENSE-hugo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-18 10:54:33.000000 hugo-0.125.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-18 10:54:37.450910 hugo-0.125.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19810 2024-04-18 10:54:33.000000 hugo-0.125.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-18 10:54:33.000000 hugo-0.125.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:54:37.450910 hugo-0.125.1/hugo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-18 10:54:33.000000 hugo-0.125.1/hugo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 10:54:37.450910 hugo-0.125.1/hugo/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 10:54:33.000000 hugo-0.125.1/hugo/binaries/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-18 10:54:33.000000 hugo-0.125.1/hugo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-04-18 10:54:33.000000 hugo-0.125.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 10:54:37.450910 hugo-0.125.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-18 10:54:33.000000 hugo-0.125.1/setup.py
```

### Comparing `hugo-0.125.0/CODE_OF_CONDUCT.md` & `hugo-0.125.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/LICENSE` & `hugo-0.125.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/LICENSE-hugo.txt` & `hugo-0.125.1/LICENSE-hugo.txt`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/PKG-INFO` & `hugo-0.125.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.125.0
+Version: 0.125.1
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
```

### Comparing `hugo-0.125.0/README.md` & `hugo-0.125.1/README.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/SECURITY.md` & `hugo-0.125.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/hugo/cli.py` & `hugo-0.125.1/hugo/cli.py`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/pyproject.toml` & `hugo-0.125.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hugo-0.125.0/setup.py` & `hugo-0.125.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 
 import pooch
 from setuptools import Command, Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from wheel.bdist_wheel import bdist_wheel
 
-HUGO_VERSION = "0.125.0"
+HUGO_VERSION = "0.125.1"
 HUGO_RELEASE = (
     f"https://github.com/gohugoio/hugo/archive/refs/tags/v{HUGO_VERSION}.tar.gz"
 )
 # Commit hash for current HUGO_VERSION, needs to be updated when HUGO_VERSION is updated
 # Tip: git ls-remote --tags https://github.com/gohugoio/hugo v<HUGO_VERSION>
-HUGO_RELEASE_COMMIT_HASH = "a32400b5f4e704daf7de19f44584baf77a4501ab"
+HUGO_RELEASE_COMMIT_HASH = "68c5ad638c2072969e47262926b912e80fd71a77"
 # The pooch tool will download the tarball into the hugo_cache/ directory.
 # We will point the build command to that location to build Hugo from source
 HUGO_CACHE_DIR = "hugo_cache"
-HUGO_SHA256 = "035535de873ce70da5bb39872a860b42134364b3a6a95f075cbc07e96b7ef127"
+HUGO_SHA256 = "dc902d7a2983925b218e17d21e510867a97e0b8c0e0093e4a6a22dabdb21c230"
 FILE_EXT = (
     ".exe" if (sys.platform == "win32" or os.environ.get("GOOS") == "windows") else ""
 )
 
 # The vendor name is used to set the vendorInfo variable in the Hugo binary
 HUGO_VENDOR_NAME = "hugo-python-distributions"
```

