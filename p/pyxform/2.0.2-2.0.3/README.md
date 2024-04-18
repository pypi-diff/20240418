# Comparing `tmp/pyxform-2.0.2.tar.gz` & `tmp/pyxform-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxform-2.0.2.tar", last modified: Fri Jan 26 18:45:49 2024, max compression
+gzip compressed data, was "pyxform-2.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyxform-2.0.2.tar` & `pyxform-2.0.3.tar`

### file list

```diff
@@ -1,66 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.900980 pyxform-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-01-26 18:45:37.000000 pyxform-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-01-26 18:45:49.900980 pyxform-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-01-26 18:45:37.000000 pyxform-2.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.888980 pyxform-2.0.2/pyxform/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)    17495 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.888980 pyxform-2.0.2/pyxform/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/entities/entities_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/entities/entity_declaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/external_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/iana_subtags.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.888980 pyxform-2.0.2/pyxform/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/parsing/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/parsing/instance_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    13326 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/question.py
--rw-r--r--   0 runner    (1001) docker     (127)    13190 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/question_type_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/section.py
--rw-r--r--   0 runner    (1001) docker     (127)    51086 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/survey.py
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/survey_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.892980 pyxform-2.0.2/pyxform/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/util/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.892980 pyxform-2.0.2/pyxform/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.892980 pyxform-2.0.2/pyxform/validators/enketo_validate/
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/enketo_validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/error_cleaner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.892980 pyxform-2.0.2/pyxform/validators/odk_validate/
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/odk_validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.900980 pyxform-2.0.2/pyxform/validators/odk_validate/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)  5618270 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/odk_validate/bin/ODK_Validate.jar
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/odk_validate/bin/installed.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.900980 pyxform-2.0.2/pyxform/validators/pyxform/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/pyxform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/pyxform/android_package_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/pyxform/parameters_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/pyxform/select_from_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/pyxform/translations_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)    23748 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/validators/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    26804 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/xform2json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/xform_instance_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    71894 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/xls2json.py
--rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/xls2json_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     6142 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/xls2xform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-01-26 18:45:37.000000 pyxform-2.0.2/pyxform/xlsparseutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:45:49.888980 pyxform-2.0.2/pyxform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-01-26 18:45:49.000000 pyxform-2.0.2/pyxform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-26 18:45:49.000000 pyxform-2.0.2/pyxform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 18:45:49.000000 pyxform-2.0.2/pyxform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-26 18:45:49.000000 pyxform-2.0.2/pyxform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-26 18:45:49.000000 pyxform-2.0.2/pyxform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-26 18:45:49.000000 pyxform-2.0.2/pyxform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-26 18:45:49.900980 pyxform-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-01-26 18:45:37.000000 pyxform-2.0.2/setup.py
+-rw-r--r--   0        0        0    12314 2024-04-18 21:22:56.300911 pyxform-2.0.3/README.rst
+-rw-r--r--   0        0        0     3017 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0      703 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/__init__.py
+-rw-r--r--   0        0        0     6369 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/aliases.py
+-rw-r--r--   0        0        0    17270 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/builder.py
+-rw-r--r--   0        0        0     4912 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/constants.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/entities/__init__.py
+-rw-r--r--   0        0        0     5069 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/entities/entities_parsing.py
+-rw-r--r--   0        0        0     4524 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/entities/entity_declaration.py
+-rw-r--r--   0        0        0      239 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/errors.py
+-rw-r--r--   0        0        0      336 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/external_instance.py
+-rw-r--r--   0        0        0     1185 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/file_utils.py
+-rw-r--r--   0        0        0    32366 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/iana_subtags.txt
+-rw-r--r--   0        0        0     3167 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/instance.py
+-rw-r--r--   0        0        0     6936 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/json_form_schema.json
+-rw-r--r--   0        0        0        0 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/parsing/__init__.py
+-rw-r--r--   0        0        0      424 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/parsing/expression.py
+-rw-r--r--   0        0        0     5002 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/parsing/instance_expression.py
+-rw-r--r--   0        0        0    13305 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/question.py
+-rw-r--r--   0        0        0    13166 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/question_type_dictionary.py
+-rw-r--r--   0        0        0    37376 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/question_types/all.xls
+-rw-r--r--   0        0        0    22528 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/question_types/base.xls
+-rw-r--r--   0        0        0    15872 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/question_types/beorse.xls
+-rw-r--r--   0        0        0     8704 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/question_types/nigeria.xls
+-rw-r--r--   0        0        0     7477 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/section.py
+-rw-r--r--   0        0        0    51497 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/survey.py
+-rw-r--r--   0        0        0    18830 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/survey_element.py
+-rw-r--r--   0        0        0     2707 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/translator.py
+-rw-r--r--   0        0        0   222269 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/translators/nigeria.json
+-rw-r--r--   0        0        0        0 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/util/__init__.py
+-rw-r--r--   0        0        0     1266 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/util/enum.py
+-rw-r--r--   0        0        0    16215 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/utils.py
+-rw-r--r--   0        0        0        0 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/validators/__init__.py
+-rw-r--r--   0        0        0     2400 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/validators/enketo_validate/__init__.py
+-rw-r--r--   0        0        0     2960 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/validators/error_cleaner.py
+-rw-r--r--   0        0        0       20 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/validators/odk_validate/.last_check
+-rw-r--r--   0        0        0      362 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/validators/odk_validate/README.rst
+-rw-r--r--   0        0        0     3235 2024-04-18 21:22:56.304911 pyxform-2.0.3/pyxform/validators/odk_validate/__init__.py
+-rwxr-xr-x   0        0        0  5618270 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/odk_validate/bin/ODK_Validate.jar
+-rw-r--r--   0        0        0     3825 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/odk_validate/bin/installed.json
+-rw-r--r--   0        0        0        0 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/pyxform/__init__.py
+-rw-r--r--   0        0        0     1198 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/pyxform/android_package_name.py
+-rw-r--r--   0        0        0     1399 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/pyxform/parameters_generic.py
+-rw-r--r--   0        0        0     2358 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/pyxform/select_from_file.py
+-rw-r--r--   0        0        0     6110 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/pyxform/translations_checks.py
+-rw-r--r--   0        0        0    23639 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/updater.py
+-rw-r--r--   0        0        0     6899 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/util.py
+-rw-r--r--   0        0        0    47999 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/validators/xlsform_spec_test.xml
+-rw-r--r--   0        0        0    27572 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/xform2json.py
+-rw-r--r--   0        0        0     4877 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/xform_instance_parser.py
+-rw-r--r--   0        0        0    71179 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/xls2json.py
+-rw-r--r--   0        0        0    16476 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/xls2json_backends.py
+-rw-r--r--   0        0        0     6178 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/xls2xform.py
+-rw-r--r--   0        0        0     1437 2024-04-18 21:22:56.332911 pyxform-2.0.3/pyxform/xlsparseutils.py
+-rw-r--r--   0        0        0    12960 1970-01-01 00:00:00.000000 pyxform-2.0.3/PKG-INFO
```

### Comparing `pyxform-2.0.2/PKG-INFO` & `pyxform-2.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,235 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyxform
-Version: 2.0.2
+Version: 2.0.3
 Summary: A Python package to create XForms for ODK Collect.
-Home-page: http://pypi.python.org/pypi/pyxform/
-Author: github.com/xlsform
-Author-email: info@xlsform.org
-License: UNKNOWN
-Description: ========
-        pyxform
-        ========
-        
-        |pypi| |python| |black|
-        
-        .. |pypi| image:: https://badge.fury.io/py/pyxform.svg
-            :target: https://badge.fury.io/py/pyxform
-        
-        .. |python| image:: https://img.shields.io/badge/python-3.7,3.8,3.9-blue.svg
-            :target: https://www.python.org/downloads
-        
-        .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-            :target: https://github.com/python/black
-        
-        pyxform is a Python library that makes writing forms for ODK Collect and Enketo easy by converting XLSForms (Excel spreadsheets) into ODK XForms. The XLSForms format is used in a `number of tools <http://xlsform.org/en/#tools-that-support-xlsforms>`_.
-        
-        XLS(X) documents used as input must follow to the `XLSForm standard <http://xlsform.org/>`_ and the resulting output follows the `ODK XForms <https://github.com/opendatakit/xforms-spec>`_ standard.
-        
-        
-        pyxform is a major rewrite of `xls2xform <http://github.com/mvpdev/xls2xform/>`_.
-        
-        Running the latest release of pyxform
-        =====================================
-        For those who want to convert forms at the command line, the latest official release of pyxform can be installed using `pip <https://en.wikipedia.org/wiki/Pip_(package_manager)>`_::
-        
-            pip install pyxform
-        
-        The ``xls2xform`` command can then be used::
-        
-            xls2xform path_to_XLSForm [output_path]
-        
-        The currently supported Python versions for ``pyxform`` are 3.7, 3.8 and 3.9.
-        
-        Running pyxform from local source
-        =================================
-        
-        Note that you must uninstall any globally installed ``pyxform`` instance in order to use local modules. Please install java 8 or newer version.
-        
-        From the command line, complete the following. These steps use a `virtualenv <https://docs.python.org/3.8/tutorial/venv.html>`_ to make dependency management easier, and to keep the global site-packages directory clean::
-        
-            # Get a copy of the repository.
-            mkdir -P ~/repos/pyxform
-            cd ~/repos/pyxform
-            git clone https://github.com/XLSForm/pyxform.git repo
-        
-            # Create and activate a virtual environment for the install.
-            /usr/local/bin/python3.8 -m venv venv
-            . venv/bin/activate
-        
-            # Install the pyxform and it's production dependencies.
-            (venv)$ cd repo
-            (venv)$ pip install -e .
-            (venv)$ python pyxform/xls2xform.py --help
-            (venv)$ xls2xform --help           # same effect as previous line
-            (venv)$ which xls2xform            # ~/repos/pyxform/venv/bin/xls2xform
-        
-        To leave and return to the virtualenv::
-        
-            (venv)$ deactivate                 # leave the venv, scripts not on $PATH
-            $ xls2xform --help
-            # -bash: xls2xform: command not found
-            $ . ~/repos/pyxform/venv/bin/activate     # reactivate the venv
-            (venv)$ which xls2xform                   # scripts available on $PATH again
-            ~/repos/pyxform/venv/bin/xls2xform
-        
-        Installing pyxform from remote source
-        =====================================
-        ``pip`` can install from the GitHub repository. Only do this if you want to install from the master branch, which is likely to have pre-release code. To install the latest release, see above.::
-        
-            pip install git+https://github.com/XLSForm/pyxform.git@master#egg=pyxform
-        
-        You can then run xls2xform from the commandline::
-        
-            xls2xform path_to_XLSForm [output_path]
-        
-        Development
-        ===========
-        To set up for development / contributing, first complete the above steps for "Running pyxform from local source", then complete the below.::
-        
-            pip install -r dev_requirements.pip
-        
-        You can run tests with::
-        
-            nosetests
-        
-        On Windows, use::
-        
-            nosetests -v -v --traverse-namespace ./tests
-        
-        Before committing, make sure to format the code using ``black``::
-        
-            black pyxform tests
-        
-        If you are using a copy of black outside your virtualenv, make sure it is the same version as listed in requirements_dev.pip.
-        
-        In case the pre-commit.sh hooks don't run, also run the code through ``isort`` (sorts imports) and ``flake8`` (misc code quality suggestions). The syntax is the same as above for ``black``.
-        
-        Writing tests
-        -------------
-        Make sure to include tests for the changes you're working on. When writing new tests you should add them in ``tests`` folder. Add to an existing test module, or create a new test module. Test modules are named after the corresponding source file, or if the tests concern many files then module name is the topic or feature under test.
-        
-        When creating new test cases, where possible use ``PyxformTestCase`` as a base class instead of ``unittest.TestCase``. The ``PyxformTestCase`` is a toolkit for writing XLSForms as MarkDown tables, compiling example XLSForms, and making assertions on the resulting XForm. This makes code review much easier by putting the XLSForm content inline with the test, instead of in a separate file. A ``unittest.TestCase`` may be used if the new tests do not involve compiling an XLSForm (but most will). Do not add new tests using the old style ``XFormTestCase``.
-        
-        When writing new ``PyxformTestCase`` tests that make content assertions, it is strongly recommended that the ``xml__xpath*`` matchers are used, in particular ``xml__xpath_match``. Most older tests use matchers like ``xml__contains`` and ``xml__excludes``, which are simple string matches of XML snippets against the result XForm. The ``xml__xpath_match`` kwarg accepts an XPath expression and expects 1 match. The main benefits of using XPath are 1) it allows specifying a document location, and 2) it does not require a particular document order for elements or attributes or whitespace output. To take full advantage of 1), the XPath expressions should specify the full document path (e.g. ``/h:html/h:head/x:model``) rather than a search (e.g. ``.//x:model``). To take full advantage of 2), the expression should include element predicates that specify the expected attribute values, e.g. ``/h:html/h:body/x:input[@ref='/trigger-column/a']``. To specify the absence of an element, an expression like the following may be used with ``xml__xpath_match``: ``/h:html[not(descendant::x:input)]``, or alternatively ``xml__xpath_count``: ``.//x:input`` with an expected count of 0 (zero).
-        
-        Documentation
-        =============
-        To check out the documentation for pyxform do the following::
-        
-            pip install Sphinx==1.0.7
-            cd your-virtual-env-dir/src/pyxform/docs
-            make html
-        
-        Change Log
-        ==========
-        `Changelog <CHANGES.txt>`_
-        
-        Releasing pyxform
-        =================
-        
-        1. Make sure the version of ODK Validate in the repo is up-to-date::
-        
-            pyxform_validator_update odk update ODK-Validate-vx.x.x.jar
-        
-        2. Run all tests through Validate by setting the default for ``run_odk_validate`` to ``kwargs.get("run_odk_validate", True)`` in ``tests/pyxform_test_case.py``.
-        3. Draft a new GitHub release with the list of merged PRs. Follow the title and description pattern of the previous release.
-        4. Checkout a release branch from latest upstream master.
-        5. Update ``CHANGES.txt`` with the text of the draft release.
-        6. Update ``setup.py``, ``pyxform/__init__.py`` with the new release version number.
-        7. Commit, push the branch, and initiate a pull request. Wait for tests to pass, then merge the PR.
-        8. Tag the release and it will automatically be published
-        
-        Manually releasing
-        ===================
-        Releases are now automatic. These instructions are provided for forks or for a future change in process.
-        
-        1. In a clean new release only directory, check out master.
-        2. Create a new virtualenv in this directory to ensure a clean Python environment::
-        
-             /usr/local/bin/python3.8 -m venv pyxform-release
-             . pyxform-release/bin/activate
-        
-        3. Install the production and packaging requirements::
-        
-             pip install -e .
-             pip install wheel twine
-        
-        4. Clean up build and dist folders::
-        
-             rm -rf build dist pyxform.egg-info
-        
-        5. Prepare ``sdist`` and ``bdist_wheel`` distributions::
-        
-             python setup.py sdist bdist_wheel
-        
-        6. Publish release to PyPI with ``twine``::
-        
-             twine upload dist/pyxform-*-py3-none-any.whl dist/pyxform-*.tar.gz
-        
-        7. Tag the GitHub release and publish it.
-        
-Platform: UNKNOWN
+Author-email: "github.com/xlsform" <support@getodk.org>
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Requires-Dist: xlrd==2.0.1
+Requires-Dist: openpyxl==3.1.2
+Requires-Dist: defusedxml==0.7.1
+Requires-Dist: formencode==2.1.0 ; extra == "dev"
+Requires-Dist: lxml==5.1.0 ; extra == "dev"
+Requires-Dist: psutil==5.9.8 ; extra == "dev"
+Requires-Dist: ruff==0.2.1 ; extra == "dev"
+Project-URL: Homepage, https://pypi.python.org/pypi/pyxform/
+Project-URL: Repository, https://github.com/XLSForm/pyxform/
+Provides-Extra: dev
+
+========
+pyxform
+========
+
+|pypi| |python| |black|
+
+.. |pypi| image:: https://badge.fury.io/py/pyxform.svg
+    :target: https://badge.fury.io/py/pyxform
+
+.. |python| image:: https://img.shields.io/badge/python-3.7,3.8,3.9-blue.svg
+    :target: https://www.python.org/downloads
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/python/black
+
+``pyxform`` is a Python library that simplifies writing forms for ODK Collect and Enketo by converting spreadsheets that follow the `XLSForm standard <http://xlsform.org/>`_ into `ODK XForms <https://github.com/opendatakit/xforms-spec>`_. The XLSForms format is used in a `number of tools <http://xlsform.org/en/#tools-that-support-xlsforms>`_.
+
+Project status
+===============
+``pyxform`` is actively maintained by `ODK <https://getodk.org/about/team.html>`_.
+
+Current goals for the project include:
+
+* Enable more complex workflows through sophisticated XPath expressions and `entities <https://getodk.github.io/xforms-spec/entities>`_
+* Improve error messages and make troubleshooting easier
+* Improve experience, particularly for multi-language forms
+
+``pyxform`` was started at the `Sustainable Engineering Lab at Columbia University <https://qsel.columbia.edu/>`_, and until 2018 was maintained primarily by `Ona <https://ona.io/>`_.
+
+Using ``pyxform``
+==================
+For user support, please start by posting to `the ODK forum <https://forum.getodk.org/c/support/6>`__ where your question will get the most visibility.
+
+There are 3 main ways that ``pyxform`` is used:
+
+* Through a form server, such as the `pyxform-http service wrapper <https://github.com/getodk/pyxform-http>`_, or `ODK Central <https://docs.getodk.org/getting-started/>`_.
+* The command line utility ``xls2xform``, which can be helpful for troubleshooting or as part of a broader form creation pipeline.
+* As a library, meaning that another python project imports functionality from ``pyxform``.
+
+Running the latest release of pyxform
+-------------------------------------
+To convert forms at the command line, the latest official release of pyxform can be installed using `pip <https://en.wikipedia.org/wiki/Pip_(package_manager)>`_::
+
+    pip install pyxform
+
+The ``xls2xform`` command can then be used::
+
+    xls2xform path_to_XLSForm [output_path]
+
+The currently supported Python versions for ``pyxform`` are 3.7, 3.8 and 3.9.
+
+Running pyxform from local source
+---------------------------------
+
+Note that you must uninstall any globally installed ``pyxform`` instance in order to use local modules. Please install java 8 or newer version.
+
+From the command line, complete the following. These steps use a `virtualenv <https://docs.python.org/3.8/tutorial/venv.html>`_ to make dependency management easier, and to keep the global site-packages directory clean::
+
+    # Get a copy of the repository.
+    mkdir -P ~/repos/pyxform
+    cd ~/repos/pyxform
+    git clone https://github.com/XLSForm/pyxform.git repo
+
+    # Create and activate a virtual environment for the install.
+    /usr/local/bin/python3.8 -m venv venv
+    . venv/bin/activate
+
+    # Install the pyxform and it's production dependencies.
+    (venv)$ cd repo
+    # If this doesn't work, upgrade pip ``pip install --upgrade pip`` and retry.
+    (venv)$ pip install -e .
+    (venv)$ python pyxform/xls2xform.py --help
+    (venv)$ xls2xform --help           # same effect as previous line
+    (venv)$ which xls2xform            # ~/repos/pyxform/venv/bin/xls2xform
+
+To leave and return to the virtualenv::
+
+    (venv)$ deactivate                 # leave the venv, scripts not on $PATH
+    $ xls2xform --help
+    # -bash: xls2xform: command not found
+    $ . ~/repos/pyxform/venv/bin/activate     # reactivate the venv
+    (venv)$ which xls2xform                   # scripts available on $PATH again
+    ~/repos/pyxform/venv/bin/xls2xform
+
+Installing pyxform from remote source
+-------------------------------------
+``pip`` can install from the GitHub repository. Only do this if you want to install from the master branch, which is likely to have pre-release code. To install the latest release, see above.::
+
+    pip install git+https://github.com/XLSForm/pyxform.git@master#egg=pyxform
+
+You can then run xls2xform from the commandline::
+
+    xls2xform path_to_XLSForm [output_path]
+
+Development
+===========
+To set up for development / contributing, first complete the above steps for "Running pyxform from local source". Then repeat the command used to install pyxform, but with ``[dev]`` appended to the end, e.g.::
+
+    pip install -e .[dev]
+
+You can run tests with::
+
+    python -m unittest
+
+Before committing, make sure to format and lint the code using ``ruff``::
+
+    ruff format pyxform tests
+    ruff check pyxform tests
+
+If you are using a copy of ``ruff`` outside your virtualenv, make sure it is the same version as listed in ``pyproject.toml``. Use the project configuration for ``ruff`` in ``pyproject.toml``, which occurs automatically if ``ruff`` is run from the project root (where ``pyproject.toml`` is).
+
+Contributions
+-------------
+We welcome contributions that have a clearly-stated goal and are tightly focused. In general, successful contributions will first be discussed on `the ODK forum <https://forum.getodk.org/>`__ or in an issue. We prefer discussion threads on the ODK forum because ``pyxform`` issues generally involve considerations for other tools and specifications in ODK and its broader ecosystem. Opening up an issue or a pull request directly may be appropriate if there is a clear bug or an issue that only affects ``pyxform`` developers.
+
+Writing tests
+-------------
+Make sure to include tests for the changes you're working on. When writing new tests you should add them in ``tests`` folder. Add to an existing test module, or create a new test module. Test modules are named after the corresponding source file, or if the tests concern many files then module name is the topic or feature under test.
+
+When creating new test cases, where possible use ``PyxformTestCase`` as a base class instead of ``unittest.TestCase``. The ``PyxformTestCase`` is a toolkit for writing XLSForms as MarkDown tables, compiling example XLSForms, and making assertions on the resulting XForm. This makes code review much easier by putting the XLSForm content inline with the test, instead of in a separate file. A ``unittest.TestCase`` may be used if the new tests do not involve compiling an XLSForm (but most will). Do not add new tests using the old style ``XFormTestCase``.
+
+When writing new ``PyxformTestCase`` tests that make content assertions, it is strongly recommended that the ``xml__xpath*`` matchers are used, in particular ``xml__xpath_match``. Most older tests use matchers like ``xml__contains`` and ``xml__excludes``, which are simple string matches of XML snippets against the result XForm. The ``xml__xpath_match`` kwarg accepts an XPath expression and expects 1 match. The main benefits of using XPath are 1) it allows specifying a document location, and 2) it does not require a particular document order for elements or attributes or whitespace output. To take full advantage of 1), the XPath expressions should specify the full document path (e.g. ``/h:html/h:head/x:model``) rather than a search (e.g. ``.//x:model``). To take full advantage of 2), the expression should include element predicates that specify the expected attribute values, e.g. ``/h:html/h:body/x:input[@ref='/trigger-column/a']``. To specify the absence of an element, an expression like the following may be used with ``xml__xpath_match``: ``/h:html[not(descendant::x:input)]``, or alternatively ``xml__xpath_count``: ``.//x:input`` with an expected count of 0 (zero).
+
+Documentation
+=============
+For developers, ``pyxform`` uses docstrings, type annotations, and test cases. Most modern IDEs can display docstrings and type annotations in a easily navigable format, so no additional docs are compiled (e.g. sphinx). In addition to the user documentation, developers should be familiar with the `ODK XForms Specification https://getodk.github.io/xforms-spec/`.
+
+For users, ``pyxform`` has documentation at the following locations:
+* `XLSForm docs <https://xlsform.org/>`_
+* `XLSForm template <https://docs.google.com/spreadsheets/d/1v9Bumt3R0vCOGEKQI6ExUf2-8T72-XXp_CbKKTACuko/edit#gid=1052905058>`_
+* `ODK Docs <https://docs.getodk.org/>`_
+
+Change Log
+==========
+`Changelog <CHANGES.txt>`_
+
+Releasing pyxform
+=================
+
+1. Make sure the version of ODK Validate in the repo is up-to-date::
+
+    pyxform_validator_update odk update ODK-Validate-vx.x.x.jar
+
+2. Run all tests through Validate by setting the default for ``run_odk_validate`` to ``kwargs.get("run_odk_validate", True)`` in ``tests/pyxform_test_case.py``.
+3. Draft a new GitHub release with the list of merged PRs. Follow the title and description pattern of the previous release.
+4. Checkout a release branch from latest upstream master.
+5. Update ``CHANGES.txt`` with the text of the draft release.
+6. Update ``pyproject.toml``, ``pyxform/__init__.py`` with the new release version number.
+7. Commit, push the branch, and initiate a pull request. Wait for tests to pass, then merge the PR.
+8. Tag the release and it will automatically be published
+
+Manually releasing
+===================
+Releases are now automatic. These instructions are provided for forks or for a future change in process.
+
+1. In a clean new release only directory, check out master.
+2. Create a new virtualenv in this directory to ensure a clean Python environment::
+
+     /usr/local/bin/python3.8 -m venv pyxform-release
+     . pyxform-release/bin/activate
+
+3. Install the production and packaging requirements::
+
+     pip install -e .
+     pip install flit==3.9.0
+
+4. Clean up build and dist folders::
+
+     rm -rf build dist pyxform.egg-info
+
+5. Prepare ``sdist`` and ``bdist_wheel`` distributions, and publish to PyPI::
+
+     flit --debug publish --no-use-vcs
+
+6. Tag the GitHub release and publish it.
+
+Related projects
+================
+
+These projects are not vetted or endorsed but are linked here for reference.
+
+**Converters**
+
+*To XLSForm*
+
+* `cueform <https://github.com/freddieptf/cueform>`_ (Go): from CUE
+* `md2xlsform <https://github.com/joshuaberetta/md2xlsform>`_ (Python): from MarkDown
+* `xlsform <https://github.com/networkearth/xlsform>`_ (Python): from JSON
+* `yxf <https://github.com/Sjlver/yxf>`_ (Python): from YAML
+
+*From XLSForm*
+
+* `ODK2Doc <https://github.com/zaeendesouza/ODK2Doc>`_ (R): to Word
+* `OdkGraph <https://github.com/jkpr/OdkGraph>`_ (Python): to a graph
+* `Pureser <https://github.com/SwissTPH/Pureser>`_ (Swift): to HTML
+* `ppp <https://github.com/pmaengineering/ppp>`_ (Python): to HTML, PDF, Word
+* `QuestionnaireHTML <https://github.com/hedibmustapha/QuestionnaireHTML>`_ (R): to HTML
+* `xlsform-converter <https://github.com/wq/xlsform-converter>`_ (Python): to Django modules
+* `xlsform <https://github.com/networkearth/xlsform>`_ (Python): to JSON
+* `xlsform2json <https://github.com/owengrant/xlsform2json>`_ (Java): to JSON
+* `XLSform2PDF <https://github.com/HEDERA-PLATFORM/XLSform2PDF>`_ (Python): to PDF
+* `xlson <https://github.com/opensrp/xlson>`_ (Python): to OpenSRP JSON
+* `yxf <https://github.com/Sjlver/yxf>`_ (Python): to YAML
+
+**Management Tools**
+
+* `surveydesignr <https://github.com/williameoswald/surveydesignr>`_ (R): compare XLSForms
+* `ipacheckscto <https://github.com/PovertyAction/ipacheckscto>`_ (Stata): check XLSForm for errors or design issues
+* `kobocruncher <https://github.com/Edouard-Legoupil/kobocruncher>`_ (R): generate analysis Rmd from XLSForm
+* `odkmeta <https://github.com/PovertyAction/odkmeta>`_ (Stata): use XLSForm to import ODK data to Stata
+* `odktools <https://github.com/ilri/odktools>`_ (C++): convert pyxform internal data model to MySQL
+* `pmix <https://github.com/pmaengineering/pmix>`_ (Python): manage XLSForm authoring
+* `pyxform-docker <https://github.com/seadowg/pyxform-docker>`_ (Dockerfile): image for pyxform development
+* `xform-test <https://github.com/PMA-2020/xform-test>`_ (Java): test XLSForms
+* `xlsformpo <https://github.com/delcroip/xlsformpo>`_ (Python): use .po files for XLSForm translations
+* `XlsFormUtil <https://github.com/unhcr-americas/XlsFormUtil>`_ (R): manage XLSForm authoring
+
```

### Comparing `pyxform-2.0.2/pyxform/__init__.py` & `pyxform-2.0.3/pyxform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 pyxform is a Python library designed to make authoring XForms for ODK
 Collect easy.
 """
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 
 from pyxform.builder import (
     SurveyElementBuilder,
     create_survey,
     create_survey_element_from_dict,
     create_survey_from_path,
     create_survey_from_xls,
```

### Comparing `pyxform-2.0.2/pyxform/aliases.py` & `pyxform-2.0.3/pyxform/aliases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Aliases for elements which could mean the same element in XForm but is represented
 differently on the XLSForm.
 """
 from pyxform import constants
 
 # Aliases:
@@ -70,15 +69,15 @@
     "SMS Separator": constants.SMS_SEPARATOR,
     "SMS Allow Media": constants.SMS_ALLOW_MEDIA,
     "SMS Date Format": constants.SMS_DATE_FORMAT,
     "SMS DateTime Format": constants.SMS_DATETIME_FORMAT,
     "SMS Response": constants.SMS_RESPONSE,
     "compact_tag": "instance::odk:tag",  # used for compact representation
     "Type": "type",
-    "List_name": "list_name",
+    "List_name": constants.LIST_NAME_U,
     # u"repeat_count": u"jr:count",  duplicate key
     "read_only": "bind::readonly",
     "readonly": "bind::readonly",
     "relevant": "bind::relevant",
     "caption": constants.LABEL,
     "appearance": "control::appearance",  # TODO: this is also an issue
     "relevance": "bind::relevant",
@@ -108,15 +107,15 @@
     "required_message": "bind::jr:requiredMsg",
     "required message": "bind::jr:requiredMsg",
     "body": "control",
     "parameters": "parameters",
     constants.ENTITIES_SAVETO: "bind::entities:saveto",
 }
 
-entities_header = {"list_name": "dataset"}
+entities_header = {constants.LIST_NAME_U: "dataset"}
 
 # Key is the pyxform internal name, Value is the name used in error/warning messages.
 TRANSLATABLE_SURVEY_COLUMNS = {
     constants.LABEL: constants.LABEL,
     # Per ODK Spec, could include "short" once pyxform supports it.
     constants.HINT: constants.HINT,
     "guidance_hint": "guidance_hint",
@@ -132,15 +131,15 @@
     "image": "media::image",
     "big-image": "media::big-image",
     "audio": "media::audio",
     "video": "media::video",
 }
 list_header = {
     "caption": constants.LABEL,
-    "list_name": constants.LIST_NAME,
+    constants.LIST_NAME_U: constants.LIST_NAME_S,
     "value": constants.NAME,
     "image": "media::image",
     "big-image": "media::big-image",
     "audio": "media::audio",
     "video": "media::video",
 }
 # Note that most of the type aliasing happens in all.xls
@@ -177,7 +176,21 @@
     "simserial",
     "start",
     "start-geopoint",
     "today",
     "username",
 ]
 osm = {"osm": constants.OSM_TYPE}
+BINDING_CONVERSIONS = {
+    "yes": "true()",
+    "Yes": "true()",
+    "YES": "true()",
+    "true": "true()",
+    "True": "true()",
+    "TRUE": "true()",
+    "no": "false()",
+    "No": "false()",
+    "NO": "false()",
+    "false": "false()",
+    "False": "false()",
+    "FALSE": "false()",
+}
```

### Comparing `pyxform-2.0.2/pyxform/builder.py` & `pyxform-2.0.3/pyxform/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Survey builder functionality.
 """
 import copy
 import os
 import re
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
@@ -29,60 +28,57 @@
 if TYPE_CHECKING:
     from pyxform.survey_element import SurveyElement
 
 OR_OTHER_CHOICE = {
     const.NAME: "other",
     const.LABEL: "Other",
 }
+QUESTION_CLASSES = {
+    "": Question,
+    "action": Question,
+    "input": InputQuestion,
+    "odk:rank": MultipleChoiceQuestion,
+    "osm": OsmUploadQuestion,
+    "range": RangeQuestion,
+    "select": MultipleChoiceQuestion,
+    "select1": MultipleChoiceQuestion,
+    "trigger": TriggerQuestion,
+    "upload": UploadQuestion,
+}
+SECTION_CLASSES = {
+    const.GROUP: GroupedSection,
+    const.REPEAT: RepeatingSection,
+    const.SURVEY: Survey,
+}
 
 
 def copy_json_dict(json_dict):
     """
     Returns a deep copy of the input json_dict
     """
     json_dict_copy = None
     items = None
 
-    if type(json_dict) is list:
+    if isinstance(json_dict, list):
         json_dict_copy = [None] * len(json_dict)
         items = enumerate(json_dict)
-    elif type(json_dict) is dict:
+    elif isinstance(json_dict, dict):
         json_dict_copy = {}
         items = json_dict.items()
 
     for key, value in items:
-        if type(value) is dict or type(value) is list:
+        if isinstance(value, (dict, list)):
             json_dict_copy[key] = copy_json_dict(value)
         else:
             json_dict_copy[key] = value
 
     return json_dict_copy
 
 
 class SurveyElementBuilder:
-    # we use this CLASSES dict to create questions from dictionaries
-    QUESTION_CLASSES = {
-        "": Question,
-        "action": Question,
-        "input": InputQuestion,
-        "odk:rank": MultipleChoiceQuestion,
-        "osm": OsmUploadQuestion,
-        "range": RangeQuestion,
-        "select": MultipleChoiceQuestion,
-        "select1": MultipleChoiceQuestion,
-        "trigger": TriggerQuestion,
-        "upload": UploadQuestion,
-    }
-
-    SECTION_CLASSES = {
-        const.GROUP: GroupedSection,
-        const.REPEAT: RepeatingSection,
-        const.SURVEY: Survey,
-    }
-
     def __init__(self, **kwargs):
         # I don't know why we would need an explicit none option for
         # select alls
         self._add_none_option = False
         self._sections: Optional[Dict[str, Dict]] = None
         self.set_sections(kwargs.get("sections", {}))
 
@@ -93,29 +89,30 @@
 
     def set_sections(self, sections):
         """
         sections is a dict of python objects, a key in this dict is
         the name of the section and the value is a dict that can be
         used to create a whole survey.
         """
-        assert type(sections) == dict
+        if not isinstance(sections, dict):
+            raise PyXFormError("""Invalid value for `sections`.""")
         self._sections = sections
 
     def create_survey_element_from_dict(
         self, d: Dict[str, Any]
     ) -> Union["SurveyElement", List["SurveyElement"]]:
         """
         Convert from a nested python dictionary/array structure (a json dict I
         call it because it corresponds directly with a json object)
         to a survey object
         """
         if "add_none_option" in d:
             self._add_none_option = d["add_none_option"]
 
-        if d[const.TYPE] in self.SECTION_CLASSES:
+        if d[const.TYPE] in SECTION_CLASSES:
             if d[const.TYPE] == const.SURVEY:
                 self._choices = copy.deepcopy(d.get(const.CHOICES, {}))
 
             section = self._create_section_from_dict(d)
 
             if d[const.TYPE] == const.SURVEY:
                 section.setvalues_by_triggering_ref = self.setvalues_by_triggering_ref
@@ -206,26 +203,26 @@
         if len(choice_list) <= 0:
             raise PyXFormError("There should be choices for this question.")
         if not any(c[const.NAME] == OR_OTHER_CHOICE[const.NAME] for c in choice_list):
             choice_list.append(SurveyElementBuilder._get_or_other_choice(choice_list))
 
     @staticmethod
     def _get_or_other_choice(
-        choice_list: List[Dict[str, Any]]
+        choice_list: List[Dict[str, Any]],
     ) -> Dict[str, Union[str, Dict]]:
         """
         If the choices have any translations, return an OR_OTHER choice for each lang.
         """
         if any(isinstance(c.get(const.LABEL), dict) for c in choice_list):
-            langs = set(
+            langs = {
                 lang
                 for c in choice_list
                 for lang in c[const.LABEL]
                 if isinstance(c.get(const.LABEL), dict)
-            )
+            }
             return {
                 const.NAME: OR_OTHER_CHOICE[const.NAME],
                 const.LABEL: {lang: OR_OTHER_CHOICE[const.LABEL] for lang in langs},
             }
         return OR_OTHER_CHOICE
 
     @staticmethod
@@ -253,30 +250,30 @@
         """
         question_type = question_type_dictionary.get(question_type_str, {})
         control_dict = question_type.get(const.CONTROL, {})
         control_tag = control_dict.get("tag", "")
         if control_tag == "upload" and control_dict.get("mediatype") == "osm/*":
             control_tag = "osm"
 
-        return SurveyElementBuilder.QUESTION_CLASSES[control_tag]
+        return QUESTION_CLASSES[control_tag]
 
     @staticmethod
     def _create_specify_other_question_from_dict(d: Dict[str, Any]) -> InputQuestion:
         kwargs = {
             const.TYPE: "text",
             const.NAME: "%s_other" % d[const.NAME],
             const.LABEL: "Specify other.",
             const.BIND: {"relevant": "selected(../%s, 'other')" % d[const.NAME]},
         }
         return InputQuestion(**kwargs)
 
     def _create_section_from_dict(self, d):
         d_copy = d.copy()
         children = d_copy.pop(const.CHILDREN, [])
-        section_class = self.SECTION_CLASSES[d_copy[const.TYPE]]
+        section_class = SECTION_CLASSES[d_copy[const.TYPE]]
         if d[const.TYPE] == const.SURVEY and const.TITLE not in d:
             d_copy[const.TITLE] = d[const.NAME]
         result = section_class(**d_copy)
         for child in children:
             # Deep copying the child is a hacky solution to the or_other bug.
             # I don't know why it works.
             # And I hope it doesn't break something else.
@@ -332,36 +329,31 @@
         return result.children
 
     @staticmethod
     def _name_and_label_substitutions(question_template, column_headers):
         # if the label in column_headers has multiple languages setup a
         # dictionary by language to do substitutions.
         info_by_lang = {}
-        if type(column_headers[const.LABEL]) == dict:
-            info_by_lang = dict(
-                [
-                    (
-                        lang,
-                        {
-                            const.NAME: column_headers[const.NAME],
-                            const.LABEL: column_headers[const.LABEL][lang],
-                        },
-                    )
-                    for lang in column_headers[const.LABEL].keys()
-                ]
-            )
+        if isinstance(column_headers[const.LABEL], dict):
+            info_by_lang = {
+                lang: {
+                    const.NAME: column_headers[const.NAME],
+                    const.LABEL: column_headers[const.LABEL][lang],
+                }
+                for lang in column_headers[const.LABEL].keys()
+            }
 
         result = question_template.copy()
         for key in result.keys():
-            if type(result[key]) == str:
+            if isinstance(result[key], str):
                 result[key] %= column_headers
-            elif type(result[key]) == dict:
+            elif isinstance(result[key], dict):
                 result[key] = result[key].copy()
                 for key2 in result[key].keys():
-                    if type(column_headers[const.LABEL]) == dict:
+                    if isinstance(column_headers[const.LABEL], dict):
                         result[key][key2] %= info_by_lang.get(key2, column_headers)
                     else:
                         result[key][key2] %= column_headers
         return result
 
     def create_survey_element_from_json(self, str_or_path):
         d = utils.get_pyobj_from_json(str_or_path)
@@ -390,17 +382,17 @@
     survey = create_survey_element_from_dict(d)
     if not survey.id_string:
         survey.id_string = excel_reader._name
     return survey
 
 
 def create_survey(
-    name_of_main_section: str = None,
-    sections: Dict[str, Dict] = None,
-    main_section: Dict[str, Any] = None,
+    name_of_main_section: Optional[str] = None,
+    sections: Optional[Dict[str, Dict]] = None,
+    main_section: Optional[Dict[str, Any]] = None,
     id_string: Optional[str] = None,
     title: Optional[str] = None,
 ) -> Survey:
     """
     name_of_main_section -- a string key used to find the main section in the
                             sections dict if it is not supplied in the
                             main_section arg
```

### Comparing `pyxform-2.0.2/pyxform/constants.py` & `pyxform-2.0.3/pyxform/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 This file contains constants that correspond with the property names in the
 json survey format. (@see json_form_schema.json) These names are to be shared
 between X2json and json2Y programs. By putting them in a shared file,
 the literal names can be easily changed, typos can be avoided, and references
 are easier to find.
 """
@@ -38,17 +37,15 @@
 DEFAULT_LANGUAGE_VALUE = "default"
 LABEL = "label"
 HINT = "hint"
 STYLE = "style"
 ATTRIBUTE = "attribute"
 ALLOW_CHOICE_DUPLICATES = "allow_choice_duplicates"
 
-BIND = (
-    "bind"  # TODO: What should I do with the nested types? (readonly and relevant) # noqa
-)
+BIND = "bind"  # TODO: What should I do with the nested types? (readonly and relevant)
 MEDIA = "media"
 CONTROL = "control"
 APPEARANCE = "appearance"
 ITEMSET = "itemset"
 RANDOMIZE = "randomize"
 CHOICE_FILTER = "choice_filter"
 PARAMETERS = "parameters"
@@ -66,17 +63,18 @@
 SELECT_OR_OTHER_SUFFIX = " or specify other"
 RANK = "rank"
 QUESTION = "question"
 CHOICE = "choice"
 CHOICES = "choices"
 
 # XLS Specific constants
-LIST_NAME = "list name"
+LIST_NAME_S = "list name"
+LIST_NAME_U = "list_name"
 CASCADING_SELECT = "cascading_select"
-TABLE_LIST = "table-list"  # hyphenated because it goes in appearance, and convention for appearance column is dashes # noqa
+TABLE_LIST = "table-list"  # hyphenated because it goes in appearance, and convention for appearance column is dashes
 FIELD_LIST = "field-list"
 LIST_NOLABEL = "list-nolabel"
 
 SURVEY = "survey"
 SETTINGS = "settings"
 EXTERNAL_CHOICES = "external_choices"
 ENTITIES = "entities"
@@ -146,7 +144,24 @@
 ROW_FORMAT_STRING: str = "[row : %s]"
 XML_IDENTIFIER_ERROR_MESSAGE = "must begin with a letter, colon, or underscore. Other characters can include numbers, dashes, and periods."
 _MSG_SUPPRESS_SPELLING = (
     " If you do not mean to include a sheet, to suppress this message, "
     "prefix the sheet name with an underscore. For example 'setting' "
     "becomes '_setting'."
 )
+
+CONVERTIBLE_BIND_ATTRIBUTES = (
+    "readonly",
+    "required",
+    "relevant",
+    "constraint",
+    "calculate",
+)
+NSMAP = {
+    "xmlns": "http://www.w3.org/2002/xforms",
+    "xmlns:h": "http://www.w3.org/1999/xhtml",
+    "xmlns:ev": "http://www.w3.org/2001/xml-events",
+    "xmlns:xsd": "http://www.w3.org/2001/XMLSchema",
+    "xmlns:jr": "http://openrosa.org/javarosa",
+    "xmlns:orx": "http://openrosa.org/xforms",
+    "xmlns:odk": "http://www.opendatakit.org/xforms",
+}
```

### Comparing `pyxform-2.0.2/pyxform/entities/entities_parsing.py` & `pyxform-2.0.3/pyxform/entities/entities_parsing.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
             f"{error_start} '{save_to}'. Entity property names {const.XML_IDENTIFIER_ERROR_MESSAGE}"
         )
 
 
 def validate_entities_columns(row: Dict):
     extra = {k: None for k in row.keys() if k not in EC.value_list()}
     if 0 < len(extra):
-        fmt_extra = ", ".join((f"'{k}'" for k in extra.keys()))
+        fmt_extra = ", ".join(f"'{k}'" for k in extra.keys())
         msg = (
             f"The entities sheet included the following unexpected column(s): {fmt_extra}. "
             f"These columns are not supported by this version of pyxform. Please either: "
             f"check the spelling of the column names, remove the columns, or update "
             f"pyxform."
         )
         raise PyXFormError(msg)
```

### Comparing `pyxform-2.0.2/pyxform/entities/entity_declaration.py` & `pyxform-2.0.3/pyxform/entities/entity_declaration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 from pyxform import constants as const
 from pyxform.survey_element import SurveyElement
 from pyxform.utils import node
 
 EC = const.EntityColumns
```

### Comparing `pyxform-2.0.2/pyxform/file_utils.py` & `pyxform-2.0.3/pyxform/file_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 The pyxform file utility functions.
 """
 import glob
 import os
 
 from pyxform import utils
```

### Comparing `pyxform-2.0.2/pyxform/iana_subtags.txt` & `pyxform-2.0.3/pyxform/iana_subtags.txt`

 * *Files identical despite different names*

### Comparing `pyxform-2.0.2/pyxform/instance.py` & `pyxform-2.0.3/pyxform/instance.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# -*- coding: utf-8 -*-
 """
 SurveyInstance class module.
 """
+from pyxform.errors import PyXFormError
 from pyxform.xform_instance_parser import parse_xform_instance
 
 
 class SurveyInstance:
     def __init__(self, survey_object, **kwargs):
         self._survey = survey_object
         self.kwargs = kwargs  # not sure what might be passed to this
@@ -31,15 +31,15 @@
     def xpaths(self):
         # originally thought of having this method get the xpath stuff
         # but survey doesn't like when xml() is called multiple times.
         return self._xpaths
 
     def answer(self, name=None, value=None):
         if name is None:
-            raise Exception("In answering, name must be given")
+            raise PyXFormError("In answering, name must be given")
 
         # ahh. this is horrible, but we need the xpath dict in survey
         # to be up-to-date ...maybe
         # self._survey.xml()
 
         if name in self._survey._xpath.keys():
             self._answers[name] = value
@@ -53,19 +53,19 @@
         return {"node_name": self._name, "id": self._id, "children": children}
 
     def to_xml(self):
         """
         A horrible way to do this, but it works (until we need the attributes
          pumped out in order, etc)
         """
-        open_str = """<?xml version='1.0' ?><%s id="%s">""" % (self._name, self._id)
+        open_str = f"""<?xml version='1.0' ?><{self._name} id="{self._id}">"""
         close_str = """</%s>""" % self._name
         vals = ""
         for k, v in self._answers.items():
-            vals += "<%s>%s</%s>" % (k, str(v), k)
+            vals += f"<{k}>{v!s}</{k}>"
 
         output = open_str + vals + close_str
         return output
 
     def answers(self):
         """
         This returns "_answers", which is a dict with the key-value
@@ -74,15 +74,15 @@
         """
         return self._answers
 
     def import_from_xml(self, xml_string_or_filename):
         import os.path
 
         if os.path.isfile(xml_string_or_filename):
-            xml_str = open(xml_string_or_filename).read()
+            xml_str = open(xml_string_or_filename, encoding="utf-8").read()
         else:
             xml_str = xml_string_or_filename
         key_val_dict = parse_xform_instance(xml_str)
         for k, v in key_val_dict.items():
             self.answer(name=k, value=v)
 
     def __unicode__(self):
```

### Comparing `pyxform-2.0.2/pyxform/parsing/instance_expression.py` & `pyxform-2.0.3/pyxform/parsing/instance_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             boundaries.append(last_token.end)
 
     if last_token is not None:
         boundaries.append(last_token.end)
 
     # Pair up the boundaries [1, 2, 3, 4] -> [(1, 2), (3, 4)].
     bounds = iter(boundaries)
-    pos_bounds = [(x, y) for x, y in zip(bounds, bounds)]
+    pos_bounds = list(zip(bounds, bounds))
     return pos_bounds
 
 
 def replace_with_output(xml_text: str, context: "SurveyElement", survey: "Survey") -> str:
     """
     Find occurrences of instance expressions and replace them with <output/> elements.
```

### Comparing `pyxform-2.0.2/pyxform/question.py` & `pyxform-2.0.3/pyxform/question.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 XForm Survey element classes for different question types.
 """
 import os.path
 
 from pyxform.constants import (
     EXTERNAL_CHOICES_ITEMSET_REF_LABEL,
@@ -50,16 +49,17 @@
         if self.type == "calculate" or (
             ("calculate" in self.bind or self.trigger) and not (self.label or self.hint)
         ):
             nested_setvalues = self.get_root().get_setvalues_for_question_name(self.name)
             if nested_setvalues:
                 for setvalue in nested_setvalues:
                     msg = (
-                        "The question ${%s} is not user-visible so it can't be used as a calculation trigger for question ${%s}."
-                        % (self.name, setvalue[0])
+                        f"The question ${{{self.name}}} is not user-visible "
+                        "so it can't be used as a calculation trigger for "
+                        f"question ${{{setvalue[0]}}}."
                     )
                     raise PyXFormError(msg)
             return None
 
         xml_node = self.build_xml()
 
         if xml_node:
@@ -196,15 +196,16 @@
         descendants = self.iter_descendants()
         next(descendants)  # iter_descendants includes self; we need to pop it
 
         for choice in descendants:
             choice.validate()
 
     def build_xml(self):
-        assert self.bind["type"] in ["string", "odk:rank"]
+        if self.bind["type"] not in ["string", "odk:rank"]:
+            raise PyXFormError("""Invalid value for `self.bind["type"]`.""")
         survey = self.get_root()
         control_dict = self.control.copy()
         # Resolve field references in attributes
         for key, value in control_dict.items():
             control_dict[key] = survey.insert_xpaths(value, self)
         control_dict["ref"] = self.get_xpath()
 
@@ -235,21 +236,20 @@
             has_media = self.get("_itemset_has_media", False)
             has_dyn_label = self.get("_itemset_dyn_label", False)
             is_previous_question = bool(
                 PYXFORM_REFERENCE_REGEX.search(self.get("itemset"))
             )
 
             if file_extension in EXTERNAL_INSTANCE_EXTENSIONS:
-                itemset = itemset
+                pass
+            elif not multi_language and not has_media and not has_dyn_label:
+                itemset = self["itemset"]
             else:
-                if not multi_language and not has_media and not has_dyn_label:
-                    itemset = self["itemset"]
-                else:
-                    itemset = self["itemset"]
-                    itemset_label_ref = "jr:itext(itextId)"
+                itemset = self["itemset"]
+                itemset_label_ref = "jr:itext(itextId)"
 
             choice_filter = survey.insert_xpaths(
                 choice_filter, self, True, is_previous_question
             )
             if is_previous_question:
                 path = (
                     survey.insert_xpaths(self["itemset"], self, reference_parent=True)
@@ -302,24 +302,24 @@
                 result.appendChild(child.xml())
 
         return result
 
 
 class SelectOneQuestion(MultipleChoiceQuestion):
     def __init__(self, **kwargs):
-        super(SelectOneQuestion, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self._dict[self.TYPE] = "select one"
 
 
 class Tag(SurveyElement):
     def __init__(self, **kwargs):
         kwargs_copy = kwargs.copy()
         choices = kwargs_copy.pop("choices", []) + kwargs_copy.pop("children", [])
 
-        super(Tag, self).__init__(**kwargs_copy)
+        super().__init__(**kwargs_copy)
 
         if choices:
             self.children = []
 
             for choice in choices:
                 option = Option(**choice)
                 self.add_child(option)
@@ -341,15 +341,15 @@
 
 
 class OsmUploadQuestion(UploadQuestion):
     def __init__(self, **kwargs):
         kwargs_copy = kwargs.copy()
         tags = kwargs_copy.pop("tags", []) + kwargs_copy.pop("children", [])
 
-        super(OsmUploadQuestion, self).__init__(**kwargs_copy)
+        super().__init__(**kwargs_copy)
 
         if tags:
             self.children = []
 
             for tag in tags:
                 self.add_tag(**tag)
```

### Comparing `pyxform-2.0.2/pyxform/question_type_dictionary.py` & `pyxform-2.0.3/pyxform/question_type_dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 XForm survey question type mapping dictionary module.
 """
 from pyxform.xls2json import QuestionTypesReader, print_pyobj_to_json
 
 
 def generate_new_dict():
```

### Comparing `pyxform-2.0.2/pyxform/section.py` & `pyxform-2.0.3/pyxform/section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-# -*- coding: utf-8 -*-
 """
 Section survey element module.
 """
 from pyxform.errors import PyXFormError
 from pyxform.external_instance import ExternalInstance
 from pyxform.survey_element import SurveyElement
 from pyxform.utils import node
 
 
 class Section(SurveyElement):
     def validate(self):
-        super(Section, self).validate()
+        super().validate()
         for element in self.children:
             element.validate()
         self._validate_uniqueness_of_element_names()
 
     # there's a stronger test of this when creating the xpath
     # dictionary for a survey.
     def _validate_uniqueness_of_element_names(self):
         element_slugs = set()
         for element in self.children:
             elem_lower = element.name.lower()
             if elem_lower in element_slugs:
                 raise PyXFormError(
-                    "There are more than one survey elements named '%s' "
-                    "(case-insensitive) in the section named '%s'."
-                    % (elem_lower, self.name)
+                    f"There are more than one survey elements named '{elem_lower}' "
+                    f"(case-insensitive) in the section named '{self.name}'."
                 )
             element_slugs.add(elem_lower)
 
     def xml_instance(self, **kwargs):
         """
         Creates an xml representation of the section
         """
@@ -73,16 +71,15 @@
 
     def xml_instance_array(self):
         """
         This method is used for generating flat instances.
         """
         for child in self.children:
             if child.get("flat"):
-                for grandchild in child.xml_instance_array():
-                    yield grandchild
+                yield from child.xml_instance_array()
             else:
                 yield child.xml_instance()
 
     def xml_control(self):
         """
         Ideally, we'll have groups up and rolling soon, but for now
         let's just yield controls from all the children of this section
@@ -141,15 +138,15 @@
                 if dynamic_default:
                     nodes.append(dynamic_default)
                 self._dynamic_defaults_helper(e, nodes)
 
     # I'm anal about matching function signatures when overriding a function,
     # but there's no reason for kwargs to be an argument
     def template_instance(self, **kwargs):
-        return super(RepeatingSection, self).generate_repeating_template(**kwargs)
+        return super().generate_repeating_template(**kwargs)
 
 
 class GroupedSection(Section):
     # I think this might be a better place for the table-list stuff, however it
     # doesn't allow for as good of validation as putting it in xls2json
     # def __init__(self, **kwargs):
     #        control = kwargs.get(u"control")
@@ -193,10 +190,10 @@
             attributes["intent"] = survey.insert_xpaths(control_dict["intent"], self)
 
         return node("group", *children, **attributes)
 
     def to_json_dict(self):
         # This is quite hacky, might want to think about a smart way
         # to approach this problem.
-        result = super(GroupedSection, self).to_json_dict()
+        result = super().to_json_dict()
         result["type"] = "group"
         return result
```

### Comparing `pyxform-2.0.2/pyxform/survey.py` & `pyxform-2.0.3/pyxform/survey.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-# -*- coding: utf-8 -*-
 """
 Survey module with XForm Survey objects and utility functions.
 """
-import codecs
 import os
 import re
 import tempfile
 import xml.etree.ElementTree as ETree
 from collections import defaultdict
 from datetime import datetime
 from functools import lru_cache
 from typing import Generator, Iterator, List, Optional, Tuple
 
 from pyxform import aliases, constants
-from pyxform.constants import EXTERNAL_INSTANCE_EXTENSIONS
+from pyxform.constants import EXTERNAL_INSTANCE_EXTENSIONS, NSMAP
 from pyxform.errors import PyXFormError, ValidationError
 from pyxform.external_instance import ExternalInstance
 from pyxform.instance import SurveyInstance
 from pyxform.parsing import instance_expression
 from pyxform.question import Option, Question
 from pyxform.section import Section
 from pyxform.survey_element import SurveyElement
 from pyxform.utils import (
     BRACKETED_TAG_REGEX,
     LAST_SAVED_INSTANCE_NAME,
     LAST_SAVED_REGEX,
-    NSMAP,
     DetachableElement,
     PatchedText,
     get_languages_with_bad_tags,
     has_dynamic_label,
     node,
 )
 from pyxform.validators import enketo_validate, odk_validate
@@ -38,17 +35,15 @@
 RE_FUNCTION_ARGS = re.compile(r"\b[^()]+\((.*)\)$")
 RE_INDEXED_REPEAT = re.compile(r"indexed-repeat\([^)]+\)")
 RE_INSTANCE = re.compile(r"instance\([^)]+.+")
 RE_INSTANCE_SECONDARY_REF = re.compile(
     r"(instance\(.*\)\/root\/item\[.*?(\$\{.*\})\]\/.*?)\s"
 )
 RE_PULLDATA = re.compile(r"(pulldata\s*\(\s*)(.*?),")
-RE_XML_OUTPUT = re.compile(r"\n.*(<output.*>)\n(\s\s)*")
-RE_XML_TEXT = re.compile(r"(>)\n\s*(\s[^<>\s].*?)\n\s*(\s</)", re.DOTALL)
-SEARCH_APPEARANCE_REGEX = re.compile(r"search\(.*?\)")
+SEARCH_FUNCTION_REGEX = re.compile(r"search\(.*?\)")
 
 
 class InstanceInfo:
     """Standardise Instance details relevant during XML generation."""
 
     __slots__ = ("type", "context", "name", "src", "instance")
 
@@ -216,20 +211,20 @@
             "version": str,
             "choices": dict,
             "style": str,
             "attribute": dict,
             "namespaces": str,
             constants.ENTITY_FEATURES: list,
         }
-    )  # yapf: disable
+    )
 
     def validate(self):
         if self.id_string in [None, "None"]:
             raise PyXFormError("Survey cannot have an empty id_string")
-        super(Survey, self).validate()
+        super().validate()
         self._validate_uniqueness_of_section_names()
 
     def _validate_uniqueness_of_section_names(self):
         root_node_name = self.name
         section_names = []
         for element in self.iter_descendants():
             if isinstance(element, Section):
@@ -259,21 +254,19 @@
                 ns.split("=")
                 for ns in namespaces.split()
                 if len(ns.split("=")) == 2 and ns.split("=")[0] != ""
             ]
             xmlns = "xmlns:"
             nsmap = NSMAP.copy()
             nsmap.update(
-                dict(
-                    [
-                        (xmlns + k, v.replace('"', "").replace("'", ""))
-                        for k, v in nslist
-                        if xmlns + k not in nsmap
-                    ]
-                )
+                {
+                    xmlns + k: v.replace('"', "").replace("'", "")
+                    for k, v in nslist
+                    if xmlns + k not in nsmap
+                }
             )
             return nsmap
 
         return NSMAP
 
     def xml(self):
         """
@@ -356,15 +349,15 @@
 
     @staticmethod
     def _generate_external_instances(element) -> Optional[InstanceInfo]:
         if isinstance(element, ExternalInstance):
             name = element["name"]
             extension = element["type"].split("-")[0]
             prefix = "file-csv" if extension == "csv" else "file"
-            src = "jr://{}/{}.{}".format(prefix, name, extension)
+            src = f"jr://{prefix}/{name}.{extension}"
             return InstanceInfo(
                 type="external",
                 context="[type: {t}, name: {n}]".format(
                     t=element["parent"]["type"], n=element["parent"]["name"]
                 ),
                 name=name,
                 src=src,
@@ -387,21 +380,19 @@
             if seen.get(element) is None:
                 seen[element] = [i]
             else:
                 seen[element].append(i)
         errors = []
         for element, copies in seen.items():
             if len(copies) > 1:
-                contexts = ", ".join(x.context for x in copies)
+                contexts = ", ".join(f"{x.context}({x.type})" for x in copies)
                 errors.append(
                     "Instance names must be unique within a form. "
-                    "The name '{i}' was found {c} time(s), "
-                    "under these contexts: {contexts}".format(
-                        i=element, c=len(copies), contexts=contexts
-                    )
+                    f"The name '{element}' was found {len(copies)} time(s), "
+                    f"under these contexts: {contexts}"
                 )
         if errors:
             raise ValidationError("\n".join(errors))
 
     @staticmethod
     def _generate_pulldata_instances(element) -> Optional[List[InstanceInfo]]:
         def get_pulldata_functions(element):
@@ -420,15 +411,15 @@
                 functions_present.append(element["choice_filter"])
             if "pulldata(" in str(element["default"]):
                 functions_present.append(element["default"])
 
             return functions_present
 
         def get_instance_info(element, file_id):
-            uri = "jr://file-csv/{}.csv".format(file_id)
+            uri = f"jr://file-csv/{file_id}.csv"
 
             return InstanceInfo(
                 type="pulldata",
                 context="[type: {t}, name: {n}]".format(
                     t=element["parent"]["type"], n=element["parent"]["name"]
                 ),
                 name=file_id,
@@ -453,18 +444,16 @@
         return None
 
     @staticmethod
     def _generate_from_file_instances(element) -> Optional[InstanceInfo]:
         itemset = element.get("itemset")
         file_id, ext = os.path.splitext(itemset)
         if itemset and ext in EXTERNAL_INSTANCE_EXTENSIONS:
-            uri = "jr://%s/%s" % (
-                "file" if ext == ".xml" or ext == ".geojson" else "file-%s" % ext[1:],
-                itemset,
-            )
+            file_ext = "file" if ext in {".xml", ".geojson"} else f"file-{ext[1:]}"
+            uri = f"jr://{file_ext}/{itemset}"
             return InstanceInfo(
                 type="file",
                 context="[type: {t}, name: {n}]".format(
                     t=element["parent"]["type"], n=element["parent"]["name"]
                 ),
                 name=file_id,
                 src=uri,
@@ -567,24 +556,17 @@
         seen = {}
         for i in instances:
             if i.name in seen.keys() and seen[i.name].src != i.src:
                 # Instance id exists with different src URI -> error.
                 msg = (
                     "The same instance id will be generated for different "
                     "external instance source URIs. Please check the form."
-                    " Instance name: '{i}', Existing type: '{e}', "
-                    "Existing URI: '{iu}', Duplicate type: '{d}', "
-                    "Duplicate URI: '{du}', Duplicate context: '{c}'.".format(
-                        i=i.name,
-                        iu=seen[i.name].src,
-                        e=seen[i.name].type,
-                        d=i.type,
-                        du=i.src,
-                        c=i.context,
-                    )
+                    f" Instance name: '{i.name}', Existing type: '{seen[i.name].type}', "
+                    f"Existing URI: '{seen[i.name].src}', Duplicate type: '{i.type}', "
+                    f"Duplicate URI: '{i.src}', Duplicate context: '{i.context}'."
                 )
                 raise PyXFormError(msg)
             elif i.name in seen.keys() and seen[i.name].src == i.src:
                 # Instance id exists with same src URI -> ok, don't duplicate.
                 continue
             else:
                 # Instance doesn't exist yet -> add it.
@@ -617,15 +599,15 @@
             model_children.append(self.itext())
         model_children += [node("instance", self.xml_instance())]
         model_children += list(self._generate_instances())
         model_children += self.xml_descendent_bindings()
         model_children += self.xml_actions()
 
         if self.submission_url or self.public_key or self.auto_send or self.auto_delete:
-            submission_attrs = dict()
+            submission_attrs = {}
             if self.submission_url:
                 submission_attrs["action"] = self.submission_url
                 submission_attrs["method"] = "post"
             if self.public_key:
                 submission_attrs["base64RsaPublicKey"] = self.public_key
             if self.auto_send:
                 submission_attrs["orx:auto-send"] = self.auto_send
@@ -668,61 +650,70 @@
             else:
                 dicty[key] = value
             return
         if path[0] not in dicty:
             dicty[path[0]] = {}
         self._add_to_nested_dict(dicty[path[0]], path[1:], value)
 
-    @staticmethod
-    def _redirect_is_search_itext(element: SurveyElement) -> None:
+    def _redirect_is_search_itext(self, element: SurveyElement) -> bool:
         """
-        For selects using the "search()" appearance, redirect itext for in-line items.
+        For selects using the "search()" function, redirect itext for in-line items.
 
-        External selects from a "search" appearance alone don't work in Enketo. In Collect
+        External selects from a "search" function alone don't work in Enketo. In Collect
         they must have the "item" elements in the body, rather than in an "itemset".
 
         The "itemset" reference is cleared below, so that the element will get in-line
         items instead of an itemset reference to a secondary instance. The itext ref is
         passed to the options/choices so they can use the generated translations. This
-        accounts for questions with and without a "search()" appearance sharing choices.
+        accounts for questions with and without a "search()" function sharing choices.
 
         :param element: A select type question.
-        :return: None, the question/children are modified in-place.
+        :return: If True, the element uses the search function.
         """
         try:
             is_search = bool(
-                SEARCH_APPEARANCE_REGEX.search(
+                SEARCH_FUNCTION_REGEX.search(
                     element[constants.CONTROL][constants.APPEARANCE]
                 )
             )
         except (KeyError, TypeError):
             is_search = False
         if is_search:
+            file_id, ext = os.path.splitext(element[constants.ITEMSET])
+            if ext in EXTERNAL_INSTANCE_EXTENSIONS:
+                msg = (
+                    f"Question '{element[constants.NAME]}' is a select from file type, "
+                    "using 'search()'. This combination is not supported. "
+                    "Remove the 'search()' usage, or change the select type."
+                )
+                raise PyXFormError(msg)
+            itemset = element[constants.ITEMSET]
+            self.choices.pop(itemset, None)
             element[constants.ITEMSET] = ""
             for i, opt in enumerate(element.get(constants.CHILDREN, [])):
-                opt["_choice_itext_id"] = f"{element['list_name']}-{i}"
+                opt["_choice_itext_id"] = f"{element[constants.LIST_NAME_U]}-{i}"
+        return is_search
 
     def _setup_translations(self):
         """
         set up the self._translations dict which will be referenced in the
         setup media and itext functions
         """
 
         def _setup_choice_translations(
             name, choice_value, itext_id
         ) -> Generator[Tuple[List[str], str], None, None]:
-            for media_or_lang, value in choice_value.items():  # noqa
+            for media_or_lang, value in choice_value.items():
                 if isinstance(value, dict):
                     for language, val in value.items():
                         yield ([language, itext_id, media_or_lang], val)
+                elif name == constants.MEDIA:
+                    yield ([self.default_language, itext_id, media_or_lang], value)
                 else:
-                    if name == constants.MEDIA:
-                        yield ([self.default_language, itext_id, media_or_lang], value)
-                    else:
-                        yield ([media_or_lang, itext_id, "long"], value)
+                    yield ([media_or_lang, itext_id, "long"], value)
 
         itemsets_multi_language = set()
         itemsets_has_media = set()
         itemsets_has_dyn_label = set()
 
         def get_choices():
             for list_name, choice_list in self.choices.items():
@@ -759,23 +750,30 @@
 
         for path, value in get_choices():
             last_path = path.pop()
             leaf_value = {last_path: value, constants.TYPE: constants.CHOICE}
             self._add_to_nested_dict(self._translations, path, leaf_value)
 
         select_types = set(aliases.select.keys())
+        search_lists = set()
+        non_search_lists = set()
         for element in self.iter_descendants():
             itemset = element.get("itemset")
             if itemset is not None:
                 element._itemset_multi_language = itemset in itemsets_multi_language
                 element._itemset_has_media = itemset in itemsets_has_media
                 element._itemset_dyn_label = itemset in itemsets_has_dyn_label
 
             if element[constants.TYPE] in select_types:
-                self._redirect_is_search_itext(element=element)
+                select_ref = (element[constants.NAME], element[constants.LIST_NAME_U])
+                if self._redirect_is_search_itext(element=element):
+                    search_lists.add(select_ref)
+                else:
+                    non_search_lists.add(select_ref)
+
             # Skip creation of translations for choices in selects. The creation of these
             # translations is done above in this function.
             parent = element.get("parent")
             if parent is not None and parent[constants.TYPE] not in select_types:
                 for d in element.get_translations(self.default_language):
                     translation_path = d["path"]
                     form = "long"
@@ -794,26 +792,40 @@
                                 "text": d["text"],
                                 "output_context": d["output_context"],
                             },
                             constants.TYPE: constants.QUESTION,
                         }
                     )
 
+        for q_name, list_name in search_lists:
+            choice_refs = [f"'{q}'" for q, c in non_search_lists if c == list_name]
+            if len(choice_refs) > 0:
+                refs_str = ", ".join(choice_refs)
+                msg = (
+                    f"Question '{q_name}' uses 'search()', and its select type references"
+                    f" the choice list name '{list_name}'. This choice list name is "
+                    f"referenced by at least one other question that is not using "
+                    f"'search()', which will not work: {refs_str}. Either 1) use "
+                    f"'search()' for all questions using this choice list name, or 2) "
+                    f"use a different choice list name for the question using 'search()'."
+                )
+                raise PyXFormError(msg)
+
     def _add_empty_translations(self):
         """
         Adds translations so that every itext element has the same elements across every
         language. When translations are not provided "-" will be used.
         This disables any of the default_language fallback functionality.
         """
         paths = {}
-        for lang, translation in self._translations.items():
+        for translation in self._translations.values():
             for path, content in translation.items():
                 paths[path] = paths.get(path, set()).union(content.keys())
 
-        for lang, translation in self._translations.items():
+        for lang in self._translations:
             for path, content_types in paths.items():
                 if path not in self._translations[lang]:
                     self._translations[lang][path] = {}
                 for content_type in content_types:
                     if content_type not in self._translations[lang][path]:
                         self._translations[lang][path][content_type] = "-"
 
@@ -833,28 +845,26 @@
             # nested inside of a dict with key "default", e.g.
             # {"default": {"image": "my_image.jpg"}}
             media_dict_default = media_dict.get("default", None)
             if isinstance(media_dict_default, dict):
                 media_dict = media_dict_default
 
             for media_type, possibly_localized_media in media_dict.items():
-
                 if media_type not in SurveyElement.SUPPORTED_MEDIA:
                     raise PyXFormError("Media type: " + media_type + " not supported")
 
                 if isinstance(possibly_localized_media, dict):
                     # media is localized
                     localized_media = possibly_localized_media
                 else:
                     # media is not localized so create a localized version
                     # using the default language
                     localized_media = {self.default_language: possibly_localized_media}
 
                 for language, media in localized_media.items():
-
                     # Create the required dictionaries in _translations,
                     # then add media as a leaf value:
                     if language not in self._translations:
                         self._translations[language] = {}
 
                     translations_language = self._translations[language]
 
@@ -893,15 +903,15 @@
                 result.append(node("translation", lang=lang))
 
             for label_name, content in translation.items():
                 itext_nodes = []
                 label_type = label_name.partition(":")[-1]
 
                 if not isinstance(content, dict):
-                    raise Exception()
+                    raise PyXFormError("""Invalid value for `content`.""")
 
                 for media_type, media_value in content.items():
                     # Ignore key indicating Question or Choice translation type.
                     if media_type == constants.TYPE:
                         continue
                     if isinstance(media_value, dict):
                         value, output_inserted = self.insert_output_values(
@@ -928,61 +938,48 @@
 
                     if media_type == "long":
                         # I'm ignoring long types for now because I don't know
                         # how they are supposed to work.
                         itext_nodes.append(
                             node("value", value, toParseString=output_inserted)
                         )
-                    elif media_type == "image" or media_type == "big-image":
+                    elif media_type in {"image", "big-image"}:
                         if value != "-":
                             itext_nodes.append(
                                 node(
                                     "value",
                                     "jr://images/" + value,
                                     form=media_type,
                                     toParseString=output_inserted,
                                 )
                             )
-                    else:
-                        if value != "-":
-                            itext_nodes.append(
-                                node(
-                                    "value",
-                                    "jr://" + media_type + "/" + value,
-                                    form=media_type,
-                                    toParseString=output_inserted,
-                                )
+                    elif value != "-":
+                        itext_nodes.append(
+                            node(
+                                "value",
+                                "jr://" + media_type + "/" + value,
+                                form=media_type,
+                                toParseString=output_inserted,
                             )
+                        )
 
                 result[-1].appendChild(node("text", *itext_nodes, id=label_name))
 
         return node("itext", *result)
 
     def date_stamp(self):
         """Returns a date string with the format of %Y_%m_%d."""
         return self._created.strftime("%Y_%m_%d")
 
     def _to_ugly_xml(self):
         return '<?xml version="1.0"?>' + self.xml().toxml()
 
     def _to_pretty_xml(self):
-        """
-        I want the to_xml method to by default validate the xml we are
-        producing.
-        """
-        # Hacky way of pretty printing xml without adding extra white
-        # space to text
-        # TODO: check out pyxml
-        # http://ronrothman.com/public/leftbraned/xml-dom-minidom-toprettyxml-and-silly-whitespace/
-        xml_with_linebreaks = self.xml().toprettyxml(indent="  ")
-        pretty_xml = RE_XML_TEXT.sub(
-            lambda m: "".join(m.group(1, 2, 3)), xml_with_linebreaks
-        )
-        inline_output = RE_XML_OUTPUT.sub(r"\g<1>", pretty_xml)
-        return '<?xml version="1.0"?>\n' + inline_output
+        """Get the XForm with human readable formatting."""
+        return '<?xml version="1.0"?>\n' + self.xml().toprettyxml(indent="  ")
 
     def __repr__(self):
         return self.__unicode__()
 
     def __unicode__(self):
         return "<pyxform.survey.Survey instance at %s>" % hex(id(self))
 
@@ -1049,22 +1046,20 @@
 
         def _is_return_relative_path() -> bool:
             """Determine condition to return relative xpath of current ${name}."""
             indexed_repeat_relative_path_args_index = [0, 1, 3, 5]
             current_matchobj = matchobj
 
             if not last_saved and context:
-
                 if not is_indexed_repeat:
                     return True
 
                 # It is possible to have multiple indexed-repeat in an expression
                 indexed_repeats_iter = RE_INDEXED_REPEAT.finditer(matchobj.string)
                 for indexed_repeat in indexed_repeats_iter:
-
                     # Make sure current ${name} is in the correct indexed-repeat
                     if current_matchobj.end() > indexed_repeat.end():
                         try:
                             next(indexed_repeats_iter)
                             continue
                         except StopIteration:
                             return True
@@ -1078,30 +1073,30 @@
 
                     indexed_repeat_name_index = None
                     indexed_repeat_args = (
                         RE_FUNCTION_ARGS.search(indexed_repeat.group())
                         .group(1)
                         .split(",")
                     )
-                    name_arg = "${{{0}}}".format(name)
+                    name_arg = f"${{{name}}}"
                     for idx, arg in enumerate(indexed_repeat_args):
                         if name_arg in arg.strip():
                             indexed_repeat_name_index = idx
 
                     return (
                         indexed_repeat_name_index is not None
                         and indexed_repeat_name_index
                         not in indexed_repeat_relative_path_args_index
                     )
 
             return False
 
         intro = (
-            "There has been a problem trying to replace %s with the "
-            "XPath to the survey element named '%s'." % (matchobj.group(0), name)
+            f"There has been a problem trying to replace {matchobj.group(0)} with the "
+            f"XPath to the survey element named '{name}'."
         )
         if name not in self._xpath:
             raise PyXFormError(intro + " There is no survey element with this name.")
         if self._xpath[name] is None:
             raise PyXFormError(
                 intro + " There are multiple survey elements" " with this name."
             )
@@ -1185,35 +1180,35 @@
         throwing exceptions and adding warnings to the warnings array.
         """
         if warnings is None:
             warnings = []
         if not path:
             path = self._print_name + ".xml"
         try:
-            with codecs.open(path, mode="w", encoding="utf-8") as file_obj:
+            with open(path, mode="w", encoding="utf-8") as file_obj:
                 if pretty_print:
                     file_obj.write(self._to_pretty_xml())
                 else:
                     file_obj.write(self._to_ugly_xml())
-        except Exception as error:
+        except Exception:
             if os.path.exists(path):
                 os.unlink(path)
-            raise error
+            raise
         if validate:
             warnings.extend(odk_validate.check_xform(path))
         if enketo:
             warnings.extend(enketo_validate.check_xform(path))
 
         # Warn if one or more translation is missing a valid IANA subtag
         translations = self._translations.keys()
         if translations:
             bad_languages = get_languages_with_bad_tags(translations)
             if bad_languages:
                 warnings.append(
-                    "\tThe following language declarations do not contain "
+                    "The following language declarations do not contain "
                     "valid machine-readable codes: "
                     + ", ".join(bad_languages)
                     + ". "
                     + "Learn more: http://xlsform.org#multiple-language-support"
                 )
 
     def to_xml(self, validate=True, pretty_print=True, warnings=None, enketo=False):
```

### Comparing `pyxform-2.0.2/pyxform/survey_element.py` & `pyxform-2.0.3/pyxform/survey_element.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,82 +1,92 @@
-# -*- coding: utf-8 -*-
 """
 Survey Element base class for all survey elements.
 """
 import json
 import re
 from collections import deque
 from functools import lru_cache
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, ClassVar, Dict, List
 
-from pyxform import constants
+from pyxform import aliases as alias
+from pyxform import constants as const
 from pyxform.errors import PyXFormError
 from pyxform.question_type_dictionary import QUESTION_TYPE_DICT
 from pyxform.utils import (
     BRACKETED_TAG_REGEX,
     INVALID_XFORM_TAG_REGEXP,
     default_is_dynamic,
     node,
 )
 from pyxform.xls2json import print_pyobj_to_json
 from pyxform.xlsparseutils import is_valid_xml_tag
 
 if TYPE_CHECKING:
-    from typing import List
-
     from pyxform.utils import DetachableElement
 
+# The following are important keys for the underlying dict that describes SurveyElement
+FIELDS = {
+    "name": str,
+    const.COMPACT_TAG: str,  # used for compact (sms) representation
+    "sms_field": str,
+    "sms_option": str,
+    "label": str,
+    "hint": str,
+    "guidance_hint": str,
+    "default": str,
+    "type": str,
+    "appearance": str,
+    "parameters": dict,
+    "intent": str,
+    "jr:count": str,
+    "bind": dict,
+    "instance": dict,
+    "control": dict,
+    "media": dict,
+    # this node will also have a parent and children, like a tree!
+    "parent": lambda: None,
+    "children": list,
+    "itemset": str,
+    "choice_filter": str,
+    "query": str,
+    "autoplay": str,
+    "flat": lambda: False,
+    "action": str,
+    const.LIST_NAME_U: str,
+    "trigger": str,
+}
+
 
 def _overlay(over, under):
-    if type(under) == dict:
+    if isinstance(under, dict):
         result = under.copy()
         result.update(over)
         return result
     return over if over else under
 
 
+@lru_cache(maxsize=65536)
+def any_repeat(survey_element: "SurveyElement", parent_xpath: str) -> bool:
+    """Return True if there ia any repeat in `parent_xpath`."""
+    for item in survey_element.iter_descendants():
+        if item.get_xpath() == parent_xpath and item.type == const.REPEAT:
+            return True
+
+    return False
+
+
 class SurveyElement(dict):
     """
     SurveyElement is the base class we'll looks for the following keys
     in kwargs: name, label, hint, type, bind, control, parent,
     children, and question_type_dictionary.
     """
 
-    # the following are important keys for the underlying dict that
-    # describes this survey element
-    FIELDS = {
-        "name": str,
-        constants.COMPACT_TAG: str,  # used for compact (sms) representation
-        "sms_field": str,
-        "sms_option": str,
-        "label": str,
-        "hint": str,
-        "guidance_hint": str,
-        "default": str,
-        "type": str,
-        "appearance": str,
-        "parameters": dict,
-        "intent": str,
-        "jr:count": str,
-        "bind": dict,
-        "instance": dict,
-        "control": dict,
-        "media": dict,
-        # this node will also have a parent and children, like a tree!
-        "parent": lambda: None,
-        "children": list,
-        "itemset": str,
-        "choice_filter": str,
-        "query": str,
-        "autoplay": str,
-        "flat": lambda: False,
-        "action": str,
-        "list_name": str,
-        "trigger": str,
-    }
+    __name__ = "SurveyElement"
+    FIELDS: ClassVar[Dict[str, Any]] = FIELDS.copy()
 
     def _default(self):
         # TODO: need way to override question type dictionary
         defaults = QUESTION_TYPE_DICT
         return defaults.get(self.get("type"), {})
 
     def __getattr__(self, key):
@@ -91,18 +101,14 @@
                 return over
             return _overlay(over, under)
         raise AttributeError(key)
 
     def __hash__(self):
         return hash(id(self))
 
-    @property
-    def __name__(self):
-        return "SurveyElement"
-
     def __setattr__(self, key, value):
         self[key] = value
 
     def __init__(self, **kwargs):
         for key, default in self.FIELDS.items():
             self[key] = kwargs.get(key, default())
         self._link_children()
@@ -119,75 +125,46 @@
             child.parent = self
 
     def add_child(self, child):
         self.children.append(child)
         child.parent = self
 
     def add_children(self, children):
-        if type(children) == list:
+        if isinstance(children, list):
             for child in children:
                 self.add_child(child)
         else:
             self.add_child(children)
 
-    BINDING_CONVERSIONS = {
-        "yes": "true()",
-        "Yes": "true()",
-        "YES": "true()",
-        "true": "true()",
-        "True": "true()",
-        "TRUE": "true()",
-        "no": "false()",
-        "No": "false()",
-        "NO": "false()",
-        "false": "false()",
-        "False": "false()",
-        "FALSE": "false()",
-    }
-
-    CONVERTIBLE_BIND_ATTRIBUTES = (
-        "readonly",
-        "required",
-        "relevant",
-        "constraint",
-        "calculate",
-    )
-
     # Supported media types for attaching to questions
     SUPPORTED_MEDIA = ("image", "big-image", "audio", "video")
 
     def validate(self):
         if not is_valid_xml_tag(self.name):
             invalid_char = re.search(INVALID_XFORM_TAG_REGEXP, self.name)
             raise PyXFormError(
-                f"The name '{self.name}' contains an invalid character '{invalid_char.group(0)}'. Names {constants.XML_IDENTIFIER_ERROR_MESSAGE}"
+                f"The name '{self.name}' contains an invalid character '{invalid_char.group(0)}'. Names {const.XML_IDENTIFIER_ERROR_MESSAGE}"
             )
 
     # TODO: Make sure renaming this doesn't cause any problems
     def iter_descendants(self):
         """
         A survey_element is a dictionary of survey_elements
         This method does a preorder traversal over them.
         For the time being this survery_element is included among its
         descendants
         """
         # it really seems like this method should not yield self
         yield self
         for e in self.children:
-            for f in e.iter_descendants():
-                yield f
+            yield from e.iter_descendants()
 
-    @lru_cache(maxsize=None)
-    def any_repeat(self, parent_xpath):
+    def any_repeat(self, parent_xpath: str) -> bool:
         """Return True if there ia any repeat in `parent_xpath`."""
-        for item in self.iter_descendants():
-            if item.get_xpath() == parent_xpath and item.type == constants.REPEAT:
-                return True
-
-        return False
+        return any_repeat(survey_element=self, parent_xpath=parent_xpath)
 
     def get_lineage(self):
         """
         Return a the list [root, ..., self._parent, self]
         """
         result = deque((self,))
         current_element = self
@@ -278,17 +255,17 @@
 
     def get_translations(self, default_language):
         """
         Returns translations used by this element so they can be included in
         the <itext> block. @see survey._setup_translations
         """
         bind_dict = self.get("bind")
-        if bind_dict and type(bind_dict) is dict:
+        if bind_dict and isinstance(bind_dict, dict):
             constraint_msg = bind_dict.get("jr:constraintMsg")
-            if type(constraint_msg) is dict:
+            if isinstance(constraint_msg, dict):
                 for lang, text in constraint_msg.items():
                     yield {
                         "path": self._translation_path("jr:constraintMsg"),
                         "lang": lang,
                         "text": text,
                         "output_context": self,
                     }
@@ -297,15 +274,15 @@
                     "path": self._translation_path("jr:constraintMsg"),
                     "lang": default_language,
                     "text": constraint_msg,
                     "output_context": self,
                 }
 
             required_msg = bind_dict.get("jr:requiredMsg")
-            if type(required_msg) is dict:
+            if isinstance(required_msg, dict):
                 for lang, text in required_msg.items():
                     yield {
                         "path": self._translation_path("jr:requiredMsg"),
                         "lang": lang,
                         "text": text,
                         "output_context": self,
                     }
@@ -313,30 +290,30 @@
                 yield {
                     "path": self._translation_path("jr:requiredMsg"),
                     "lang": default_language,
                     "text": required_msg,
                     "output_context": self,
                 }
             no_app_error_string = bind_dict.get("jr:noAppErrorString")
-            if type(no_app_error_string) is dict:
+            if isinstance(no_app_error_string, dict):
                 for lang, text in no_app_error_string.items():
                     yield {
                         "path": self._translation_path("jr:noAppErrorString"),
                         "lang": lang,
                         "text": text,
                         "output_context": self,
                     }
 
         for display_element in ["label", "hint", "guidance_hint"]:
             label_or_hint = self[display_element]
 
             if (
                 display_element == "label"
                 and self.needs_itext_ref()
-                and type(label_or_hint) is not dict
+                and not isinstance(label_or_hint, dict)
                 and label_or_hint
             ):
                 label_or_hint = {default_language: label_or_hint}
 
             # always use itext for guidance hints because that's
             # how they're defined - https://opendatakit.github.io/xforms-spec/#languages
             if (
@@ -352,15 +329,15 @@
                 and not isinstance(label_or_hint, dict)
                 and len(label_or_hint) > 0
                 and "guidance_hint" in self.keys()
                 and len(self["guidance_hint"]) > 0
             ):
                 label_or_hint = {default_language: label_or_hint}
 
-            if type(label_or_hint) is dict:
+            if isinstance(label_or_hint, dict):
                 for lang, text in label_or_hint.items():
                     yield {
                         "display_element": display_element,  # Not used
                         "path": self._translation_path(display_element),
                         "element": self,  # Not used
                         "output_context": self,
                         "lang": lang,
@@ -371,16 +348,16 @@
         """
         @deprected
         I'm leaving this in just in case it has outside references.
         """
         return {"media": "%s:media" % self.get_xpath()}
 
     def needs_itext_ref(self):
-        return type(self.label) is dict or (
-            type(self.media) is dict and len(self.media) > 0
+        return isinstance(self.label, dict) or (
+            isinstance(self.media, dict) and len(self.media) > 0
         )
 
     def get_setvalue_node_for_dynamic_default(self, in_repeat=False):
         if not self.default or not default_is_dynamic(self.default, self.type):
             return None
 
         default_with_xpath_paths = self.get_root().insert_xpaths(self.default, self)
@@ -412,15 +389,15 @@
         if isinstance(self.hint, dict) or self.guidance_hint:
             path = self._translation_path("hint")
             return node("hint", ref="jr:itext('%s')" % path)
         else:
             hint, output_inserted = self.get_root().insert_output_values(self.hint, self)
             return node("hint", hint, toParseString=output_inserted)
 
-    def xml_label_and_hint(self) -> "List[DetachableElement]":
+    def xml_label_and_hint(self) -> List["DetachableElement"]:
         """
         Return a list containing one node for the label and if there
         is a hint one node for the hint.
         """
         result = []
         label_appended = False
         if self.label or self.media:
@@ -463,27 +440,27 @@
                 del bind_dict["calculate"]
 
             for k, v in bind_dict.items():
                 # I think all the binding conversions should be happening on
                 # the xls2json side.
                 if (
                     hashable(v)
-                    and v in self.BINDING_CONVERSIONS
-                    and k in self.CONVERTIBLE_BIND_ATTRIBUTES
+                    and v in alias.BINDING_CONVERSIONS
+                    and k in const.CONVERTIBLE_BIND_ATTRIBUTES
                 ):
-                    v = self.BINDING_CONVERSIONS[v]
+                    v = alias.BINDING_CONVERSIONS[v]
                 if k == "jr:constraintMsg" and (
-                    type(v) is dict or re.search(BRACKETED_TAG_REGEX, v)
+                    isinstance(v, dict) or re.search(BRACKETED_TAG_REGEX, v)
                 ):
                     v = "jr:itext('%s')" % self._translation_path("jr:constraintMsg")
                 if k == "jr:requiredMsg" and (
-                    type(v) is dict or re.search(BRACKETED_TAG_REGEX, v)
+                    isinstance(v, dict) or re.search(BRACKETED_TAG_REGEX, v)
                 ):
                     v = "jr:itext('%s')" % self._translation_path("jr:requiredMsg")
-                if k == "jr:noAppErrorString" and type(v) is dict:
+                if k == "jr:noAppErrorString" and isinstance(v, dict):
                     v = "jr:itext('%s')" % self._translation_path("jr:noAppErrorString")
                 bind_dict[k] = survey.insert_xpaths(v, context=self)
             return [node("bind", nodeset=self.get_xpath(), **bind_dict)]
         return None
 
     def xml_descendent_bindings(self):
         """
```

### Comparing `pyxform-2.0.2/pyxform/translator.py` & `pyxform-2.0.3/pyxform/translator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Translator class module.
 """
 from collections import defaultdict
 
 
 def infinite_dict():
```

### Comparing `pyxform-2.0.2/pyxform/util/enum.py` & `pyxform-2.0.3/pyxform/util/enum.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     """Base Enum class with common helper function."""
 
     # Copied from Python 3.11 enum.py. In many cases can use members as strings, but
     # sometimes need to deref with ".value" property e.g. `EnumClass.MEMBERNAME.value`.
     def __new__(cls, *values):
         "values must already be of type `str`"
         if len(values) > 3:
-            raise TypeError("too many arguments for str(): %r" % (values,))
+            raise TypeError(f"too many arguments for str(): {values!r}")
         if len(values) == 1:
             # it must be a string
             if not isinstance(values[0], str):
-                raise TypeError("%r is not a string" % (values[0],))
+                raise TypeError(f"{values[0]!r} is not a string")
         if len(values) >= 2:
             # check that encoding argument is a string
             if not isinstance(values[1], str):
-                raise TypeError("encoding must be a string, not %r" % (values[1],))
+                raise TypeError(f"encoding must be a string, not {values[1]!r}")
         if len(values) == 3:
             # check that errors argument is a string
             if not isinstance(values[2], str):
-                raise TypeError("errors must be a string, not %r" % (values[2]))
+                raise TypeError(f"errors must be a string, not {values[2]!r}")
         value = str(*values)
         member = str.__new__(cls, value)
         member._value_ = value
         return member
 
     @classmethod
     def value_list(cls):
```

### Comparing `pyxform-2.0.2/pyxform/utils.py` & `pyxform-2.0.3/pyxform/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-# -*- coding: utf-8 -*-
 """
 pyxform utils module.
 """
-import codecs
 import copy
 import csv
 import json
 import os
 import re
-from collections import namedtuple
 from json.decoder import JSONDecodeError
-from typing import Dict, List, Tuple
-from xml.dom.minidom import Element, Text, parseString
+from typing import Dict, List, NamedTuple, Tuple
+from xml.dom import Node
+from xml.dom.minidom import Element, Text, _write_data
 
 import openpyxl
 import xlrd
+from defusedxml.minidom import parseString
 
+from pyxform.errors import PyXFormError
 from pyxform.xls2json_backends import is_empty, xls_value_to_unicode, xlsx_value_to_str
 
 SEP = "_"
 
 INVALID_XFORM_TAG_REGEXP = r"[^a-zA-Z:_][^a-zA-Z:_0-9\-.]*"
 
 LAST_SAVED_INSTANCE_NAME = "__last-saved"
 BRACKETED_TAG_REGEX = re.compile(r"\${(last-saved#)?(.*?)}")
 LAST_SAVED_REGEX = re.compile(r"\${last-saved#(.*?)}")
 PYXFORM_REFERENCE_REGEX = re.compile(r"\$\{(.*?)\}")
-
-
-NSMAP = {
-    "xmlns": "http://www.w3.org/2002/xforms",
-    "xmlns:h": "http://www.w3.org/1999/xhtml",
-    "xmlns:ev": "http://www.w3.org/2001/xml-events",
-    "xmlns:xsd": "http://www.w3.org/2001/XMLSchema",
-    "xmlns:jr": "http://openrosa.org/javarosa",
-    "xmlns:orx": "http://openrosa.org/xforms",
-    "xmlns:odk": "http://www.opendatakit.org/xforms",
-}
+NODE_TYPE_TEXT = (Node.TEXT_NODE, Node.CDATA_SECTION_NODE)
 
 
 class DetachableElement(Element):
     """
     Element classes are not meant to be instantiated directly.   This
     restriction was not strictly enforced in Python 2, but is effectively
     enforced in Python 3 via http://bugs.python.org/issue15290.
@@ -50,19 +40,52 @@
     document.createElement rather than Element.
     """
 
     def __init__(self, *args, **kwargs):
         Element.__init__(self, *args, **kwargs)
         self.ownerDocument = None
 
+    def writexml(self, writer, indent="", addindent="", newl=""):
+        # indent = current indentation
+        # addindent = indentation to add to higher levels
+        # newl = newline string
+        writer.write(indent + "<" + self.tagName)
+
+        attrs = self._get_attributes()
+
+        for a_name in attrs.keys():
+            writer.write(' %s="' % a_name)
+            _write_data(writer, attrs[a_name].value)
+            writer.write('"')
+        if self.childNodes:
+            writer.write(">")
+            # For text or mixed content, write without adding indents or newlines.
+            if 0 < len([c for c in self.childNodes if c.nodeType in NODE_TYPE_TEXT]):
+                # Conditions to match old Survey.py regex for remaining whitespace.
+                child_nodes = len(self.childNodes)
+                for idx, cnode in enumerate(self.childNodes):
+                    if 1 < child_nodes and idx == 0 and cnode.nodeType in NODE_TYPE_TEXT:
+                        writer.write(" ")
+                    cnode.writexml(writer, "", "", "")
+                    if 1 < child_nodes and (idx + 1) == child_nodes:
+                        writer.write(" ")
+            else:
+                writer.write(newl)
+                for cnode in self.childNodes:
+                    cnode.writexml(writer, indent + addindent, addindent, newl)
+                writer.write(indent)
+            writer.write(f"</{self.tagName}>{newl}")
+        else:
+            writer.write(f"/>{newl}")
+
 
 class PatchedText(Text):
     def writexml(self, writer, indent="", addindent="", newl=""):
         """Same as original but no replacing double quotes with '&quot;'."""
-        data = "%s%s%s" % (indent, self.data, newl)
+        data = "".join((indent, self.data, newl))
         if data:
             data = data.replace("&", "&amp;").replace("<", "&lt;").replace(">", "&gt;")
         writer.write(data)
 
 
 def node(*args, **kwargs) -> DetachableElement:
     """
@@ -72,16 +95,17 @@
     kwargs -- attributes
     returns a xml.dom.minidom.Element
     """
     blocked_attributes = ["tag"]
     tag = args[0] if len(args) > 0 else kwargs["tag"]
     args = args[1:]
     result = DetachableElement(tag)
-    unicode_args = [u for u in args if type(u) == str]
-    assert len(unicode_args) <= 1
+    unicode_args = [u for u in args if isinstance(u, str)]
+    if len(unicode_args) > 1:
+        raise PyXFormError("""Invalid value for `unicode_args`.""")
     parsed_string = False
 
     # Convert the kwargs xml attribute dictionary to a xml.dom.minidom.Element.
     for k, v in iter(kwargs.items()):
         if k in blocked_attributes:
             continue
         if k == "toParseString":
@@ -108,43 +132,42 @@
             result.setAttribute(k, v)
 
     if len(unicode_args) == 1 and not parsed_string:
         text_node = PatchedText()
         text_node.data = unicode_args[0]
         result.appendChild(text_node)
     for n in args:
-        if type(n) == int or type(n) == float or type(n) == bytes:
+        if isinstance(n, (int, float, bytes)):
             text_node = PatchedText()
             text_node.data = str(n)
             result.appendChild(text_node)
-        elif type(n) is not str:
+        elif not isinstance(n, str):
             result.appendChild(n)
     return result
 
 
 def get_pyobj_from_json(str_or_path):
     """
     This function takes either a json string or a path to a json file,
     it loads the json into memory and returns the corresponding Python
     object.
     """
     try:
         # see if treating str_or_path as a path works
-        fp = codecs.open(str_or_path, mode="r", encoding="utf-8")
-        doc = json.load(fp)
-    except (IOError, JSONDecodeError, OSError):
+        with open(str_or_path, encoding="utf-8") as fp:
+            doc = json.load(fp)
+    except (JSONDecodeError, OSError):
         # if it doesn't work load the text
         doc = json.loads(str_or_path)
     return doc
 
 
 def flatten(li):
     for subli in li:
-        for it in subli:
-            yield it
+        yield from subli
 
 
 def sheet_to_csv(workbook_path, csv_path, sheet_name):
     if workbook_path.endswith(".xls"):
         return xls_sheet_to_csv(workbook_path, csv_path, sheet_name)
     else:
         return xlsx_sheet_to_csv(workbook_path, csv_path, sheet_name)
@@ -154,15 +177,15 @@
     wb = xlrd.open_workbook(workbook_path)
     try:
         sheet = wb.sheet_by_name(sheet_name)
     except xlrd.biffh.XLRDError:
         return False
     if not sheet or sheet.nrows < 2:
         return False
-    with open(csv_path, "w", newline="") as f:
+    with open(csv_path, mode="w", encoding="utf-8", newline="") as f:
         writer = csv.writer(f, quoting=csv.QUOTE_ALL)
         mask = [v and len(v.strip()) > 0 for v in sheet.row_values(0)]
         for row_idx in range(sheet.nrows):
             csv_data = []
             try:
                 for v, m in zip(sheet.row(row_idx), mask):
                     if m:
@@ -182,15 +205,15 @@
 def xlsx_sheet_to_csv(workbook_path, csv_path, sheet_name):
     wb = openpyxl.open(workbook_path, read_only=True, data_only=True)
     try:
         sheet = wb[sheet_name]
     except KeyError:
         return False
 
-    with open(csv_path, "w", newline="") as f:
+    with open(csv_path, mode="w", encoding="utf-8", newline="") as f:
         writer = csv.writer(f, quoting=csv.QUOTE_ALL)
         mask = [not is_empty(cell.value) for cell in sheet[1]]
         for row in sheet.rows:
             csv_data = []
             try:
                 for v, m in zip(row, mask):
                     if m:
@@ -222,25 +245,26 @@
     return False
 
 
 def get_languages_with_bad_tags(languages):
     """
     Returns languages with invalid or missing IANA subtags.
     """
-    with open(os.path.join(os.path.dirname(__file__), "iana_subtags.txt")) as f:
+    path = os.path.join(os.path.dirname(__file__), "iana_subtags.txt")
+    with open(path, encoding="utf-8") as f:
         iana_subtags = f.read().splitlines()
 
     lang_code_regex = re.compile(r"\((.*)\)$")
 
     languages_with_bad_tags = []
     for lang in languages:
         lang_code = re.search(lang_code_regex, lang)
 
         if lang != "default" and (
-            not lang_code or not lang_code.group(1) in iana_subtags
+            not lang_code or lang_code.group(1) not in iana_subtags
         ):
             languages_with_bad_tags.append(lang)
     return languages_with_bad_tags
 
 
 def default_is_dynamic(element_default, element_type=None):
     """
@@ -303,30 +327,30 @@
     :param b: The second string to compare.
     :return:
     """
     m = len(a)
     n = len(b)
 
     # create two work vectors of integer distances
-    v1 = [0 for _ in range(0, n + 1)]
+    v1 = [0 for _ in range(n + 1)]
 
     # initialize v0 (the previous row of distances)
     # this row is A[0][i]: edit distance for an empty s
     # the distance is just the number of characters to delete from t
-    v0 = [i for i in range(0, n + 1)]
+    v0 = list(range(n + 1))
 
-    for i in range(0, m):
+    for i in range(m):
         # calculate v1 (current row distances) from the previous row v0
 
         # first element of v1 is A[i+1][0]
         #   edit distance is delete (i+1) chars from s to match empty t
         v1[0] = i + 1
 
         # use formula to fill in the rest of the row
-        for j in range(0, n):
+        for j in range(n):
             # calculating costs for A[i+1][j+1]
             deletion_cost = v0[j + 1] + 1
             insertion_cost = v1[j] + 1
             if a[i] == b[j]:
                 substitution_cost = v0[j]
             else:
                 substitution_cost = v0[j] + 1
@@ -336,15 +360,15 @@
         # copy v1 (current row) to v0 (previous row) for next iteration
         # since data in v1 is always invalidated, a swap without copy could be more efficient
         v0 = copy.copy(v1)
     # after the last swap, the results of v1 are now in v0
     return v0[n]
 
 
-def get_expression_lexer() -> re.Scanner:  # noqa
+def get_expression_lexer() -> re.Scanner:
     """
     Get a expression lexer (scanner) for parsing.
     """
     # ncname regex adapted from eulxml https://github.com/emory-libraries/eulxml/blob/2e1a9f71ffd1fd455bd8326ec82125e333b352e0/eulxml/xpath/lexrules.py
     # (C) 2010,2011 Emory University Libraries [Apache v2.0 License]
     # They in turn adapted it from https://www.w3.org/TR/REC-xml/#NT-NameStartChar
     # and https://www.w3.org/TR/REC-xml-names/#NT-NCName
@@ -400,19 +424,25 @@
             return ExpLexerToken(name, value, scan.match.start(), scan.match.end())
 
         return tokenizer
 
     lexicon = [(v, get_tokenizer(k)) for k, v in lexer_rules.items()]
     # re.Scanner is undocumented but has been around since at least 2003
     # https://mail.python.org/pipermail/python-dev/2003-April/035075.html
-    return re.Scanner(lexicon)  # noqa
+    return re.Scanner(lexicon)
 
 
 # Scanner takes a few 100ms to compile so use this shared instance.
-ExpLexerToken = namedtuple("ExpLexerToken", ["name", "value", "start", "end"])
+class ExpLexerToken(NamedTuple):
+    name: str
+    value: str
+    start: int
+    end: int
+
+
 EXPRESSION_LEXER = get_expression_lexer()
 
 
 def parse_expression(text: str) -> Tuple[List[ExpLexerToken], str]:
     """
     Parse a "default" expression, well enough to identify dynamic defaults vs. not.
```

### Comparing `pyxform-2.0.2/pyxform/validators/enketo_validate/__init__.py` & `pyxform-2.0.3/pyxform/validators/enketo_validate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 Validate XForms using Enketo validator.
 """
 import os
 from typing import TYPE_CHECKING
 
 from pyxform.validators.error_cleaner import ErrorCleaner
@@ -20,16 +19,14 @@
 CURRENT_DIRECTORY = os.path.dirname(os.path.realpath(__file__))
 ENKETO_VALIDATE_PATH = os.path.join(CURRENT_DIRECTORY, "bin", "validate")
 
 
 class EnketoValidateError(Exception):
     """Common base class for Enketo validate exceptions."""
 
-    pass
-
 
 def install_exists():
     """
     Check if Enketo-validate is installed.
     """
     return os.path.exists(ENKETO_VALIDATE_PATH)
 
@@ -59,30 +56,29 @@
     - return code 1: raise error with the stderr content.
     - return code 0: append warning with the stdout content (possibly none).
 
     :param path_to_xform: Path to the XForm to be validated.
     :return: warnings or List[str]
     """
     if not install_exists():
-        raise EnvironmentError(
+        raise OSError(
             "Enketo-validate dependency not found. "
             "Please use the updater tool to install the latest version."
         )
 
     returncode, timeout, stdout, stderr = _call_validator(path_to_xform=path_to_xform)
     warnings = []
     stderr = decode_stream(stderr)
     stdout = decode_stream(stdout)
 
     if timeout:
         return ["XForm took to long to completely validate."]
-    else:
-        if returncode > 0:  # Error invalid
-            raise EnketoValidateError(
-                "Enketo Validate Errors:\n" + ErrorCleaner.enketo_validate(stderr)
-            )
-        elif returncode == 0:
-            if stdout:
-                warnings.append("Enketo Validate Warnings:\n" + stdout)
-            return warnings
-        elif returncode < 0:
-            return ["Bad return code from Enketo Validate."]
+    elif returncode > 0:  # Error invalid
+        raise EnketoValidateError(
+            "Enketo Validate Errors:\n" + ErrorCleaner.enketo_validate(stderr)
+        )
+    elif returncode == 0:
+        if stdout:
+            warnings.append("Enketo Validate Warnings:\n" + stdout)
+        return warnings
+    elif returncode < 0:
+        return ["Bad return code from Enketo Validate."]
```

### Comparing `pyxform-2.0.2/pyxform/validators/error_cleaner.py` & `pyxform-2.0.3/pyxform/validators/error_cleaner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
 """
 Cleans up error messages from the validators.
 """
 import re
 
 
 class ErrorCleaner:
     """Cleans up raw error messages from XForm validators for end users."""
 
     @staticmethod
     def _replace_xpath_with_tokens(match):
         strmatch = match.group()
         # eliminate e.g /html/body/select1[@ref=/id_string/elId]/item/value
         # instance('q4')/root/item[...]
-        if (
-            strmatch.startswith("/html/body")
-            or strmatch.startswith("/root/item")
-            or strmatch.startswith("/html/head/model/bind")
-            or strmatch.endswith("/item/value")
-        ):
+        if strmatch.startswith(
+            (("/html/body"), ("/root/item"), ("/html/head/model/bind"))
+        ) or strmatch.endswith("/item/value"):
             return strmatch
         line = match.group().split("/")
         return "${%s}" % line[len(line) - 1]
 
     @staticmethod
     def _cleanup_errors(error_message):
         pattern = r"(/[a-z0-9\-_]+(?:/[a-z0-9\-_]+)+)"
```

### Comparing `pyxform-2.0.2/pyxform/validators/odk_validate/__init__.py` & `pyxform-2.0.3/pyxform/validators/odk_validate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 odk_validate.py
 A python wrapper around ODK Validate
 """
 import logging
 import os
 import shutil
@@ -23,16 +22,14 @@
 CURRENT_DIRECTORY = os.path.dirname(os.path.realpath(__file__))
 ODK_VALIDATE_PATH = os.path.join(CURRENT_DIRECTORY, "bin", "ODK_Validate.jar")
 
 
 class ODKValidateError(Exception):
     """ODK Validation exception error."""
 
-    pass
-
 
 def install_exists():
     """Returns True if ODK_VALIDATE_PATH exists."""
     return os.path.exists(ODK_VALIDATE_PATH)
 
 
 def _call_validator(path_to_xform, bin_file_path=ODK_VALIDATE_PATH) -> "PopenResult":
@@ -64,15 +61,15 @@
     if java_path is not None:
         return
     msg = (
         "Form validation failed because Java (8+ required) could not be found. "
         "To fix this, please either: 1) install Java, or 2) run pyxform with the "
         "--skip_validate flag, or 3) add the installed Java to the environment path."
     )
-    raise EnvironmentError(msg)
+    raise OSError(msg)
 
 
 def check_xform(path_to_xform):
     """Run ODK Validate against the XForm in `path_to_xform`.
 
     Returns an array of warnings if the form is valid.
     Throws an exception if it is not
@@ -88,24 +85,23 @@
     # stderr is treated as a warning if the form is valid or an error
     # if it is invalid.
     result = _call_validator(path_to_xform=path_to_xform)
     warnings = []
 
     if result.timeout:
         return ["XForm took to long to completely validate."]
-    else:
-        if result.return_code > 0:  # Error invalid
-            raise ODKValidateError(
-                "ODK Validate Errors:\n" + ErrorCleaner.odk_validate(result.stderr)
-            )
-        elif result.return_code == 0:
-            if result.stderr:
-                warnings.append("ODK Validate Warnings:\n" + result.stderr)
-        elif result.return_code < 0:
-            return ["Bad return code from ODK Validate."]
+    elif result.return_code > 0:  # Error invalid
+        raise ODKValidateError(
+            "ODK Validate Errors:\n" + ErrorCleaner.odk_validate(result.stderr)
+        )
+    elif result.return_code == 0:
+        if result.stderr:
+            warnings.append("ODK Validate Warnings:\n" + result.stderr)
+    elif result.return_code < 0:
+        return ["Bad return code from ODK Validate."]
 
     return warnings
 
 
 if __name__ == "__main__":
     logger = logging.getLogger(__name__)
     logger.addHandler(logging.StreamHandler())
```

### Comparing `pyxform-2.0.2/pyxform/validators/odk_validate/bin/ODK_Validate.jar` & `pyxform-2.0.3/pyxform/validators/odk_validate/bin/ODK_Validate.jar`

 * *Files identical despite different names*

### Comparing `pyxform-2.0.2/pyxform/validators/odk_validate/bin/installed.json` & `pyxform-2.0.3/pyxform/validators/odk_validate/bin/installed.json`

 * *Files identical despite different names*

### Comparing `pyxform-2.0.2/pyxform/validators/pyxform/android_package_name.py` & `pyxform-2.0.3/pyxform/validators/pyxform/android_package_name.py`

 * *Files identical despite different names*

### Comparing `pyxform-2.0.2/pyxform/validators/pyxform/parameters_generic.py` & `pyxform-2.0.3/pyxform/validators/pyxform/parameters_generic.py`

 * *Files identical despite different names*

### Comparing `pyxform-2.0.2/pyxform/validators/pyxform/select_from_file.py` & `pyxform-2.0.3/pyxform/validators/pyxform/select_from_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,24 @@
     :param name: The name of the parameter value.
     :param value: The parameter value to validate.
     :param row_number: The survey sheet row number.
     """
     if not value_or_label_test(value=value):
         msg = value_or_label_format_msg(name=name, row_number=row_number)
         raise PyXFormError(msg)
-    return None
 
 
 def validate_list_name_extension(
     select_command: str, list_name: str, row_number: int
 ) -> None:
     """For select_from_file types, the list_name should end with a supported extension."""
     list_path = Path(list_name)
     if select_command in aliases.select_from_file and (
         1 != len(list_path.suffixes)
         or list_path.suffix not in EXTERNAL_INSTANCE_EXTENSIONS
     ):
-        exts = ", ".join((f"'{e}'" for e in EXTERNAL_INSTANCE_EXTENSIONS))
+        exts = ", ".join(f"'{e}'" for e in EXTERNAL_INSTANCE_EXTENSIONS)
         raise PyXFormError(
             ROW_FORMAT_STRING % row_number
             + f" File name for '{select_command} {list_name}' should end with one of "
             + f"the supported file extensions: {exts}"
         )
```

### Comparing `pyxform-2.0.2/pyxform/validators/pyxform/translations_checks.py` & `pyxform-2.0.3/pyxform/validators/pyxform/translations_checks.py`

 * *Files identical despite different names*

### Comparing `pyxform-2.0.2/pyxform/validators/updater.py` & `pyxform-2.0.3/pyxform/validators/updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# -*- coding: utf-8 -*-
 """
 pyxform_validator_update - command to update XForm validators.
 """
 import argparse
 import fnmatch
-import io
 import json
 import logging
 import os
 import shutil
 import sys
 from datetime import datetime
 from stat import S_IXGRP, S_IXUSR
@@ -60,15 +58,15 @@
         self.latest_path = os.path.join(self.mod_path, "latest.json")
         self.last_check_path = os.path.join(self.mod_path, ".last_check")
 
         self.bin_path = os.path.join(self.mod_path, "bin")
         self.installed_path = os.path.join(self.bin_path, "installed.json")
         self.bin_new_path = os.path.join(self.mod_path, "bin_new")
 
-        self.manual_msg = "Download manually from: {r}.".format(r=self.repo_url)
+        self.manual_msg = f"Download manually from: {self.repo_url}."
 
 
 class _UpdateHandler:
     """
     Handles tasks related to updating external XForm validators.
 
     Where possible, minimise calls to the GitHub API because doing so without an
@@ -84,57 +82,57 @@
         """
         content = request_get(url=url)
         return json.loads(content.decode("utf-8"))
 
     @staticmethod
     def _check_path(file_path):
         if not os.path.exists(file_path):
-            raise PyXFormError("Expected path does not exist: {p}" "".format(p=file_path))
+            raise PyXFormError(f"Expected path does not exist: {file_path}" "")
         else:
             return True
 
     @staticmethod
     def _read_json(file_path):
         """
         Read the JSON file to a string.
         """
         _UpdateHandler._check_path(file_path=file_path)
-        with io.open(file_path, mode="r") as in_file:
+        with open(file_path, encoding="utf-8") as in_file:
             return json.load(in_file)
 
     @staticmethod
     def _write_json(file_path, content):
         """
         Save the JSON data to a file.
         """
-        with io.open(file_path, mode="w", newline="\n") as out_file:
+        with open(file_path, mode="w", encoding="utf-8", newline="\n") as out_file:
             data = json.dumps(content, indent=2, sort_keys=True)
             out_file.write(str(data))
 
     @staticmethod
     def _read_last_check(file_path):
         """
         Read the .last_check file.
         """
         _UpdateHandler._check_path(file_path=file_path)
-        with io.open(file_path, mode="r") as in_file:
+        with open(file_path, encoding="utf-8") as in_file:
             first_line = in_file.readline()
         try:
             last_check = datetime.strptime(first_line, UTC_FMT)
         except ValueError:
             return None
         else:
             return last_check
 
     @staticmethod
     def _write_last_check(file_path, content):
         """
         Write the .last_check file.
         """
-        with io.open(file_path, mode="w", newline="\n") as out_file:
+        with open(file_path, mode="w", encoding="utf-8", newline="\n") as out_file:
             out_file.write(str(content.strftime(UTC_FMT)))
 
     @staticmethod
     def _check_necessary(update_info, utc_now):
         """
         Determine whether a check for the latest version is necessary.
         """
@@ -169,15 +167,15 @@
             )
         else:
             latest = _UpdateHandler._read_json(file_path=update_info.latest_path)
         return latest
 
     @staticmethod
     def _get_release_message(json_data):
-        template = "- Tag name = {tag_name}\n" "- Tag URL = {tag_url}\n\n"
+        template = "- Tag name = {tag_name}\n- Tag URL = {tag_url}\n\n"
         return template.format(
             tag_name=json_data["tag_name"], tag_url=json_data["html_url"]
         )
 
     @staticmethod
     def list(update_info):
         """
@@ -190,15 +188,15 @@
         else:
             installed = _UpdateHandler._read_json(file_path=update_info.installed_path)
             installed_info = _UpdateHandler._get_release_message(json_data=installed)
 
         latest = _UpdateHandler._get_latest(update_info=update_info)
         latest_files = latest["assets"]
         if len(latest_files) == 0:
-            file_message = "- None!\n\n{m}".format(m=update_info.manual_msg)
+            file_message = f"- None!\n\n{update_info.manual_msg}"
         else:
             file_names = ["- {n}".format(n=x["name"]) for x in latest_files]
             file_message = "\n".join(file_names)
 
         template = (
             "\nInstalled release:\n\n{installed}"
             "Latest release:\n\n{latest}"
@@ -217,25 +215,24 @@
         Find the download URL for the file in the GitHub API JSON response doc.
         """
         rel_name = json_data["tag_name"]
         files = json_data["assets"]
 
         if len(files) == 0:
             raise PyXFormError(
-                "No files attached to release '{r}'.\n\n{h}"
-                "".format(r=rel_name, h=update_info.manual_msg)
+                f"No files attached to release '{rel_name}'.\n\n{update_info.manual_msg}"
             )
 
         file_urls = [x["browser_download_url"] for x in files if x["name"] == file_name]
 
         urls_len = len(file_urls)
         if 0 == urls_len:
             raise PyXFormError(
-                "No files with the name '{n}' attached to release '{r}'."
-                "\n\n{h}".format(n=file_name, r=rel_name, h=update_info.manual_msg)
+                f"No files with the name '{file_name}' attached to release '{rel_name}'."
+                f"\n\n{update_info.manual_msg}"
             )
         elif 1 < urls_len:
             raise PyXFormError(
                 "{c} files with the name '{n}' attached to release '{r}'."
                 "\n\n{h}".format(
                     c=urls_len, n=file_name, r=rel_name, h=update_info.manual_msg
                 )
@@ -244,15 +241,15 @@
             return file_urls[0]
 
     @staticmethod
     def _download_file(url, file_path):
         """
         Save response content from the URL to a binary file at the file path.
         """
-        with io.open(file_path, mode="wb") as out_file:
+        with open(file_path, mode="wb") as out_file:
             file_data = request_get(url=url)
             out_file.write(file_data)
 
     @staticmethod
     def _get_bin_paths(update_info, file_path):
         """
         Get the mapping of zip file paths to extract paths for the file_name.
@@ -266,16 +263,17 @@
             main_bin = "*validate.exe"
         elif "linux" in file_base:
             main_bin = "*validate"
         elif "macos" in file_base:
             main_bin = "*validate"
         else:
             raise PyXFormError(
-                "Did not find a supported main binary for file: {p}.\n\n{h}"
-                "".format(p=file_path, h=update_info.manual_msg)
+                "Did not find a supported main binary for file: {p}.\n\n{h}".format(
+                    p=file_path, h=update_info.manual_msg
+                )
             )
         return [
             (main_bin, update_info.validator_basename),
             (
                 "*node_modules/libxmljs-mt/build*/xmljs.node",
                 "node_modules/libxmljs-mt/build/xmljs.node",
             ),
@@ -305,16 +303,15 @@
                     maybe_existing_match = zip_jobs.get(file_out_path, None)
                     if maybe_existing_match is not None:
                         if maybe_existing_match.CRC == zip_item.CRC:
                             continue
                     zip_jobs[file_out_path] = zip_item
         if len(bin_paths) != len(zip_jobs.keys()):
             raise PyXFormError(
-                "Expected {e} zip job files, found: {c}"
-                "".format(e=len(bin_paths), c=len(zip_jobs.keys()))
+                f"Expected {len(bin_paths)} zip job files, found: {len(zip_jobs.keys())}"
             )
         return zip_jobs
 
     @staticmethod
     def _unzip_extract_file(open_zip_file, zip_item, file_out_path):
         """
         Extract the content for item in zip file to a specific location.
@@ -324,15 +321,15 @@
         works by reading all the files in the archive, doing the same thing.
         """
         out_parent = os.path.dirname(file_out_path)
         if not os.path.exists(out_parent):
             os.makedirs(out_parent)
         with open_zip_file.open(zip_item, mode="r") as zip_item_file:
             zip_item_data = zip_item_file.read()
-            with io.open(file_out_path, "wb") as file_out_file:
+            with open(file_out_path, "wb") as file_out_file:
                 file_out_file.write(zip_item_data)
 
     @staticmethod
     def _unzip(update_info, file_path, out_path):
         """
         Unzip the contents of a zip file to an existing output path.
         """
@@ -385,16 +382,16 @@
             else:
                 os.rename(file_path, new_bin_file_path)
 
             # For macos / linux: chmod ug+x the new bin file. No-op on Windows.
             current_mode = os.stat(new_bin_file_path).st_mode
             os.chmod(new_bin_file_path, current_mode | S_IXUSR | S_IXGRP)
 
-        except PyXFormError as e:
-            raise PyXFormError("\n\nUpdate failed!\n\n" + str(e))
+        except PyXFormError as px_err:
+            raise PyXFormError("\n\nUpdate failed!\n\n" + str(px_err)) from px_err
         else:
             return latest
 
     @staticmethod
     def _replace_old_bin_path(update_info):
         if os.path.exists(update_info.bin_path):
             shutil.rmtree(update_info.bin_path)
@@ -493,15 +490,14 @@
             message = template.format(
                 installed=_UpdateHandler._get_release_message(json_data=installed)
             )
             raise PyXFormError(message)
 
 
 class _UpdateService:
-
     update_info = None
 
     def list(self):
         return _UpdateHandler.list(update_info=self.update_info)
 
     def update(self, file_name, force):
         return _UpdateHandler.update(
@@ -552,19 +548,18 @@
         if bin_file_path is None:
             return odk_validate.install_ok()
         else:
             return odk_validate.install_ok(bin_file_path=bin_file_path)
 
 
 def _build_validator_menu(main_subparser, validator_name, updater_instance):
-
     main = main_subparser.add_parser(
         validator_name.lower(),
-        description="{v} Sub-menu".format(v=validator_name),
-        help="For help, use '{v} -h'.".format(v=validator_name.lower()),
+        description=f"{validator_name} Sub-menu",
+        help=f"For help, use '{validator_name.lower()} -h'.",
     )
     subs = main.add_subparsers(metavar="<sub_command>")
 
     cmd_list = subs.add_parser(
         "list", help="List available files for the latest release."
     )
     cmd_list.set_defaults(command=updater_instance.list)
```

### Comparing `pyxform-2.0.2/pyxform/validators/util.py` & `pyxform-2.0.3/pyxform/validators/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# -*- coding: utf-8 -*-
 """
 The validators utility functions.
 """
-import collections
-import io
 import logging
 import os
 import signal
 import subprocess
 import tempfile
 import threading
 import time
 from contextlib import closing
 from subprocess import PIPE, Popen
+from typing import Dict, List, NamedTuple
 from urllib.error import HTTPError, URLError
 from urllib.request import Request, urlopen
 
 from pyxform.errors import PyXFormError
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 XFORM_SPEC_PATH = os.path.join(HERE, "xlsform_spec_test.xml")
@@ -44,15 +42,14 @@
     """
     kill_check = threading.Event()
 
     def _kill_process_after_a_timeout(pid):
         os.kill(pid, signal.SIGTERM)
         kill_check.set()  # tell the main routine that we had to kill
         # use SIGKILL if hard to kill...
-        return
 
     startup_info = None
     env = None
     if os.name == "nt":
         # Workarounds for pyinstaller
         # https://github.com/pyinstaller/pyinstaller/wiki/Recipe-subprocess
         # disable command window when run from pyinstaller
@@ -97,40 +94,47 @@
     try:
         return stream.decode("utf-8")
     except UnicodeDecodeError as ude:
         try:
             return stream.decode("latin-1")
         except BaseException as be:
             msg = "Failed to decode validate stderr as utf-8 or latin-1."
-            raise IOError(msg, ude, be)
+            raise OSError(msg, ude, be) from be
 
 
 def request_get(url):
     """
     Get the response content from URL.
     """
     try:
+        if not url.startswith(("http:", "https:")):
+            raise ValueError("URL must start with 'http:' or 'https:'")
         r = Request(url)
         r.add_header("Accept", "application/json")
         with closing(urlopen(r)) as u:
             content = u.read()
         if len(content) == 0:
-            raise PyXFormError("Empty response from URL: '{u}'.".format(u=url))
+            raise PyXFormError(f"Empty response from URL: '{url}'.")
         else:
             return content
-    except HTTPError as e:
+    except HTTPError as http_err:
         raise PyXFormError(
-            "Unable to fulfill request. Error code: '{c}'. "
-            "Reason: '{r}'. URL: '{u}'."
-            "".format(r=e.reason, c=e.code, u=url)
-        )
-    except URLError as e:
+            f"Unable to fulfill request. Error code: '{http_err.code}'. "
+            f"Reason: '{http_err.reason}'. URL: '{url}'."
+            ""
+        ) from http_err
+    except URLError as url_err:
         raise PyXFormError(
-            "Unable to reach a server. Reason: {r}. " "URL: {u}".format(r=e.reason, u=url)
-        )
+            f"Unable to reach a server. Reason: {url_err.reason}. " f"URL: {url}"
+        ) from url_err
+
+
+class _LoggingWatcher(NamedTuple):
+    records: List
+    output: Dict
 
 
 class CapturingHandler(logging.Handler):
     """
     A logging handler capturing all (raw and formatted) logging output.
 
     Similar concept to "from unittest.case import _CapturingHandler". However
@@ -162,15 +166,14 @@
     def emit(self, record):
         self.watcher.records.append(record)
         msg = self.format(record)
         self.watcher.output[record.levelname].append(msg)
 
     @staticmethod
     def _get_watcher():
-        _LoggingWatcher = collections.namedtuple("_LoggingWatcher", ["records", "output"])
         levels = ["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"]
         return _LoggingWatcher([], {x: [] for x in levels})
 
     def reset(self):
         self.watcher = self._get_watcher()
 
 
@@ -186,20 +189,20 @@
     :param retry_limit: Number of attempts to read the file.
     :param wait_seconds: Amount of sleep time between read attempts.
     :return: True or raise IOError.
     """
 
     def catch_try():
         try:
-            with io.open(file_path, mode="r"):
+            with open(file_path):
                 return True
-        except IOError:
+        except OSError:
             return False
 
     tries = 0
     while not catch_try():
         if tries < retry_limit:
             tries += 1
             time.sleep(wait_seconds)
         else:
-            raise IOError("Could not read file: {f}".format(f=file_path))
+            raise OSError(f"Could not read file: {file_path}")
     return True
```

### Comparing `pyxform-2.0.2/pyxform/xform2json.py` & `pyxform-2.0.3/pyxform/xform2json.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,38 @@
-# -*- coding: utf-8 -*-
 """
 xform2json module - Transform an XForm to a JSON dictionary.
 """
-import codecs
 import copy
 import json
 import logging
 import re
-import xml.etree.ElementTree as ETree
-from collections import Mapping
+from collections.abc import Mapping
 from operator import itemgetter
 from typing import Any, Dict, List
+from xml.etree.ElementTree import Element
+
+from defusedxml.ElementTree import ParseError, XMLParser, fromstring, parse
 
 from pyxform import builder
+from pyxform.constants import NSMAP
 from pyxform.errors import PyXFormError
-from pyxform.utils import NSMAP
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
+QUESTION_TYPES = {
+    "select": "select all that apply",
+    "select1": "select one",
+    "int": "integer",
+    "dateTime": "datetime",
+    "string": "text",
+}
+
+
 # {{{ http://code.activestate.com/recipes/573463/ (r7)
 class XmlDictObject(dict):
     """
     Adds object like functionality to the standard dictionary.
     """
 
     def __init__(self, initdict=None):
@@ -55,15 +64,15 @@
             return [XmlDictObject.Wrap(v) for v in x]
         else:
             return x
 
     @staticmethod
     def _un_wrap(x):
         if isinstance(x, dict):
-            return dict((k, XmlDictObject._un_wrap(v)) for (k, v) in iter(x.items()))
+            return {k: XmlDictObject._un_wrap(v) for k, v in x.items()}
         elif isinstance(x, list):
             return [XmlDictObject._un_wrap(v) for v in x]
         else:
             return x
 
     def un_wrap(self):
         """
@@ -71,41 +80,42 @@
         and returns the result.
         """
 
         return XmlDictObject._un_wrap(self)
 
 
 def _convert_dict_to_xml_recurse(parent, dictitem):
-    assert not isinstance(dictitem, list)
+    if isinstance(dictitem, list):
+        raise PyXFormError("""Invalid value for `dictitem`.""")
 
     if isinstance(dictitem, dict):
-        for (tag, child) in iter(dictitem.items()):
+        for tag, child in iter(dictitem.items()):
             if str(tag) == "_text":
                 parent.text = str(child)
             elif isinstance(child, list):
                 # iterate through the array and convert
                 for listchild in child:
-                    elem = ETree.Element(tag)
+                    elem = Element(tag)
                     parent.append(elem)
                     _convert_dict_to_xml_recurse(elem, listchild)
             else:
-                elem = ETree.Element(tag)
+                elem = Element(tag)
                 parent.append(elem)
                 _convert_dict_to_xml_recurse(elem, child)
     else:
         parent.text = str(dictitem)
 
 
 def convert_dict_to_xml(xmldict):
     """
     Converts a dictionary to an XML ElementTree Element
     """
 
     roottag = xmldict.keys()[0]
-    root = ETree.Element(roottag)
+    root = Element(roottag)
     _convert_dict_to_xml_recurse(root, xmldict[roottag])
     return root
 
 
 def _convert_xml_to_dict_recurse(node, dictclass):
     nodedict = dictclass()
 
@@ -151,44 +161,44 @@
 def convert_xml_to_dict(root, dictclass=XmlDictObject):
     """
     Converts an XML file or ElementTree Element to a dictionary
     """
     # If a string is passed in, try to open it as a file
     if isinstance(root, str):
         root = _try_parse(root)
-    elif not isinstance(root, ETree.Element):
+    elif not isinstance(root, Element):
         raise TypeError("Expected ElementTree.Element or file path string")
 
     return dictclass({root.tag: _convert_xml_to_dict_recurse(root, dictclass)})
 
 
 # end of http://code.activestate.com/recipes/573463/ }}}
 
 
 def _try_parse(root, parser=None):
     """
     Try to parse the root from a string or a file/file-like object.
     """
     root = root.encode("UTF-8")
     try:
-        parsed_root = ETree.fromstring(root, parser)
-    except ETree.ParseError:
-        parsed_root = ETree.parse(root, parser=parser).getroot()
+        parsed_root = fromstring(root, parser)
+    except ParseError:
+        parsed_root = parse(root, parser=parser).getroot()
     return parsed_root
 
 
 class XFormToDict:
     def __init__(self, root):
         if isinstance(root, str):
-            parser = ETree.XMLParser(encoding="UTF-8")
+            parser = XMLParser(encoding="UTF-8")
             self._root = _try_parse(root, parser)
             self._dict = XmlDictObject(
                 {self._root.tag: _convert_xml_to_dict_recurse(self._root, XmlDictObject)}
             )
-        elif not isinstance(root, ETree.Element):
+        elif not isinstance(root, Element):
             raise TypeError("Expected ElementTree.Element or file path string")
 
     def get_dict(self):
         json_str = json.dumps(self._dict)
         for uri in NSMAP.values():
             json_str = json_str.replace("{%s}" % uri, "")
         return json.loads(json_str)
@@ -198,32 +208,30 @@
     sb = XFormToDictBuilder(xml_file)
     return sb.survey()
 
 
 class XFormToDictBuilder:
     """Experimental XFORM xml to XFORM JSON"""
 
-    QUESTION_TYPES = {
-        "select": "select all that apply",
-        "select1": "select one",
-        "int": "integer",
-        "dateTime": "datetime",
-        "string": "text",
-    }
-
     def __init__(self, xml_file):
         doc_as_dict = XFormToDict(xml_file).get_dict()
         self._xmldict = doc_as_dict
 
-        assert "html" in doc_as_dict
-        assert "body" in doc_as_dict["html"]
-        assert "head" in doc_as_dict["html"]
-        assert "model" in doc_as_dict["html"]["head"]
-        assert "title" in doc_as_dict["html"]["head"]
-        assert "bind" in doc_as_dict["html"]["head"]["model"]
+        if "html" not in doc_as_dict:
+            raise PyXFormError("""Invalid value for `doc_as_dict`.""")
+        if "body" not in doc_as_dict["html"]:
+            raise PyXFormError("""Invalid value for `doc_as_dict`.""")
+        if "head" not in doc_as_dict["html"]:
+            raise PyXFormError("""Invalid value for `doc_as_dict`.""")
+        if "model" not in doc_as_dict["html"]["head"]:
+            raise PyXFormError("""Invalid value for `doc_as_dict`.""")
+        if "title" not in doc_as_dict["html"]["head"]:
+            raise PyXFormError("""Invalid value for `doc_as_dict`.""")
+        if "bind" not in doc_as_dict["html"]["head"]["model"]:
+            raise PyXFormError("""Invalid value for `doc_as_dict`.""")
 
         self.body = doc_as_dict["html"]["body"]
         self.model = doc_as_dict["html"]["head"]["model"]
         self.bindings = copy.deepcopy(self.model["bind"])
         self._bind_list = copy.deepcopy(self.model["bind"])
         self.title = doc_as_dict["html"]["head"]["title"]
         secondary = []
@@ -353,15 +361,15 @@
         if self._bind_list:
             self._cleanup_bind_list()
 
     def _get_item_func(self, ref, name, item):
         rs = {}
         name_splits = name.split("/")
         rs["name"] = name_splits[0]
-        ref = "%s/%s" % (ref, rs["name"])
+        ref = f"""{ref}/{rs["name"]}"""
         rs["ref"] = ref
         if name_splits.__len__() > 1:
             rs["type"] = "group"
             rs["children"] = [self._get_item_func(ref, "/".join(name_splits[1:]), item)]
         return rs
 
     def survey(self):
@@ -381,16 +389,18 @@
 
     def _get_question_from_object(self, obj, type=None):
         try:
             ref = obj["ref"]
         except KeyError:
             try:
                 ref = obj["nodeset"]
-            except KeyError:
-                raise TypeError('cannot find "ref" or "nodeset" in {}'.format(repr(obj)))
+            except KeyError as node_err:
+                raise PyXFormError(
+                    f'Cannot find "ref" or "nodeset" in {obj!r}'
+                ) from node_err
         question = {
             "ref": ref,
             "__order": self._get_question_order(ref),
             "name": self._get_name_from_ref(ref),
         }
         if "hint" in obj:
             k, v = self._get_label(obj["hint"], "hint")
@@ -455,15 +465,15 @@
             question["type"] = question_type
         if type == "trigger":
             question["type"] = "acknowledge"
         if type in [
             "select1",
             "select",
         ]:  # Select bind type is 'string' https://github.com/XLSForm/pyxform/issues/168
-            question["type"] = self.QUESTION_TYPES[type]
+            question["type"] = QUESTION_TYPES[type]
         if question_type == "geopoint" and "hint" in question:
             del question["hint"]
         if "type" not in question and type:
             question["type"] = question_type
         if "itemset" in obj:
             # Secondary instances
             nodeset = obj["itemset"]["nodeset"]
@@ -501,15 +511,15 @@
                 except ValueError:
                     pass
                 rs = {}
                 for k, v in iter(item.items()):
                     if k == "nodeset":
                         continue
                     if k == "type":
-                        v = self._get_question_type(v)
+                        v = self._get_question_type(question_type=v)
                     if k in [
                         "relevant",
                         "required",
                         "constraint",
                         "constraintMsg",
                         "readonly",
                         "calculate",
@@ -542,28 +552,32 @@
                 if "preloadParams" in rs and "preload" in rs:
                     rs["type"] = rs["preloadParams"]
                     del rs["preloadParams"]
                     del rs["preload"]
                 return rs
         return None
 
-    def _get_question_type(self, type):
-        if type in self.QUESTION_TYPES.keys():
-            return self.QUESTION_TYPES[type]
-        return type
+    @staticmethod
+    def _get_question_type(question_type):
+        if question_type in QUESTION_TYPES.keys():
+            return QUESTION_TYPES[question_type]
+        return question_type
 
     def _get_translations(self) -> List[Dict]:
         if "itext" not in self.model:
             return []
-        assert "translation" in self.model["itext"]
+        if "translation" not in self.model["itext"]:
+            raise PyXFormError("""Invalid value for `self.model["itext"]`.""")
         translations = self.model["itext"]["translation"]
         if isinstance(translations, dict):
             translations = [translations]
-        assert "text" in translations[0]
-        assert "lang" in translations[0]
+        if "text" not in translations[0]:
+            raise PyXFormError("""Invalid value for `translations[0]`.""")
+        if "lang" not in translations[0]:
+            raise PyXFormError("""Invalid value for `translations[0]`.""")
         return translations
 
     def _get_label(self, label_obj, key="label"):
         if isinstance(label_obj, dict):
             try:
                 ref = label_obj["ref"].replace("jr:itext('", "").replace("')", "")
             except KeyError:
@@ -698,10 +712,10 @@
         pattern = "(/[a-z0-9-_]+(?:/[a-z0-9-_]+)+)"
         text = re.compile(pattern, flags=re.I).sub(replace_function, text)
         return text
 
 
 def write_object_to_file(filename, obj):
     """Writes to a JSON filename the dictionary obj."""
-    with codecs.open(filename, "w", encoding="utf-8") as output_file:
+    with open(filename, "w", encoding="utf-8") as output_file:
         output_file.write(json.dumps(obj, indent=2))
     logger.info("object written to file: %s", filename)
```

### Comparing `pyxform-2.0.2/pyxform/xform_instance_parser.py` & `pyxform-2.0.3/pyxform/xform_instance_parser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,75 @@
-# -*- coding: utf-8 -*-
 """
 XFormInstanceParser class module - parses an instance XML.
 """
 # todo: this has been copied from xform_manager, we need to figure out
 # where this code is actually going to live.
 
 import re
-from xml.dom import minidom
+from xml.dom.minidom import Node
+
+from defusedxml.minidom import parseString
+
+from pyxform.errors import PyXFormError
 
 XFORM_ID_STRING = "_xform_id_string"
 
 
 def _xml_node_to_dict(node):
-    assert isinstance(node, minidom.Node)
+    if not isinstance(node, Node):
+        raise PyXFormError("""Invalid value for `node`.""")
     if len(node.childNodes) == 0:
         # there's no data for this leaf node
         value = None
     elif len(node.childNodes) == 1 and node.childNodes[0].nodeType == node.TEXT_NODE:
         # there is data for this leaf node
         value = node.childNodes[0].nodeValue
     else:
         # this is an internal node
         value = {}
         for child in node.childNodes:
             d = _xml_node_to_dict(child)
             child_name = child.nodeName
-            assert list(d.keys()) == [child_name]
+            if list(d.keys()) != [child_name]:
+                raise PyXFormError("""Invalid value for `d`.""")
             if child_name not in value:
                 # copy the value into the dict
                 value[child_name] = d[child_name]
-            elif type(value[child_name]) == list:
+            elif isinstance(value[child_name], list):
                 # add to the existing list
                 value[child_name].append(d[child_name])
             else:
                 # create a new list
                 value[child_name] = [value[child_name], d[child_name]]
     return {node.nodeName: value}
 
 
 def _flatten_dict(d, prefix):
     """
     Return a list of XPath, value pairs.
     """
-    assert type(d) == dict
-    assert type(prefix) == list
+    if not isinstance(d, dict):
+        raise PyXFormError("""Invalid value for `d`.""")
+    if not isinstance(prefix, list):
+        raise PyXFormError("""Invalid value for `prefix`.""")
 
     for key, value in d.items():
-        new_prefix = prefix + [key]
-        if type(value) == dict:
+        new_prefix = [*prefix, key]
+        if isinstance(value, dict):
             for pair in _flatten_dict(value, new_prefix):
                 yield pair
-        elif type(value) == list:
+        elif isinstance(value, list):
             for i, item in enumerate(value):
                 item_prefix = list(new_prefix)  # make a copy
                 # note on indexing xpaths: IE5 and later has
                 # implemented that [0] should be the first node, but
                 # according to the W3C standard it should have been
                 # [1]. I'm adding 1 to i to start at 1.
                 item_prefix[-1] += "[%s]" % str(i + 1)
-                if type(item) == dict:
+                if isinstance(item, dict):
                     for pair in _flatten_dict(item, item_prefix):
                         yield pair
                 else:
                     yield (item_prefix, item)
         else:
             yield (new_prefix, value)
 
@@ -71,26 +78,25 @@
     """
     Go through an XML document returning all the attributes we see.
     """
     if hasattr(node, "hasAttributes") and node.hasAttributes():
         for key in node.attributes.keys():
             yield key, node.getAttribute(key)
     for child in node.childNodes:
-        for pair in _get_all_attributes(child):
-            yield pair
+        yield from _get_all_attributes(child)
 
 
 class XFormInstanceParser:
     def __init__(self, xml_str):
         self.parse(xml_str)
 
     def parse(self, xml_str):
         clean_xml_str = xml_str.strip()
-        clean_xml_str = re.sub(str(r">\s+<"), str("><"), clean_xml_str)
-        self._xml_obj = minidom.parseString(clean_xml_str)
+        clean_xml_str = re.sub(r">\s+<", "><", clean_xml_str)
+        self._xml_obj = parseString(clean_xml_str)
         self._root_node = self._xml_obj.documentElement
         self._dict = _xml_node_to_dict(self._root_node)
         self._flat_dict = {}
         for path, value in _flatten_dict(self._dict, []):
             self._flat_dict["/".join(path[1:])] = value
         self._set_attributes()
 
@@ -109,15 +115,16 @@
     def get_attributes(self):
         return self._attributes
 
     def _set_attributes(self):
         self._attributes = {}
         all_attributes = list(_get_all_attributes(self._root_node))
         for key, value in all_attributes:
-            assert key not in self._attributes
+            if key in self._attributes:
+                raise PyXFormError("""Invalid value for `self._attributes`.""")
             self._attributes[key] = value
 
     def get_xform_id_string(self):
         return self._attributes["id"]
 
     def get_flat_dict_with_attributes(self):
         result = self.to_flat_dict().copy()
```

### Comparing `pyxform-2.0.2/pyxform/xls2json.py` & `pyxform-2.0.3/pyxform/xls2json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-# -*- coding: utf-8 -*-
 """
 A Python script to convert excel files into JSON.
 """
-import codecs
 import json
 import os
 import re
 import sys
 from collections import Counter
 from typing import IO, Any, Dict, List, Optional, Tuple
 
@@ -35,17 +33,16 @@
 
 def print_pyobj_to_json(pyobj, path=None):
     """
     dump a python nested array/dict structure to the specified file
     or stdout if no file is specified
     """
     if path:
-        fp = codecs.open(path, mode="w", encoding="utf-8")
-        json.dump(pyobj, fp=fp, ensure_ascii=False, indent=4)
-        fp.close()
+        with open(path, mode="w", encoding="utf-8") as fp:
+            json.dump(pyobj, fp=fp, ensure_ascii=False, indent=4)
     else:
         sys.stdout.write(json.dumps(pyobj, ensure_ascii=False, indent=4))
 
 
 def merge_dicts(dict_a, dict_b, default_key="default"):
     """
     Recursively merge two nested dicts into a single dict.
@@ -68,15 +65,15 @@
         dict_b = {default_key: dict_b}
 
     # Union keys but retain order (as opposed to set()), preferencing dict_a then dict_b.
     # E.g. {"a": 1, "b": 2} + {"c": 3, "a": 4} -> {"a": None, "b": None, "c": None}
     all_keys = {k: None for k in dict_a.keys()}
     all_keys.update({k: None for k in dict_b.keys()})
 
-    out_dict = dict()
+    out_dict = {}
     for key in all_keys.keys():
         out_dict[key] = merge_dicts(dict_a.get(key), dict_b.get(key), default_key)
     return out_dict
 
 
 def list_to_nested_dict(lst):
     """
@@ -127,18 +124,18 @@
         {"text": {"english": "hello", "french" : "bonjour"}.
     Dealiasing is done to the first token
     (the first term separated by the delimiter).
     default_language -- used to group labels/hints/etc
     without a language specified with localized versions.
     """
     group_delimiter = "::"
-    out_dict_array = list()
+    out_dict_array = []
     seen_headers = {}
     for row in dict_array:
-        out_row = dict()
+        out_row = {}
         for header, val in row.items():
             if ignore_case:
                 header = header.lower()
 
             if use_double_colons:
                 tokens = header.split(group_delimiter)
 
@@ -226,15 +223,15 @@
 def group_dictionaries_by_key(list_of_dicts, key, remove_key=True):
     """
     Takes a list of dictionaries and returns a
     dictionary of lists of dictionaries with the same value for the given key.
     The grouping key is removed by default.
     If the key is not in any dictionary an empty dict is returned.
     """
-    dict_of_lists = dict()
+    dict_of_lists = {}
     for dicty in list_of_dicts:
         if key not in dicty:
             continue
         dicty_value = dicty[key]
         if remove_key:
             dicty.pop(key)
         if dicty_value in dict_of_lists:
@@ -248,15 +245,15 @@
     """
     Look for a column header with a doublecolon (::) and
     return true if one is found.
     """
     for sheet in workbook_dict.values():
         for row in sheet:
             for column_header in row.keys():
-                if type(column_header) is not str:
+                if not isinstance(column_header, str):
                     continue
                 if "::" in column_header:
                     return True
     return False
 
 
 def add_flat_annotations(prompt_list, parent_relevant="", name_prefix=""):
@@ -283,20 +280,19 @@
 
         children = prompt.get(constants.CHILDREN)
         if children:
             prompt["flat"] = True
             add_flat_annotations(
                 children, new_relevant, name_prefix + "_" + prompt["name"]
             )
-        else:
-            if new_relevant != "":
-                prompt["bind"] = prompt.get("bind", {})
-                prompt["bind"]["relevant"] = new_relevant
-                # if name_prefix != '':
-                #    prompt['name'] = name_prefix + prompt['name']
+        elif new_relevant != "":
+            prompt["bind"] = prompt.get("bind", {})
+            prompt["bind"]["relevant"] = new_relevant
+            # if name_prefix != '':
+            #    prompt['name'] = name_prefix + prompt['name']
 
 
 def process_range_question_type(
     row: Dict[str, Any], parameters: parameters_generic.PARAMETERS_TYPE
 ) -> Dict[str, Any]:
     """
     Returns a new row that includes the Range parameters start, end and step.
@@ -311,20 +307,24 @@
     defaults = {"start": "1", "end": "10", "step": "1"}
 
     # set defaults
     for key in parameters_map.values():
         if key not in parameters:
             parameters[key] = defaults[key]
 
+    has_float = False
     try:
-        has_float = any([float(x) and "." in str(x) for x in parameters.values()])
-    except ValueError:
+        # Check all parameters.
+        for x in parameters.values():
+            if float(x) and "." in str(x):
+                has_float = True
+    except ValueError as range_err:
         raise PyXFormError(
-            "Range parameters 'start', " "'end' or 'step' must all be numbers."
-        )
+            "Range parameters 'start', 'end' or 'step' must all be numbers."
+        ) from range_err
     else:
         # is integer by default, convert to decimal if it has any float values
         if has_float:
             new_dict["bind"] = new_dict.get("bind", {})
             new_dict["bind"].update({"type": "decimal"})
 
     new_dict["parameters"] = parameters
@@ -366,15 +366,15 @@
 
     if choice_filter:
         # External selects e.g. type = "select_one_external city".
         if question[constants.TYPE] == constants.SELECT_ONE_EXTERNAL:
             question["query"] = list_name
         elif choices.get(list_name):
             # Reference to list name for data dictionary tools (ilri/odktools).
-            question["list_name"] = list_name
+            question[constants.LIST_NAME_U] = list_name
             # Copy choices for data export tools (onaio/onadata).
             # TODO: could onadata use the list_name to look up the list for
             #  export, instead of pyxform internally duplicating choices data?
             question[constants.CHOICES] = choices[list_name]
     elif not (
         # Select with randomized choices.
         (
@@ -382,15 +382,15 @@
             and question[constants.PARAMETERS][constants.RANDOMIZE] == "true"
         )
         # Select from file e.g. type = "select_one_from_file cities.xml".
         or file_extension in EXTERNAL_INSTANCE_EXTENSIONS
         # Select from previous answers e.g. type = "select_one ${q1}".
         or bool(PYXFORM_REFERENCE_REGEX.search(list_name))
     ):
-        question["list_name"] = list_name
+        question[constants.LIST_NAME_U] = list_name
         question[constants.CHOICES] = choices[list_name]
 
 
 def workbook_to_json(
     workbook_dict,
     form_name: Optional[str] = None,
     fallback_form_name: Optional[str] = None,
@@ -418,15 +418,15 @@
     if warnings is None:
         warnings = []
     is_valid = False
     # Sheet names should be case-insensitive
     workbook_dict = {x.lower(): y for x, y in workbook_dict.items()}
     workbook_keys = workbook_dict.keys()
     if constants.SURVEY not in workbook_dict:
-        msg = "You must have a sheet named '{k}'. ".format(k=constants.SURVEY)
+        msg = f"You must have a sheet named '{constants.SURVEY}'. "
         similar = find_sheet_misspellings(key=constants.SURVEY, keys=workbook_keys)
         if similar is not None:
             msg += similar
         raise PyXFormError(msg)
 
     # ensure required headers are present
     for row in workbook_dict.get(constants.SURVEY, []):
@@ -525,50 +525,50 @@
     external_choices_sheet = dealias_and_group_headers(
         dict_array=external_choices_sheet,
         header_aliases=aliases.list_header,
         use_double_colons=use_double_colons,
         default_language=default_language,
     )
     external_choices = group_dictionaries_by_key(
-        list_of_dicts=external_choices_sheet.data, key=constants.LIST_NAME
+        list_of_dicts=external_choices_sheet.data, key=constants.LIST_NAME_S
     )
 
     # ########## Choices sheet ##########
     choices_sheet = workbook_dict.get(constants.CHOICES, [])
     for choice_item in choices_sheet:
         replace_smart_quotes_in_dict(choice_item)
     choices_sheet = dealias_and_group_headers(
         dict_array=choices_sheet,
         header_aliases=aliases.list_header,
         use_double_colons=use_double_colons,
         default_language=default_language,
     )
     combined_lists = group_dictionaries_by_key(
-        list_of_dicts=choices_sheet.data, key=constants.LIST_NAME
+        list_of_dicts=choices_sheet.data, key=constants.LIST_NAME_S
     )
     # To combine the warning into one message, the check for missing choices translation
     # columns is run with Survey sheet below.
 
     choices = combined_lists
     # Make sure all the options have the required properties:
     warnedabout = set()
     for list_name, options in choices.items():
         for option in options:
             if "name" not in option:
                 info = "[list_name : " + list_name + "]"
                 raise PyXFormError(
-                    "On the choices sheet there is " "a option with no name. " + info
+                    "On the choices sheet there is a option with no name. " + info
                 )
             if "label" not in option:
                 info = "[list_name : " + list_name + "]"
                 warnings.append(
                     "On the choices sheet there is a option with no label. " + info
                 )
             # chrislrobert's fix for a cryptic error message:
-            # see: https://code.google.com/p/opendatakit/issues/detail?id=832&start=200 # noqa
+            # see: https://code.google.com/p/opendatakit/issues/detail?id=833&start=200
             option_keys = list(option.keys())
             for headername in option_keys:
                 # Using warnings and removing the bad columns
                 # instead of throwing errors because some forms
                 # use choices column headers for notes.
                 if " " in headername:
                     if headername not in warnedabout:
@@ -586,15 +586,15 @@
                         "On the choices sheet there is a value"
                         + " in a column with no header."
                     )
                     del option[headername]
         list_name_choices = [option.get("name") for option in options]
         if len(list_name_choices) != len(set(list_name_choices)):
             duplicate_setting = settings.get("allow_choice_duplicates")
-            for k, v in Counter(list_name_choices).items():
+            for v in Counter(list_name_choices).values():
                 if v > 1:
                     if not duplicate_setting or duplicate_setting.capitalize() != "Yes":
                         choice_duplicates = [
                             item
                             for item, count in Counter(list_name_choices).items()
                             if count > 1
                         ]
@@ -603,21 +603,18 @@
                             raise PyXFormError(
                                 "The name column for the '{}' choice list contains these duplicates: {}. Duplicate names "
                                 "will be impossible to identify in analysis unless a previous value in a cascading "
                                 "select differentiates them. If this is intentional, you can set the "
                                 "allow_choice_duplicates setting to 'yes'. Learn more: https://xlsform.org/#choice-names.".format(
                                     list_name,
                                     ", ".join(
-                                        [
-                                            "'{}'".format(dupe)
-                                            for dupe in choice_duplicates
-                                        ]
+                                        [f"'{dupe}'" for dupe in choice_duplicates]
                                     ),
                                 )
-                            )  # noqa
+                            )
 
     # ########## Entities sheet ###########
     entities_sheet = workbook_dict.get(constants.ENTITIES, [])
     entities_sheet = dealias_and_group_headers(
         dict_array=entities_sheet,
         header_aliases=aliases.entities_header,
         use_double_colons=False,
@@ -653,15 +650,15 @@
     # No spell check for OSM sheet (infrequently used, many spurious matches).
     osm_sheet = dealias_and_group_headers(
         dict_array=workbook_dict.get(constants.OSM, []),
         header_aliases=aliases.list_header,
         use_double_colons=True,
     )
     osm_tags = group_dictionaries_by_key(
-        list_of_dicts=osm_sheet.data, key=constants.LIST_NAME
+        list_of_dicts=osm_sheet.data, key=constants.LIST_NAME_S
     )
     # #################################
 
     # Parse the survey sheet while generating a survey in our json format:
     row_number = 1  # We start at 1 because the column header row is not
     #                 included in the survey sheet (presumably).
     # A stack is used to keep track of begin/end expressions
@@ -778,16 +775,17 @@
                         constants.TRACK_CHANGES + " must be set to true or false: "
                         "'%s' is an invalid value" % parameters[constants.TRACK_CHANGES]
                     )
                 else:
                     new_dict["bind"] = new_dict.get("bind", {})
                     new_dict["bind"].update(
                         {
-                            "odk:"
-                            + constants.TRACK_CHANGES: parameters[constants.TRACK_CHANGES]
+                            "odk:" + constants.TRACK_CHANGES: parameters[
+                                constants.TRACK_CHANGES
+                            ]
                         }
                     )
 
             if constants.TRACK_CHANGES_REASONS in parameters.keys():
                 if parameters[constants.TRACK_CHANGES_REASONS] != "on-form-edit":
                     raise PyXFormError(
                         constants.TRACK_CHANGES_REASONS + " must be set to on-form-edit"
@@ -807,27 +805,27 @@
                         constants.IDENTIFY_USER + " must be set to true or false: "
                         "'%s' is an invalid value" % parameters[constants.IDENTIFY_USER]
                     )
                 else:
                     new_dict["bind"] = new_dict.get("bind", {})
                     new_dict["bind"].update(
                         {
-                            "odk:"
-                            + constants.IDENTIFY_USER: parameters[constants.IDENTIFY_USER]
+                            "odk:" + constants.IDENTIFY_USER: parameters[
+                                constants.IDENTIFY_USER
+                            ]
                         }
                     )
 
             location_parameters = (
                 constants.LOCATION_PRIORITY,
                 constants.LOCATION_MIN_INTERVAL,
                 constants.LOCATION_MAX_AGE,
             )
             if any(k in parameters.keys() for k in location_parameters):
                 if all(k in parameters.keys() for k in location_parameters):
-
                     if parameters[constants.LOCATION_PRIORITY] not in [
                         "no-power",
                         "low-power",
                         "balanced",
                         "high-accuracy",
                     ]:
                         raise PyXFormError(
@@ -836,35 +834,35 @@
                             + " must be set to no-power, low-power, balanced,"
                             " or high-accuracy: '%s' is an invalid value"
                             % parameters[constants.LOCATION_PRIORITY]
                         )
 
                     try:
                         int(parameters[constants.LOCATION_MIN_INTERVAL])
-                    except ValueError:
+                    except ValueError as lmi_err:
                         raise PyXFormError(
                             "Parameter "
                             + constants.LOCATION_MIN_INTERVAL
                             + " must have an integer value."
-                        )
+                        ) from lmi_err
                     if int(parameters[constants.LOCATION_MIN_INTERVAL]) < 0:
                         raise PyXFormError(
                             "Parameter "
                             + constants.LOCATION_MIN_INTERVAL
                             + " must be greater than or equal to zero."
                         )
 
                     try:
                         int(parameters[constants.LOCATION_MAX_AGE])
-                    except ValueError:
+                    except ValueError as lma_err:
                         raise PyXFormError(
                             "Parameter "
                             + constants.LOCATION_MAX_AGE
                             + " must have an integer value."
-                        )
+                        ) from lma_err
                     if int(parameters[constants.LOCATION_MAX_AGE]) < 0:
                         raise PyXFormError(
                             "Parameter "
                             + constants.LOCATION_MAX_AGE
                             + " must be greater  than or equal to zero."
                         )
 
@@ -878,24 +876,21 @@
                             + constants.LOCATION_MIN_INTERVAL
                             + "."
                         )
 
                     new_dict["bind"] = new_dict.get("bind", {})
                     new_dict["bind"].update(
                         {
-                            "odk:"
-                            + constants.LOCATION_MAX_AGE: parameters[
+                            "odk:" + constants.LOCATION_MAX_AGE: parameters[
                                 constants.LOCATION_MAX_AGE
                             ],
-                            "odk:"
-                            + constants.LOCATION_MIN_INTERVAL: parameters[
+                            "odk:" + constants.LOCATION_MIN_INTERVAL: parameters[
                                 constants.LOCATION_MIN_INTERVAL
                             ],
-                            "odk:"
-                            + constants.LOCATION_PRIORITY: parameters[
+                            "odk:" + constants.LOCATION_PRIORITY: parameters[
                                 constants.LOCATION_PRIORITY
                             ],
                         }
                     )
                 else:
                     raise PyXFormError(
                         "To include location information in"
@@ -1023,24 +1018,24 @@
                         ROW_FORMAT_STRING % row_number
                         + " %s has no label: " % control_type.capitalize()
                         + str(msg_dict)
                     )
 
                 new_json_dict = row.copy()
                 new_json_dict[constants.TYPE] = control_type
-                child_list = list()
+                child_list = []
                 new_json_dict[constants.CHILDREN] = child_list
                 if control_type is constants.LOOP:
-                    if not parse_dict.get("list_name"):
+                    if not parse_dict.get(constants.LIST_NAME_U):
                         # TODO: Perhaps warn and make repeat into a group?
                         raise PyXFormError(
                             ROW_FORMAT_STRING % row_number
                             + " Repeat loop without list name."
                         )
-                    list_name = parse_dict["list_name"]
+                    list_name = parse_dict[constants.LIST_NAME_U]
                     if list_name not in choices:
                         raise PyXFormError(
                             ROW_FORMAT_STRING % row_number
                             + " List name not in columns sheet: "
                             + list_name
                         )
                     new_json_dict[constants.COLUMNS] = choices[list_name]
@@ -1123,19 +1118,20 @@
             if parse_dict.get("select_command"):
                 select_type = aliases.select[parse_dict["select_command"]]
                 if (
                     select_type == constants.SELECT_ONE_EXTERNAL
                     and constants.CHOICE_FILTER not in row
                 ):
                     warnings.append(
-                        ROW_FORMAT_STRING % row_number
+                        ROW_FORMAT_STRING
+                        % row_number
                         + " select one external is only meant for"
                         " filtered selects."
                     )
-                list_name = parse_dict["list_name"]
+                list_name = parse_dict[constants.LIST_NAME_U]
                 file_extension = os.path.splitext(list_name)[1]
                 if (
                     select_type == constants.SELECT_ONE_EXTERNAL
                     and list_name not in external_choices
                 ):
                     if not external_choices:
                         k = constants.EXTERNAL_CHOICES
@@ -1233,18 +1229,18 @@
                             "'%s' is an invalid value" % parameters["randomize"]
                         )
 
                     if "seed" in parameters.keys():
                         if not parameters["seed"].startswith("${"):
                             try:
                                 float(parameters["seed"])
-                            except ValueError:
+                            except ValueError as seed_err:
                                 raise PyXFormError(
                                     "seed value must be a number or a reference to another field."
-                                )
+                                ) from seed_err
                 elif "seed" in parameters.keys():
                     raise PyXFormError(
                         "Parameters must include randomize=true to use a seed."
                     )
 
                 if "value" in parameters.keys():
                     select_from_file.value_or_label_check(
@@ -1291,15 +1287,15 @@
                                 + " Choice filter not supported for table-list appearance."
                             )
                             raise PyXFormError(msg)
                         table_list_header = {
                             constants.TYPE: select_type,
                             constants.NAME: "reserved_name_for_field_list_labels_"
                             + str(row_number),
-                            # Adding row number for uniqueness # noqa
+                            # Adding row number for uniqueness
                             constants.CONTROL: {constants.APPEARANCE: "label"},
                             constants.CHOICES: choices[list_name],
                             constants.ITEMSET: list_name,
                         }
                         parent_children_array.append(table_list_header)
 
                     if table_list != list_name:
@@ -1323,16 +1319,16 @@
         # Try to parse question as osm:
         osm_parse = osm_regexp.search(question_type)
         if osm_parse:
             parse_dict = osm_parse.groupdict()
             new_dict = row.copy()
             new_dict["type"] = constants.OSM
 
-            if parse_dict.get("list_name") is not None:
-                tags = osm_tags.get(parse_dict.get("list_name"))
+            if parse_dict.get(constants.LIST_NAME_U) is not None:
+                tags = osm_tags.get(parse_dict.get(constants.LIST_NAME_U))
                 for tag in tags:
                     if osm_tags.get(tag.get("name")):
                         tag["choices"] = osm_tags.get(tag.get("name"))
                 new_dict["tags"] = tags
 
             parent_children_array.append(new_dict)
 
@@ -1347,19 +1343,19 @@
         if question_type == "text":
             new_dict = row.copy()
             parameters_generic.validate(parameters=parameters, allowed=("rows",))
 
             if "rows" in parameters.keys():
                 try:
                     int(parameters["rows"])
-                except ValueError:
+                except ValueError as rows_err:
                     raise PyXFormError(
                         (ROW_FORMAT_STRING % row_number)
                         + " Parameter rows must have an integer value."
-                    )
+                    ) from rows_err
 
                 new_dict["control"] = new_dict.get("control", {})
                 new_dict["control"].update({"rows": parameters["rows"]})
 
             parent_children_array.append(new_dict)
             continue
 
@@ -1374,16 +1370,18 @@
                     "max-pixels",
                     "app",
                 ),
             )
             if "max-pixels" in parameters.keys():
                 try:
                     int(parameters["max-pixels"])
-                except ValueError:
-                    raise PyXFormError("Parameter max-pixels must have an integer value.")
+                except ValueError as mp_err:
+                    raise PyXFormError(
+                        "Parameter max-pixels must have an integer value."
+                    ) from mp_err
 
                 new_dict["bind"] = new_dict.get("bind", {})
                 new_dict["bind"].update({"orx:max-pixels": parameters["max-pixels"]})
             else:
                 warnings.append(
                     (ROW_FORMAT_STRING % row_number)
                     + " Use the max-pixels parameter to speed up submission sending and save storage space. Learn more: https://xlsform.org/#image"
@@ -1471,29 +1469,29 @@
             new_dict["control"] = new_dict.get("control", {})
             if "capture-accuracy" in parameters.keys():
                 try:
                     float(parameters["capture-accuracy"])
                     new_dict["control"].update(
                         {"accuracyThreshold": parameters["capture-accuracy"]}
                     )
-                except ValueError:
+                except ValueError as ca_err:
                     raise PyXFormError(
                         "Parameter capture-accuracy must have a numeric value"
-                    )
+                    ) from ca_err
 
             if "warning-accuracy" in parameters.keys():
                 try:
                     float(parameters["warning-accuracy"])
                     new_dict["control"].update(
                         {"unacceptableAccuracyThreshold": parameters["warning-accuracy"]}
                     )
-                except ValueError:
+                except ValueError as wa_err:
                     raise PyXFormError(
                         "Parameter warning-accuracy must have a numeric value"
-                    )
+                    ) from wa_err
 
             parent_children_array.append(new_dict)
             continue
         # TODO: Consider adding some question_type validation here.
 
         # Put the row in the json dict as is:
         parent_children_array.append(row)
@@ -1506,15 +1504,15 @@
             + str(stack[-1]["control_type"] + " (" + stack[-1]["control_name"] + ")")
         )
 
     if settings.get("flat", False):
         # print "Generating flattened instance..."
         add_flat_annotations(stack[0]["parent_children"])
 
-    meta_children = [] + survey_meta
+    meta_children = [*survey_meta]
 
     if aliases.yes_no.get(settings.get("omit_instanceID")):
         if settings.get("public_key"):
             raise PyXFormError("Cannot omit instanceID, it is required for encryption.")
     else:
         # Automatically add an instanceID element:
         meta_children.append(
@@ -1585,15 +1583,15 @@
         raise PyXFormError("File was not recognized")
 
 
 def get_filename(path):
     """
     Get the extensionless filename from a path
     """
-    return os.path.splitext((os.path.basename(path)))[0]
+    return os.path.splitext(os.path.basename(path))[0]
 
 
 def parse_file_to_json(
     path: str,
     default_name: str = "data",
     default_language: str = constants.DEFAULT_LANGUAGE_VALUE,
     warnings: Optional[List[str]] = None,
@@ -1626,15 +1624,15 @@
     """
     result = {}
     for dicty in dict_list:
         if key in dicty:
             dicty_copy = dicty.copy()
             val = dicty_copy.pop(key)
             if val in result:
-                raise Exception("Duplicate key: " + val)
+                raise PyXFormError("Duplicate key: " + val)
             result[val] = dicty_copy
     return result
 
 
 class SpreadsheetReader:
     def __init__(self, path_or_file):
         path = path_or_file
@@ -1679,27 +1677,27 @@
             warnings=self._warnings,
             file_object=self._file_object,
         )
         self._path = path
 
     def print_warning_log(self, warn_out_file):
         # Open file to print warning log to.
-        warn_out = open(warn_out_file, "w")
+        warn_out = open(warn_out_file, mode="w", encoding="utf-8")
         warn_out.write("\n".join(self._warnings))
 
 
 class QuestionTypesReader(SpreadsheetReader):
     """
     Class for reading spreadsheet file that specifies the available
     question types.
     @see question_type_dictionary
     """
 
     def __init__(self, path):
-        super(QuestionTypesReader, self).__init__(path)
+        super().__init__(path)
         self._setup_question_types_dictionary()
 
     def _setup_question_types_dictionary(self):
         use_double_colons = has_double_colon(self._dict)
         types_sheet = "question types"
         self._dict = self._dict[types_sheet]
         self._dict = dealias_and_group_headers(
@@ -1707,36 +1705,14 @@
             header_aliases={},
             use_double_colons=use_double_colons,
             default_language=constants.DEFAULT_LANGUAGE_VALUE,
         ).data
         self._dict = organize_by_values(self._dict, "name")
 
 
-# Not used internally (or on formhub)
-# TODO: If this is used anywhere else it is probably broken
-#      from the changes I made to SpreadsheetReader.
-class VariableNameReader(SpreadsheetReader):
-    def __init__(self, path):
-        SpreadsheetReader.__init__(self, path)
-        self._organize_renames()
-
-    def _organize_renames(self):
-        new_dict = {}
-        variable_names_so_far = []
-        assert "Dictionary" in self._dict
-        for d in self._dict["Dictionary"]:
-            if "Variable Name" in d:
-                assert d["Variable Name"] not in variable_names_so_far, d["Variable Name"]
-                variable_names_so_far.append(d["Variable Name"])
-                new_dict[d["XPath"]] = d["Variable Name"]
-            else:
-                variable_names_so_far.append(d["XPath"])
-        self._dict = new_dict
-
-
 if __name__ == "__main__":
     # Open the excel file specified by the argument of this python call,
     # convert that file to json, then print it
     if len(sys.argv) < 2:
         # print "You must supply a file argument."
         _filename = "xlsform_spec_test.xls"
         _path = "/home/user/python-dev/xlsform/pyxform/tests/example_xls/"
```

### Comparing `pyxform-2.0.2/pyxform/xls2json_backends.py` & `pyxform-2.0.3/pyxform/xls2json_backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-# -*- coding: utf-8 -*-
 """
 XLS-to-dict and csv-to-dict are essentially backends for xls2json.
 """
 import csv
 import datetime
+import os
 import re
 from collections import OrderedDict
+from contextlib import closing
 from functools import reduce
 from io import StringIO
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 from zipfile import BadZipFile
 
-import openpyxl
 import xlrd
 from openpyxl.cell import Cell as pyxlCell
+from openpyxl.reader.excel import ExcelReader
+from openpyxl.workbook import Workbook as pyxlWorkbook
+from openpyxl.worksheet.worksheet import Worksheet as pyxlWorksheet
+from xlrd.book import Book as xlrdBook
 from xlrd.sheet import Cell as xlrdCell
+from xlrd.sheet import Sheet as xlrdSheet
 from xlrd.xldate import XLDateAmbiguous
 
 from pyxform import constants
 from pyxform.errors import PyXFormError
 
 aCell = Union[xlrdCell, pyxlCell]
 XL_DATE_AMBIGOUS_MSG = (
@@ -49,15 +54,15 @@
         a_list = a_list[:offset]
     return a_list
 
 
 def get_excel_column_headers(first_row: Iterator[Optional[str]]) -> List[Optional[str]]:
     """Get column headers from the first row; stop if there's a run of empty columns."""
     max_adjacent_empty_columns = 20
-    column_header_list = list()
+    column_header_list = []
     adjacent_empty_cols = 0
     for column_header in first_row:
         if is_empty(column_header):
             # Preserve column order (will filter later)
             column_header_list.append(None)
             # After a run of empty cols, assume we've reached the end of the data.
             if max_adjacent_empty_columns == adjacent_empty_cols:
@@ -117,67 +122,84 @@
     Return a Python dictionary with a key for each worksheet
     name. For each sheet there is a list of dictionaries, each
     dictionary corresponds to a single row in the worksheet. A
     dictionary has keys taken from the column headers and values
     equal to the cell value for that row and column.
     All the keys and leaf elements are unicode text.
     """
-    try:
-        if isinstance(path_or_file, str):
-            workbook = xlrd.open_workbook(filename=path_or_file)
-        else:
-            workbook = xlrd.open_workbook(file_contents=path_or_file.read())
-    except xlrd.XLRDError as error:
-        raise PyXFormError("Error reading .xls file: %s" % error)
 
-    def xls_clean_cell(cell: xlrdCell, row_n: int, col_key: str) -> Optional[str]:
+    def xls_clean_cell(
+        wb: xlrdBook, wb_sheet: xlrdSheet, cell: xlrdCell, row_n: int, col_key: str
+    ) -> Optional[str]:
         value = cell.value
         if isinstance(value, str):
             value = value.strip()
         if not is_empty(value):
             try:
-                return xls_value_to_unicode(value, cell.ctype, workbook.datemode)
-            except XLDateAmbiguous:
-                raise PyXFormError(XL_DATE_AMBIGOUS_MSG % (wb_sheet.name, col_key, row_n))
+                return xls_value_to_unicode(value, cell.ctype, wb.datemode)
+            except XLDateAmbiguous as date_err:
+                raise PyXFormError(
+                    XL_DATE_AMBIGOUS_MSG % (wb_sheet.name, col_key, row_n)
+                ) from date_err
 
         return None
 
-    def xls_to_dict_normal_sheet(sheet):
+    def xls_to_dict_normal_sheet(wb: xlrdBook, wb_sheet: xlrdSheet):
         # XLS format: max cols 256, max rows 65536
-        first_row = (c.value for c in next(sheet.get_rows(), []))
+        first_row = (c.value for c in next(wb_sheet.get_rows(), []))
         headers = get_excel_column_headers(first_row=first_row)
         row_iter = (
-            tuple(sheet.cell(r, c) for c in range(0, len(headers)))
-            for r in range(1, sheet.nrows)
+            tuple(wb_sheet.cell(r, c) for c in range(len(headers)))
+            for r in range(1, wb_sheet.nrows)
         )
-        rows = get_excel_rows(headers=headers, rows=row_iter, cell_func=xls_clean_cell)
+
+        # Inject wb/sheet as closure since functools.partial isn't typing friendly.
+        def clean_func(cell: xlrdCell, row_n: int, col_key: str) -> Optional[str]:
+            return xls_clean_cell(
+                wb=wb, wb_sheet=wb_sheet, cell=cell, row_n=row_n, col_key=col_key
+            )
+
+        rows = get_excel_rows(headers=headers, rows=row_iter, cell_func=clean_func)
         column_header_list = [key for key in headers if key is not None]
         return rows, _list_to_dict_list(column_header_list)
 
-    result_book = OrderedDict()
-    for wb_sheet in workbook.sheets():
-        # Note that the sheet exists but do no further processing here.
-        result_book[wb_sheet.name] = []
-        # Do not process sheets that have nothing to do with XLSForm.
-        if wb_sheet.name not in constants.SUPPORTED_SHEET_NAMES:
-            if len(workbook.sheets()) == 1:
-                (
-                    result_book[constants.SURVEY],
-                    result_book["%s_header" % constants.SURVEY],
-                ) = xls_to_dict_normal_sheet(wb_sheet)
+    def process_workbook(wb: xlrdBook):
+        result_book = OrderedDict()
+        for wb_sheet in wb.sheets():
+            # Note that the sheet exists but do no further processing here.
+            result_book[wb_sheet.name] = []
+            # Do not process sheets that have nothing to do with XLSForm.
+            if wb_sheet.name not in constants.SUPPORTED_SHEET_NAMES:
+                if len(wb.sheets()) == 1:
+                    (
+                        result_book[constants.SURVEY],
+                        result_book["%s_header" % constants.SURVEY],
+                    ) = xls_to_dict_normal_sheet(wb=wb, wb_sheet=wb_sheet)
+                else:
+                    continue
             else:
-                continue
-        else:
-            (
-                result_book[wb_sheet.name],
-                result_book["%s_header" % wb_sheet.name],
-            ) = xls_to_dict_normal_sheet(wb_sheet)
+                (
+                    result_book[wb_sheet.name],
+                    result_book["%s_header" % wb_sheet.name],
+                ) = xls_to_dict_normal_sheet(wb=wb, wb_sheet=wb_sheet)
+        return result_book
 
-    workbook.release_resources()
-    return result_book
+    try:
+        if isinstance(path_or_file, (str, bytes, os.PathLike)):
+            file = open(path_or_file, mode="rb")
+        else:
+            file = path_or_file
+        with closing(file) as wb_file:
+            workbook = xlrd.open_workbook(file_contents=wb_file.read())
+            try:
+                return process_workbook(wb=workbook)
+            finally:
+                workbook.release_resources()
+    except xlrd.XLRDError as read_err:
+        raise PyXFormError("Error reading .xls file: %s" % read_err) from read_err
 
 
 def xls_value_to_unicode(value, value_type, datemode) -> str:
     """
     Take a xls formatted value and try to make a unicode string representation.
     """
     if value_type == xlrd.XL_CELL_BOOLEAN:
@@ -211,59 +233,70 @@
     Return a Python dictionary with a key for each worksheet
     name. For each sheet there is a list of dictionaries, each
     dictionary corresponds to a single row in the worksheet. A
     dictionary has keys taken from the column headers and values
     equal to the cell value for that row and column.
     All the keys and leaf elements are strings.
     """
-    try:
-        workbook = openpyxl.open(filename=path_or_file, read_only=True, data_only=True)
-    except (OSError, BadZipFile, KeyError) as error:
-        raise PyXFormError("Error reading .xlsx file: %s" % error)
 
     def xlsx_clean_cell(cell: pyxlCell, row_n: int, col_key: str) -> Optional[str]:
         value = cell.value
         if isinstance(value, str):
             value = value.strip()
         if not is_empty(value):
             return xlsx_value_to_str(value)
 
         return None
 
-    def xlsx_to_dict_normal_sheet(sheet):
+    def xlsx_to_dict_normal_sheet(sheet: pyxlWorksheet):
         # XLSX format: max cols 16384, max rows 1048576
         first_row = (c.value for c in next(sheet.rows, []))
         headers = get_excel_column_headers(first_row=first_row)
         row_iter = sheet.iter_rows(min_row=2, max_col=len(headers))
         rows = get_excel_rows(headers=headers, rows=row_iter, cell_func=xlsx_clean_cell)
         column_header_list = [key for key in headers if key is not None]
         return rows, _list_to_dict_list(column_header_list)
 
-    result_book = OrderedDict()
-    for sheetname in workbook.sheetnames:
-        wb_sheet = workbook[sheetname]
-        # Note that the sheet exists but do no further processing here.
-        result_book[sheetname] = []
-        # Do not process sheets that have nothing to do with XLSForm.
-        if sheetname not in constants.SUPPORTED_SHEET_NAMES:
-            if len(workbook.sheetnames) == 1:
+    def process_workbook(wb: pyxlWorkbook):
+        result_book = OrderedDict()
+        for sheetname in wb.sheetnames:
+            wb_sheet = wb[sheetname]
+            # Note that the sheet exists but do no further processing here.
+            result_book[sheetname] = []
+            # Do not process sheets that have nothing to do with XLSForm.
+            if sheetname not in constants.SUPPORTED_SHEET_NAMES:
+                if len(wb.sheetnames) == 1:
+                    (
+                        result_book[constants.SURVEY],
+                        result_book[f"{constants.SURVEY}_header"],
+                    ) = xlsx_to_dict_normal_sheet(wb_sheet)
+                else:
+                    continue
+            else:
                 (
-                    result_book[constants.SURVEY],
-                    result_book[f"{constants.SURVEY}_header"],
+                    result_book[sheetname],
+                    result_book[f"{sheetname}_header"],
                 ) = xlsx_to_dict_normal_sheet(wb_sheet)
-            else:
-                continue
-        else:
-            (
-                result_book[sheetname],
-                result_book[f"{sheetname}_header"],
-            ) = xlsx_to_dict_normal_sheet(wb_sheet)
+        return result_book
 
-    workbook.close()
-    return result_book
+    try:
+        if isinstance(path_or_file, (str, bytes, os.PathLike)):
+            file = open(path_or_file, mode="rb")
+        else:
+            file = path_or_file
+        with closing(file) as wb_file:
+            reader = ExcelReader(wb_file, read_only=True, data_only=True)
+            reader.read()
+            try:
+                return process_workbook(wb=reader.wb)
+            finally:
+                reader.wb.close()
+                reader.archive.close()
+    except (OSError, BadZipFile, KeyError) as read_err:
+        raise PyXFormError("Error reading .xlsx file: %s" % read_err) from read_err
 
 
 def xlsx_value_to_str(value) -> str:
     """
     Take a xls formatted value and try to make a string representation.
     """
     if value is True:
@@ -307,30 +340,30 @@
             def replace_prefix(d, prefix):
                 for k, v in d.items():
                     if isinstance(v, str):
                         d[k] = v.replace("$PREFIX$", prefix)
                     elif isinstance(v, dict):
                         d[k] = replace_prefix(v, prefix)
                     elif isinstance(v, list):
-                        d[k] = map(lambda x: replace_prefix(x, prefix), v)
+                        d[k] = (replace_prefix(x, prefix) for x in v)
                 return d
 
             return_list.append(replace_prefix(row["lambda"], prefix))
     raise PyXFormError(
         "Found a cascading_select "
         + level
         + ", but could not find "
         + level
         + "in cascades sheet."
     )
 
 
 def csv_to_dict(path_or_file):
     if isinstance(path_or_file, str):
-        csv_data = open(path_or_file, "r", encoding="utf-8", newline="")
+        csv_data = open(path_or_file, encoding="utf-8", newline="")
     else:
         csv_data = path_or_file
 
     _dict = OrderedDict()
 
     def first_column_as_sheet_name(row):
         if len(row) == 0:
@@ -417,11 +450,11 @@
             out_row = []
             for key in row.keys():
                 if key not in out_keys:
                     out_keys.append(key)
             for out_key in out_keys:
                 out_row.append(row.get(out_key, None))
             out_rows.append(out_row)
-        writer.writerow([None] + out_keys)
+        writer.writerow([None, *out_keys])
         for out_row in out_rows:
-            writer.writerow([None] + out_row)
+            writer.writerow([None, *out_row])
     return foo.getvalue()
```

### Comparing `pyxform-2.0.2/pyxform/xls2xform.py` & `pyxform-2.0.3/pyxform/xls2xform.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """
 xls2xform converts properly formatted Excel documents into XForms for
 use with ODK Collect.
 """
 import argparse
 import json
 import logging
@@ -170,21 +169,21 @@
             warnings = xls2xform_convert(
                 xlsform_path=args.path_to_XLSForm,
                 xform_path=args.output_path,
                 validate=args.odk_validate,
                 pretty_print=args.pretty_print,
                 enketo=args.enketo_validate,
             )
-        except EnvironmentError as e:
+        except OSError:
             # Do not crash if 'java' not installed
-            logger.error(e)
-        except ODKValidateError as e:
+            logger.exception("EnvironmentError during conversion")
+        except ODKValidateError:
             # Remove output file if there is an error
             os.remove(args.output_path)
-            logger.error(e)
+            logger.exception("ODKValidateError during conversion.")
         else:
             if len(warnings) > 0:
                 logger.warning("Warnings:")
             for w in warnings:
                 logger.warning(w)
             logger.info("Conversion complete!")
```

### Comparing `pyxform-2.0.2/pyxform/xlsparseutils.py` & `pyxform-2.0.3/pyxform/xlsparseutils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pyxform import constants
 from pyxform.utils import levenshtein_distance
 
 # http://www.w3.org/TR/REC-xml/
 TAG_START_CHAR = r"[a-zA-Z:_]"
 TAG_CHAR = r"[a-zA-Z:_0-9\-.]"
-XFORM_TAG_REGEXP = "%(start)s%(char)s*" % {"start": TAG_START_CHAR, "char": TAG_CHAR}
+XFORM_TAG_REGEXP = f"{TAG_START_CHAR}{TAG_CHAR}*"
 
 
 def find_sheet_misspellings(key: str, keys: "KeysView") -> "Optional[str]":
     """
     Find possible sheet name misspellings to warn the user about.
 
     It's possible that this will warn about sheet names for sheets that have
@@ -28,15 +28,15 @@
         and _k not in constants.SUPPORTED_SHEET_NAMES
         and not _k.startswith("_")
     )
     if 0 < len(candidates):
         msg = (
             "When looking for a sheet named '{k}', the following sheets with "
             "similar names were found: {c}."
-        ).format(k=key, c=str(", ".join(("'{}'".format(c) for c in candidates))))
+        ).format(k=key, c=str(", ".join(f"'{c}'" for c in candidates)))
         return msg
     else:
         return None
 
 
 def is_valid_xml_tag(tag):
     """
```

