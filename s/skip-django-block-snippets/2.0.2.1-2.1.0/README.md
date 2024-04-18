# Comparing `tmp/skip-django-block-snippets-2.0.2.1.tar.gz` & `tmp/skip_django_block_snippets-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-block-snippets-2.0.2.1.tar", last modified: Mon Jan 16 00:50:55 2023, max compression
+gzip compressed data, was "skip_django_block_snippets-2.1.0.tar", last modified: Thu Apr 18 13:42:34 2024, max compression
```

## Comparing `skip-django-block-snippets-2.0.2.1.tar` & `skip_django_block_snippets-2.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.646340 skip-django-block-snippets-2.0.2.1/block_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.642340 skip-django-block-snippets-2.0.2.1/block_snippets/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.642340 skip-django-block-snippets-2.0.2.1/block_snippets/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.646340 skip-django-block-snippets-2.0.2.1/block_snippets/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.646340 skip-django-block-snippets-2.0.2.1/block_snippets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/templatetags/snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/block_snippets/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.646340 skip-django-block-snippets-2.0.2.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.646340 skip-django-block-snippets-2.0.2.1/example/dj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.646340 skip-django-block-snippets-2.0.2.1/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/tests/snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/apps/app/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/dj/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/example/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-01-16 00:50:46.000000 skip-django-block-snippets-2.0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 00:50:55.650340 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-01-16 00:50:55.000000 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-01-16 00:50:55.000000 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 00:50:55.000000 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 00:50:55.000000 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-16 00:50:55.000000 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-16 00:50:55.000000 skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.643451 skip_django_block_snippets-2.1.0/block_snippets/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.643451 skip_django_block_snippets-2.1.0/block_snippets/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.643451 skip_django_block_snippets-2.1.0/block_snippets/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.643451 skip_django_block_snippets-2.1.0/block_snippets/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.643451 skip_django_block_snippets-2.1.0/block_snippets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/templatetags/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/block_snippets/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.643451 skip_django_block_snippets-2.1.0/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/example/dj/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/apps/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/apps/app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/example/dj/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/apps/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/apps/app/tests/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/apps/app/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/dj/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/example/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-18 13:42:31.000000 skip_django_block_snippets-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 13:42:34.647451 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-18 13:42:34.000000 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-18 13:42:34.000000 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:42:34.000000 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 13:42:34.000000 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 13:42:34.000000 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 13:42:34.000000 skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/top_level.txt
```

### Comparing `skip-django-block-snippets-2.0.2.1/LICENSE` & `skip_django_block_snippets-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-block-snippets-2.0.2.1/PKG-INFO` & `skip_django_block_snippets-2.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-block-snippets
-Version: 2.0.2.1
+Version: 2.1.0
 Summary: Django block snippets.
 Home-page: https://github.com/skip-pay/django-block-snippets
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,snippets
 Classifier: Development Status :: 3 - Alpha
@@ -15,7 +15,8 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 License-File: LICENSE
+Requires-Dist: django>=4.2
```

### Comparing `skip-django-block-snippets-2.0.2.1/block_snippets/locale/cs/LC_MESSAGES/django.po` & `skip_django_block_snippets-2.1.0/block_snippets/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-block-snippets-2.0.2.1/block_snippets/response.py` & `skip_django_block_snippets-2.1.0/block_snippets/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import json
 
 from block_snippets.utils import clean_html
 
-from django.utils.translation import ugettext
+from django.utils.translation import gettext
 from django.template.response import TemplateResponse
 from django.http.response import Http404
 from django.utils.html import escape
 
 
 class SnippetsTemplateResponse(TemplateResponse):
 
     def __init__(self, *args, **kwargs):
         self.snippet_names = kwargs.pop('snippet_names', None)
         super(SnippetsTemplateResponse, self).__init__(*args, **kwargs)
 
     def render_snippet(self, context, snippet_name):
         snippet_template = context.render_context.get('snippets', {}).get(snippet_name)
         if snippet_template is None:
-            raise Http404(ugettext('Invalid snippet name "{}"').format(escape(snippet_name)))
+            raise Http404(gettext('Invalid snippet name "{}"').format(escape(snippet_name)))
 
         return snippet_template._rendered_context if snippet_template is not None else None
 
     @property
     def rendered_content(self):
         template = self.resolve_template(self.template_name)
         context = self.resolve_context(self.context_data)
```

### Comparing `skip-django-block-snippets-2.0.2.1/block_snippets/templatetags/snippets.py` & `skip_django_block_snippets-2.1.0/block_snippets/templatetags/snippets.py`

 * *Files identical despite different names*

### Comparing `skip-django-block-snippets-2.0.2.1/block_snippets/views.py` & `skip_django_block_snippets-2.1.0/block_snippets/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-block-snippets-2.0.2.1/example/dj/apps/app/tests/snippets.py` & `skip_django_block_snippets-2.1.0/example/dj/apps/app/tests/snippets.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,70 @@
 import json
 
-from django.utils.encoding import force_text
+from django.utils.encoding import force_str
 
 from germanium.tools import assert_equal, assert_http_not_found
 from germanium.test_cases.client import ClientTestCase
 
 
 class SnippetTestCase(ClientTestCase):
 
     SNIPPET_URL = '/snippet/'
     JSON_SNIPPET_URL = '/json-snippet/'
 
     def test_return_snippet_content_without_snippet(self):
         resp = self.get(self.SNIPPET_URL)
         assert_equal(
-            force_text(resp.content),
+            force_str(resp.content),
             '<div class="snippet snippet-1" data-snippet="test-snippet-1" data-snippet-type="replace">'
             'test-snippet-1-content</div><div class="snippet snippet-2" data-snippet="test-snippet-2" '
             'data-snippet-type="replace">test-snippet-2-content</div>'
         )
         assert_equal(resp['content-type'], 'text/html; charset=utf-8')
 
     def test_return_json_snippet_content_without_snippet(self):
         resp = self.get(self.JSON_SNIPPET_URL)
         assert_equal(
-            force_text(resp.content),
+            force_str(resp.content),
             '<div class="snippet snippet-1" data-snippet="test-snippet-1" data-snippet-type="replace">'
             'test-snippet-1-content</div><div class="snippet snippet-2" data-snippet="test-snippet-2" '
             'data-snippet-type="replace">test-snippet-2-content</div>'
         )
         assert_equal(resp['content-type'], 'text/html; charset=utf-8')
 
     def test_return_snippet_content_with_snippet(self):
         resp = self.get(self.SNIPPET_URL + '?snippet=test-snippet-1')
-        assert_equal(force_text(resp.content), 'test-snippet-1-content')
+        assert_equal(force_str(resp.content), 'test-snippet-1-content')
         assert_equal(resp['content-type'], 'text/html; charset=utf-8')
 
         resp = self.get(self.SNIPPET_URL + '?snippet=test-snippet-2')
-        assert_equal(force_text(resp.content), 'test-snippet-2-content')
+        assert_equal(force_str(resp.content), 'test-snippet-2-content')
         assert_equal(resp['content-type'], 'text/html; charset=utf-8')
 
         resp = self.get(self.SNIPPET_URL + '?snippet=test-snippet-2&snippet=test-snippet-1')
-        assert_equal(force_text(resp.content), 'test-snippet-2-content')
+        assert_equal(force_str(resp.content), 'test-snippet-2-content')
         assert_equal(resp['content-type'], 'text/html; charset=utf-8')
 
         resp = self.get(self.SNIPPET_URL + '?snippet=test-snippet-1&snippet=test-snippet-2')
-        assert_equal(force_text(resp.content), 'test-snippet-1-content')
+        assert_equal(force_str(resp.content), 'test-snippet-1-content')
         assert_equal(resp['content-type'], 'text/html; charset=utf-8')
 
     def test_return_json_snippet_content_with_snippet(self):
         resp = self.get(self.JSON_SNIPPET_URL + '?snippet=test-snippet-1')
-        assert_equal(json.loads(force_text(resp.content)).get('snippets').get('test-snippet-1'),
+        assert_equal(json.loads(force_str(resp.content)).get('snippets').get('test-snippet-1'),
                      'test-snippet-1-content')
         assert_equal(resp['content-type'], 'text/plain')
 
         resp = self.get(self.JSON_SNIPPET_URL + '?snippet=test-snippet-2')
-        assert_equal(json.loads(force_text(resp.content)).get('snippets').get('test-snippet-2'),
+        assert_equal(json.loads(force_str(resp.content)).get('snippets').get('test-snippet-2'),
                      'test-snippet-2-content')
         assert_equal(resp['content-type'], 'text/plain')
 
         resp = self.get(self.JSON_SNIPPET_URL + '?snippet=test-snippet-2&snippet=test-snippet-1')
-        assert_equal(json.loads(force_text(resp.content)).get('snippets').get('test-snippet-1'),
+        assert_equal(json.loads(force_str(resp.content)).get('snippets').get('test-snippet-1'),
                      'test-snippet-1-content')
-        assert_equal(json.loads(force_text(resp.content)).get('snippets').get('test-snippet-2'),
+        assert_equal(json.loads(force_str(resp.content)).get('snippets').get('test-snippet-2'),
                      'test-snippet-2-content')
         assert_equal(resp['content-type'], 'text/plain')
 
     def test_bad_request_for_invalid_snippet_name_should_be_returned(self):
         assert_http_not_found(self.get(self.JSON_SNIPPET_URL + '?snippet=invalid'))
```

### Comparing `skip-django-block-snippets-2.0.2.1/example/dj/settings/base.py` & `skip_django_block_snippets-2.1.0/example/dj/settings/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django settings.
 import os
 
 try:
-    from django.utils.translation import ugettext_lazy as _
+    from django.utils.translation import gettext_lazy as _
 except ImportError:
     def _(val): return val
 
 PROJECT_DIR = os.path.abspath(
     os.path.join(os.path.dirname(__file__), '..', '..')
 )
```

### Comparing `skip-django-block-snippets-2.0.2.1/example/dj/wsgi.py` & `skip_django_block_snippets-2.1.0/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-block-snippets-2.0.2.1/setup.py` & `skip_django_block_snippets-2.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,11 +24,11 @@
         'Natural Language :: Czech',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Internet :: WWW/HTTP :: Site Management',
     ],
     install_requires=[
-        'django>=1.10',
+        'django>=4.2',
     ],
     zip_safe=False
 )
```

### Comparing `skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/PKG-INFO` & `skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-block-snippets
-Version: 2.0.2.1
+Version: 2.1.0
 Summary: Django block snippets.
 Home-page: https://github.com/skip-pay/django-block-snippets
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,snippets
 Classifier: Development Status :: 3 - Alpha
@@ -15,7 +15,8 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: Czech
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management
 License-File: LICENSE
+Requires-Dist: django>=4.2
```

### Comparing `skip-django-block-snippets-2.0.2.1/skip_django_block_snippets.egg-info/SOURCES.txt` & `skip_django_block_snippets-2.1.0/skip_django_block_snippets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

