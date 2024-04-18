# Comparing `tmp/edc-prn-0.3.8.tar.gz` & `tmp/edc-prn-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-prn-0.3.8.tar", last modified: Thu Sep  8 11:35:16 2022, max compression
+gzip compressed data, was "edc-prn-0.3.9.tar", last modified: Sun Sep 25 22:12:16 2022, max compression
```

## Comparing `edc-prn-0.3.8.tar` & `edc-prn-0.3.9.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.204839 edc-prn-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       81 2021-09-12 16:35:32.000000 edc-prn-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 01:24:59.000000 edc-prn-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.198346 edc-prn-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.201310 edc-prn-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 01:13:38.000000 edc-prn-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-05-25 15:10:19.000000 edc-prn-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-10 01:13:38.000000 edc-prn-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 01:13:38.000000 edc-prn-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:10:19.000000 edc-prn-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:10:19.000000 edc-prn-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:29:32.000000 edc-prn-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-05-25 15:10:19.000000 edc-prn-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-08 11:35:16.204936 edc-prn-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      632 2021-02-08 01:24:59.000000 edc-prn-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-08 11:35:08.000000 edc-prn-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 01:13:38.000000 edc-prn-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.202072 edc-prn-0.3.8/edc_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)       83 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      384 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)       16 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2973 2022-09-08 11:35:08.000000 edc-prn-0.3.8/edc_prn/prn.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2518 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/site_prn_forms.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.198568 edc-prn-0.3.8/edc_prn/templates/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.202796 edc-prn-0.3.8/edc_prn/templates/edc_prn/
--rw-r--r--   0 erikvw     (501) staff       (20)     1300 2022-09-08 11:35:08.000000 edc-prn-0.3.8/edc_prn/templates/edc_prn/add_prn_popover.html
--rw-r--r--   0 erikvw     (501) staff       (20)     1074 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/templates/edc_prn/list_prns.html
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.202997 edc-prn-0.3.8/edc_prn/templatetags/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/templatetags/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     3759 2022-09-08 11:35:08.000000 edc-prn-0.3.8/edc_prn/templatetags/edc_prn_extras.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.203540 edc-prn-0.3.8/edc_prn/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.204525 edc-prn-0.3.8/edc_prn/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1895 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)      234 2021-09-11 14:24:28.000000 edc-prn-0.3.8/edc_prn/tests/models.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.204732 edc-prn-0.3.8/edc_prn/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1796 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/tests/tests/test_prn.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-09-12 16:35:32.000000 edc-prn-0.3.8/edc_prn/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-08 11:35:16.202605 edc-prn-0.3.8/edc_prn.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-08 11:35:16.000000 edc-prn-0.3.8/edc_prn.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1122 2022-09-08 11:35:16.000000 edc-prn-0.3.8/edc_prn.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-08 11:35:16.000000 edc-prn-0.3.8/edc_prn.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:29:52.000000 edc-prn-0.3.8/edc_prn.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        8 2022-09-08 11:35:16.000000 edc-prn-0.3.8/edc_prn.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1716 2022-08-10 01:13:38.000000 edc-prn-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1919 2021-09-12 16:35:32.000000 edc-prn-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-09-08 11:35:16.205222 edc-prn-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.865226 edc-prn-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       81 2021-09-12 16:35:32.000000 edc-prn-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-08 01:24:59.000000 edc-prn-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.857805 edc-prn-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.861158 edc-prn-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-10 01:13:38.000000 edc-prn-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)      968 2022-05-25 15:10:19.000000 edc-prn-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:12:09.000000 edc-prn-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-10 01:13:38.000000 edc-prn-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:10:19.000000 edc-prn-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 15:10:19.000000 edc-prn-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-04 23:29:32.000000 edc-prn-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      112 2022-05-25 15:10:19.000000 edc-prn-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-25 22:12:16.865323 edc-prn-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      632 2021-02-08 01:24:59.000000 edc-prn-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:12:09.000000 edc-prn-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      166 2022-08-10 01:13:38.000000 edc-prn-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.862286 edc-prn-0.3.9/edc_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)       83 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      384 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1135 2022-09-25 22:12:09.000000 edc-prn-0.3.9/edc_prn/modelform_mixins.py
+-rw-r--r--   0 erikvw     (501) staff       (20)       16 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2973 2022-09-08 11:35:08.000000 edc-prn-0.3.9/edc_prn/prn.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2518 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/site_prn_forms.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.858020 edc-prn-0.3.9/edc_prn/templates/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.863081 edc-prn-0.3.9/edc_prn/templates/edc_prn/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1300 2022-09-25 22:12:09.000000 edc-prn-0.3.9/edc_prn/templates/edc_prn/add_prn_popover.html
+-rw-r--r--   0 erikvw     (501) staff       (20)     1074 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/templates/edc_prn/list_prns.html
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.863307 edc-prn-0.3.9/edc_prn/templatetags/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/templatetags/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     3911 2022-09-25 22:12:09.000000 edc-prn-0.3.9/edc_prn/templatetags/edc_prn_extras.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.863898 edc-prn-0.3.9/edc_prn/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.864913 edc-prn-0.3.9/edc_prn/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1895 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)      234 2021-09-11 14:24:28.000000 edc-prn-0.3.9/edc_prn/tests/models.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.865114 edc-prn-0.3.9/edc_prn/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1796 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/tests/tests/test_prn.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2021-09-12 16:35:32.000000 edc-prn-0.3.9/edc_prn/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:12:16.862855 edc-prn-0.3.9/edc_prn.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1617 2022-09-25 22:12:16.000000 edc-prn-0.3.9/edc_prn.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1150 2022-09-25 22:12:16.000000 edc-prn-0.3.9/edc_prn.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:12:16.000000 edc-prn-0.3.9/edc_prn.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-04 23:29:52.000000 edc-prn-0.3.9/edc_prn.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        8 2022-09-25 22:12:16.000000 edc-prn-0.3.9/edc_prn.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1716 2022-08-10 01:13:38.000000 edc-prn-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1919 2021-09-12 16:35:32.000000 edc-prn-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1244 2022-09-25 22:12:16.865629 edc-prn-0.3.9/setup.cfg
```

### Comparing `edc-prn-0.3.8/.github/workflows/build.yml` & `edc-prn-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/.gitignore` & `edc-prn-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/.pre-commit-config.yaml` & `edc-prn-0.3.9/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
-        language_version: python3.8
+        language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
```

### Comparing `edc-prn-0.3.8/LICENSE` & `edc-prn-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/PKG-INFO` & `edc-prn-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-prn
-Version: 0.3.8
+Version: 0.3.9
 Summary: classes and utils for PRN forms in the clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-prn
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc PRN forms,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-prn-0.3.8/README.rst` & `edc-prn-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/prn.py` & `edc-prn-0.3.9/edc_prn/prn.py`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/site_prn_forms.py` & `edc-prn-0.3.9/edc_prn/site_prn_forms.py`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/templates/edc_prn/add_prn_popover.html` & `edc-prn-0.3.9/edc_prn/templates/edc_prn/add_prn_popover.html`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 href="javascript://" data-toggle="popover" data-placement="auto" data-html="true" title="Add PRN {{ label|title }}" role="button"
 data-content="
 <div class='list-group'>
 	{% if not prn_forms%}<small>There are no PRN {{ label }}s to add.</small>{% endif %}
 {% for prn_form in prn_forms %}
 <a id='show-link-to-add-{{ prn_form.model }}' class='list-group-item list-group-item-success'
 title='click to add'
-href='{{ prn_form.add_url }}?next={{ subject_dashboard_url }},appointment,subject_identifier&subject_identifier={{ subject_identifier }}&appointment={{ appointment_pk }}&{{ prn_form.related_visit_model_attr }}={{ prn_form.subject_visit }}&panel={{ prn_form.panel.pk }}'>
+href='{{ prn_form.add_url }}?next={{ subject_dashboard_url }},appointment,subject_identifier&subject_identifier={{ subject_identifier }}&appointment={{ appointment_pk }}&{{ prn_form.related_visit_model_attr }}={{ prn_form.related_visit }}&panel={{ prn_form.panel.pk }}'>
 <span class='text text-default text-nowrap small'><i class='fas fa-plus fa-1x fa-fw' aria-hidden='true'></i> {{ prn_form.verbose_name }} {% if label == REQUISITION and not prn_form.panel.pk %}Invalid Panel!{% endif %}</span>
 </a>
 {% endfor %}
 </div>
 <p><a title='close' class='btn btn-sm btn-primary pull-right'><i class='fas fa-times fa-fw' aria-hidden='true'></i></a><br></p>">
 <span class="text text-default" title="Click to see more ..."><i class="fas fa-caret-left" aria-hidden="true"></i> <small>Add PRN {{ label }}s</small></span>
 </a>
```

### Comparing `edc-prn-0.3.8/edc_prn/templates/edc_prn/list_prns.html` & `edc-prn-0.3.9/edc_prn/templates/edc_prn/list_prns.html`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/templatetags/edc_prn_extras.py` & `edc-prn-0.3.9/edc_prn/templatetags/edc_prn_extras.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 from django import template
 from django.core.exceptions import ObjectDoesNotExist
 from edc_metadata.constants import KEYED, REQUIRED
 from edc_metadata.models import CrfMetadata, RequisitionMetadata
 
 from ..site_prn_forms import site_prn_forms
 
+if TYPE_CHECKING:
+    from edc_appointment.models import Appointment
 register = template.Library()
 
 CRF = "CRF"
 REQUISITION = "Requisition"
 
 
 @register.inclusion_tag("edc_prn/list_prns.html")
@@ -32,29 +38,29 @@
             visit_code_sequence=appointment.visit_code_sequence,
             model=crf.model,
             entry_status__in=[REQUIRED, KEYED],
         ).exists():
             subject_visit_id = getattr(appointment.related_visit, "pk", None)
             crf.add_url = crf.model_cls().get_absolute_url()
             crf.related_visit_model_attr = crf.model_cls.related_visit_model_attr()
-            crf.subject_visit = str(subject_visit_id) if subject_visit_id else None
+            crf.related_visit = str(subject_visit_id) if subject_visit_id else None
             prn_forms.append(crf)
     return dict(
         label=CRF,
         CRF=CRF,
         REQUISITION=REQUISITION,
         prn_forms=prn_forms,
         appointment_pk=str(appointment.pk),
         subject_identifier=appointment.subject_identifier,
         subject_dashboard_url=subject_dashboard_url,
     )
 
 
 @register.inclusion_tag("edc_prn/add_prn_popover.html")
-def add_prn_requisition_popover(appointment, subject_dashboard_url):
+def add_prn_requisition_popover(appointment: Appointment, subject_dashboard_url):
     prn_forms = []
     for requisition in appointment.visits.get(appointment.visit_code).requisitions_prn:
         try:
             RequisitionMetadata.objects.get(
                 subject_identifier=appointment.subject_identifier,
                 visit_schedule_name=appointment.visit_schedule_name,
                 schedule_name=appointment.schedule_name,
@@ -65,15 +71,15 @@
                 entry_status__in=[REQUIRED, KEYED],
             )
         except ObjectDoesNotExist:
             requisition.add_url = requisition.model_cls().get_absolute_url()
             requisition.related_visit_model_attr = (
                 requisition.model_cls.related_visit_model_attr()
             )
-            requisition.subject_visit = str(getattr(appointment.related_visit, "id", ""))
+            requisition.related_visit = str(getattr(appointment.related_visit, "id", ""))
             try:
                 panel_id = requisition.model_cls.panel.field.remote_field.model.objects.get(
                     name=requisition.panel.name
                 ).id
             except ObjectDoesNotExist:
                 requisition.panel.id = None
                 requisition.panel.pk = None
```

### Comparing `edc-prn-0.3.8/edc_prn/tests/etc/user-rsa-local-private.pem` & `edc-prn-0.3.9/edc_prn/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/tests/etc/user-rsa-restricted-private.pem` & `edc-prn-0.3.9/edc_prn/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/tests/holidays.csv` & `edc-prn-0.3.9/edc_prn/tests/holidays.csv`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn/tests/tests/test_prn.py` & `edc-prn-0.3.9/edc_prn/tests/tests/test_prn.py`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/edc_prn.egg-info/PKG-INFO` & `edc-prn-0.3.9/edc_prn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-prn
-Version: 0.3.8
+Version: 0.3.9
 Summary: classes and utils for PRN forms in the clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-prn
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc PRN forms,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-prn-0.3.8/edc_prn.egg-info/SOURCES.txt` & `edc-prn-0.3.9/edc_prn.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 codecov.yml
 pyproject.toml
 runtests.py
 setup.cfg
 .github/workflows/build.yml
 edc_prn/__init__.py
 edc_prn/apps.py
+edc_prn/modelform_mixins.py
 edc_prn/models.py
 edc_prn/prn.py
 edc_prn/site_prn_forms.py
 edc_prn.egg-info/PKG-INFO
 edc_prn.egg-info/SOURCES.txt
 edc_prn.egg-info/dependency_links.txt
 edc_prn.egg-info/not-zip-safe
```

### Comparing `edc-prn-0.3.8/pyproject.toml` & `edc-prn-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/runtests.py` & `edc-prn-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-prn-0.3.8/setup.cfg` & `edc-prn-0.3.9/setup.cfg`

 * *Files identical despite different names*

