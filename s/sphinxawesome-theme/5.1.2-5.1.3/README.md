# Comparing `tmp/sphinxawesome_theme-5.1.2.tar.gz` & `tmp/sphinxawesome_theme-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-5.1.2.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.1.3.tar", max compression
```

## Comparing `sphinxawesome_theme-5.1.2.tar` & `sphinxawesome_theme-5.1.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1066 2024-04-18 11:38:12.271352 sphinxawesome_theme-5.1.2/LICENSE
--rw-r--r--   0        0        0     2294 2024-04-18 11:38:12.271352 sphinxawesome_theme-5.1.2/README.md
--rw-r--r--   0        0        0     2683 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/pyproject.toml
--rw-r--r--   0        0        0     7311 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     4166 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/deprecated.py
--rw-r--r--   0        0        0     1394 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2841 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/genindex.html
--rw-r--r--   0        0        0     7675 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12751 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0     1013 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1192 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     5135 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     3242 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/logos.py
--rw-r--r--   0        0        0      895 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7816 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0     1603 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      656 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      932 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1226 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     2462 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      416 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar_main_nav_links.html
--rw-r--r--   0        0        0      256 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar_toc.html
--rw-r--r--   0        0        0    30104 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/06b2bbbc4b7413514f6a.woff
--rw-r--r--   0        0        0    21956 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
--rw-r--r--   0        0        0    21088 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
--rw-r--r--   0        0        0    28620 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
--rw-r--r--   0        0        0    23072 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
--rw-r--r--   0        0        0    23148 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
--rw-r--r--   0        0        0    30232 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
--rw-r--r--   0        0        0    29416 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
--rw-r--r--   0        0        0    28636 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
--rw-r--r--   0        0        0    22188 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
--rw-r--r--   0        0        0    21820 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
--rw-r--r--   0        0        0     4495 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-docsearch.css
--rw-r--r--   0        0        0        0 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-docsearch.js
--rw-r--r--   0        0        0     1338 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-sphinx-design.css
--rw-r--r--   0        0        0        0 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-sphinx-design.js
--rw-r--r--   0        0        0    27896 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
--rw-r--r--   0        0        0    49649 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.css
--rw-r--r--   0        0        0    55861 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.js
--rw-r--r--   0        0        0       93 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
--rw-r--r--   0        0        0      470 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0      358 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/toc.html
--rw-r--r--   0        0        0     2369 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/toc.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-18 12:40:01.359816 sphinxawesome_theme-5.1.3/LICENSE
+-rw-r--r--   0        0        0     2294 2024-04-18 12:40:01.359816 sphinxawesome_theme-5.1.3/README.md
+-rw-r--r--   0        0        0     2682 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7311 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     4166 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     1394 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2841 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/genindex.html
+-rw-r--r--   0        0        0     7675 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12751 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     1013 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1192 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5135 2024-04-18 12:40:01.363816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3242 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7816 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      932 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1226 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    30104 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/06b2bbbc4b7413514f6a.woff
+-rw-r--r--   0        0        0    21956 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
+-rw-r--r--   0        0        0    21088 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
+-rw-r--r--   0        0        0    28620 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
+-rw-r--r--   0        0        0    23072 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
+-rw-r--r--   0        0        0    23148 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
+-rw-r--r--   0        0        0    30232 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
+-rw-r--r--   0        0        0    29416 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
+-rw-r--r--   0        0        0    28636 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
+-rw-r--r--   0        0        0    22188 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
+-rw-r--r--   0        0        0    21820 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
+-rw-r--r--   0        0        0     4495 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-docsearch.css
+-rw-r--r--   0        0        0        0 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-docsearch.js
+-rw-r--r--   0        0        0     1338 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-sphinx-design.css
+-rw-r--r--   0        0        0        0 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-sphinx-design.js
+-rw-r--r--   0        0        0    27896 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
+-rw-r--r--   0        0        0    49649 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.css
+-rw-r--r--   0        0        0    55861 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.js
+-rw-r--r--   0        0        0       93 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      358 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2369 2024-04-18 12:40:01.367816 sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3537 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.3/PKG-INFO
```

### Comparing `sphinxawesome_theme-5.1.2/LICENSE` & `sphinxawesome_theme-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/README.md` & `sphinxawesome_theme-5.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/pyproject.toml` & `sphinxawesome_theme-5.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "5.1.2"
+version = "5.1.3"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -20,15 +20,15 @@
   { include = "sphinxawesome_theme", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sphinx = [
   { version = "<7.2", python = ">=3.8,<3.9"},
-  { version = "^7.2,<7.3", python = ">=3.9,<=3.12"},
+  { version = "^7.2,<7.3", python = ">=3.9,<3.13"},
 ]
 beautifulsoup4 = "^4.9.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = [
   { version = "^2021", python = ">=3.8,<3.9"},
   { version = "^2024.2.4", python = ">=3.9,<=3.12"},
```

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/deprecated.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/deprecated.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/genindex.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/header.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/highlighting.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/jsonimpl.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/logos.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/logos.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/page.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/postprocess.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/06b2bbbc4b7413514f6a.woff` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/06b2bbbc4b7413514f6a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-docsearch.css` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-docsearch.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-sphinx-design.css` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/awesome-sphinx-design.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.css` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.js` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/static/theme.js`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/toc.py` & `sphinxawesome_theme-5.1.3/src/sphinxawesome_theme/toc.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.2/PKG-INFO` & `sphinxawesome_theme-5.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 5.1.2
+Version: 5.1.3
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: sphinx (<7.2) ; python_version >= "3.8" and python_version < "3.9"
-Requires-Dist: sphinx (>=7.2,<7.3) ; python_version >= "3.9" and python_full_version <= "3.12.0"
+Requires-Dist: sphinx (>=7.2,<7.3) ; python_version >= "3.9" and python_version < "3.13"
 Project-URL: Documentation, https://sphinxawesome.xyz
 Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
 Description-Content-Type: text/markdown
 
 <h1 align="center">Sphinx awesome theme</h1>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.2 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.3 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx Classifier: Topic :: Software
 Development :: Documentation Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
 Requires-Dist: sphinx (<7.2) ; python_version >= "3.8" and python_version <
 "3.9" Requires-Dist: sphinx (>=7.2,<7.3) ; python_version >= "3.9" and
-python_full_version <= "3.12.0" Project-URL: Documentation, https://
-sphinxawesome.xyz Project-URL: Repository, https://github.com/kai687/
-sphinxawesome-theme Description-Content-Type: text/markdown
+python_version < "3.13" Project-URL: Documentation, https://sphinxawesome.xyz
+Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
+Description-Content-Type: text/markdown
                       ************ SSpphhiinnxx aawweessoommee tthheemmee ************
       [MIT license][PyPI version][Netlify Deploy][GitHub Workflow Status]
  Create beautiful and awesome documentation websites with _S_p_h_i_n_x. See how the
                     theme looks like on _s_p_h_i_n_x_a_w_e_s_o_m_e_._x_y_z.
 ## Get started 1. Install the theme as a Python package: ```console pip install
 sphinxawesome-theme ``` For more information, see [Install the theme](https://
 sphinxawesome.xyz/how-to/install/). 1. Add `sphinxawesome_theme` as an HTML
```

