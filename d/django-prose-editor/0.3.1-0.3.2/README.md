# Comparing `tmp/django_prose_editor-0.3.1.tar.gz` & `tmp/django_prose_editor-0.3.2.tar.gz`

## Comparing `django_prose_editor-0.3.1.tar` & `django_prose_editor-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/fields.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/sanitized.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/widgets.py
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/editor.css
--rw-r--r--   0        0        0   224395 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/editor.js
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/init.js
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/material-icons.css
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/material-icons.woff2
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/LICENSE
--rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/README.rst
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 django_prose_editor-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/fields.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/sanitized.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/widgets.py
+-rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/editor.css
+-rw-r--r--   0        0        0   224395 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/editor.js
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/init.js
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/material-icons.css
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/material-icons.woff2
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4358 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/README.rst
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 django_prose_editor-0.3.2/PKG-INFO
```

### Comparing `django_prose_editor-0.3.1/django_prose_editor/fields.py` & `django_prose_editor-0.3.2/django_prose_editor/fields.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,32 @@
+import re
+
 from django import forms
 from django.db import models
 from django.utils.html import strip_tags
 from django.utils.text import Truncator
 
 from django_prose_editor.widgets import ProseEditorWidget
 
 
-def _identity(x):
+def _actually_empty(x):
+    """
+    ProseMirror's schema always adds at least one empty paragraph
+
+    We want empty fields to actually be empty strings so that those field
+    values evaluate as ``False`` in a boolean context.
+    """
+    if re.match(r"^<(?P<tag>\w+)></(?P=tag)>$", x):
+        return ""
     return x
 
 
 class ProseEditorField(models.TextField):
     def __init__(self, *args, **kwargs):
-        self.sanitize = kwargs.pop("sanitize", _identity)
+        self.sanitize = kwargs.pop("sanitize", _actually_empty)
         self.config = kwargs.pop("config", {})
         super().__init__(*args, **kwargs)
 
     def clean(self, value, instance):
         return self.sanitize(super().clean(value, instance))
 
     def contribute_to_class(self, cls, name, **kwargs):
```

### Comparing `django_prose_editor-0.3.1/django_prose_editor/widgets.py` & `django_prose_editor-0.3.2/django_prose_editor/widgets.py`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/editor.css` & `django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/editor.css`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/editor.js` & `django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/editor.js`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/init.js` & `django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/init.js`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/material-icons.css` & `django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/material-icons.css`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/django_prose_editor/static/django_prose_editor/material-icons.woff2` & `django_prose_editor-0.3.2/django_prose_editor/static/django_prose_editor/material-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/LICENSE` & `django_prose_editor-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/README.rst` & `django_prose_editor-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/pyproject.toml` & `django_prose_editor-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_prose_editor-0.3.1/PKG-INFO` & `django_prose_editor-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prose-editor
-Version: 0.3.1
+Version: 0.3.2
 Summary: Prose editor for the Django admin based on ProseMirror
 Project-URL: Homepage, https://github.com/matthiask/django-prose-editor/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

