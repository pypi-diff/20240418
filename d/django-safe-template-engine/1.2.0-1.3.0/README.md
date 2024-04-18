# Comparing `tmp/django_safe_template_engine-1.2.0.tar.gz` & `tmp/django_safe_template_engine-1.3.0.tar.gz`

## Comparing `django_safe_template_engine-1.2.0.tar` & `django_safe_template_engine-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/.flake8
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/isort.cfg
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/mypy.ini
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/run_tests.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/.github/workflows/build.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/src/django_safe_template_engine/__init__.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/src/django_safe_template_engine/engine.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/src/django_safe_template_engine/trusted_filters.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/src/django_safe_template_engine/trusted_tags.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/src/django_safe_template_engine/validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/requirements.txt
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/settings.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/test_validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/filters/__init__.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/filters/test_trusted_filters.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/filters/test_untrusted_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/loaders/__init__.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/loaders/test_untrusted_loaders.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/tags/__init__.py
--rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/tags/test_trusted_tags.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/tests/tags/test_untrusted_tags.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/.gitignore
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/LICENSE
--rw-r--r--   0        0        0     9761 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12415 2020-02-02 00:00:00.000000 django_safe_template_engine-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/.flake8
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/isort.cfg
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/mypy.ini
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/run_tests.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tox.ini
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/src/django_safe_template_engine/__init__.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/src/django_safe_template_engine/engine.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/src/django_safe_template_engine/trusted_filters.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/src/django_safe_template_engine/trusted_tags.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/src/django_safe_template_engine/validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/settings.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/test_validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/filters/__init__.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/filters/test_trusted_filters.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/filters/test_untrusted_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/loaders/__init__.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/loaders/test_untrusted_loaders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/tags/__init__.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/tags/test_trusted_tags.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/tests/tags/test_untrusted_tags.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/LICENSE
+-rw-r--r--   0        0        0     8899 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/README.md
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12296 2020-02-02 00:00:00.000000 django_safe_template_engine-1.3.0/PKG-INFO
```

### Comparing `django_safe_template_engine-1.2.0/CHANGELOG.md` & `django_safe_template_engine-1.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 # Changelog
 
+## 1.3.0 - 2024-04-18
+
+- Lower Django version requirement to 3.0
+- Lower Python version requirement to 3.7
+- Add official support for Django 3.0 to 5.0 with:
+    - Addition of automated test coverage
+    - Review of all the built-in template tags and filters (no changes needed)
+- Use [tox](https://tox.wiki/) to manage test suite environment
+
 ## 1.2.0 - 2024-04-18
 
 - Add official support for Python 3.12
 - Reformat source code with with [black](https://pypi.org/project/black/)
 - Set up project for PyPi release
     - Update `pyproject.toml` with build system and other details for PyPi
     - Add contributing guidelines to `README.md`
 - Add `.git-blame-ignore-revs` with revisions to ignore in `git blame`
 - Sort filters by alphabetical order in the documentation and source code
 
 ## 1.1.0 - 2024-02-04
 
 - Add official support for Django 3.2:
-    - Use Django 3.2 in technical tests
+    - Use Django 3.2 in automated tests
     - Review all the Django 3.2 built-in template tags and filters (no changes needed)
 - Drop official support for Django 3.0 (still unofficially supported in this version as there are no breaking changes)
 - Remove Python 3.7 from supported versions in `pyproject.toml` (never officially supported)
 - Start keeping a changelog in `CHANGELOG.md`
 
 ## 1.0.0 - 2023-08-10
 
 - Review all the Django 3.0 built-in template tags and filters:
     - Allow the ones considered safe
     - Make sure the rest is forbidden with technical test coverage
-- Add official support for Python 3.8 to Python 3.11 (covered by technical tests)
-- Add official support for Django 3.0 (covered by technical tests)
+- Add official support for Python 3.8 to Python 3.11 (covered by automated tests)
+- Add official support for Django 3.0 (covered by automated tests)
```

### Comparing `django_safe_template_engine-1.2.0/src/django_safe_template_engine/trusted_filters.py` & `django_safe_template_engine-1.3.0/src/django_safe_template_engine/trusted_filters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django import VERSION
 from django.template.defaultfilters import (
     add,
     addslashes,
     capfirst,
     center,
     cut,
     date,
@@ -69,14 +70,20 @@
 register.filter(default_if_none, is_safe=False)
 register.filter(default, is_safe=False)
 register.filter(dictsort, is_safe=False)
 register.filter(dictsortreversed, is_safe=False)
 register.filter(divisibleby, is_safe=False)
 register.filter("escape", escape_filter, is_safe=True)
 register.filter("escapejs", escapejs_filter)
+
+if VERSION[0] == 5:
+    from django.template.defaultfilters import escapeseq
+
+    register.filter(escapeseq)
+
 register.filter(filesizeformat, is_safe=True)
 register.filter(first, is_safe=False)
 register.filter(floatformat, is_safe=True)
 register.filter(force_escape, is_safe=True)
 register.filter(get_digit, is_safe=False)
 register.filter(iriencode, is_safe=True)
 register.filter(join, is_safe=True, needs_autoescape=True)
```

### Comparing `django_safe_template_engine-1.2.0/src/django_safe_template_engine/trusted_tags.py` & `django_safe_template_engine-1.3.0/src/django_safe_template_engine/trusted_tags.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/tests/test_validators.py` & `django_safe_template_engine-1.3.0/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/tests/filters/test_trusted_filters.py` & `django_safe_template_engine-1.3.0/tests/filters/test_trusted_filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django import VERSION
 from django.template.base import Template
 from django.template.context import Context
 
 from django_safe_template_engine.engine import SafeTemplateEngine
 
 
 class TestTrustedFilters:
@@ -42,21 +43,35 @@
             context={"value": False},
         )
         assert result == expected
 
     # TODO: Write test for dictsort
     # TODO: Write test for dictsortreversed
     # TODO: Write test for divisibleby
-    # TODO: Write test for escape
+
+    def test_trust_escape(self):
+        expected = "&lt;b&gt;T&amp;Cs&lt;/b&gt;"
+        result = self._render("{{ value|escape }}", context={"value": "<b>T&Cs</b>"})
+        assert result == expected
 
     def test_trust_escapejs(self):
         expected = "\\u003Ctest\\u0026test\\u003E"
         result = self._render('{{ "<test&test>"|escapejs }}')
         assert result == expected
 
+    if VERSION[0] == 5:
+
+        def test_trust_escapeseq(self):
+            expected = "T&amp;Cs, &#x27;Test&#x27;"
+            result = self._render(
+                '{{ value|escapeseq|join:", " }}',
+                context={"value": ["T&Cs", "'Test'"]},
+            )
+            assert result == expected
+
     # FIXME
     # def test_trust_filesizeformat(self):
     #     expected = '117.7 MB'
     #     result = self._render('{{ "123456789"|filesizeformat }}')
     #     assert result == expected
 
     def test_trust_first(self):
```

### Comparing `django_safe_template_engine-1.2.0/tests/filters/test_untrusted_filters.py` & `django_safe_template_engine-1.3.0/tests/filters/test_untrusted_filters.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/tests/loaders/test_untrusted_loaders.py` & `django_safe_template_engine-1.3.0/tests/loaders/test_untrusted_loaders.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/tests/tags/test_trusted_tags.py` & `django_safe_template_engine-1.3.0/tests/tags/test_trusted_tags.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/tests/tags/test_untrusted_tags.py` & `django_safe_template_engine-1.3.0/tests/tags/test_untrusted_tags.py`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/.gitignore` & `django_safe_template_engine-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/LICENSE` & `django_safe_template_engine-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_safe_template_engine-1.2.0/README.md` & `django_safe_template_engine-1.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 
 Django template engine to render untrusted template code
 
 ## Table of contents
 
 * __[Requirements](#requirements)__
 * __[Available tools](#available-tools)__
-  * [Template engine](#template-engine)
-  * [Validator](#validator)
+    * [Template engine](#template-engine)
+    * [Validator](#validator)
 * __[Trusted built-ins](#trusted-built-ins)__
-  * [Trusted tags](#trusted-tags)
-  * [Trusted filters](#trusted-filters)
+    * [Trusted tags](#trusted-tags)
+    * [Trusted filters](#trusted-filters)
 * __[Contribute](#contribute)__
-  * [How to contribute](#how-to-contribute)
-  * [Code formatting and tests](#code-formatting-and-tests)
-  * [Ignore code formatting revisions from git blame](#ignore-code-formatting-revisions-from-git-blame)
+    * [How to contribute](#how-to-contribute)
+    * [Code formatting and tests](#code-formatting-and-tests)
+    * [Ignore code formatting revisions from git blame](#ignore-code-formatting-revisions-from-git-blame)
 
 ## Requirements
 
-- Python 3.8 to 3.12
-- Django 3.2 (officially supported in automated tests, all built-in template tags and filters reviewed)
+Django 3.0 to 5.0
 
 ## Available tools
 
 ### Template engine
 
 ```py
 from django.template import Template
@@ -46,151 +45,110 @@
 
 ## Trusted built-ins
 
 The following tags and filters are allowed by this template engine.
 
 ### Trusted tags
 
-- [`autoescape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#autoescape)
-- [`comment`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#comment)
-- [`cycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cycle)
-- [`filter`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filter)
-- [`firstof`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#firstof)
-- [`for`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for)
-- [`for … empty`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for-empty)
-- [`if`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#if)
-- [`ifchanged`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ifchanged)
-- [`lorem`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lorem)
-- [`now`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#now)
-- [`regroup`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#regroup)
-- [`resetcycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#resetcycle)
-- [`spaceless`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#spaceless)
-- [`templatetag`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#templatetag)
-- [`url`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#url)
-- [`verbatim`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#verbatim)
-- [`widthratio`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#widthratio)
-- [`with`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#with)
+- [`autoescape`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#autoescape)
+- [`comment`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#comment)
+- [`cycle`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#cycle)
+- [`filter`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#filter)
+- [`firstof`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#firstof)
+- [`for`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#for)
+- [`for … empty`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#for-empty)
+- [`if`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#if)
+- [`ifchanged`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#ifchanged)
+- [`lorem`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#lorem)
+- [`now`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#now)
+- [`regroup`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#regroup)
+- [`resetcycle`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#resetcycle)
+- [`spaceless`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#spaceless)
+- [`templatetag`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#templatetag)
+- [`url`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#url)
+- [`verbatim`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#verbatim)
+- [`widthratio`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#widthratio)
+- [`with`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#with)
 
 ### Trusted filters
 
 <!-- TODO: Check for dead links -->
-- [`add`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#add)
-- [`addslashes`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#addslashes)
-- [`capfirst`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#capfirst)
-- [`center`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#center)
-- [`cut`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cut)
-- [`date`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#date)
-- [`default_if_none`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default_if_none)
-- [`default`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default)
-- [`dictsort`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsort)
-- [`dictsortreversed`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsortreversed)
-- [`divisibleby`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#divisibleby)
-- [`escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escape)
-- [`escapejs`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escapejs)
-- [`filesizeformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filesizeformat)
-- [`first`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#first)
-- [`floatformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#floatformat)
-- [`force_escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#force_escape)
-- [`get_digit`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#get_digit)
-- [`iriencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#iriencode)
-- [`join`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#join)
-- [`json_script`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#json_script)
-- [`last`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#last)
-- [`length_is`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length_is)
-- [`length`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length)
-- [`linebreaks`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaks)
-- [`linebreaksbr`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaksbr)
-- [`linenumbers`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linenumbers)
-- [`ljust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ljust)
-- [`lower`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lower)
-- [`make_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#make_list)
-- [`phone2numeric`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#phone2numeric)
-- [`pluralize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#pluralize)
-- [`random`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#random)
-- [`rjust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#rjust)
-- [`safe`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safe)
-- [`safeseq`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safeseq)
-- [`slice`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slice)
-- [`slugify`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slugify)
-- [`stringformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#stringformat)
-- [`striptags`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#striptags)
-- [`time`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#time)
-- [`timesince`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timesince)
-- [`timeuntil`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timeuntil)
-- [`title`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#title)
-- [`truncatechars_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars_html)
-- [`truncatechars`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars)
-- [`truncatewords_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords_html)
-- [`truncatewords`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords)
-- [`unordered_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#unordered_list)
-- [`upper`](https://docs.djangopr§oject.com/en/3.2/ref/templates/builtins/#upper)
-- [`urlencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlencode)
-- [`urlize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlize)
-- [`urlizetrunc`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlizetrunc)
-- [`wordcount`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordcount)
-- [`wordwrap`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordwrap)
-- [`yesno`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#yesno)
+- [`add`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#add)
+- [`addslashes`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#addslashes)
+- [`capfirst`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#capfirst)
+- [`center`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#center)
+- [`cut`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#cut)
+- [`date`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#date)
+- [`default_if_none`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#default_if_none)
+- [`default`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#default)
+- [`dictsort`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#dictsort)
+- [`dictsortreversed`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#dictsortreversed)
+- [`divisibleby`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#divisibleby)
+- [`escape`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#escape)
+- [`escapejs`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#escapejs)
+- [`filesizeformat`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#filesizeformat)
+- [`first`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#first)
+- [`floatformat`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#floatformat)
+- [`force_escape`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#force_escape)
+- [`get_digit`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#get_digit)
+- [`iriencode`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#iriencode)
+- [`join`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#join)
+- [`json_script`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#json_script)
+- [`last`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#last)
+- [`length_is`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#length_is)
+- [`length`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#length)
+- [`linebreaks`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#linebreaks)
+- [`linebreaksbr`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#linebreaksbr)
+- [`linenumbers`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#linenumbers)
+- [`ljust`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#ljust)
+- [`lower`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#lower)
+- [`make_list`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#make_list)
+- [`phone2numeric`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#phone2numeric)
+- [`pluralize`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#pluralize)
+- [`random`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#random)
+- [`rjust`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#rjust)
+- [`safe`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#safe)
+- [`safeseq`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#safeseq)
+- [`slice`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#slice)
+- [`slugify`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#slugify)
+- [`stringformat`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#stringformat)
+- [`striptags`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#striptags)
+- [`time`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#time)
+- [`timesince`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#timesince)
+- [`timeuntil`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#timeuntil)
+- [`title`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#title)
+- [`truncatechars_html`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatechars_html)
+- [`truncatechars`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatechars)
+- [`truncatewords_html`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatewords_html)
+- [`truncatewords`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatewords)
+- [`unordered_list`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#unordered_list)
+- [`upper`](https://docs.djangopr§oject.com/en/4.2/ref/templates/builtins/#upper)
+- [`urlencode`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#urlencode)
+- [`urlize`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#urlize)
+- [`urlizetrunc`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#urlizetrunc)
+- [`wordcount`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#wordcount)
+- [`wordwrap`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#wordwrap)
+- [`yesno`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#yesno)
 
 ## Contribute
 
 ### How to contribute
 
 You want to add awesome features to Django Safe Template Engine? Here's how!
 
 1. [Fork](https://github.com/ronanboiteau/django_safe_template_engine/fork) this repository
 2. Commit and push to your forked repository
 3. Open a [pull request](https://github.com/ronanboiteau/django_safe_template_engine/pulls) to merge your work into this repository
 
 ### Code formatting and tests
 
-Here is how to run the code formatting / type checking tools, and run the test suite.
-
-1. [Recommended] Create a Python venv for this repository:
-
-    ```sh
-    python3 -m venv .venv
-    source .venv/bin/activate
-    ```
-
-2. Install the dependencies:
-
-    ```sh
-    cd tests/ && pip install -r requirements.txt && cd ..
-    ```
-
-3. Run the code formatting tools:
-
-    [`black`](https://pypi.org/project/black/) code formatter:
-
-    ```sh
-    black src tests
-    ```
-
-    [`isort`](https://pypi.org/project/isort/) import sorter:
-
-    ```sh
-    isort --settings-path isort.cfg src tests
-    ```
-
-    [`flake8`](https://pypi.org/project/flake8/) coding style checker:
-
-    ```sh
-    flake8 --config .flake8 src tests
-    ```
-
-    [`mypy`](https://pypi.org/project/mypy/) type checker:
-
-    ```sh
-    mypy --config-file mypy.ini src tests
-    ```
-
-4. Run the test suite:
+You can use [tox](https://tox.wiki/) to run the code formatting / type checking tools, and run the test suite:
 
     ```sh
-    python run_tests.py
+    tox run
     ```
 
 ### Ignore code formatting revisions from git blame
 
 For a more relevant git blame you can set up your git to use the file [`.git-blame-ignore-revs`](.git-blame-ignore-revs) in [`blame.ignoreRevsFile`](https://www.git-scm.com/docs/git-blame#Documentation/git-blame.txt---ignore-revs-fileltfilegt):
 
 ```sh
```

### Comparing `django_safe_template_engine-1.2.0/PKG-INFO` & `django_safe_template_engine-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django_safe_template_engine
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Django template engine to render untrusted template code
 Project-URL: Documentation, https://github.com/ronanboiteau/django_safe_template_engine/blob/main/README.md
 Project-URL: Repository, https://github.com/ronanboiteau/django_safe_template_engine.git
 Project-URL: Issues, https://github.com/ronanboiteau/django_safe_template_engine/issues
 Project-URL: Changelog, https://github.com/ronanboiteau/django_safe_template_engine/blob/main/CHANGELOG.md
 Author-email: Ronan Boiteau <ronan@boiteau.eu>
 Maintainer-email: Ronan Boiteau <ronan@boiteau.eu>
@@ -34,45 +34,61 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Keywords: django,engine,safe,template
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: django<4,>=3.2
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Requires-Dist: django>=3.0
 Description-Content-Type: text/markdown
 
 ![GitHub Actions build status](https://github.com/ronanboiteau/django_safe_template_engine/actions/workflows/build.yml/badge.svg?branch=main)
 
 # Django Safe Template Engine
 
 Django template engine to render untrusted template code
 
 ## Table of contents
 
 * __[Requirements](#requirements)__
 * __[Available tools](#available-tools)__
-  * [Template engine](#template-engine)
-  * [Validator](#validator)
+    * [Template engine](#template-engine)
+    * [Validator](#validator)
 * __[Trusted built-ins](#trusted-built-ins)__
-  * [Trusted tags](#trusted-tags)
-  * [Trusted filters](#trusted-filters)
+    * [Trusted tags](#trusted-tags)
+    * [Trusted filters](#trusted-filters)
 * __[Contribute](#contribute)__
-  * [How to contribute](#how-to-contribute)
-  * [Code formatting and tests](#code-formatting-and-tests)
-  * [Ignore code formatting revisions from git blame](#ignore-code-formatting-revisions-from-git-blame)
+    * [How to contribute](#how-to-contribute)
+    * [Code formatting and tests](#code-formatting-and-tests)
+    * [Ignore code formatting revisions from git blame](#ignore-code-formatting-revisions-from-git-blame)
 
 ## Requirements
 
-- Python 3.8 to 3.12
-- Django 3.2 (officially supported in automated tests, all built-in template tags and filters reviewed)
+Django 3.0 to 5.0
 
 ## Available tools
 
 ### Template engine
 
 ```py
 from django.template import Template
@@ -93,151 +109,110 @@
 
 ## Trusted built-ins
 
 The following tags and filters are allowed by this template engine.
 
 ### Trusted tags
 
-- [`autoescape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#autoescape)
-- [`comment`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#comment)
-- [`cycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cycle)
-- [`filter`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filter)
-- [`firstof`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#firstof)
-- [`for`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for)
-- [`for … empty`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#for-empty)
-- [`if`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#if)
-- [`ifchanged`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ifchanged)
-- [`lorem`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lorem)
-- [`now`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#now)
-- [`regroup`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#regroup)
-- [`resetcycle`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#resetcycle)
-- [`spaceless`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#spaceless)
-- [`templatetag`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#templatetag)
-- [`url`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#url)
-- [`verbatim`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#verbatim)
-- [`widthratio`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#widthratio)
-- [`with`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#with)
+- [`autoescape`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#autoescape)
+- [`comment`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#comment)
+- [`cycle`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#cycle)
+- [`filter`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#filter)
+- [`firstof`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#firstof)
+- [`for`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#for)
+- [`for … empty`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#for-empty)
+- [`if`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#if)
+- [`ifchanged`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#ifchanged)
+- [`lorem`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#lorem)
+- [`now`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#now)
+- [`regroup`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#regroup)
+- [`resetcycle`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#resetcycle)
+- [`spaceless`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#spaceless)
+- [`templatetag`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#templatetag)
+- [`url`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#url)
+- [`verbatim`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#verbatim)
+- [`widthratio`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#widthratio)
+- [`with`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#with)
 
 ### Trusted filters
 
 <!-- TODO: Check for dead links -->
-- [`add`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#add)
-- [`addslashes`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#addslashes)
-- [`capfirst`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#capfirst)
-- [`center`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#center)
-- [`cut`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#cut)
-- [`date`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#date)
-- [`default_if_none`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default_if_none)
-- [`default`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#default)
-- [`dictsort`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsort)
-- [`dictsortreversed`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#dictsortreversed)
-- [`divisibleby`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#divisibleby)
-- [`escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escape)
-- [`escapejs`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#escapejs)
-- [`filesizeformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#filesizeformat)
-- [`first`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#first)
-- [`floatformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#floatformat)
-- [`force_escape`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#force_escape)
-- [`get_digit`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#get_digit)
-- [`iriencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#iriencode)
-- [`join`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#join)
-- [`json_script`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#json_script)
-- [`last`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#last)
-- [`length_is`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length_is)
-- [`length`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#length)
-- [`linebreaks`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaks)
-- [`linebreaksbr`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linebreaksbr)
-- [`linenumbers`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#linenumbers)
-- [`ljust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#ljust)
-- [`lower`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#lower)
-- [`make_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#make_list)
-- [`phone2numeric`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#phone2numeric)
-- [`pluralize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#pluralize)
-- [`random`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#random)
-- [`rjust`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#rjust)
-- [`safe`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safe)
-- [`safeseq`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#safeseq)
-- [`slice`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slice)
-- [`slugify`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#slugify)
-- [`stringformat`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#stringformat)
-- [`striptags`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#striptags)
-- [`time`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#time)
-- [`timesince`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timesince)
-- [`timeuntil`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#timeuntil)
-- [`title`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#title)
-- [`truncatechars_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars_html)
-- [`truncatechars`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatechars)
-- [`truncatewords_html`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords_html)
-- [`truncatewords`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#truncatewords)
-- [`unordered_list`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#unordered_list)
-- [`upper`](https://docs.djangopr§oject.com/en/3.2/ref/templates/builtins/#upper)
-- [`urlencode`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlencode)
-- [`urlize`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlize)
-- [`urlizetrunc`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#urlizetrunc)
-- [`wordcount`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordcount)
-- [`wordwrap`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#wordwrap)
-- [`yesno`](https://docs.djangoproject.com/en/3.2/ref/templates/builtins/#yesno)
+- [`add`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#add)
+- [`addslashes`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#addslashes)
+- [`capfirst`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#capfirst)
+- [`center`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#center)
+- [`cut`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#cut)
+- [`date`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#date)
+- [`default_if_none`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#default_if_none)
+- [`default`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#default)
+- [`dictsort`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#dictsort)
+- [`dictsortreversed`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#dictsortreversed)
+- [`divisibleby`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#divisibleby)
+- [`escape`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#escape)
+- [`escapejs`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#escapejs)
+- [`filesizeformat`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#filesizeformat)
+- [`first`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#first)
+- [`floatformat`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#floatformat)
+- [`force_escape`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#force_escape)
+- [`get_digit`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#get_digit)
+- [`iriencode`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#iriencode)
+- [`join`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#join)
+- [`json_script`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#json_script)
+- [`last`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#last)
+- [`length_is`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#length_is)
+- [`length`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#length)
+- [`linebreaks`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#linebreaks)
+- [`linebreaksbr`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#linebreaksbr)
+- [`linenumbers`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#linenumbers)
+- [`ljust`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#ljust)
+- [`lower`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#lower)
+- [`make_list`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#make_list)
+- [`phone2numeric`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#phone2numeric)
+- [`pluralize`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#pluralize)
+- [`random`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#random)
+- [`rjust`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#rjust)
+- [`safe`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#safe)
+- [`safeseq`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#safeseq)
+- [`slice`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#slice)
+- [`slugify`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#slugify)
+- [`stringformat`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#stringformat)
+- [`striptags`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#striptags)
+- [`time`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#time)
+- [`timesince`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#timesince)
+- [`timeuntil`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#timeuntil)
+- [`title`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#title)
+- [`truncatechars_html`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatechars_html)
+- [`truncatechars`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatechars)
+- [`truncatewords_html`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatewords_html)
+- [`truncatewords`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#truncatewords)
+- [`unordered_list`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#unordered_list)
+- [`upper`](https://docs.djangopr§oject.com/en/4.2/ref/templates/builtins/#upper)
+- [`urlencode`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#urlencode)
+- [`urlize`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#urlize)
+- [`urlizetrunc`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#urlizetrunc)
+- [`wordcount`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#wordcount)
+- [`wordwrap`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#wordwrap)
+- [`yesno`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#yesno)
 
 ## Contribute
 
 ### How to contribute
 
 You want to add awesome features to Django Safe Template Engine? Here's how!
 
 1. [Fork](https://github.com/ronanboiteau/django_safe_template_engine/fork) this repository
 2. Commit and push to your forked repository
 3. Open a [pull request](https://github.com/ronanboiteau/django_safe_template_engine/pulls) to merge your work into this repository
 
 ### Code formatting and tests
 
-Here is how to run the code formatting / type checking tools, and run the test suite.
-
-1. [Recommended] Create a Python venv for this repository:
-
-    ```sh
-    python3 -m venv .venv
-    source .venv/bin/activate
-    ```
-
-2. Install the dependencies:
-
-    ```sh
-    cd tests/ && pip install -r requirements.txt && cd ..
-    ```
-
-3. Run the code formatting tools:
-
-    [`black`](https://pypi.org/project/black/) code formatter:
-
-    ```sh
-    black src tests
-    ```
-
-    [`isort`](https://pypi.org/project/isort/) import sorter:
-
-    ```sh
-    isort --settings-path isort.cfg src tests
-    ```
-
-    [`flake8`](https://pypi.org/project/flake8/) coding style checker:
-
-    ```sh
-    flake8 --config .flake8 src tests
-    ```
-
-    [`mypy`](https://pypi.org/project/mypy/) type checker:
-
-    ```sh
-    mypy --config-file mypy.ini src tests
-    ```
-
-4. Run the test suite:
+You can use [tox](https://tox.wiki/) to run the code formatting / type checking tools, and run the test suite:
 
     ```sh
-    python run_tests.py
+    tox run
     ```
 
 ### Ignore code formatting revisions from git blame
 
 For a more relevant git blame you can set up your git to use the file [`.git-blame-ignore-revs`](.git-blame-ignore-revs) in [`blame.ignoreRevsFile`](https://www.git-scm.com/docs/git-blame#Documentation/git-blame.txt---ignore-revs-fileltfilegt):
 
 ```sh
```

