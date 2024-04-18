# Comparing `tmp/django_includecontents-0.3.tar.gz` & `tmp/django_includecontents-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_includecontents-0.3.tar", last modified: Tue Apr  9 21:53:12 2024, max compression
+gzip compressed data, was "django_includecontents-0.4.tar", last modified: Thu Apr 18 04:25:32 2024, max compression
```

## Comparing `django_includecontents-0.3.tar` & `django_includecontents-0.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     3801 2024-04-09 21:50:46.122302 django_includecontents-0.3/README.md
--rw-r--r--   0        0        0     1218 2024-04-09 21:53:12.195867 django_includecontents-0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.3/src/djangox/__init__.py
--rw-r--r--   0        0        0      144 2024-04-09 04:42:05.196722 django_includecontents-0.3/tests/settings.py
--rw-r--r--   0        0        0      181 2024-04-09 04:42:05.196722 django_includecontents-0.3/tests/templates/components/card.html
--rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.3/tests/templates/multiline.html
--rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.3/tests/templates/test_component/attrs.html
--rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.3/tests/templates/test_component/index.html
--rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.3/tests/templates/test_component/missing_attr.html
--rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.3/tests/templates/test_component/missing_closing_tag.html
--rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.3/tests/templates/test_tag/basic.html
--rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.3/tests/templates/test_tag/inner.html
--rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.3/tests/templates/test_tag/with_attr.html
--rw-r--r--   0        0        0     1013 2024-04-09 21:50:46.125635 django_includecontents-0.3/tests/test_component.py
--rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.3/tests/test_multiline.py
--rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.3/tests/test_tag.py
--rw-r--r--   0        0        0     4815 1970-01-01 00:00:00.000000 django_includecontents-0.3/PKG-INFO
+-rw-r--r--   0        0        0     4998 2024-04-18 04:23:29.581817 django_includecontents-0.4/README.md
+-rw-r--r--   0        0        0     1218 2024-04-18 04:25:32.355405 django_includecontents-0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-08 01:37:55.796699 django_includecontents-0.4/src/djangox/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-09 04:42:05.196722 django_includecontents-0.4/tests/settings.py
+-rw-r--r--   0        0        0      168 2024-04-18 02:43:29.856564 django_includecontents-0.4/tests/templates/components/card.html
+-rw-r--r--   0        0        0      160 2024-04-18 03:09:23.179458 django_includecontents-0.4/tests/templates/components/card_extend.html
+-rw-r--r--   0        0        0       81 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/templates/multiline.html
+-rw-r--r--   0        0        0      115 2024-04-09 21:50:46.125635 django_includecontents-0.4/tests/templates/test_component/attrs.html
+-rw-r--r--   0        0        0      162 2024-04-18 03:24:57.041361 django_includecontents-0.4/tests/templates/test_component/extend_class.html
+-rw-r--r--   0        0        0       73 2024-04-09 21:50:46.125635 django_includecontents-0.4/tests/templates/test_component/index.html
+-rw-r--r--   0        0        0       34 2024-04-09 21:51:49.385743 django_includecontents-0.4/tests/templates/test_component/missing_attr.html
+-rw-r--r--   0        0        0       24 2024-04-09 21:51:57.449090 django_includecontents-0.4/tests/templates/test_component/missing_closing_tag.html
+-rw-r--r--   0        0        0      118 2024-04-09 21:50:46.115635 django_includecontents-0.4/tests/templates/test_tag/basic.html
+-rw-r--r--   0        0        0       57 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/templates/test_tag/inner.html
+-rw-r--r--   0        0        0      135 2024-04-09 21:50:46.115635 django_includecontents-0.4/tests/templates/test_tag/with_attr.html
+-rw-r--r--   0        0        0     1478 2024-04-18 04:13:01.650516 django_includecontents-0.4/tests/test_component.py
+-rw-r--r--   0        0        0      130 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/test_multiline.py
+-rw-r--r--   0        0        0      454 2024-04-09 04:52:09.297567 django_includecontents-0.4/tests/test_tag.py
+-rw-r--r--   0        0        0     6012 1970-01-01 00:00:00.000000 django_includecontents-0.4/PKG-INFO
```

### Comparing `django_includecontents-0.3/pyproject.toml` & `django_includecontents-0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-includecontents"
-version = "0.3"
+version = "0.4"
 description = "Django includecontents component-like tag"
 authors = [
     { name = "Chris Beaven", email = "smileychris@gmail.com" },
 ]
 dependencies = [
     "django",
 ]
```

### Comparing `django_includecontents-0.3/tests/test_component.py` & `django_includecontents-0.4/tests/test_component.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
     )
 
 
 def test_attrs():
     assert render_to_string("test_component/attrs.html") == (
         """<main>
-  <section id="topcard" class="mycard">
+  <section class="mycard" id="topcard">
   <h3 class="large">hello</h3>
   <div>
     some content
   </div>
 </section>
 </main>
 """
@@ -41,7 +41,33 @@
 
 def test_missing_closing_tag():
     with pytest.raises(
         TemplateSyntaxError,
         match=re.compile(r"Unclosed tag.*<include:card>.*</include:card>"),
     ):
         render_to_string("test_component/missing_closing_tag.html")
+
+
+def test_extend_class():
+    assert render_to_string("test_component/extend_class.html") == (
+        """<main>
+  <section class="mycard card lg">
+  <h3 >hello</h3>
+  <div>
+    some content
+  </div>
+</section>
+</main>
+"""
+    )
+
+    assert render_to_string("test_component/extend_class.html", {"red": True}) == (
+        """<main>
+  <section class="mycard card lg">
+  <h3 class="text-red">hello</h3>
+  <div>
+    some content
+  </div>
+</section>
+</main>
+"""
+    )
```

### Comparing `django_includecontents-0.3/PKG-INFO` & `django_includecontents-0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,14 @@
-Metadata-Version: 2.1
-Name: django-includecontents
-Version: 0.3
-Summary: Django includecontents component-like tag
-Author-Email: Chris Beaven <smileychris@gmail.com>
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Classifier: Framework :: Django :: 5.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Repository, https://github.com/SmileyChris/django-includecontents
-Requires-Python: >=3.8
-Requires-Dist: django
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-django; extra == "test"
-Provides-Extra: test
-Description-Content-Type: text/markdown
-
 # Django IncludeContents tag
 
 Provides a component-like `{% includecontents %}` tag to Django.
 
 For example:
 
-```html
+```jinja
 {% load includecontents %}
 {% includecontents "hello.html" %}
     <p>World</p>
 {% endincludecontents %}
 ```
 
 It also provides a simple Django template engine that extends this tag to work
@@ -46,15 +20,15 @@
 <include:card title="Hello">
   <p>World</p>
 </include:card>
 ```
 
 This engine also allows for multi-line template tags. For example:
 
-```html
+```jinja
 {% if 
   user.is_authenticated
   and user.is_staff
 %}
 ...
 {% endif %}
 ```
@@ -83,48 +57,48 @@
 ```python
 INSTALLED_APPS = [
     ...
     'includecontents',
 ]
 ```
 
-```html
+```jinja
 {% load includecontents %}
 
 ...
 
 {% includecontents %}...{% endincludecontents %}
 ```
 
 ## Template tag usage
 
 The `includecontents` tag works like the `include` tag but the contents is rendered and passed to the included template as a `contents` variable.
 
-```html
+```jinja
 {% includecontents "hello.html" %}
     <p>World</p>
 {% endincludecontents %}
 ```
 
 ### Named contents blocks
 
 You can also have named contents blocks within the component content.
 
 For example:
 
-```html
+```jinja
 {% includecontents "hello.html" %}
     <p>World</p>
     {% contents footer %}Footer{% endcontents %}
 {% endincludecontents %}
 ```
 
 Where `hello.html` template could look something like:
 
-```html
+```jinja
 <div class="card">
   <div class="content">
     {{ contents }}
   </div>
   {% if contents.footer %}
   <div class="footer">
     {{ contents.footer }}
@@ -157,27 +131,70 @@
 <include:card title="Hello">
   <p>World</p>
 </include:card>
 ```
 
 You can use named [`{% contents %}` blocks](#named-contents-blocks), just like with the `includecontents` tag.
 
-### Attrs
+Some HTML formatters (like prettier) insist on quoting HTML attribute values, you can avoid this by wrapping template values in `{}`:
 
-You can define which attributes should be passed to the component in a comment at the top of the component template, and others that can have a default value.
+```html
+<include:card title={mytitle}></include:card>
+``` 
 
-Any other attributes passed to the component will be added to an `attrs` context variable that can render them as HTML attributes.
-You can also provide default values for these attributes via the `default_attrs` filter.
+### Component Props
 
-```html
-{# def title, large=False #}
-<div {{ attrs|default_attrs:'class="card"' }}>
+You can define the required or default props of the component in a comment at the top of its template that begins with `props `  (or `def ` to match what JinjaX uses). An exception will be raised if a required prop is not provided.
+
+Any other attributes passed to the component that are not listed in this definition will be added to an `attrs` context variable that can render them as HTML attributes.
+
+```jinja
+{# props #}
+<div {{ attrs }}>
+  {{ contents }}
+</div>
+```
+
+You can also provide default values for these attributes via the `{% attrs %}` template tag.
+
+```jinja
+{# props title, large=False #}
+
+<div {% attrs class="card" %}>
+...
 ```
 
-This would require a `title` attribute and allow an optional `large` attribute. Any other attributes will be rendered on the div, with a default class of `card` if you don't specify any other class.
-So the following tags would all be valid:
+This example component above would require a `title` attribute and allow an optional `large` attribute. Any other attributes will be rendered on the div, with a default class of `card` if you don't specify a class attribute.
+
+If you want to provide multiple groups of undefined attributes, you can use `group.name` as the format.
+Then render them with `{{ attrs.group }}` (or `{% attrs.group %}` if you want fallback values).
+
+For example to call a component like this:
 
 ```html
-<include:card title="Hello"></include:card>
-<include:card title="Hello" large></include:card>
-<include:card title="Hello" id="topcard" class="my-card"></include:card>
-```
+<include:field label="Name" name="first_name" value="John" input.class="wide"></include:field>
+```
+
+It could be defined like this:
+
+```jinja
+{# props value, label="" #}
+
+<div {% attrs class="field" %}>
+  {% if label %}{{ '<label>'|safe }}{% endif %}
+  {{ label }}
+  <input {% attrs.input type="text" value=value %}>
+  {% if label %}{{ '</label>'|safe }}{% endif %}
+</div>
+```
+
+#### Conditional classes
+
+You can also provide conditional classes for the `class` attribute using the following format:
+
+```jinja
+{# props large=False #}
+
+{% attrs class="lg" %}     {# sets class attribute to "lg" but can be overridden #}
+{% attrs class:lg %}       {# always adds 'lg' class #}
+{% attrs class:lg=large %} {# adds 'lg' class if large prop is truthy #}
+```
```

