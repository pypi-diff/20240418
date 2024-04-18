# Comparing `tmp/edx-django-sites-extensions-4.0.2.tar.gz` & `tmp/edx-django-sites-extensions-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-sites-extensions-4.0.2.tar", last modified: Wed Oct 11 10:49:05 2023, max compression
+gzip compressed data, was "edx-django-sites-extensions-4.1.0.tar", last modified: Wed Apr 17 20:32:22 2024, max compression
```

## Comparing `edx-django-sites-extensions-4.0.2.tar` & `edx-django-sites-extensions-4.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 10:49:05.977272 edx-django-sites-extensions-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    35116 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-10-11 10:49:05.977272 edx-django-sites-extensions-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 10:49:05.977272 edx-django-sites-extensions-4.0.2/django_sites_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/django_sites_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/django_sites_extensions/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/django_sites_extensions/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/django_sites_extensions/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/django_sites_extensions/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 10:49:05.977272 edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-10-11 10:49:05.000000 edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-10-11 10:49:05.000000 edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-11 10:49:05.000000 edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-11 10:49:05.000000 edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-11 10:49:05.000000 edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-11 10:49:05.977272 edx-django-sites-extensions-4.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      584 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-11 10:49:05.977272 edx-django-sites-extensions-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2023-10-11 10:49:01.000000 edx-django-sites-extensions-4.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:32:22.025743 edx-django-sites-extensions-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    35116 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-17 20:32:22.025743 edx-django-sites-extensions-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:32:22.021743 edx-django-sites-extensions-4.1.0/django_sites_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/django_sites_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/django_sites_extensions/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/django_sites_extensions/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/django_sites_extensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/django_sites_extensions/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:32:22.021743 edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-17 20:32:22.000000 edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-17 20:32:22.000000 edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:32:22.000000 edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 20:32:22.000000 edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-17 20:32:22.000000 edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:32:22.021743 edx-django-sites-extensions-4.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 20:32:22.025743 edx-django-sites-extensions-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-17 20:32:15.000000 edx-django-sites-extensions-4.1.0/setup.py
```

### Comparing `edx-django-sites-extensions-4.0.2/LICENSE.txt` & `edx-django-sites-extensions-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-django-sites-extensions-4.0.2/PKG-INFO` & `edx-django-sites-extensions-4.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: edx-django-sites-extensions
-Version: 4.0.2
+Version: 4.1.0
 Summary: Custom extensions for the Django sites framework
 Home-page: https://github.com/openedx/edx-django-sites-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Keywords: Django sites edx
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django
+Requires-Dist: setuptools
+Requires-Dist: wheel
 
 Part of `edX code <http://code.edx.org/>`_.
 
 edx-django-sites-extensions  |CI|_ |Codecov|_
 =================================================
 .. |CI| image:: https://github.com/openedx/edx-django-sites-extensions/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/edx-django-sites-extensions/actions?query=workflow%3A%22Python+CI%22
@@ -112,15 +115,13 @@
 
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code in the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_.
-
-
```

### Comparing `edx-django-sites-extensions-4.0.2/README.rst` & `edx-django-sites-extensions-4.1.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -89,13 +89,13 @@
 
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code in the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_.
```

### Comparing `edx-django-sites-extensions-4.0.2/django_sites_extensions/apps.py` & `edx-django-sites-extensions-4.1.0/django_sites_extensions/apps.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,12 +7,11 @@
     """ django_sites_extensions application configuration """
     name = 'django_sites_extensions'
     verbose_name = 'Django Sites Extensions'
 
     # noinspection PyUnresolvedReferences
     def ready(self):
         """ Set up for django_sites_extensions app """
-        # pylint: disable=unused-variable
         # pylint: disable=unused-import
         # pylint: disable=import-outside-toplevel
         from django_sites_extensions import models
         from django_sites_extensions import signals
```

### Comparing `edx-django-sites-extensions-4.0.2/django_sites_extensions/middleware.py` & `edx-django-sites-extensions-4.1.0/django_sites_extensions/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-sites-extensions-4.0.2/django_sites_extensions/models.py` & `edx-django-sites-extensions-4.1.0/django_sites_extensions/models.py`

 * *Files identical despite different names*

### Comparing `edx-django-sites-extensions-4.0.2/django_sites_extensions/signals.py` & `edx-django-sites-extensions-4.1.0/django_sites_extensions/signals.py`

 * *Files identical despite different names*

### Comparing `edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/PKG-INFO` & `edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: edx-django-sites-extensions
-Version: 4.0.2
+Version: 4.1.0
 Summary: Custom extensions for the Django sites framework
 Home-page: https://github.com/openedx/edx-django-sites-extensions
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Keywords: Django sites edx
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.2
 License-File: LICENSE.txt
 License-File: AUTHORS
+Requires-Dist: Django
+Requires-Dist: setuptools
+Requires-Dist: wheel
 
 Part of `edX code <http://code.edx.org/>`_.
 
 edx-django-sites-extensions  |CI|_ |Codecov|_
 =================================================
 .. |CI| image:: https://github.com/openedx/edx-django-sites-extensions/workflows/Python%20CI/badge.svg?branch=master
 .. _CI: https://github.com/openedx/edx-django-sites-extensions/actions?query=workflow%3A%22Python+CI%22
@@ -112,15 +115,13 @@
 
 Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 
 Reporting Security Issues
 -------------------------
 
-Please do not report security issues in public. Please email security@edx.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 Mailing List and IRC Channel
 ----------------------------
 
 You can discuss this code in the `edx-code Google Group <https://groups.google.com/forum/#!forum/edx-code>`_.
-
-
```

### Comparing `edx-django-sites-extensions-4.0.2/edx_django_sites_extensions.egg-info/SOURCES.txt` & `edx-django-sites-extensions-4.1.0/edx_django_sites_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-django-sites-extensions-4.0.2/requirements/constraints.txt` & `edx-django-sites-extensions-4.1.0/requirements/constraints.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,7 +6,11 @@
 # When pinning something here, please provide an explanation of why.  Ideally,
 # link to other information that will help people in the future to remove the
 # pin when possible.  Writing an issue against the offending project and
 # linking to it here is good.
 
 # This file contains all common constraints for edx-repos
 -c https://raw.githubusercontent.com/edx/edx-lint/master/edx_lint/files/common_constraints.txt
+
+
+# Temporary to Support the python 3.11 Upgrade
+backports.zoneinfo;python_version<"3.9"  # Newer versions have zoneinfo available in the standard library
```

### Comparing `edx-django-sites-extensions-4.0.2/setup.py` & `edx-django-sites-extensions-4.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,19 +129,20 @@
     description='Custom extensions for the Django sites framework',
     long_description=long_description,
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU Affero General Public License v3',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet',
         'Intended Audience :: Developers',
         'Environment :: Web Environment',
         'Framework :: Django',
-        'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.2',
     ],
     keywords='Django sites edx',
     url='https://github.com/openedx/edx-django-sites-extensions',
     author='edX',
     author_email='oscm@edx.org',
     license='AGPL',
```

