# Comparing `tmp/songbirdcore-0.0.7.tar.gz` & `tmp/songbirdcore-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songbirdcore-0.0.7.tar", last modified: Wed Apr 17 19:35:17 2024, max compression
+gzip compressed data, was "songbirdcore-0.0.8.tar", last modified: Thu Apr 18 17:28:27 2024, max compression
```

## Comparing `songbirdcore-0.0.7.tar` & `songbirdcore-0.0.8.tar`

### file list

```diff
@@ -1,52 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.527976 songbirdcore-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/pages.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/style.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/docs/songbirdcore/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/common.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/gdrive.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/itunes.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/docs/songbirdcore/models/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/models/itunes_api.md
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/models/modes.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/web.md
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/docs/songbirdcore/youtube.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.531976 songbirdcore-0.0.7/songbirdcore/
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10587 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/itunes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/songbirdcore/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/models/itunes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/models/modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/requirements.txt.blank
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/web.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/songbirdcore/youtube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/songbirdcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 19:35:17.000000 songbirdcore-0.0.7/songbirdcore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.527976 songbirdcore-0.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:17.535976 songbirdcore-0.0.7/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_gdrive.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_itunes.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_web.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-17 19:35:10.000000 songbirdcore-0.0.7/tests/unit/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.002456 songbirdcore-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.006456 songbirdcore-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/.github/workflows/pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/.github/workflows/style.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.006456 songbirdcore-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.006456 songbirdcore-0.0.8/docs/songbirdcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/gdrive.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/itunes.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.006456 songbirdcore-0.0.8/docs/songbirdcore/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/models/itunes_api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/models/modes.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/web.md
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/docs/songbirdcore/youtube.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.010456 songbirdcore-0.0.8/songbirdcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10056 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/itunes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.010456 songbirdcore-0.0.8/songbirdcore/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/models/itunes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/models/modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/requirements.txt.blank
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/songbirdcore/youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/songbirdcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-18 17:28:26.000000 songbirdcore-0.0.8/songbirdcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-18 17:28:26.000000 songbirdcore-0.0.8/songbirdcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:28:26.000000 songbirdcore-0.0.8/songbirdcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-18 17:28:26.000000 songbirdcore-0.0.8/songbirdcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-18 17:28:26.000000 songbirdcore-0.0.8/songbirdcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.002456 songbirdcore-0.0.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.010456 songbirdcore-0.0.8/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.010456 songbirdcore-0.0.8/tests/unit/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    81031 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/resources/empty.m4a
+-rw-r--r--   0 runner    (1001) docker     (127)    52059 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/resources/empty.mp3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.002456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.002456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/artist0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/artist0/album/
+-rw-r--r--   0 runner    (1001) docker     (127)    81031 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/artist0/album/empty.m4a
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.002456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/artist1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/artist1/album/
+-rw-r--r--   0 runner    (1001) docker     (127)    52059 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/artist1/album/empty.mp3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.006456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/dolly parton/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:27.014456 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/dolly parton/album/
+-rw-r--r--   0 runner    (1001) docker     (127)    52059 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/resources/mock-itunes-lib/dolly parton/album/jolene.mp3
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/test_gdrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/test_itunes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-18 17:28:22.000000 songbirdcore-0.0.8/tests/unit/test_youtube.py
```

### Comparing `songbirdcore-0.0.7/.github/workflows/pages.yaml` & `songbirdcore-0.0.8/.github/workflows/pages.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -39,15 +39,14 @@
           pip install -e .[dev]
       - name: test the site builds
         run: make docs-build
 
   deploy:
     runs-on: ubuntu-latest
     if: startsWith(github.ref, 'refs/tags/')
-    needs: [lint, test]
     steps:
       - uses: actions/checkout@v4
       - name: set up Python 3.11
         uses: actions/setup-python@v5
         with:
           python-version: 3.11
       - name: install dependencies
@@ -64,8 +63,8 @@
       # the below steps are referenced from
       # https://github.com/jimporter/mike#deploying-via-ci
         run: |
           git fetch origin gh-pages --depth=1
           git config user.name github-actions
           git config user.email github-actions@github.com
           mike deploy --push --update-aliases ${{ steps.tag.outputs.tag }} latest
-          mike set-default --push latest
+          mike set-default --push latest
```

### Comparing `songbirdcore-0.0.7/.github/workflows/pypi-publish.yaml` & `songbirdcore-0.0.8/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/.github/workflows/tests.yaml` & `songbirdcore-0.0.8/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/LICENSE` & `songbirdcore-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/Makefile` & `songbirdcore-0.0.8/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -64,8 +64,11 @@
 	mkdocs build --strict --verbose --site-dir public
 
 lint:
 	black $(APP_NAME)/.
 	black tests
 
 test:
-	python -m pytest --doctest-modules --junitxml=junit/test-results.xml --cov=songbirdcore --cov-report=xml --cov-report=html tests/unit -v
+	python -m pytest --doctest-modules --junitxml=junit/test-results.xml --cov=songbirdcore --cov-report=xml --cov-report=html tests/unit -v
+
+test-stdout:
+	python -m pytest --cov=songbirdcore tests/unit -v
```

### Comparing `songbirdcore-0.0.7/PKG-INFO` & `songbirdcore-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcore
-Version: 0.0.7
+Version: 0.0.8
 Summary: core low level api for songbird
 Author: Christian Boin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `songbirdcore-0.0.7/README.md` & `songbirdcore-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/mkdocs.yml` & `songbirdcore-0.0.8/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -62,12 +62,12 @@
     handlers:
       python:
         options:
           show_root_heading: true
           show_root_full_path: true
           show_root_toc_entry: true
           docstring_section_style: list
-          show_source: false
+          show_source: true
           show_bases: true
           merge_init_into_class: true
           show_symbol_type_heading: true
           show_symbol_type_toc: true
```

### Comparing `songbirdcore-0.0.7/pyproject.toml` & `songbirdcore-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "songbirdcore"
 authors = [
     {name = "Christian Boin"},
 ]
-version = "0.0.7"
+version = "0.0.8"
 description = "core low level api for songbird"
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["songbirdcore/requirements.txt"]}
```

### Comparing `songbirdcore-0.0.7/songbirdcore/common.py` & `songbirdcore-0.0.8/songbirdcore/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from .models import itunes_api, modes
 from .version import version
 
 logger = logging.getLogger(__name__)
 
 
-def load_version(toml_path: str):
+def load_toml(toml_path: str):
     with open(toml_path, "rb") as f:
         data = tomllib.load(f)
     return data
 
 
 def set_logger_config_globally(log_level=logging.INFO) -> None:
     """Sets the python logging module settings for output
@@ -122,26 +122,26 @@
         List[str]: list of paths found that match
     """
     paths = glob.glob(os.path.join(path, filename))
     return paths
 
 
 def pretty_list_of_basemodel_printer(
-    list_of_dicts: List[BaseModel], ignore_keys: Optional[List[str]] = None
+    list_of_models: List[BaseModel], ignore_keys: Optional[List[str]] = None
 ):
     """
     renders a list to stdio given a list of pydantic BaseModel objects
 
     Args:
-        list_of_dicts (List[BaseModel]): list of dictionaries to print
+        list_of_models (List[BaseModel]): list of pydantic models to print
         ignore_keys (Optional[List[str]], optional): any keys/fields in BaseModel not to print
     """
-    i = len(list_of_dicts) - 1
+    i = len(list_of_models) - 1
     logger.info("------------------------")
-    for element in reversed(list_of_dicts):
+    for element in reversed(list_of_models):
         logger.info(i)
         for k, v in element.model_dump().items():
             if ignore_keys is not None:
                 if (
                     k not in ignore_keys
                 ):  # print the key and value if not in ignore_keys or special_dict
                     print("\t%s - %s" % (k, v))
```

### Comparing `songbirdcore-0.0.7/songbirdcore/gdrive.py` & `songbirdcore-0.0.8/songbirdcore/gdrive.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/songbirdcore/itunes.py` & `songbirdcore-0.0.8/songbirdcore/itunes.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 
         response = artwork_searcher(url=song_tag_data.artworkUrl100)
 
         # Set all the tags for the mp3, all without if statement were checked for existence.
         audiofile = eyed3.load(mp3_path)
         audiofile.tag.artist = song_tag_data.artistName
         audiofile.tag.album = song_tag_data.collectionName
-        audiofile.tag.title = song_tag_data.TRACK_NAME
+        audiofile.tag.title = song_tag_data.trackName
         audiofile.tag.genre = song_tag_data.primaryGenreName
         audiofile.tag.track_num = (song_tag_data.trackNumber, song_tag_data.trackCount)
         audiofile.tag.disc_num = (song_tag_data.discNumber, song_tag_data.discCount)
         audiofile.tag.recording_date = song_tag_data.releaseDate
 
         if (
             song_tag_data.collectionArtistName is not None
@@ -177,28 +177,14 @@
     except Exception as e:
         logger.exception(
             f"Unexpected error occured while trying to tag your mp3 file: {e}"
         )
         return False
 
 
-def convert_mp3_to_itunes_format(input_filename):
-    """Convert the mp3 file to itunes format, updating tags to the new itunes standard.
-    Args:
-        input_filename (str): the full path of the file
-    Returns:
-        str: the path to the modified file.
-    """
-    pydub.AudioSegment.ffmpeg = updates.get_path_to_ffmpeg()
-    song_file = pydub.AudioSegment.from_mp3(input_filename)
-    output_filename = input_filename.replace(".mp3", ".m4a")
-    song_file.export(output_filename, format="ipod")
-    return output_filename
-
-
 def query_api(
     search_variable: str, limit: int, mode: modes.Modes, lookup: bool = False
 ) -> List[Union[itunes_api.ItunesApiSongModel, itunes_api.ItunesApiAlbumKeys]]:
     """
     Args:
         search_variable (str): the term to search itunes api for
         limit  (int): limit of the search in the api
@@ -250,15 +236,15 @@
                 ]  # will grab the year from date formatted 2016-06-01
                 result.releaseDate = year
             elif mode == modes.Modes.ALBUM:
                 result = itunes_api.ItunesApiAlbumKeys.model_validate(search_result)
 
             parsed_results_list.append(result)
         except ValidationError as e:
-            logger.warn(
+            logger.warning(
                 f"Skipping the display of song at index [{index}] as it could not be loaded into expected format.\n{e}"
             )
 
     return parsed_results_list
 
 
 def artwork_searcher(url: str) -> Optional[Response]:
```

### Comparing `songbirdcore-0.0.7/songbirdcore/models/itunes_api.py` & `songbirdcore-0.0.8/songbirdcore/models/itunes_api.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/songbirdcore/requirements.txt` & `songbirdcore-0.0.8/songbirdcore/requirements.txt`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/songbirdcore/web.py` & `songbirdcore-0.0.8/songbirdcore/web.py`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/songbirdcore/youtube.py` & `songbirdcore-0.0.8/songbirdcore/youtube.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,25 +54,25 @@
             )
             tries += 1
             log_attempts = False
             continue
         # Get the list of hrefs to each video on the home page
         links = response.html.find("#video-title")
         if len(links) == 0:
-            logger.warn(f"{tries+1}:{retry_count}.")
+            logger.warning(f"{tries+1}:{retry_count}.")
             tries += 1
             log_attempts = False
         else:
             break
     session.close()
     if tries >= retry_count:
         logger.error(
             f"Failed to get links from {youtube_home_url} after {retry_count} tries."
         )
-        return None
+        return None, None
 
     link_list = []
     # create a user friendly list, containing videos with title and href refs.
     for idx, link in enumerate(links):
         if "title" in link.attrs and "href" in link.attrs:
             link_list.append(
                 f"{link.attrs['title']} - {youtube_home_url+link.attrs['href']}"
```

### Comparing `songbirdcore-0.0.7/songbirdcore.egg-info/PKG-INFO` & `songbirdcore-0.0.8/songbirdcore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: songbirdcore
-Version: 0.0.7
+Version: 0.0.8
 Summary: core low level api for songbird
 Author: Christian Boin
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: beautifulsoup4==4.12.3
```

### Comparing `songbirdcore-0.0.7/songbirdcore.egg-info/SOURCES.txt` & `songbirdcore-0.0.8/songbirdcore.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -32,8 +32,13 @@
 songbirdcore.egg-info/top_level.txt
 songbirdcore/models/itunes_api.py
 songbirdcore/models/modes.py
 tests/unit/test_common.py
 tests/unit/test_gdrive.py
 tests/unit/test_itunes.py
 tests/unit/test_web.py
-tests/unit/test_youtube.py
+tests/unit/test_youtube.py
+tests/unit/resources/empty.m4a
+tests/unit/resources/empty.mp3
+tests/unit/resources/mock-itunes-lib/artist0/album/empty.m4a
+tests/unit/resources/mock-itunes-lib/artist1/album/empty.mp3
+tests/unit/resources/mock-itunes-lib/dolly parton/album/jolene.mp3
```

### Comparing `songbirdcore-0.0.7/songbirdcore.egg-info/requires.txt` & `songbirdcore-0.0.8/songbirdcore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `songbirdcore-0.0.7/tests/unit/test_youtube.py` & `songbirdcore-0.0.8/tests/unit/test_youtube.py`

 * *Files identical despite different names*

