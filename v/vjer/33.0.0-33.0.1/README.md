# Comparing `tmp/vjer-33.0.0.tar.gz` & `tmp/vjer-33.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vjer-33.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vjer-33.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vjer-33.0.0.tar` & `vjer-33.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1788 2024-04-18 18:07:15.937749 vjer-33.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2134 2024-04-18 18:07:15.937749 vjer-33.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     5245 2024-04-18 18:07:15.937749 vjer-33.0.0/.gitignore
--rw-r--r--   0        0        0     4999 2024-04-18 18:07:15.937749 vjer-33.0.0/.p4ignore
--rw-r--r--   0        0        0       42 2024-04-18 18:07:15.937749 vjer-33.0.0/.readthedocs.yml
--rw-r--r--   0        0        0    40183 2024-04-18 18:07:15.937749 vjer-33.0.0/CHANGELOG.md
--rw-r--r--   0        0        0       64 2024-04-18 18:07:15.937749 vjer-33.0.0/DOCUMENTATION.md
--rw-r--r--   0        0        0     1072 2024-04-18 18:07:15.937749 vjer-33.0.0/LICENSE
--rw-r--r--   0        0        0       90 2024-04-18 18:07:15.937749 vjer-33.0.0/MANIFEST.in
--rw-r--r--   0        0        0      973 2024-04-18 18:07:15.937749 vjer-33.0.0/README.md
--rwxr-xr-x   0        0        0      878 2024-04-18 18:07:15.937749 vjer-33.0.0/cicd-support/cicd.sh
--rw-r--r--   0        0        0      634 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/Makefile
--rw-r--r--   0        0        0     9167 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/coding_standards.py
--rw-r--r--   0        0        0     2103 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/conf.py
--rw-r--r--   0        0        0      795 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/make.bat
--rw-r--r--   0        0        0       59 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/modules.rst
--rw-r--r--   0        0        0      229 2024-04-18 18:07:15.937749 vjer-33.0.0/docs/requirements.txt
--rw-r--r--   0        0        0     2180 2024-04-18 18:07:53.677923 vjer-33.0.0/pyproject.toml
--rw-r--r--   0        0        0      305 2024-04-18 18:07:15.937749 vjer-33.0.0/util/New-Env.ps1
--rw-r--r--   0        0        0      259 2024-04-18 18:07:15.937749 vjer-33.0.0/util/Update-Env.ps1
--rwxr-xr-x   0        0        0      261 2024-04-18 18:07:15.937749 vjer-33.0.0/util/new-env.sh
--rwxr-xr-x   0        0        0      234 2024-04-18 18:07:15.937749 vjer-33.0.0/util/update-env.sh
--rw-r--r--   0        0        0      476 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer.yml
--rw-r--r--   0        0        0      654 2024-04-18 18:07:53.677923 vjer-33.0.0/vjer/__init__.py
--rw-r--r--   0        0        0      205 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/__main__.py
--rw-r--r--   0        0        0     5278 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/build.py
--rw-r--r--   0        0        0     1185 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/deploy.py
--rw-r--r--   0        0        0     2875 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/freeze.py
--rw-r--r--   0        0        0     1613 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/pre_release.py
--rw-r--r--   0        0        0        0 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/py.typed
--rw-r--r--   0        0        0     3170 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/release.py
--rw-r--r--   0        0        0      769 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/rollback.py
--rw-r--r--   0        0        0     3457 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/test.py
--rw-r--r--   0        0        0     2946 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/tool_reporter.py
--rw-r--r--   0        0        0    25691 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/utils.py
--rwxr-xr-x   0        0        0     2825 2024-04-18 18:07:15.937749 vjer-33.0.0/vjer/vjer.py
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 vjer-33.0.0/setup.py
--rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 vjer-33.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1788 2024-04-18 18:47:56.171917 vjer-33.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2134 2024-04-18 18:47:56.171917 vjer-33.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     5245 2024-04-18 18:47:56.171917 vjer-33.0.1/.gitignore
+-rw-r--r--   0        0        0     4999 2024-04-18 18:47:56.171917 vjer-33.0.1/.p4ignore
+-rw-r--r--   0        0        0       42 2024-04-18 18:47:56.171917 vjer-33.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0    40281 2024-04-18 18:47:56.171917 vjer-33.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0       64 2024-04-18 18:47:56.171917 vjer-33.0.1/DOCUMENTATION.md
+-rw-r--r--   0        0        0     1072 2024-04-18 18:47:56.171917 vjer-33.0.1/LICENSE
+-rw-r--r--   0        0        0       90 2024-04-18 18:47:56.171917 vjer-33.0.1/MANIFEST.in
+-rw-r--r--   0        0        0      973 2024-04-18 18:47:56.171917 vjer-33.0.1/README.md
+-rwxr-xr-x   0        0        0      878 2024-04-18 18:47:56.171917 vjer-33.0.1/cicd-support/cicd.sh
+-rw-r--r--   0        0        0      634 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/Makefile
+-rw-r--r--   0        0        0     9167 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/coding_standards.py
+-rw-r--r--   0        0        0     2103 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/conf.py
+-rw-r--r--   0        0        0      795 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/make.bat
+-rw-r--r--   0        0        0       59 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/modules.rst
+-rw-r--r--   0        0        0      229 2024-04-18 18:47:56.171917 vjer-33.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0     2184 2024-04-18 18:48:25.336224 vjer-33.0.1/pyproject.toml
+-rw-r--r--   0        0        0      305 2024-04-18 18:47:56.171917 vjer-33.0.1/util/New-Env.ps1
+-rw-r--r--   0        0        0      259 2024-04-18 18:47:56.171917 vjer-33.0.1/util/Update-Env.ps1
+-rwxr-xr-x   0        0        0      261 2024-04-18 18:47:56.171917 vjer-33.0.1/util/new-env.sh
+-rwxr-xr-x   0        0        0      234 2024-04-18 18:47:56.171917 vjer-33.0.1/util/update-env.sh
+-rw-r--r--   0        0        0      476 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer.yml
+-rw-r--r--   0        0        0      654 2024-04-18 18:48:25.336224 vjer-33.0.1/vjer/__init__.py
+-rw-r--r--   0        0        0      205 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/__main__.py
+-rw-r--r--   0        0        0     5278 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/build.py
+-rw-r--r--   0        0        0     1185 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/deploy.py
+-rw-r--r--   0        0        0     2875 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/freeze.py
+-rw-r--r--   0        0        0     1613 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/pre_release.py
+-rw-r--r--   0        0        0        0 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/py.typed
+-rw-r--r--   0        0        0     3170 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/release.py
+-rw-r--r--   0        0        0      769 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/rollback.py
+-rw-r--r--   0        0        0     3457 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/test.py
+-rw-r--r--   0        0        0     2946 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/tool_reporter.py
+-rw-r--r--   0        0        0    25691 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/utils.py
+-rwxr-xr-x   0        0        0     2825 2024-04-18 18:47:56.175917 vjer-33.0.1/vjer/vjer.py
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 vjer-33.0.1/setup.py
+-rw-r--r--   0        0        0     1315 1970-01-01 00:00:00.000000 vjer-33.0.1/PKG-INFO
```

### Comparing `vjer-33.0.0/.github/workflows/build.yml` & `vjer-33.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/.github/workflows/publish.yml` & `vjer-33.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/.gitignore` & `vjer-33.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/.p4ignore` & `vjer-33.0.1/.p4ignore`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/CHANGELOG.md` & `vjer-33.0.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,29 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## Current Release
 
+### [33.0.1] - 2024-04-18
+
+- Changed
+  - Switched flit to be a required module. (GitHub #9)
+
+## Release History
+
 ### [33.0.0] - 2024-04-18
 
 - Added
   - Added support for multiple Docker tags and Helm versions at build. (GitHub #8)
 
 - Changed
   - Required specification of full Docker and Helm repo info in config file.
 
-## Release History
-
 ### [32.1.0] - 2024-04-11
 
 - Changed
   - Cleanup version output and add --version option. (GitHub #5)
   - Fix tagging on release. (GitHub #7)
 
 ### [32.0.0] - 2024-04-10
```

### Comparing `vjer-33.0.0/LICENSE` & `vjer-33.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/README.md` & `vjer-33.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/cicd-support/cicd.sh` & `vjer-33.0.1/cicd-support/cicd.sh`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/docs/Makefile` & `vjer-33.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/docs/coding_standards.py` & `vjer-33.0.1/docs/coding_standards.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/docs/conf.py` & `vjer-33.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/docs/make.bat` & `vjer-33.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/pyproject.toml` & `vjer-33.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,22 @@
 dependencies = [
     "BatCave",
     "bumpver",
     "junitparser",
     "flake8",
     "flake8-annotations",
     "flake8-pyproject",
+    "flit",
     "mypy",
     "pylint",
     "unittest-xml-reporting",
 ]
 
 [project.optional-dependencies]
-dev = ["flit", "twine"]
+dev = ["twine"]
 test = ["types-PyYAML", "types-requests"]
 # doc = []
 
 [project.scripts]
 vjer = "vjer.vjer:main"
 
 [project.urls]
@@ -80,15 +81,15 @@
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = "xmlrunner.*"
 ignore_missing_imports = true
 
 [tool.bumpver]
-current_version = "v33.0.0"
+current_version = "v33.0.1"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version} [skip ci]"
 commit = true
 tag = false
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `vjer-33.0.0/vjer/build.py` & `vjer-33.0.1/vjer/build.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/deploy.py` & `vjer-33.0.1/vjer/deploy.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/freeze.py` & `vjer-33.0.1/vjer/freeze.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/pre_release.py` & `vjer-33.0.1/vjer/pre_release.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/release.py` & `vjer-33.0.1/vjer/release.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/rollback.py` & `vjer-33.0.1/vjer/rollback.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/test.py` & `vjer-33.0.1/vjer/test.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/tool_reporter.py` & `vjer-33.0.1/vjer/tool_reporter.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/utils.py` & `vjer-33.0.1/vjer/utils.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/vjer/vjer.py` & `vjer-33.0.1/vjer/vjer.py`

 * *Files identical despite different names*

### Comparing `vjer-33.0.0/setup.py` & `vjer-33.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 install_requires = \
 ['BatCave',
  'bumpver',
  'junitparser',
  'flake8',
  'flake8-annotations',
  'flake8-pyproject',
+ 'flit',
  'mypy',
  'pylint',
  'unittest-xml-reporting']
 
 extras_require = \
-{'dev': ['flit', 'twine'], 'test': ['types-PyYAML', 'types-requests']}
+{'dev': ['twine'], 'test': ['types-PyYAML', 'types-requests']}
 
 entry_points = \
 {'console_scripts': ['vjer = vjer.vjer:main']}
 
 setup(name='vjer',
-      version='33.0.0',
+      version='33.0.1',
       description='Vjer CI/CD module.',
       author=None,
       author_email='"Jeffery G. Smith" <web@pobox.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `vjer-33.0.0/PKG-INFO` & `vjer-33.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vjer
-Version: 33.0.0
+Version: 33.0.1
 Summary: Vjer CI/CD module.
 Keywords: python,programming,utilities
 Author-email: "Jeffery G. Smith" <web@pobox.com>
 Requires-Python: ~=3.11
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -15,18 +15,18 @@
 Classifier: Natural Language :: English
 Requires-Dist: BatCave
 Requires-Dist: bumpver
 Requires-Dist: junitparser
 Requires-Dist: flake8
 Requires-Dist: flake8-annotations
 Requires-Dist: flake8-pyproject
+Requires-Dist: flit
 Requires-Dist: mypy
 Requires-Dist: pylint
 Requires-Dist: unittest-xml-reporting
-Requires-Dist: flit ; extra == "dev"
 Requires-Dist: twine ; extra == "dev"
 Requires-Dist: types-PyYAML ; extra == "test"
 Requires-Dist: types-requests ; extra == "test"
 Project-URL: changelog, https://github.com/tardis4500/vjer/blob/main/CHANGELOG.md
 Project-URL: documentation, https://vjer.readthedocs.io
 Project-URL: homepage, https://github.com/tardis4500/vjer/
 Project-URL: repository, https://github.com/tardis4500/vjer/
```

