# Comparing `tmp/sphinxawesome_theme-5.1.1.tar.gz` & `tmp/sphinxawesome_theme-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-5.1.1.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.1.2.tar", max compression
```

## Comparing `sphinxawesome_theme-5.1.1.tar` & `sphinxawesome_theme-5.1.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1066 2024-02-23 10:15:29.529358 sphinxawesome_theme-5.1.1/LICENSE
--rw-r--r--   0        0        0     2284 2024-02-23 10:15:29.529358 sphinxawesome_theme-5.1.1/README.md
--rw-r--r--   0        0        0     2701 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     7311 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0     1194 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     4165 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/deprecated.py
--rw-r--r--   0        0        0     1394 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2841 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/genindex.html
--rw-r--r--   0        0        0     7631 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12728 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0     1012 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1191 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     5135 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     3241 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/logos.py
--rw-r--r--   0        0        0      895 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7771 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0     1603 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      656 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      932 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1226 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     2462 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      416 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/sidebar_main_nav_links.html
--rw-r--r--   0        0        0      256 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/sidebar_toc.html
--rw-r--r--   0        0        0    21956 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
--rw-r--r--   0        0        0    30184 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/1d5fc702ab9000c3247a.woff
--rw-r--r--   0        0        0    21088 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
--rw-r--r--   0        0        0    28620 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
--rw-r--r--   0        0        0    23072 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
--rw-r--r--   0        0        0    23148 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
--rw-r--r--   0        0        0    30232 2024-02-23 10:15:29.533358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
--rw-r--r--   0        0        0    29416 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
--rw-r--r--   0        0        0    28636 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
--rw-r--r--   0        0        0    22188 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
--rw-r--r--   0        0        0    21820 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
--rw-r--r--   0        0        0     4498 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/awesome-docsearch.css
--rw-r--r--   0        0        0        0 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/awesome-docsearch.js
--rw-r--r--   0        0        0     1338 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/awesome-sphinx-design.css
--rw-r--r--   0        0        0        0 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/awesome-sphinx-design.js
--rw-r--r--   0        0        0    27896 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
--rw-r--r--   0        0        0    49385 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/theme.css
--rw-r--r--   0        0        0    55550 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/theme.js
--rw-r--r--   0        0        0       93 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
--rw-r--r--   0        0        0      470 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0      358 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/toc.html
--rw-r--r--   0        0        0     2369 2024-02-23 10:15:29.537358 sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/toc.py
--rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-18 11:38:12.271352 sphinxawesome_theme-5.1.2/LICENSE
+-rw-r--r--   0        0        0     2294 2024-04-18 11:38:12.271352 sphinxawesome_theme-5.1.2/README.md
+-rw-r--r--   0        0        0     2683 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7311 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     4166 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     1394 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2841 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/genindex.html
+-rw-r--r--   0        0        0     7675 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12751 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     1013 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1192 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5135 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3242 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7816 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      932 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1226 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2024-04-18 11:38:12.275353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    30104 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/06b2bbbc4b7413514f6a.woff
+-rw-r--r--   0        0        0    21956 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2
+-rw-r--r--   0        0        0    21088 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2
+-rw-r--r--   0        0        0    28620 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff
+-rw-r--r--   0        0        0    23072 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2
+-rw-r--r--   0        0        0    23148 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2
+-rw-r--r--   0        0        0    30232 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff
+-rw-r--r--   0        0        0    29416 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff
+-rw-r--r--   0        0        0    28636 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff
+-rw-r--r--   0        0        0    22188 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2
+-rw-r--r--   0        0        0    21820 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2
+-rw-r--r--   0        0        0     4495 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-docsearch.css
+-rw-r--r--   0        0        0        0 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-docsearch.js
+-rw-r--r--   0        0        0     1338 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-sphinx-design.css
+-rw-r--r--   0        0        0        0 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-sphinx-design.js
+-rw-r--r--   0        0        0    27896 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff
+-rw-r--r--   0        0        0    49649 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.css
+-rw-r--r--   0        0        0    55861 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.js
+-rw-r--r--   0        0        0       93 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      358 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2369 2024-04-18 11:38:12.279353 sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.1.2/PKG-INFO
```

### Comparing `sphinxawesome_theme-5.1.1/LICENSE` & `sphinxawesome_theme-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/README.md` & `sphinxawesome_theme-5.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,9 +53,9 @@
 
 ### Better headerlinks
 
 Clicking the link icon after headers or captions automatically copies the URL to the clipboard.
 
 ### DocSearch
 
-This theme supports the [`sphinx-docsearch`](https://sphinx-docsearch.readthedocs.io/en/latest/)
+This theme supports the [`sphinx-docsearch`](https://sphinx-docsearch.readthedocs.io/en/latest/) extension
 to replace the built-in search with Algolia DocSearch.
```

#### html2text {}

```diff
@@ -15,8 +15,8 @@
 If you load the bundled `sphinxawesome_theme.highlighting`, you can use these
 additional options in your `code-block` directives: - `emphasize-added`.
 Highlight lines that should be added - `emphasize-removed`. Highlight lines
 that should be removed - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code
 block ### Better headerlinks Clicking the link icon after headers or captions
 automatically copies the URL to the clipboard. ### DocSearch This theme
 supports the [`sphinx-docsearch`](https://sphinx-docsearch.readthedocs.io/en/
-latest/) to replace the built-in search with Algolia DocSearch.
+latest/) extension to replace the built-in search with Algolia DocSearch.
```

### Comparing `sphinxawesome_theme-5.1.1/pyproject.toml` & `sphinxawesome_theme-5.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "5.1.1"
+version = "5.1.2"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -36,63 +36,61 @@
 sphinx-sitemap = "^2.2.0"
 sphinx-design = ">=0.4.1,<0.6.0"
 sphinx-docsearch = "^0.0.4"
 python-dotenv = ">=0.19,<1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8"
-pytest-cov = "^4.0"
+pytest-cov = ">=4,<6"
 coverage = { extras = ["toml"], version = "^7.2" }
 types-docutils = ">=0.19.1.6,<0.21.0.0"
 mypy = "^1.0"
 
 [tool.poetry.group.lint.dependencies]
-black = ">=23.1,<25.0"
 pre-commit = [
   { version = "^3.5", python = ">=3.8,<3.9"},
   { version = "^3.6", python = ">=3.9,<=3.12"},
 ]
-ruff = ">=0.0.269,<0.2.3"
+ruff = ">=0.0.269,<0.3.8"
 
 [tool.poetry.group.netlify.dependencies]
-nox = {version = "^2023.4.22", python = "3.8"}
+nox = {version = ">=2023.4.22,<2025.0.0", python = "3.8"}
 poetry = {version = "^1.4.2", python = "3.8"}
 pipx = {version = "^1.2.0", python = "3.8"}
 pip = {version = ">=23.1.2,<25.0.0", python = "3.8"}
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.run]
 branch = true
 source = ["sphinxawesome_theme"]
 
 [tool.coverage.report]
 show_missing = true
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["E", "F", "B", "Q", "W", "I", "C90", "D", "UP", "YTT", "S", "ANN", "SIM", "N"]
-target-version = "py38"
 ignore = ["ANN401", "D203", "D213", "SIM105", "E501"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101"]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.mypy]
 files = ["src/sphinxawesome_theme/*.py", "tests/*.py", "noxfile.py", "docs/*.py"]
 show_error_codes = true
 show_error_context = true
 pretty = true
 strict = true
 show_column_numbers = true
 warn_unreachable = true
-warn_unused_ignores = true
+warn_unused_ignores = false
 
 [[tool.mypy.overrides]]
 module = ["pygments.*", "dotenv", "sphinxcontrib.serializinghtml", "bs4"]
 ignore_missing_imports = true
 
 [tool.poetry.plugins."sphinx.html_themes"]
 sphinxawesome_theme = "sphinxawesome_theme"
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/deprecated.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/deprecated.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
    :caption: |conf|
 
    extensions += ["sphinxawesome_theme.deprecated"]
 
 :copyright: Kai Welke.
 :license: MIT, see LICENSE for details
 """
+
 from __future__ import annotations
 
 from typing import Any
 
 from sphinx.application import Sphinx
 from sphinx.config import Config
 from sphinx.util import logging
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/genindex.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/header.html`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
         {% endif %}
         {%- endfor %}
         {%- endif %}
 
         {%- block theme_switcher %}
         <button @click="darkMode = darkMode === 'light' ? 'dark' : 'light'"
           class="relative inline-flex items-center justify-center px-0 text-sm font-medium transition-colors rounded-md hover:bg-accent hover:text-accent-foreground h-9 w-9"
-          type="button">
+          type="button"
+          aria-label="Color theme switcher">
           <svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor"
             class="absolute transition-all scale-100 rotate-0 dark:-rotate-90 dark:scale-0">
             <path
               d="M480 685q45.456 0 77.228-31.772Q589 621.456 589 576q0-45.456-31.772-77.228Q525.456 467 480 467q-45.456 0-77.228 31.772Q371 530.544 371 576q0 45.456 31.772 77.228Q434.544 685 480 685Zm0 91q-83 0-141.5-58.5T280 576q0-83 58.5-141.5T480 376q83 0 141.5 58.5T680 576q0 83-58.5 141.5T480 776ZM80 621.5q-19.152 0-32.326-13.174T34.5 576q0-19.152 13.174-32.326T80 530.5h80q19.152 0 32.326 13.174T205.5 576q0 19.152-13.174 32.326T160 621.5H80Zm720 0q-19.152 0-32.326-13.174T754.5 576q0-19.152 13.174-32.326T800 530.5h80q19.152 0 32.326 13.174T925.5 576q0 19.152-13.174 32.326T880 621.5h-80Zm-320-320q-19.152 0-32.326-13.174T434.5 256v-80q0-19.152 13.174-32.326T480 130.5q19.152 0 32.326 13.174T525.5 176v80q0 19.152-13.174 32.326T480 301.5Zm0 720q-19.152 0-32.326-13.17Q434.5 995.152 434.5 976v-80q0-19.152 13.174-32.326T480 850.5q19.152 0 32.326 13.174T525.5 896v80q0 19.152-13.174 32.33-13.174 13.17-32.326 13.17ZM222.174 382.065l-43-42Q165.5 327.391 166 308.239t13.174-33.065q13.435-13.674 32.587-13.674t32.065 13.674l42.239 43q12.674 13.435 12.555 31.706-.12 18.272-12.555 31.946-12.674 13.674-31.445 13.413-18.772-.261-32.446-13.174Zm494 494.761-42.239-43q-12.674-13.435-12.674-32.087t12.674-31.565Q686.609 756.5 705.38 757q18.772.5 32.446 13.174l43 41.761Q794.5 824.609 794 843.761t-13.174 33.065Q767.391 890.5 748.239 890.5t-32.065-13.674Zm-42-494.761Q660.5 369.391 661 350.62q.5-18.772 13.174-32.446l41.761-43Q728.609 261.5 747.761 262t33.065 13.174q13.674 13.435 13.674 32.587t-13.674 32.065l-43 42.239q-13.435 12.674-31.706 12.555-18.272-.12-31.946-12.555Zm-495 494.761Q165.5 863.391 165.5 844.239t13.674-32.065l43-42.239q13.435-12.674 32.087-12.674t31.565 12.674Q299.5 782.609 299 801.38q-.5 18.772-13.174 32.446l-41.761 43Q231.391 890.5 212.239 890t-33.065-13.174ZM480 576Z" />
           </svg>
           <svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor"
             class="absolute transition-all scale-0 rotate-90 dark:rotate-0 dark:scale-100">
```

#### html2text {}

```diff
@@ -20,11 +20,11 @@
 theme_extra_header_link_icons|tobool %} {%- for text,url in
 theme_extra_header_link_icons.items() %} {%- if url is mapping %}
 _{_{_ _u_r_l_._i_c_o_n_ _}_}
 {% endif %} {%- endfor %} {%- endif %} {%- block theme_switcher %}
 click="darkMode = darkMode === 'light' ? 'dark' : 'light'" class="relative
 inline-flex items-center justify-center px-0 text-sm font-medium transition-
 colors rounded-md hover:bg-accent hover:text-accent-foreground h-9 w-9"
-type="button"> {%- endblock theme_switcher %} {%- endblock
-extra_header_link_icons %}
+type="button" aria-label="Color theme switcher"> {%- endblock theme_switcher %}
+{%- endblock extra_header_link_icons %}
 {%- endblock header_right %}
 {%- block header_after %}{%- endblock header_after %}
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/highlighting.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
    if the option for it is present.
 
 5. Monkey-patch the ``PygmentsBridge.highlight_block`` method to pass the option for highlighting text to the ``get_lexer`` method.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details.
 """
+
 from __future__ import annotations
 
 import re
 from typing import Any, Generator, Literal, Pattern, Tuple, Union
 
 from docutils import nodes
 from docutils.nodes import Node
@@ -226,15 +227,15 @@
 
     new_options = {
         "emphasize-added": directives.unchanged_required,
         "emphasize-removed": directives.unchanged_required,
         "emphasize-text": directives.unchanged_required,
     }
 
-    option_spec = CodeBlock.option_spec
+    option_spec = CodeBlock.option_spec  # type: ignore[misc]
     option_spec.update(new_options)
 
     def _get_line_numbers(
         self: AwesomeCodeBlock, option: Literal["emphasize-added", "emphasize-removed"]
     ) -> list[int] | None:
         """Parse the line numbers for the ``:emphasize-added:`` and ``:emphasize-removed:`` options."""
         document = self.state.document
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jinja_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Define custom filters for Jinja2 templates.
 
 :copyright: Copyright, Kai Welke.
 :license: MIT, see LICENSE for details.
 """
+
 from __future__ import annotations
 
 import posixpath
 from typing import Any
 
 from docutils.nodes import Node
 from sphinx.application import Sphinx
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/jsonimpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 The awesome theme uses custom jinja2 helper functions which are
 non-serializable by default. Hence, I need to use a custom JSON
 serializer.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details.
 """
+
 from __future__ import annotations
 
 import json
 from typing import IO, Any
 
 
 class AwesomeJSONEncoder(json.JSONEncoder):
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/layout.html`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
       class="scroll-smooth"
       :class="{'dark': darkMode === 'dark' || (darkMode === 'system' && window.matchMedia('(prefers-color-scheme: dark)').matches)}"
 >
 <head>
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <meta charset="utf-8" />
   <meta name="theme-color" media="(prefers-color-scheme: light)" content="white" />
-  <meta name="theme-color" metia="(prefers-color-scheme: dark)" content="black" />
+  <meta name="theme-color" media="(prefers-color-scheme: dark)" content="black" />
   {{ metatags }}
 
   {%- block htmltitle %}
     <title>{{ title|striptags|e if title else docstitle }}{{ titlesuffix }}</title>
     <meta property="og:title" content="{{ title|striptags|e if title else docstitle }}{{ titlesuffix }}" />
     <meta name="twitter:title" content="{{ title|striptags|e if title else docstitle }}{{ titlesuffix }}" />
   {%- endblock htmltitle %}
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/logos.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/logos.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
    }
 
 Provide a path relative to the Sphinx configuration directory (with the :file:`conf.py` file).
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details
 """
+
 from __future__ import annotations
 
 import os
 from pathlib import Path
 from typing import Any
 
 from docutils.nodes import Node
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/page.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/page.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Note: This file is not processed by Webpack; don't use Tailwind utility classes.
 They might not show up in the final CSS.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE.
 """
+
 from __future__ import annotations
 
 import os
 import pathlib
 from dataclasses import dataclass
 
 from bs4 import BeautifulSoup, Comment
@@ -65,17 +66,17 @@
     """Make navigation links with children collapsible."""
     for link in tree.select("#left-sidebar a"):
         # Check if the link has "children"
         children = link.next_sibling
         if children and children.name == "ul":
             # State must be available in the link and the list
             li = link.parent
-            li[
-                "x-data"
-            ] = "{ expanded: $el.classList.contains('current') ? true : false }"
+            li["x-data"] = (
+                "{ expanded: $el.classList.contains('current') ? true : false }"
+            )
             link["@click"] = "expanded = !expanded"
             # The expandable class is a hack because we can't use Tailwind
             # I want to have _only_ expandable links with `justify-between`
             link["class"].append("expandable")
             link[":class"] = "{ 'expanded' : expanded }"
             children["x-show"] = "expanded"
 
@@ -105,32 +106,32 @@
         if len(children) == 1 and not children[0].strip():
             div.extract()
 
 
 def headerlinks(tree: BeautifulSoup) -> None:
     """Make headerlinks copy their URL on click."""
     for link in tree("a", class_="headerlink"):
-        link[
-            "@click.prevent"
-        ] = "window.navigator.clipboard.writeText($el.href); $el.setAttribute('data-tooltip', 'Copied!'); setTimeout(() => $el.setAttribute('data-tooltip', 'Copy link to this element'), 2000)"
+        link["@click.prevent"] = (
+            "window.navigator.clipboard.writeText($el.href); $el.setAttribute('data-tooltip', 'Copied!'); setTimeout(() => $el.setAttribute('data-tooltip', 'Copy link to this element'), 2000)"
+        )
         del link["title"]
         link["aria-label"] = "Copy link to this element"
         link["data-tooltip"] = "Copy link to this element"
 
 
 def scrollspy(tree: BeautifulSoup) -> None:
     """Add an active class to current TOC links in the right sidebar."""
     for link in tree("a", class_="headerlink"):
         if link.parent.name in ["h2", "h3"] or (
             link.parent.name == "dt" and "sig" in link.parent.get("class", "")
         ):
             active_link = link["href"]
-            link[
-                "x-intersect.margin.0%.0%.-70%.0%"
-            ] = f"activeSection = '{active_link}'"
+            link["x-intersect.margin.0%.0%.-70%.0%"] = (
+                f"activeSection = '{active_link}'"
+            )
 
     for link in tree.select("#right-sidebar a"):
         active_link = link["href"]
         link[":data-current"] = f"activeSection === '{active_link}'"
 
 
 def external_links(tree: BeautifulSoup) -> None:
@@ -189,15 +190,16 @@
     if exc is not None:
         return
 
     if app.builder is not None and app.builder.name not in ["html", "dirhtml"]:
         return
 
     files_to_postprocess = [
-        app.builder.get_outfilename(doc) for doc in app.env.awesome_changed_docs  # type: ignore[attr-defined]
+        app.builder.get_outfilename(doc)  # type: ignore[attr-defined]
+        for doc in app.env.awesome_changed_docs  # type: ignore[attr-defined]
     ]
 
     if len(files_to_postprocess) == 0:
         return
 
     for doc in status_iterator(
         files_to_postprocess,
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/scrolltop.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/0fecf1cc5677455886b4.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/2fe080a3bf49bdc12fcb.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/39bd78ffb50669d6855a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/4f183a25813446a47ad9.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/5f68b8c26e28d783a591.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/63a0f5d460fb58135365.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/70e1dc5f5622381d6e9e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/84504970850f0632d9c3.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a1e4997bd1fb9d7822e1.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/a61d04152f1635036f0d.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/awesome-docsearch.css` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-docsearch.css`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-:root{--docsearch-primary-color:hsl(var(--primary));--docsearch-key-gradient:transparent;--docsearch-key-shadow:transparent;--docsearch-text-color:hsl(var(--popover-foreground));--docsearch-modal-width:760px;--docsearch-modal-background:hsl(var(--popover));--docsearch-footer-background:hsl(var(--popover));--docsearch-searchbox-focus-background:hsl(var(--popover));--docsearch-container-background:hsl(var(--background)/0.8);--docsearch-spacing:0.5rem;--docsearch-hit-active-color:hsl(var(--accent-foreground));--docsearch-hit-background:transparent;--docsearch-searchbox-shadow:none;--docsearch-hit-shadow:none;--docsearch-modal-shadow:none;--docsearch-footer-shadow:none}.DocSearch-Button{background-color:transparent;border-color:hsl(var(--input));border-radius:.5em;border-style:solid;border-width:1px;display:flex;font-size:.875rem;line-height:1.25rem;width:90%;--tw-ring-offset-color:hsl(var(--background));transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.DocSearch-Button:hover{--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;box-shadow:0 0 transparent,0 0 transparent,0 0 transparent;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.DocSearch-Button:focus,.DocSearch-Button:hover{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Button:focus-visible{outline:2px solid transparent;outline-offset:2px;--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-inset) 0 0 0 2px var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 4px hsl(var(--ring)),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 transparent);--tw-ring-color:hsl(var(--ring));--tw-ring-offset-width:2px}.DocSearch-Button-Placeholder{display:block;font-size:.875rem;font-weight:500;line-height:1.25rem}.DocSearch-Button-Key{background-color:hsl(var(--muted));border-color:hsl(var(--border));border-radius:.25rem;border-style:solid;border-width:1px;color:hsl(var(--muted-foreground));font-size:12px}.DocSearch-Container{position:fixed;--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.DocSearch-Modal{border-color:hsl(var(--border));border-radius:var(--radius);border-width:1px}.DocSearch-SearchBar{border-bottom-left-radius:0;border-bottom-right-radius:0;border-bottom-width:1px;border-color:hsl(var(--input));border-top-left-radius:var(--radius);border-top-right-radius:var(--radius);padding:0}.DocSearch-Form{border-bottom-left-radius:0;border-bottom-right-radius:0;border-top-left-radius:var(--radius);border-top-right-radius:var(--radius)}.DocSearch-Cancel{color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;padding-left:.5rem;padding-right:.5rem}.DocSearch-MagnifierLabel,.DocSearch-Search-Icon{stroke-width:2;opacity:.5}.DocSearch-Hit-source{color:hsl(var(--muted-foreground))}.DocSearch-Hit,.DocSearch-Hit a{border-radius:calc(var(--radius) - 4px)}.DocSearch-Hit a:focus-visible{outline-offset:-2px}.DocSearch-Hit[aria-selected=true] a{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Commands{display:none}.DocSearch-Footer{border-color:hsl(var(--border));border-top-width:1px}
+:root{--docsearch-primary-color:hsl(var(--primary));--docsearch-muted-color:hsl(var(--muted-foreground));--docsearch-key-gradient:transparent;--docsearch-key-shadow:transparent;--docsearch-text-color:hsl(var(--popover-foreground));--docsearch-modal-width:760px;--docsearch-modal-background:hsl(var(--popover));--docsearch-footer-background:hsl(var(--popover));--docsearch-searchbox-focus-background:hsl(var(--popover));--docsearch-container-background:hsl(var(--background)/0.8);--docsearch-spacing:0.5rem;--docsearch-hit-active-color:hsl(var(--accent-foreground));--docsearch-hit-background:transparent;--docsearch-searchbox-shadow:none;--docsearch-hit-shadow:none;--docsearch-modal-shadow:none;--docsearch-footer-shadow:none}.DocSearch-Button{background-color:transparent;border-color:hsl(var(--input));border-radius:.5em;border-style:solid;border-width:1px;display:flex;font-size:.875rem;line-height:1.25rem;width:90%;--tw-ring-offset-color:hsl(var(--background));transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.DocSearch-Button:hover{--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;box-shadow:0 0 transparent,0 0 transparent,0 0 transparent;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.DocSearch-Button:focus,.DocSearch-Button:hover{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Button:focus-visible{outline:2px solid transparent;outline-offset:2px;--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 transparent);--tw-ring-color:hsl(var(--ring));--tw-ring-offset-width:2px}.DocSearch-Button-Placeholder{display:block;font-size:.875rem;font-weight:500;line-height:1.25rem}.DocSearch-Button-Key{background-color:hsl(var(--muted));border-color:hsl(var(--border));border-radius:.25rem;border-style:solid;border-width:1px;color:hsl(var(--muted-foreground));font-size:12px}.DocSearch-Container{position:fixed;--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.DocSearch-Modal{border-color:hsl(var(--border));border-radius:var(--radius);border-width:1px}.DocSearch-SearchBar{border-bottom-left-radius:0;border-bottom-right-radius:0;border-bottom-width:1px;border-color:hsl(var(--input));border-top-left-radius:var(--radius);border-top-right-radius:var(--radius);padding:0}.DocSearch-Form{border-bottom-left-radius:0;border-bottom-right-radius:0;border-top-left-radius:var(--radius);border-top-right-radius:var(--radius)}.DocSearch-Cancel{color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;padding-left:.5rem;padding-right:.5rem}.DocSearch-MagnifierLabel,.DocSearch-Search-Icon{stroke-width:2;opacity:.5}.DocSearch-Hit-source{color:hsl(var(--muted-foreground))}.DocSearch-Hit,.DocSearch-Hit a{border-radius:calc(var(--radius) - 4px)}.DocSearch-Hit a:focus-visible{outline-offset:-2px}.DocSearch-Hit[aria-selected=true] a{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Commands{display:none}.DocSearch-Footer{border-color:hsl(var(--border));border-top-width:1px}
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/awesome-sphinx-design.css` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/awesome-sphinx-design.css`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/c226d7283d0d52c2d32c.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/theme.css` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.css`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:400;src:url(a1e4997bd1fb9d7822e1.woff2) format("woff2"),url(70e1dc5f5622381d6e9e.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:400;src:url(2fe080a3bf49bdc12fcb.woff2) format("woff2"),url(c226d7283d0d52c2d32c.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:500;src:url(4f183a25813446a47ad9.woff2) format("woff2"),url(63a0f5d460fb58135365.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:500;src:url(a61d04152f1635036f0d.woff2) format("woff2"),url(39bd78ffb50669d6855a.woff) format("woff")}
-@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(5f68b8c26e28d783a591.woff2) format("woff2"),url(1d5fc702ab9000c3247a.woff) format("woff")}
+@font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(5f68b8c26e28d783a591.woff2) format("woff2"),url(06b2bbbc4b7413514f6a.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:700;src:url(0fecf1cc5677455886b4.woff2) format("woff2"),url(84504970850f0632d9c3.woff) format("woff")}
-/*! tailwindcss v3.4.1 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal;-moz-tab-size:4;-o-tab-size:4;tab-size:4;-webkit-tap-highlight-color:transparent}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-feature-settings:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}:root{--background:0 0% 100%;--foreground:222.2 47.4% 11.2%;--muted:210 40% 96.1%;--muted-foreground:215.4 16.3% 46.9%;--popover:0 0% 100%;--popover-foreground:222.2 47.4% 11.2%;--border:214.3 31.8% 91.4%;--input:214.3 31.8% 91.4%;--card:0 0% 100%;--card-foreground:222.2 47.4% 11.2%;--primary:222.2 47.4% 11.2%;--primary-foreground:210 40% 98%;--secondary:210 40% 96.1%;--secondary-foreground:222.2 47.4% 11.2%;--accent:210 40% 96.1%;--accent-foreground:222.2 47.4% 11.2%;--destructive:0 100% 50%;--destructive-foreground:210 40% 98%;--ring:215 20.2% 65.1%;--radius:0.5rem}.dark{--background:224 71% 4%;--foreground:213 31% 91%;--muted:223 47% 11%;--muted-foreground:215.4 16.3% 56.9%;--accent:216 34% 17%;--accent-foreground:210 40% 98%;--popover:224 71% 4%;--popover-foreground:215 20.2% 65.1%;--border:216 34% 17%;--input:216 34% 17%;--card:224 71% 4%;--card-foreground:213 31% 91%;--primary:210 40% 98%;--primary-foreground:222.2 47.4% 1.2%;--secondary:222.2 47.4% 11.2%;--secondary-foreground:210 40% 98%;--destructive:0 63% 31%;--destructive-foreground:210 40% 98%;--ring:216 34% 17%;--radius:0.5rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{margin-left:auto;margin-right:auto;padding-left:2rem;padding-right:2rem;width:100%}@media (min-width:1400px){.container{max-width:1400px}}#content svg{display:inline}#content hr{border-color:#e1e7ef;border-color:hsl(var(--border));margin-bottom:1rem;margin-top:1rem}@media (min-width:768px){#content hr{margin-bottom:1.5rem;margin-top:1.5rem}}#content h1{font-size:2.25rem;font-weight:700;line-height:2.5rem;margin-bottom:.5rem}#content h2{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));font-size:1.875rem;font-weight:600;line-height:2.25rem;margin-top:3rem;padding-bottom:.5rem}#content h3{font-size:1.5rem;font-weight:600;line-height:2rem;margin-top:2rem}#content .rubric,#content h4{font-size:1.25rem;font-weight:600;line-height:1.75rem;margin-top:2rem}#content section{scroll-margin:5rem}#content section>p{line-height:1.75rem;margin-top:1.5rem}#content section>p.rubric,#content section>p:first-child{margin-top:0}#content section>p.lead{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.125rem;line-height:1.75rem}#content .centered{text-align:center}#content a:not(.toc-backref){color:#0f1729;color:hsl(var(--primary));font-weight:500;text-decoration-line:underline;text-decoration-thickness:from-font;text-underline-offset:4px}#content ul:not(.search){list-style-type:disc;margin-left:1.5rem;margin-top:1.5rem}#content ul:not(.search) p,#content ul:not(.search)>li{margin-top:1.5rem}#content ul:not(.search) ul{margin-top:0}#content ol{list-style-type:decimal;margin-left:1.5rem;margin-top:1.5rem}#content ol ::marker{font-weight:500}#content ol::marker{font-weight:500}#content ol p,#content ol>li{margin-top:1.5rem}#content ol ol{margin-top:0}#content dl{margin-top:1.5rem}#content dl dt:not(.sig){font-weight:500;margin-top:1.5rem}#content dl dt:not(.sig):first-child{margin-bottom:0;margin-top:0}#content dl dd{margin-left:1.5rem}#content dl p{margin-bottom:.5rem;margin-top:.5rem}#content .align-center{margin-left:auto;margin-right:auto;text-align:center}#content .align-right{margin-left:auto;text-align:right}#content img{margin-top:1.5rem}#content figure img{display:inline-block}#content figcaption{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:3rem}#content figcaption>*{margin-top:1rem}blockquote{border-left-width:2px;font-style:italic;margin-bottom:1.5rem;margin-top:1.5rem;padding-left:1.5rem}blockquote .attribution{font-style:normal;margin-top:.5rem}table{font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;width:100%}table caption{color:#65758b;color:hsl(var(--muted-foreground));margin-bottom:1.5rem;text-align:left}table thead{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table th{font-weight:500;padding-bottom:.5rem;padding-left:.5rem;text-align:left}table th:first-child{padding-left:0}.dark table th{font-weight:600}table tbody tr{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table tbody td{padding:.5rem}table tbody td:first-child{padding-left:0}.footnote>.label{float:left;padding-right:.5rem}.footnote>:not(.label){margin-bottom:1.5rem;margin-left:2rem;margin-top:1.5rem}.footnote .footnote-reference,.footnote [role=doc-backlink]{text-decoration-line:none!important}.admonition{background-color:#fff;background-color:hsl(var(--background));border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;color:#0f1729;color:hsl(var(--foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-top:.5rem}.admonition .admonition-title{margin-top:0!important}.admonition-title{font-weight:500}.dark .admonition-title{font-weight:600;letter-spacing:.025em}.note{--tw-border-opacity:1;border-color:#0284c7;border-color:rgba(2,132,199,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0f9ff;background-color:rgba(240,249,255,var(--tw-bg-opacity));--tw-text-opacity:1;color:#0c4a6e;color:rgba(12,74,110,var(--tw-text-opacity))}.dark .note{background-color:rgba(96,165,250,.15);--tw-text-opacity:1;color:#e0f2fe;color:rgba(224,242,254,var(--tw-text-opacity))}.hint,.tip{--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0fdf4;background-color:rgba(240,253,244,var(--tw-bg-opacity));--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.dark .hint,.dark .tip{background-color:rgba(74,222,128,.15);--tw-text-opacity:1;color:#dcfce7;color:rgba(220,252,231,var(--tw-text-opacity))}.danger,.error{--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fef2f2;background-color:rgba(254,242,242,var(--tw-bg-opacity));--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.dark .danger,.dark .error{background-color:hsla(0,91%,71%,.15);--tw-text-opacity:1;color:#fee2e2;color:rgba(254,226,226,var(--tw-text-opacity))}.attention,.caution,.important,.warning{--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fefce8;background-color:rgba(254,252,232,var(--tw-bg-opacity));--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}.dark .attention,.dark .caution,.dark .important,.dark .warning{background-color:rgba(250,204,21,.15);--tw-text-opacity:1;color:#fef9c3;color:rgba(254,249,195,var(--tw-text-opacity))}div.versionadded{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionadded p{margin-top:0!important}div.versionadded p:last-child{margin-bottom:0!important}div.versionadded .versionmodified{font-weight:500;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.dark div.versionadded .versionmodified{letter-spacing:.025em;--tw-text-opacity:1;color:#22c55e;color:rgba(34,197,94,var(--tw-text-opacity))}div.versionchanged{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionchanged p{margin-top:0!important}div.versionchanged p:last-child{margin-bottom:0!important}div.versionchanged .versionmodified{font-weight:500;--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}.dark div.versionchanged .versionmodified{letter-spacing:.025em;--tw-text-opacity:1;color:#eab308;color:rgba(234,179,8,var(--tw-text-opacity))}div.deprecated{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.deprecated p{margin-top:0!important}div.deprecated p:last-child{margin-bottom:0!important}div.deprecated .versionmodified{font-weight:500;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.dark div.deprecated .versionmodified{letter-spacing:.025em;--tw-text-opacity:1;color:#f87171;color:rgba(248,113,113,var(--tw-text-opacity))}.highlight{background-color:transparent;position:relative}.highlight:hover .copy{opacity:1}.highlight .gp,.highlight-pycon .go,.highlight-python .go{-webkit-user-select:none;-moz-user-select:none;user-select:none}.literal-block-wrapper{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;margin-left:0;margin-right:0;margin-top:1.5rem;max-width:none;padding-left:0;padding-right:0}.literal-block-wrapper pre{border-radius:0;border-style:none;margin-top:0}.literal-block-wrapper .code-block-caption{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));border-top-left-radius:.5rem;border-top-left-radius:var(--radius);border-top-right-radius:.5rem;border-top-right-radius:var(--radius);color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;letter-spacing:.025em;line-height:1.25rem;padding:.5rem 1rem}code{background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:.875rem;line-height:1.25rem;padding:.2em .3em;position:relative;white-space:nowrap}code .ge,code em{color:#0f1729;color:hsl(var(--accent-foreground));font-weight:700;letter-spacing:.025em}:where(h1,h2,h3,h4,h5,h6) code{font-size:inherit}pre{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;margin-top:1.5rem;overflow-x:auto;padding-bottom:1rem;padding-top:1rem}pre[data-theme=dark]{background-color:#fff;background-color:hsl(var(--background))}pre[data-theme=light]{--tw-bg-opacity:1;background-color:#fff;background-color:rgba(255,255,255,var(--tw-bg-opacity))}pre.literal-block{padding-left:1rem;padding-right:1rem}pre code{background-color:transparent;padding:0;white-space:pre}pre code>[id^=line-]{display:block;padding-left:1rem;padding-right:1rem}pre code [id^=line-]:has(.gd),pre code [id^=line-]:has(.gi),pre code [id^=line-]:has(del),pre code [id^=line-]:has(ins),pre code [id^=line-]:has(mark){padding-left:0;padding-right:0}pre code [id^=line-] del,pre code [id^=line-] ins,pre code [id^=line-] mark{display:block;padding-left:1rem;padding-right:1rem;position:relative}pre code [id^=line-] mark{background-color:#f1f5f9;background-color:hsl(var(--muted));color:inherit;--tw-shadow:2px 0 currentColor inset;--tw-shadow-colored:inset 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 2px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.dark pre code [id^=line-] mark{--tw-bg-opacity:1;background-color:#334155;background-color:rgba(51,65,85,var(--tw-bg-opacity));--tw-shadow:3px 0 currentColor inset;--tw-shadow-colored:inset 3px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 3px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] ins{background-color:rgba(34,197,94,.3);--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] ins:before{left:2px;position:absolute;--tw-content:"\002b";content:"\002b";content:var(--tw-content)}.dark pre code [id^=line-] ins{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}pre code [id^=line-] del{background-color:rgba(239,68,68,.3);--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] del:before{left:2px;position:absolute;--tw-content:"\2212";content:"\2212";content:var(--tw-content)}.dark pre code [id^=line-] del{--tw-bg-opacity:1;--tw-text-opacity:1;color:#fecaca;color:rgba(254,202,202,var(--tw-text-opacity))}pre .linenos{padding-left:0;padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight-diff .gi{background-color:rgba(34,197,94,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.dark .highlight-diff .gi{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.highlight-diff .gd{background-color:rgba(239,68,68,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.dark .highlight-diff .gd{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.guilabel,.menuselection{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500;padding:1px .5rem}#content kbd:not(.compound){background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;border-width:1px;font-size:.875rem;font-weight:500;letter-spacing:.025em;line-height:1.25rem;padding:1px .25rem}.sig{border-color:#e1e7ef;border-color:hsl(var(--border));border-top-width:1px;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-weight:700;padding-top:1.5rem;scroll-margin:5rem}.sig-name{color:#0f1729;color:hsl(var(--accent-foreground))}em.property{color:#65758b;color:hsl(var(--muted-foreground))}.option .sig-prename{font-style:italic}.viewcode-link{color:#65758b;color:hsl(var(--muted-foreground));float:right}.option-list kbd{background-color:transparent!important;border-style:none!important;font-size:1em!important;font-weight:700!important}.headerlink{align-items:center;display:inline-flex;margin-left:.25rem;position:relative;vertical-align:middle}.headerlink:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}.headerlink:focus:after,.headerlink:focus:before,.headerlink:hover:after,.headerlink:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.headerlink:after{margin-top:6px;right:50%;top:100%}.headerlink:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.headerlink:after{margin-right:-16px}.headerlink>*{visibility:hidden;fill:currentColor;color:#65758b;color:hsl(var(--muted-foreground))}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#left-sidebar .caption{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);font-size:.875rem;font-weight:600;line-height:1.25rem;margin-bottom:.25rem;padding:1.5rem .5rem .25rem}#left-sidebar .caption:first-child{padding-top:0}#left-sidebar ul{display:grid;font-size:.875rem;grid-auto-flow:row;grid-auto-rows:max-content;line-height:1.25rem;overflow:hidden;transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.3s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}@media (prefers-reduced-motion:reduce){#left-sidebar ul{transition-property:none}}#left-sidebar ul ul{margin-left:.75rem;opacity:1;padding:.5rem 0 .5rem .75rem;position:relative;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar ul ul:before{bottom:.25rem;left:0;position:absolute;top:.25rem;width:1px;--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgba(229,231,235,var(--tw-bg-opacity));--tw-content:"";content:"";content:var(--tw-content)}.dark #left-sidebar ul ul:before{content:var(--tw-content);--tw-bg-opacity:1;background-color:#262626;background-color:rgba(38,38,38,var(--tw-bg-opacity))}#left-sidebar a{align-items:center;border-color:transparent;border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);border-width:1px;display:flex;padding:.375rem .5rem;width:100%}#left-sidebar a:hover{text-decoration-line:underline}#left-sidebar a:focus-visible{outline-offset:-1px}#left-sidebar a>button{border-radius:.25rem;color:#65758b;color:hsl(var(--muted-foreground))}#left-sidebar a>button:hover{background-color:rgba(15,23,41,.1);background-color:hsl(var(--primary)/.1)}#left-sidebar a>button>svg{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform-origin:center;transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar a.current{background-color:#f1f5f9;background-color:hsl(var(--accent));border-color:#e1e7ef;border-color:hsl(var(--border));border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500}#left-sidebar a.expandable{justify-content:space-between}#left-sidebar a.expandable.expanded>button>svg{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}#right-sidebar ul{margin:0}#right-sidebar ul li{margin-top:0;padding-top:.5rem}#right-sidebar ul li a{color:#65758b;color:hsl(var(--muted-foreground));display:inline-block;text-decoration-line:none;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}#right-sidebar ul li a:hover{color:#0f1729;color:hsl(var(--foreground))}#right-sidebar ul li a:focus-visible{outline-offset:-1px}#right-sidebar ul li a[data-current=true]{color:#0f1729;color:hsl(var(--foreground));font-weight:500}#right-sidebar ul li ul{padding-left:1rem}#right-sidebar ul:not(:last-child){padding-bottom:.5rem}.contents>:not([hidden])~:not([hidden]),.toctree-wrapper>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.contents,.toctree-wrapper{font-size:.875rem;line-height:1.25rem}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{font-weight:500;padding-top:1.5rem}.contents ul,.toctree-wrapper ul{list-style-type:none!important;margin:0!important}.contents ul li a.reference,.toctree-wrapper ul li a.reference{color:#65758b!important;color:hsl(var(--muted-foreground))!important;display:inline-block;font-weight:400!important;text-decoration-line:none!important;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.contents ul li a.reference:hover,.toctree-wrapper ul li a.reference:hover{color:#0f1729;color:hsl(var(--foreground))}.contents ul li ul,.toctree-wrapper ul li ul{padding-left:1rem}.contents ul:not(:last-child),.toctree-wrapper ul:not(:last-child){padding-bottom:.5rem}#search-results .search-summary{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.25rem;line-height:1.75rem;margin-top:1.5rem}#search-results ul.search,#search-results ul.search li{margin-top:1.5rem}#search-results ul.search .context{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-top:.5rem}.highlighted{background-color:#f1f5f9;background-color:hsl(var(--accent));text-decoration-line:underline;text-decoration-thickness:2px}.highlight-link{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;padding:.5rem 1rem;position:fixed;right:.5rem;top:4rem}.highlight-link:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}@media (min-width:1024px){.highlight-link{right:4rem}}.tooltipped{position:relative}.tooltipped:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.sr-only{height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px;clip:rect(0,0,0,0);border-width:0;white-space:nowrap}.pointer-events-none{pointer-events:none}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-1{right:.25rem}.right-1\.5{right:.375rem}.right-4{right:1rem}.right-8{right:2rem}.top-0{top:0}.top-16{top:4rem}.top-2{top:.5rem}.top-4{top:1rem}.z-10{z-index:10}.z-20{z-index:20}.z-40{z-index:40}.z-50{z-index:50}.z-\[100\]{z-index:100}.mx-auto{margin-left:auto;margin-right:auto}.my-4{margin-bottom:1rem;margin-top:1rem}.my-6{margin-bottom:1.5rem;margin-top:1.5rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mt-10{margin-top:-2.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-0{margin-left:0}.ml-2{margin-left:.5rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-4{margin-right:1rem}.mr-6{margin-right:1.5rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-4{margin-top:1rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.hidden{display:none}.h-10{height:2.5rem}.h-14{height:3.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-9{height:2.25rem}.h-\[14px\]{height:14px}.h-\[calc\(100vh-8rem\)\]{height:calc(100vh - 8rem)}.h-full{height:100%}.max-h-\[calc\(var\(--vh\)-4rem\)\]{max-height:calc(var(--vh) - 4rem)}.max-h-\[calc\(var\(100vh\)-5rem\)\]{max-height:calc(var(100vh) - 5rem)}.min-h-screen{min-height:100vh}.w-4{width:1rem}.w-5\/6{width:83.333333%}.w-6{width:1.5rem}.w-9{width:2.25rem}.w-\[14px\]{width:14px}.w-full{width:100%}.min-w-0{min-width:0}.min-w-full{min-width:100%}.max-w-prose{max-width:65ch}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1)}.scale-100,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-center{align-items:center}.\!justify-start{justify-content:flex-start!important}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-1{gap:.25rem}.gap-4{gap:1rem}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.25rem;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.25rem*var(--tw-space-x-reverse))}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.5rem;margin-left:calc(.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.5rem*var(--tw-space-x-reverse))}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1.5rem;margin-left:calc(1.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1.5rem*var(--tw-space-x-reverse))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-\[0\.5rem\]{border-radius:.5rem}.rounded-md{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px)}.rounded-sm{border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px)}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-border{border-color:#e1e7ef;border-color:hsl(var(--border))}.border-input{border-color:#e1e7ef;border-color:hsl(var(--input))}.bg-background{background-color:#fff;background-color:hsl(var(--background))}.bg-background\/80{background-color:hsla(0,0%,100%,.8);background-color:hsl(var(--background)/.8)}.bg-background\/95{background-color:hsla(0,0%,100%,.95);background-color:hsl(var(--background)/.95)}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgba(55,65,81,var(--tw-bg-opacity))}.bg-muted{background-color:#f1f5f9;background-color:hsl(var(--muted))}.bg-transparent{background-color:transparent}.fill-current{fill:currentColor}.p-2{padding:.5rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-0{padding-left:0;padding-right:0}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-6{padding-bottom:1.5rem;padding-top:1.5rem}.pr-6{padding-right:1.5rem}.pt-2{padding-top:.5rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.font-mono{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-\[10px\]{font-size:10px}.text-base{font-size:1rem;line-height:1.5rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-loose{line-height:2}.text-foreground{color:#0f1729;color:hsl(var(--foreground))}.text-foreground\/60{color:rgba(15,23,41,.6);color:hsl(var(--foreground)/.6)}.text-muted-foreground{color:#65758b;color:hsl(var(--muted-foreground))}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgba(185,28,28,var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgba(255,255,255,var(--tw-text-opacity))}.underline{text-decoration-line:underline}.no-underline{text-decoration-line:none}.underline-offset-4{text-underline-offset:4px}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-100{opacity:1}.opacity-70{opacity:.7}.shadow-sm{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.05);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 1px 2px 0 rgba(0,0,0,.05);box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.ring-offset-background{--tw-ring-offset-color:hsl(var(--background))}.backdrop-blur{--tw-backdrop-blur:blur(8px);-webkit-backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-colors{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}[x-cloak]{display:none!important}@media (max-width:640px){.container{padding-left:1rem;padding-right:1rem}}.hover\:bg-accent:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.hover\:bg-muted:hover{background-color:#f1f5f9;background-color:hsl(var(--muted))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:text-accent-foreground:hover{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:text-foreground:hover{color:#0f1729;color:hsl(var(--foreground))}.hover\:text-foreground\/80:hover{color:rgba(15,23,41,.8);color:hsl(var(--foreground)/.8)}.hover\:placeholder-accent-foreground:hover::-moz-placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:placeholder-accent-foreground:hover::placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:opacity-100:hover{opacity:1}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-accent:focus{background-color:#f1f5f9;background-color:hsl(var(--accent))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.focus\:text-accent-foreground:focus{color:#0f1729;color:hsl(var(--accent-foreground))}.focus\:opacity-100:focus{opacity:1}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent;outline-offset:2px}.focus-visible\:outline-offset-\[-1px\]:focus-visible{outline-offset:-1px}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 transparent)}.focus-visible\:ring-ring:focus-visible{--tw-ring-color:hsl(var(--ring))}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width:2px}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:opacity-50:disabled{opacity:.5}.group:hover .group-hover\:bg-accent{background-color:#f1f5f9;background-color:hsl(var(--accent))}.group:hover .group-hover\:text-accent-foreground{color:#0f1729;color:hsl(var(--accent-foreground))}.dark .dark\:block{display:block}.dark .dark\:hidden{display:none}.dark .dark\:-rotate-90{--tw-rotate:-90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(-90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:invert{--tw-invert:invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) invert(100%) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}@media (min-width:640px){.sm\:inline-block{display:inline-block}.sm\:flex{display:flex}.sm\:space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1rem;margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1rem*var(--tw-space-x-reverse))}.sm\:pr-12{padding-right:3rem}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-14{top:3.5rem}.md\:z-30{z-index:30}.md\:my-0{margin-bottom:0;margin-top:0}.md\:-ml-2{margin-left:-.5rem}.md\:inline{display:inline}.md\:flex{display:flex}.md\:grid{display:grid}.md\:\!hidden{display:none!important}.md\:hidden{display:none}.md\:h-24{height:6rem}.md\:h-\[calc\(100vh-3\.5rem\)\]{height:calc(100vh - 3.5rem)}.md\:h-auto{height:auto}.md\:w-40{width:10rem}.md\:w-auto{width:auto}.md\:w-full{width:100%}.md\:flex-none{flex:none}.md\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.md\:grid-cols-\[220px_minmax\(0\2c 1fr\)\]{grid-template-columns:220px minmax(0,1fr)}.md\:flex-row{flex-direction:row}.md\:justify-end{justify-content:flex-end}.md\:gap-2{gap:.5rem}.md\:gap-6{gap:1.5rem}.md\:overflow-auto{overflow:auto}.md\:bg-transparent{background-color:transparent}.md\:p-0{padding:0}.md\:px-0{padding-left:0;padding-right:0}.md\:py-0{padding-bottom:0;padding-top:0}.md\:text-left{text-align:left}}@media (min-width:1024px){.lg\:my-8{margin-bottom:2rem;margin-top:2rem}.lg\:w-64{width:16rem}.lg\:grid-cols-\[240px_minmax\(0\2c 1fr\)\]{grid-template-columns:240px minmax(0,1fr)}.lg\:gap-10{gap:2.5rem}.lg\:py-8{padding-bottom:2rem;padding-top:2rem}}@media (min-width:1280px){.xl\:block{display:block}.xl\:grid{display:grid}.xl\:grid-cols-\[1fr_300px\]{grid-template-columns:1fr 300px}}
+/*! tailwindcss v3.4.3 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal;-moz-tab-size:4;-o-tab-size:4;tab-size:4;-webkit-tap-highlight-color:transparent}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-feature-settings:normal;font-size:1em;font-variation-settings:normal}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-feature-settings:inherit;font-size:100%;font-variation-settings:inherit;font-weight:inherit;letter-spacing:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}:root{--background:0 0% 100%;--foreground:222.2 47.4% 11.2%;--muted:210 40% 96.1%;--muted-foreground:215.4 16.3% 46.9%;--popover:0 0% 100%;--popover-foreground:222.2 47.4% 11.2%;--border:214.3 31.8% 91.4%;--input:214.3 31.8% 91.4%;--card:0 0% 100%;--card-foreground:222.2 47.4% 11.2%;--primary:222.2 47.4% 11.2%;--primary-foreground:210 40% 98%;--secondary:210 40% 96.1%;--secondary-foreground:222.2 47.4% 11.2%;--accent:210 40% 96.1%;--accent-foreground:222.2 47.4% 11.2%;--destructive:0 100% 50%;--destructive-foreground:210 40% 98%;--ring:215 20.2% 65.1%;--radius:0.5rem}.dark{--background:224 71% 4%;--foreground:213 31% 91%;--muted:223 47% 11%;--muted-foreground:215.4 16.3% 56.9%;--accent:216 34% 17%;--accent-foreground:210 40% 98%;--popover:224 71% 4%;--popover-foreground:215 20.2% 65.1%;--border:216 34% 17%;--input:216 34% 17%;--card:224 71% 4%;--card-foreground:213 31% 91%;--primary:210 40% 98%;--primary-foreground:222.2 47.4% 1.2%;--secondary:222.2 47.4% 11.2%;--secondary-foreground:210 40% 98%;--destructive:0 63% 31%;--destructive-foreground:210 40% 98%;--ring:216 34% 17%;--radius:0.5rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }.container{margin-left:auto;margin-right:auto;padding-left:2rem;padding-right:2rem;width:100%}@media (min-width:1400px){.container{max-width:1400px}}#content svg{display:inline}#content hr{border-color:#e1e7ef;border-color:hsl(var(--border));margin-bottom:1rem;margin-top:1rem}@media (min-width:768px){#content hr{margin-bottom:1.5rem;margin-top:1.5rem}}#content h1{font-size:2.25rem;font-weight:700;line-height:2.5rem;margin-bottom:.5rem}#content h2{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));font-size:1.875rem;font-weight:600;line-height:2.25rem;margin-top:3rem;padding-bottom:.5rem}#content h3{font-size:1.5rem;font-weight:600;line-height:2rem;margin-top:2rem}#content .rubric,#content h4{font-size:1.25rem;font-weight:600;line-height:1.75rem;margin-top:2rem}#content section{scroll-margin:5rem}#content section>p{line-height:1.75rem;margin-top:1.5rem}#content section>p:first-child{margin-top:0}#content section>p.lead{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.125rem;line-height:1.75rem}#content .centered{text-align:center}#content a.viewcode-back{color:#65758b!important;color:hsl(var(--muted-foreground))!important;position:absolute;right:0}#content a:not(.toc-backref){color:#0f1729;color:hsl(var(--primary));font-weight:500;text-decoration-line:underline;text-decoration-thickness:from-font;text-underline-offset:4px}#content ul:not(.search){list-style-type:disc;margin-left:1.5rem;margin-top:1.5rem}#content ul:not(.search) p,#content ul:not(.search)>li{margin-top:1.5rem}#content ul:not(.search) ul{margin-top:0}#content ol{list-style-type:decimal;margin-left:1.5rem;margin-top:1.5rem}#content ol ::marker{font-weight:500}#content ol::marker{font-weight:500}#content ol p,#content ol>li{margin-top:1.5rem}#content ol ol{margin-top:0}#content dl{margin-top:1.5rem}#content dl dt:not(.sig){font-weight:500;margin-top:1.5rem}#content dl dt:not(.sig):first-child{margin-bottom:0;margin-top:0}#content dl dd{margin-left:1.5rem}#content dl p{margin-bottom:.5rem;margin-top:.5rem}#content .align-center{margin-left:auto;margin-right:auto;text-align:center}#content .align-right{margin-left:auto;text-align:right}#content img{margin-top:1.5rem}#content figure img{display:inline-block}#content figcaption{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:3rem}#content figcaption>*{margin-top:1rem}blockquote{border-left-width:2px;font-style:italic;margin-bottom:1.5rem;margin-top:1.5rem;padding-left:1.5rem}blockquote .attribution{font-style:normal;margin-top:.5rem}table{font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;width:100%}table caption{color:#65758b;color:hsl(var(--muted-foreground));margin-bottom:1.5rem;text-align:left}table thead{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table th{font-weight:500;padding-bottom:.5rem;padding-left:.5rem;text-align:left}table th:first-child{padding-left:0}table th:is(.dark *){font-weight:600}table tbody tr{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border))}table tbody td{padding:.5rem}table tbody td:first-child{padding-left:0}.footnote>.label{float:left;padding-right:.5rem}.footnote>:not(.label){margin-bottom:1.5rem;margin-left:2rem;margin-top:1.5rem}.footnote .footnote-reference,.footnote [role=doc-backlink]{text-decoration-line:none!important}.admonition{background-color:#fff;background-color:hsl(var(--background));border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;color:#0f1729;color:hsl(var(--foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-top:.5rem}.admonition .admonition-title{margin-top:0!important}.admonition-title{font-weight:500}.dark .admonition-title{font-weight:600;letter-spacing:.025em}.note{--tw-border-opacity:1;border-color:#0284c7;border-color:rgba(2,132,199,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0f9ff;background-color:rgba(240,249,255,var(--tw-bg-opacity));--tw-text-opacity:1;color:#0c4a6e;color:rgba(12,74,110,var(--tw-text-opacity))}.dark .note{background-color:rgba(96,165,250,.15);--tw-text-opacity:1;color:#e0f2fe;color:rgba(224,242,254,var(--tw-text-opacity))}.hint,.tip{--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#f0fdf4;background-color:rgba(240,253,244,var(--tw-bg-opacity));--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.dark .hint,.dark .tip{background-color:rgba(74,222,128,.15);--tw-text-opacity:1;color:#dcfce7;color:rgba(220,252,231,var(--tw-text-opacity))}.danger,.error{--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fef2f2;background-color:rgba(254,242,242,var(--tw-bg-opacity));--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.dark .danger,.dark .error{background-color:hsla(0,91%,71%,.15);--tw-text-opacity:1;color:#fee2e2;color:rgba(254,226,226,var(--tw-text-opacity))}.attention,.caution,.important,.warning{--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));--tw-bg-opacity:1;background-color:#fefce8;background-color:rgba(254,252,232,var(--tw-bg-opacity));--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}.dark .attention,.dark .caution,.dark .important,.dark .warning{background-color:rgba(250,204,21,.15);--tw-text-opacity:1;color:#fef9c3;color:rgba(254,249,195,var(--tw-text-opacity))}div.versionadded{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#16a34a;border-color:rgba(22,163,74,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionadded p{margin-top:0!important}div.versionadded p:last-child{margin-bottom:0!important}div.versionadded .versionmodified{font-weight:500;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}div.versionadded .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#22c55e;color:rgba(34,197,94,var(--tw-text-opacity))}div.versionchanged{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#ca8a04;border-color:rgba(202,138,4,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.versionchanged p{margin-top:0!important}div.versionchanged p:last-child{margin-bottom:0!important}div.versionchanged .versionmodified{font-weight:500;--tw-text-opacity:1;color:#713f12;color:rgba(113,63,18,var(--tw-text-opacity))}div.versionchanged .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#eab308;color:rgba(234,179,8,var(--tw-text-opacity))}div.deprecated{border-left-width:3px;margin-top:1rem;--tw-border-opacity:1;border-color:#dc2626;border-color:rgba(220,38,38,var(--tw-border-opacity));font-size:.875rem;line-height:1.25rem;padding:.25rem 1rem}div.deprecated p{margin-top:0!important}div.deprecated p:last-child{margin-bottom:0!important}div.deprecated .versionmodified{font-weight:500;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}div.deprecated .versionmodified:is(.dark *){letter-spacing:.025em;--tw-text-opacity:1;color:#f87171;color:rgba(248,113,113,var(--tw-text-opacity))}.highlight{background-color:transparent;position:relative}.highlight:hover .copy{opacity:1}.highlight .gp,.highlight-pycon .go,.highlight-python .go{-webkit-user-select:none;-moz-user-select:none;user-select:none}.literal-block-wrapper{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;margin-left:0;margin-right:0;margin-top:1.5rem;max-width:none;padding-left:0;padding-right:0}.literal-block-wrapper pre{border-radius:0;border-style:none;margin-top:0}.literal-block-wrapper .code-block-caption{border-bottom-width:1px;border-color:#e1e7ef;border-color:hsl(var(--border));border-top-left-radius:.5rem;border-top-left-radius:var(--radius);border-top-right-radius:.5rem;border-top-right-radius:var(--radius);color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;letter-spacing:.025em;line-height:1.25rem;padding:.5rem 1rem}code{background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:.875rem;line-height:1.25rem;padding:.2em .3em;position:relative;white-space:nowrap}code .ge,code em{color:#0f1729;color:hsl(var(--accent-foreground));font-weight:700;letter-spacing:.025em}:where(h1,h2,h3,h4,h5,h6) code{font-size:inherit}pre{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;margin-top:1.5rem;overflow-x:auto;padding-bottom:1rem;padding-top:1rem}pre[data-theme=dark]{background-color:#fff;background-color:hsl(var(--background))}pre[data-theme=light]{--tw-bg-opacity:1;background-color:#fff;background-color:rgba(255,255,255,var(--tw-bg-opacity))}pre.literal-block{padding-left:1rem;padding-right:1rem}pre code{background-color:transparent;padding:0;white-space:pre}pre code>[id^=line-]{display:block;padding-left:1rem;padding-right:1rem}pre code [id^=line-]:has(.gd),pre code [id^=line-]:has(.gi),pre code [id^=line-]:has(del),pre code [id^=line-]:has(ins),pre code [id^=line-]:has(mark){padding-left:0;padding-right:0}pre code [id^=line-] del,pre code [id^=line-] ins,pre code [id^=line-] mark{display:block;padding-left:1rem;padding-right:1rem;position:relative}pre code [id^=line-] mark{background-color:#f1f5f9;background-color:hsl(var(--muted));color:inherit;--tw-shadow:2px 0 currentColor inset;--tw-shadow-colored:inset 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 2px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] mark:is(.dark *){--tw-bg-opacity:1;background-color:#334155;background-color:rgba(51,65,85,var(--tw-bg-opacity));--tw-shadow:3px 0 currentColor inset;--tw-shadow-colored:inset 3px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,inset 3px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}pre code [id^=line-] ins{background-color:rgba(34,197,94,.3);--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] ins:before{left:2px;position:absolute;--tw-content:"\002b";content:"\002b";content:var(--tw-content)}pre code [id^=line-] ins:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}pre code [id^=line-] del{background-color:rgba(239,68,68,.3);--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] del:before{left:2px;position:absolute;--tw-content:"\2212";content:"\2212";content:var(--tw-content)}pre code [id^=line-] del:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#fecaca;color:rgba(254,202,202,var(--tw-text-opacity))}pre .linenos{padding-left:0;padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight-diff .gi{background-color:rgba(34,197,94,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#14532d;color:rgba(20,83,45,var(--tw-text-opacity))}.highlight-diff .gi:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.highlight-diff .gd{background-color:rgba(239,68,68,.3);display:inline-block;padding-left:1rem;padding-right:1rem;width:100%;--tw-text-opacity:1;color:#7f1d1d;color:rgba(127,29,29,var(--tw-text-opacity))}.highlight-diff .gd:is(.dark *){--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgba(187,247,208,var(--tw-text-opacity))}.guilabel,.menuselection{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500;padding:1px .5rem}#content kbd:not(.compound){background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;border-width:1px;font-size:.875rem;font-weight:500;letter-spacing:.025em;line-height:1.25rem;padding:1px .25rem}.sig{border-color:#e1e7ef;border-color:hsl(var(--border));border-top-width:1px;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-weight:700;padding-top:1.5rem;scroll-margin:5rem}.sig-name{color:#0f1729;color:hsl(var(--accent-foreground))}em.property{color:#65758b;color:hsl(var(--muted-foreground))}.option .sig-prename{font-style:italic}.viewcode-link{color:#65758b;color:hsl(var(--muted-foreground));float:right}.option-list kbd{background-color:transparent!important;border-style:none!important;font-size:1em!important;font-weight:700!important}.headerlink{align-items:center;display:inline-flex;margin-left:.25rem;position:relative;vertical-align:middle}.headerlink:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}.headerlink:focus:after,.headerlink:focus:before,.headerlink:hover:after,.headerlink:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.headerlink:after{margin-top:6px;right:50%;top:100%}.headerlink:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.headerlink:after{margin-right:-16px}.headerlink>*{visibility:hidden;fill:currentColor;color:#65758b;color:hsl(var(--muted-foreground))}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#left-sidebar .caption{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);font-size:.875rem;font-weight:600;line-height:1.25rem;margin-bottom:.25rem;padding:1.5rem .5rem .25rem}#left-sidebar .caption:first-child{padding-top:0}#left-sidebar ul{display:grid;font-size:.875rem;grid-auto-flow:row;grid-auto-rows:max-content;line-height:1.25rem;overflow:hidden;transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.3s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}@media (prefers-reduced-motion:reduce){#left-sidebar ul{transition-property:none}}#left-sidebar ul ul{margin-left:.75rem;opacity:1;padding:.5rem 0 .5rem .75rem;position:relative;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar ul ul:before{bottom:.25rem;left:0;position:absolute;top:.25rem;width:1px;--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgba(229,231,235,var(--tw-bg-opacity));--tw-content:"";content:"";content:var(--tw-content)}#left-sidebar ul ul:is(.dark *):before{content:var(--tw-content);--tw-bg-opacity:1;background-color:#262626;background-color:rgba(38,38,38,var(--tw-bg-opacity))}#left-sidebar a{align-items:center;border-color:transparent;border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);border-width:1px;display:flex;padding:.375rem .5rem;width:100%}#left-sidebar a:hover{text-decoration-line:underline}#left-sidebar a:focus-visible{outline-offset:-1px}#left-sidebar a>button{border-radius:.25rem;color:#65758b;color:hsl(var(--muted-foreground))}#left-sidebar a>button:hover{background-color:rgba(15,23,41,.1);background-color:hsl(var(--primary)/.1)}#left-sidebar a>button>svg{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform-origin:center;transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar a.current{background-color:#f1f5f9;background-color:hsl(var(--accent));border-color:#e1e7ef;border-color:hsl(var(--border));border-width:1px;color:#0f1729;color:hsl(var(--accent-foreground));font-weight:500}#left-sidebar a.expandable{justify-content:space-between}#left-sidebar a.expandable.expanded>button>svg{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}#right-sidebar ul{margin:0}#right-sidebar ul li{margin-top:0;padding-top:.5rem}#right-sidebar ul li a{color:#65758b;color:hsl(var(--muted-foreground));display:inline-block;text-decoration-line:none;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}#right-sidebar ul li a:hover{color:#0f1729;color:hsl(var(--foreground))}#right-sidebar ul li a:focus-visible{outline-offset:-1px}#right-sidebar ul li a[data-current=true]{color:#0f1729;color:hsl(var(--foreground));font-weight:500}#right-sidebar ul li ul{padding-left:1rem}#right-sidebar ul:not(:last-child){padding-bottom:.5rem}.contents>:not([hidden])~:not([hidden]),.toctree-wrapper>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.contents,.toctree-wrapper{font-size:.875rem;line-height:1.25rem}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{font-weight:500;padding-top:1.5rem}.contents ul,.toctree-wrapper ul{list-style-type:none!important;margin:0!important}.contents ul li a.reference,.toctree-wrapper ul li a.reference{color:#65758b!important;color:hsl(var(--muted-foreground))!important;display:inline-block;font-weight:400!important;text-decoration-line:none!important;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.contents ul li a.reference:hover,.toctree-wrapper ul li a.reference:hover{color:#0f1729;color:hsl(var(--foreground))}.contents ul li ul,.toctree-wrapper ul li ul{padding-left:1rem}.contents ul:not(:last-child),.toctree-wrapper ul:not(:last-child){padding-bottom:.5rem}#search-results .search-summary{color:#65758b;color:hsl(var(--muted-foreground));font-size:1.25rem;line-height:1.75rem;margin-top:1.5rem}#search-results ul.search,#search-results ul.search li{margin-top:1.5rem}#search-results ul.search .context{color:#65758b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-top:.5rem}.highlighted{background-color:#f1f5f9;background-color:hsl(var(--accent));text-decoration-line:underline;text-decoration-thickness:2px}.highlight-link{border-color:#e1e7ef;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;padding:.5rem 1rem;position:fixed;right:.5rem;top:4rem}.highlight-link:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}@media (min-width:1024px){.highlight-link{right:4rem}}.tooltipped{position:relative}.tooltipped:after{z-index:1000000;-webkit-font-smoothing:subpixel-antialiased;letter-spacing:normal;text-shadow:none;text-transform:none;word-wrap:break-word;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);content:attr(data-tooltip);display:none;pointer-events:none;position:absolute;white-space:pre;--tw-bg-opacity:0.75;color:#65758b;color:hsl(var(--muted-foreground));font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;line-height:1rem;opacity:0;padding:.25rem;text-align:center;text-decoration-line:none}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.sr-only{height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;width:1px;clip:rect(0,0,0,0);border-width:0;white-space:nowrap}.pointer-events-none{pointer-events:none}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-1{right:.25rem}.right-1\.5{right:.375rem}.right-4{right:1rem}.right-8{right:2rem}.top-0{top:0}.top-16{top:4rem}.top-2{top:.5rem}.top-4{top:1rem}.z-10{z-index:10}.z-20{z-index:20}.z-40{z-index:40}.z-50{z-index:50}.z-\[100\]{z-index:100}.mx-auto{margin-left:auto;margin-right:auto}.my-4{margin-bottom:1rem;margin-top:1rem}.my-6{margin-bottom:1.5rem;margin-top:1.5rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mt-10{margin-top:-2.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-0{margin-left:0}.ml-2{margin-left:.5rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-4{margin-right:1rem}.mr-6{margin-right:1.5rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-4{margin-top:1rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.hidden{display:none}.h-10{height:2.5rem}.h-14{height:3.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-9{height:2.25rem}.h-\[14px\]{height:14px}.h-\[calc\(100vh-8rem\)\]{height:calc(100vh - 8rem)}.h-full{height:100%}.max-h-\[calc\(var\(--vh\)-4rem\)\]{max-height:calc(var(--vh) - 4rem)}.max-h-\[calc\(var\(100vh\)-5rem\)\]{max-height:calc(var(100vh) - 5rem)}.min-h-screen{min-height:100vh}.w-4{width:1rem}.w-5\/6{width:83.333333%}.w-6{width:1.5rem}.w-9{width:2.25rem}.w-\[14px\]{width:14px}.w-full{width:100%}.min-w-0{min-width:0}.min-w-full{min-width:100%}.max-w-prose{max-width:65ch}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1)}.scale-100,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-center{align-items:center}.\!justify-start{justify-content:flex-start!important}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-1{gap:.25rem}.gap-4{gap:1rem}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.25rem;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.25rem*var(--tw-space-x-reverse))}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.5rem;margin-left:calc(.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.5rem*var(--tw-space-x-reverse))}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1.5rem;margin-left:calc(1.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1.5rem*var(--tw-space-x-reverse))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-\[0\.5rem\]{border-radius:.5rem}.rounded-md{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px)}.rounded-sm{border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px)}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-border{border-color:#e1e7ef;border-color:hsl(var(--border))}.border-input{border-color:#e1e7ef;border-color:hsl(var(--input))}.bg-background{background-color:#fff;background-color:hsl(var(--background))}.bg-background\/80{background-color:hsla(0,0%,100%,.8);background-color:hsl(var(--background)/.8)}.bg-background\/95{background-color:hsla(0,0%,100%,.95);background-color:hsl(var(--background)/.95)}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgba(55,65,81,var(--tw-bg-opacity))}.bg-muted{background-color:#f1f5f9;background-color:hsl(var(--muted))}.bg-transparent{background-color:transparent}.fill-current{fill:currentColor}.p-2{padding:.5rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-0{padding-left:0;padding-right:0}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-6{padding-bottom:1.5rem;padding-top:1.5rem}.pr-6{padding-right:1.5rem}.pt-2{padding-top:.5rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.font-mono{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-\[10px\]{font-size:10px}.text-base{font-size:1rem;line-height:1.5rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-loose{line-height:2}.text-foreground{color:#0f1729;color:hsl(var(--foreground))}.text-foreground\/60{color:rgba(15,23,41,.6);color:hsl(var(--foreground)/.6)}.text-muted-foreground{color:#65758b;color:hsl(var(--muted-foreground))}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgba(185,28,28,var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgba(255,255,255,var(--tw-text-opacity))}.underline{text-decoration-line:underline}.no-underline{text-decoration-line:none}.underline-offset-4{text-underline-offset:4px}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-100{opacity:1}.opacity-70{opacity:.7}.shadow-sm{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.05);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 1px 2px 0 rgba(0,0,0,.05);box-shadow:var(--tw-ring-offset-shadow,0 0 transparent),var(--tw-ring-shadow,0 0 transparent),var(--tw-shadow)}.ring-offset-background{--tw-ring-offset-color:hsl(var(--background))}.backdrop-blur{--tw-backdrop-blur:blur(8px);-webkit-backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-colors{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}[x-cloak]{display:none!important}@media (max-width:640px){.container{padding-left:1rem;padding-right:1rem}}.hover\:bg-accent:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.hover\:bg-muted:hover{background-color:#f1f5f9;background-color:hsl(var(--muted))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:text-accent-foreground:hover{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:text-foreground:hover{color:#0f1729;color:hsl(var(--foreground))}.hover\:text-foreground\/80:hover{color:rgba(15,23,41,.8);color:hsl(var(--foreground)/.8)}.hover\:placeholder-accent-foreground:hover::-moz-placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:placeholder-accent-foreground:hover::placeholder{color:#0f1729;color:hsl(var(--accent-foreground))}.hover\:opacity-100:hover{opacity:1}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-accent:focus{background-color:#f1f5f9;background-color:hsl(var(--accent))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgba(3,7,18,var(--tw-bg-opacity))}.focus\:text-accent-foreground:focus{color:#0f1729;color:hsl(var(--accent-foreground))}.focus\:opacity-100:focus{opacity:1}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent;outline-offset:2px}.focus-visible\:outline-offset-\[-1px\]:focus-visible{outline-offset:-1px}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 transparent)}.focus-visible\:ring-ring:focus-visible{--tw-ring-color:hsl(var(--ring))}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width:2px}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:opacity-50:disabled{opacity:.5}.group:hover .group-hover\:bg-accent{background-color:#f1f5f9;background-color:hsl(var(--accent))}.group:hover .group-hover\:text-accent-foreground{color:#0f1729;color:hsl(var(--accent-foreground))}.dark .dark\:block{display:block}.dark .dark\:hidden{display:none}.dark .dark\:-rotate-90{--tw-rotate:-90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(-90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:invert{--tw-invert:invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) invert(100%) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}@media (min-width:640px){.sm\:inline-block{display:inline-block}.sm\:flex{display:flex}.sm\:space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1rem;margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1rem*var(--tw-space-x-reverse))}.sm\:pr-12{padding-right:3rem}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-14{top:3.5rem}.md\:z-30{z-index:30}.md\:my-0{margin-bottom:0;margin-top:0}.md\:-ml-2{margin-left:-.5rem}.md\:inline{display:inline}.md\:flex{display:flex}.md\:grid{display:grid}.md\:\!hidden{display:none!important}.md\:hidden{display:none}.md\:h-24{height:6rem}.md\:h-\[calc\(100vh-3\.5rem\)\]{height:calc(100vh - 3.5rem)}.md\:h-auto{height:auto}.md\:w-40{width:10rem}.md\:w-auto{width:auto}.md\:w-full{width:100%}.md\:flex-none{flex:none}.md\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.md\:grid-cols-\[220px_minmax\(0\2c 1fr\)\]{grid-template-columns:220px minmax(0,1fr)}.md\:flex-row{flex-direction:row}.md\:justify-end{justify-content:flex-end}.md\:gap-2{gap:.5rem}.md\:gap-6{gap:1.5rem}.md\:overflow-auto{overflow:auto}.md\:bg-transparent{background-color:transparent}.md\:p-0{padding:0}.md\:px-0{padding-left:0;padding-right:0}.md\:py-0{padding-bottom:0;padding-top:0}.md\:text-left{text-align:left}}@media (min-width:1024px){.lg\:my-8{margin-bottom:2rem;margin-top:2rem}.lg\:w-64{width:16rem}.lg\:grid-cols-\[240px_minmax\(0\2c 1fr\)\]{grid-template-columns:240px minmax(0,1fr)}.lg\:gap-10{gap:2.5rem}.lg\:py-8{padding-bottom:2rem;padding-top:2rem}}@media (min-width:1280px){.xl\:block{display:block}.xl\:grid{display:grid}.xl\:grid-cols-\[1fr_300px\]{grid-template-columns:1fr 300px}}
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/static/theme.js` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/static/theme.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -69,24 +69,24 @@
                                     function h(e, t) {
                                         for (var n = 0; n < t.length; n++) {
                                             var r = t[n];
                                             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
                                         }
                                     }
 
-                                    function v(e, t) {
-                                        return v = Object.setPrototypeOf || function(e, t) {
+                                    function y(e, t) {
+                                        return y = Object.setPrototypeOf || function(e, t) {
                                             return e.__proto__ = t, e
-                                        }, v(e, t)
+                                        }, y(e, t)
                                     }
 
-                                    function y(e) {
-                                        return y = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                                    function v(e) {
+                                        return v = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                                             return e.__proto__ || Object.getPrototypeOf(e)
-                                        }, y(e)
+                                        }, v(e)
                                     }
 
                                     function m(e, t) {
                                         var n = "data-clipboard-".concat(e);
                                         if (t.hasAttribute(n)) return t.getAttribute(n)
                                     }
                                     var g = function(e) {
@@ -94,29 +94,29 @@
                                                 if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                                                 e.prototype = Object.create(t && t.prototype, {
                                                     constructor: {
                                                         value: e,
                                                         writable: !0,
                                                         configurable: !0
                                                     }
-                                                }), t && v(e, t)
+                                                }), t && y(e, t)
                                             }(l, e);
                                             var t, n, r, i, o, s = (i = l, o = function() {
                                                 if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                                                 if (Reflect.construct.sham) return !1;
                                                 if ("function" == typeof Proxy) return !0;
                                                 try {
                                                     return Date.prototype.toString.call(Reflect.construct(Date, [], (function() {}))), !0
                                                 } catch (e) {
                                                     return !1
                                                 }
                                             }(), function() {
-                                                var e, t, n = y(i);
+                                                var e, t, n = v(i);
                                                 if (o) {
-                                                    var r = y(this).constructor;
+                                                    var r = v(this).constructor;
                                                     e = Reflect.construct(n, arguments, r)
                                                 } else e = n.apply(this, arguments);
                                                 return !(t = e) || "object" !== _(t) && "function" != typeof t ? function(e) {
                                                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                                                     return e
                                                 }(this) : t
                                             });
@@ -451,26 +451,26 @@
             }
             var _ = !0;
 
             function h(e) {
                 o = e
             }
 
-            function v(e, t) {
+            function y(e, t) {
                 let n, r = !0,
                     i = o((() => {
                         let i = e();
                         JSON.stringify(i), r ? n = i : queueMicrotask((() => {
                             t(i, n), n = i
                         })), r = !1
                     }));
                 return () => a(i)
             }
 
-            function y(e, t, n = {}) {
+            function v(e, t, n = {}) {
                 e.dispatchEvent(new CustomEvent(t, {
                     detail: n,
                     bubbles: !0,
                     composed: !0,
                     cancelable: !0
                 }))
             }
@@ -531,16 +531,16 @@
                     };
                     t(e, ((e, t) => {
                         n(e, t), C.forEach((n => n(e, t))), xe(e, e.attributes).forEach((e => e())), e._x_ignore && t()
                     })), we = !1, o()
                 }()
             }
 
-            function L(e) {
-                m(e, (e => {
+            function L(e, t = m) {
+                t(e, (e => {
                     I(e),
                         function(e) {
                             if (e._x_cleanups)
                                 for (; e._x_cleanups.length;) e._x_cleanups.pop()()
                         }(e)
                 }))
             }
@@ -561,44 +561,44 @@
             }
 
             function I(e, t) {
                 e._x_attributeCleanups && Object.entries(e._x_attributeCleanups).forEach((([n, r]) => {
                     (void 0 === t || t.includes(n)) && (r.forEach((e => e())), delete e._x_attributeCleanups[n])
                 }))
             }
-            var z = new MutationObserver(K),
-                B = !1;
+            var D = new MutationObserver(K),
+                z = !1;
 
-            function D() {
-                z.observe(document, {
+            function B() {
+                D.observe(document, {
                     subtree: !0,
                     childList: !0,
                     attributes: !0,
                     attributeOldValue: !0
-                }), B = !0
+                }), z = !0
             }
 
             function F() {
                 ! function() {
-                    let e = z.takeRecords();
+                    let e = D.takeRecords();
                     H.push((() => e.length > 0 && K(e)));
                     let t = H.length;
                     queueMicrotask((() => {
                         if (H.length === t)
                             for (; H.length > 0;) H.shift()()
                     }))
-                }(), z.disconnect(), B = !1
+                }(), D.disconnect(), z = !1
             }
             var H = [];
 
             function W(e) {
-                if (!B) return e();
+                if (!z) return e();
                 F();
                 let t = e();
-                return D(), t
+                return B(), t
             }
             var V = !1,
                 U = [];
 
             function K(e) {
                 if (V) return void(U = U.concat(e));
                 let t = new Set,
@@ -659,20 +659,20 @@
                     objects: e
                 }) {
                     return Array.from(new Set(e.flatMap((e => Object.keys(e)))))
                 },
                 has({
                     objects: e
                 }, t) {
-                    return t != Symbol.unscopables && e.some((e => Object.prototype.hasOwnProperty.call(e, t)))
+                    return t != Symbol.unscopables && e.some((e => Object.prototype.hasOwnProperty.call(e, t) || Reflect.has(e, t)))
                 },
                 get({
                     objects: e
                 }, t, n) {
-                    return "toJSON" == t ? Q : Reflect.get(e.find((e => Object.prototype.hasOwnProperty.call(e, t))) || {}, t, n)
+                    return "toJSON" == t ? Q : Reflect.get(e.find((e => Reflect.has(e, t))) || {}, t, n)
                 },
                 set({
                     objects: e
                 }, t, n, r) {
                     const i = e.find((e => Object.prototype.hasOwnProperty.call(e, t))) || e[e.length - 1],
                         o = Object.getOwnPropertyDescriptor(i, t);
                     return o?.set && o?.get ? Reflect.set(i, t, n, r) : Reflect.set(i, t, n)
@@ -686,14 +686,15 @@
             function ee(e) {
                 let t = (n, r = "") => {
                     Object.entries(Object.getOwnPropertyDescriptors(n)).forEach((([i, {
                         value: o,
                         enumerable: a
                     }]) => {
                         if (!1 === a || void 0 === o) return;
+                        if ("object" == typeof o && null !== o && o.__v_skip) return;
                         let s = "" === r ? i : `${r}.${i}`;
                         var l;
                         "object" == typeof o && null !== o && o._x_interceptor ? n[i] = o.initialize(e, s, i) : "object" != typeof(l = o) || Array.isArray(l) || null === l || o === n || o instanceof Element || t(o, s)
                     }))
                 };
                 return t(e)
             }
@@ -839,18 +840,18 @@
 
             function he(e, t, n, r, i) {
                 if (le && "function" == typeof t) {
                     let o = t.apply(n, r);
                     o instanceof Promise ? o.then((t => he(e, t, n, r))).catch((e => se(e, i, t))) : e(o)
                 } else "object" == typeof t && t instanceof Promise ? t.then((t => e(t))) : e(t)
             }
-            var ve = "x-";
+            var ye = "x-";
 
-            function ye(e = "") {
-                return ve + e
+            function ve(e = "") {
+                return ye + e
             }
             var me = {};
 
             function ge(e, t) {
                 return me[e] = t, {
                     before(t) {
                         if (!me[t]) return void console.warn(String.raw`Cannot find directive \`${t}\`. \`${e}\` will use the default order of execution`);
@@ -965,15 +966,15 @@
             }
 
             function Te({
                 name: e
             }) {
                 return Le().test(e)
             }
-            var Le = () => new RegExp(`^${ve}([^:^.]+)\\b`),
+            var Le = () => new RegExp(`^${ye}([^:^.]+)\\b`),
                 $e = "DEFAULT",
                 Me = ["ignore", "ref", "data", "id", "anchor", "bind", "init", "for", "model", "modelable", "transition", "show", "if", $e, "teleport"];
 
             function Ne(e, t) {
                 let n = -1 === Me.indexOf(e.type) ? $e : e.type,
                     r = -1 === Me.indexOf(t.type) ? $e : t.type;
                 return Me.indexOf(n) - Me.indexOf(r)
@@ -993,47 +994,47 @@
                 }))
             }
 
             function Ie() {
                 for (Re = !1; Pe.length;) Pe.shift()()
             }
 
-            function ze(e, t) {
-                return Array.isArray(t) ? Be(e, t.join(" ")) : "object" == typeof t && null !== t ? function(e, t) {
+            function De(e, t) {
+                return Array.isArray(t) ? ze(e, t.join(" ")) : "object" == typeof t && null !== t ? function(e, t) {
                     let n = e => e.split(" ").filter(Boolean),
                         r = Object.entries(t).flatMap((([e, t]) => !!t && n(e))).filter(Boolean),
                         i = Object.entries(t).flatMap((([e, t]) => !t && n(e))).filter(Boolean),
                         o = [],
                         a = [];
                     return i.forEach((t => {
                         e.classList.contains(t) && (e.classList.remove(t), a.push(t))
                     })), r.forEach((t => {
                         e.classList.contains(t) || (e.classList.add(t), o.push(t))
                     })), () => {
                         a.forEach((t => e.classList.add(t))), o.forEach((t => e.classList.remove(t)))
                     }
-                }(e, t) : "function" == typeof t ? ze(e, t()) : Be(e, t)
+                }(e, t) : "function" == typeof t ? De(e, t()) : ze(e, t)
             }
 
-            function Be(e, t) {
+            function ze(e, t) {
                 return t = !0 === t ? t = "" : t || "", n = t.split(" ").filter((t => !e.classList.contains(t))).filter(Boolean), e.classList.add(...n), () => {
                     e.classList.remove(...n)
                 };
                 var n
             }
 
-            function De(e, t) {
+            function Be(e, t) {
                 return "object" == typeof t && null !== t ? function(e, t) {
                     let n = {};
                     return Object.entries(t).forEach((([t, r]) => {
                         n[t] = e.style[t], t.startsWith("--") || (t = t.replace(/([a-z])([A-Z])/g, "$1-$2").toLowerCase()), e.style.setProperty(t, r)
                     })), setTimeout((() => {
                         0 === e.style.length && e.removeAttribute("style")
                     })), () => {
-                        De(e, n)
+                        Be(e, n)
                     }
                 }(e, t) : function(e, t) {
                     let n = e.getAttribute("style", t);
                     return e.setAttribute("style", t), () => {
                         e.setAttribute("style", n || "")
                     }
                 }(e, t)
@@ -1150,15 +1151,15 @@
                 value: t,
                 modifiers: n,
                 expression: r
             }, {
                 evaluate: i
             }) => {
                 "function" == typeof r && (r = i(r)), !1 !== r && (r && "boolean" != typeof r ? function(e, t, n) {
-                    He(e, ze, ""), {
+                    He(e, De, ""), {
                         enter: t => {
                             e._x_transition.enter.during = t
                         },
                         "enter-start": t => {
                             e._x_transition.enter.start = t
                         },
                         "enter-end": t => {
@@ -1171,15 +1172,15 @@
                             e._x_transition.leave.start = t
                         },
                         "leave-end": t => {
                             e._x_transition.leave.end = t
                         }
                     } [n](t)
                 }(e, r, t) : function(e, t, n) {
-                    He(e, De);
+                    He(e, Be);
                     let r = !t.includes("in") && !t.includes("out") && !n,
                         i = r || t.includes("in") || ["enter"].includes(n),
                         o = r || t.includes("out") || ["leave"].includes(n);
                     t.includes("in") && !r && (t = t.filter(((e, n) => n < t.indexOf("out")))), t.includes("out") && !r && (t = t.filter(((e, n) => n > t.indexOf("out"))));
                     let a = !t.includes("opacity") && !t.includes("scale"),
                         s = a || t.includes("opacity") ? 0 : 1,
                         l = a || t.includes("scale") ? Ue(t, "scale", 95) / 100 : 1,
@@ -1271,20 +1272,20 @@
                                 if (e.value === t) return;
                                 e.value = void 0 === t ? "" : t
                             }
                         }(e, n);
                         break;
                     case "style":
                         ! function(e, t) {
-                            e._x_undoAddedStyles && e._x_undoAddedStyles(), e._x_undoAddedStyles = De(e, t)
+                            e._x_undoAddedStyles && e._x_undoAddedStyles(), e._x_undoAddedStyles = Be(e, t)
                         }(e, n);
                         break;
                     case "class":
                         ! function(e, t) {
-                            e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedClasses = ze(e, t)
+                            e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedClasses = De(e, t)
                         }(e, n);
                         break;
                     case "selected":
                     case "checked":
                         ! function(e, t, n) {
                             et(e, t, n),
                                 function(e, t, n) {
@@ -1310,15 +1311,15 @@
             }
 
             function nt(e) {
                 return !![1, "1", "true", "on", "yes", !0].includes(e) || ![0, "0", "false", "off", "no", !1].includes(e) && (e ? Boolean(e) : null)
             }
 
             function rt(e) {
-                return ["disabled", "checked", "required", "readonly", "hidden", "open", "selected", "autofocus", "itemscope", "multiple", "novalidate", "allowfullscreen", "allowpaymentrequest", "formnovalidate", "autoplay", "controls", "loop", "muted", "playsinline", "default", "ismap", "reversed", "async", "defer", "nomodule"].includes(e)
+                return ["disabled", "checked", "required", "readonly", "open", "selected", "autofocus", "itemscope", "multiple", "novalidate", "allowfullscreen", "allowpaymentrequest", "formnovalidate", "autoplay", "controls", "loop", "muted", "playsinline", "default", "ismap", "reversed", "async", "defer", "nomodule"].includes(e)
             }
 
             function it(e, t, n) {
                 let r = e.getAttribute(t);
                 return null === r ? "function" == typeof n ? n() : n : "" === r || (rt(t) ? !![t, "true"].includes(r) : r)
             }
 
@@ -1399,23 +1400,23 @@
                     },
                     get effect() {
                         return o
                     },
                     get raw() {
                         return s
                     },
-                    version: "3.13.5",
+                    version: "3.13.8",
                     flushAndStopDeferringMutations: function() {
                         V = !1, K(U), U = []
                     },
                     dontAutoEvaluateFunctions: ce,
                     disableEffectScheduling: function(e) {
                         _ = !1, e(), _ = !0
                     },
-                    startObservingMutations: D,
+                    startObservingMutations: B,
                     stopObservingMutations: F,
                     setReactivityEngine: function(e) {
                         i = e.reactive, a = e.release, o = t => e.effect(t, {
                             scheduler: e => {
                                 _ ? function(e) {
                                     var t;
                                     t = e, u.includes(t) || u.push(t), c || l || (l = !0, queueMicrotask(p))
@@ -1456,42 +1457,42 @@
                     },
                     findClosest: j,
                     onElRemoved: P,
                     closestRoot: k,
                     destroyTree: L,
                     interceptor: te,
                     transition: Ve,
-                    setStyles: De,
+                    setStyles: Be,
                     mutateDom: W,
                     directive: ge,
                     entangle: st,
                     throttle: at,
                     debounce: ot,
                     evaluate: ue,
                     initTree: T,
                     nextTick: qe,
-                    prefixed: ye,
+                    prefixed: ve,
                     prefix: function(e) {
-                        ve = e
+                        ye = e
                     },
                     plugin: function(e) {
                         (Array.isArray(e) ? e : [e]).forEach((e => e(_t)))
                     },
                     magic: ie,
                     store: function(e, t) {
                         if (ut || (ct = i(ct), ut = !0), void 0 === t) return ct[e];
                         ct[e] = t, "object" == typeof t && null !== t && t.hasOwnProperty("init") && "function" == typeof t.init && ct[e].init(), ee(ct[e])
                     },
                     start: function() {
                         var e;
-                        x && g("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), x = !0, document.body || g("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), y(document, "alpine:init"), y(document, "alpine:initializing"), D(), e = e => T(e, m), N.push(e), P((e => L(e))), R(((e, t) => {
+                        x && g("Alpine has already been initialized on this page. Calling Alpine.start() more than once can cause problems."), x = !0, document.body || g("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), v(document, "alpine:init"), v(document, "alpine:initializing"), B(), e = e => T(e, m), N.push(e), P((e => L(e))), R(((e, t) => {
                             xe(e, t).forEach((e => e()))
                         })), Array.from(document.querySelectorAll(S().join(","))).filter((e => !k(e.parentElement, !0))).forEach((e => {
                             T(e)
-                        })), y(document, "alpine:initialized")
+                        })), v(document, "alpine:initialized")
                     },
                     clone: function(e, t) {
                         t._x_dataStack || (t._x_dataStack = e._x_dataStack), Ke = !0, Ye = !0, Ge((() => {
                             ! function(e) {
                                 let t = !1;
                                 T(e, ((e, n) => {
                                     m(e, ((e, r) => {
@@ -1511,15 +1512,15 @@
                             }))
                         })), Ke = !1
                     },
                     bound: function(e, t, n) {
                         return e._x_bindings && void 0 !== e._x_bindings[t] ? e._x_bindings[t] : it(e, t, n)
                     },
                     $data: Z,
-                    watch: v,
+                    watch: y,
                     walk: m,
                     data: function(e, t) {
                         pt[e] = t
                     },
                     bind: function(e, t) {
                         let n = "function" != typeof t ? () => t : t;
                         return e instanceof Element ? dt(e, n()) : (ft[e] = n, () => {})
@@ -1528,15 +1529,15 @@
 
             function ht(e, t) {
                 const n = Object.create(null),
                     r = e.split(",");
                 for (let e = 0; e < r.length; e++) n[r[e]] = !0;
                 return t ? e => !!n[e.toLowerCase()] : e => !!n[e]
             }
-            var vt, yt = Object.freeze({}),
+            var yt, vt = Object.freeze({}),
                 mt = (Object.freeze([]), Object.prototype.hasOwnProperty),
                 gt = (e, t) => mt.call(e, t),
                 xt = Array.isArray,
                 bt = e => "[object Map]" === At(e),
                 wt = e => "symbol" == typeof e,
                 Et = e => null !== e && "object" == typeof e,
                 St = Object.prototype.toString,
@@ -1562,42 +1563,42 @@
                     deps: t
                 } = e;
                 if (t.length) {
                     for (let n = 0; n < t.length; n++) t[n].delete(e);
                     t.length = 0
                 }
             }
-            var zt = !0,
-                Bt = [];
+            var Dt = !0,
+                zt = [];
 
-            function Dt() {
-                const e = Bt.pop();
-                zt = void 0 === e || e
+            function Bt() {
+                const e = zt.pop();
+                Dt = void 0 === e || e
             }
 
             function Ft(e, t, n) {
-                if (!zt || void 0 === vt) return;
+                if (!Dt || void 0 === yt) return;
                 let r = Mt.get(e);
                 r || Mt.set(e, r = new Map);
                 let i = r.get(n);
-                i || r.set(n, i = new Set), i.has(vt) || (i.add(vt), vt.deps.push(i), vt.options.onTrack && vt.options.onTrack({
-                    effect: vt,
+                i || r.set(n, i = new Set), i.has(yt) || (i.add(yt), yt.deps.push(i), yt.options.onTrack && yt.options.onTrack({
+                    effect: yt,
                     target: e,
                     type: t,
                     key: n
                 }))
             }
 
             function Ht(e, t, n, r, i, o) {
                 const a = Mt.get(e);
                 if (!a) return;
                 const s = new Set,
                     l = e => {
                         e && e.forEach((e => {
-                            (e !== vt || e.allowRecurse) && s.add(e)
+                            (e !== yt || e.allowRecurse) && s.add(e)
                         }))
                     };
                 if ("clear" === t) a.forEach(l);
                 else if ("length" === n && xt(e)) a.forEach(((e, t) => {
                     ("length" === t || t >= r) && l(e)
                 }));
                 else switch (void 0 !== n && l(a.get(n)), t) {
@@ -1635,17 +1636,17 @@
                         const n = Ln(this);
                         for (let e = 0, t = this.length; e < t; e++) Ft(n, "get", e + "");
                         const r = n[t](...e);
                         return -1 === r || !1 === r ? n[t](...e.map(Ln)) : r
                     }
                 })), ["push", "pop", "shift", "unshift", "splice"].forEach((t => {
                     e[t] = function(...e) {
-                        Bt.push(zt), zt = !1;
+                        zt.push(Dt), Dt = !1;
                         const n = Ln(this)[t].apply(this, e);
-                        return Dt(), n
+                        return Bt(), n
                     }
                 })), e
             }
 
             function Xt(e = !1, t = !1) {
                 return function(n, r, i) {
                     if ("__v_isReactive" === r) return !e;
@@ -1870,18 +1871,18 @@
                         clear: _n("clear"),
                         forEach: dn(!0, !0)
                     };
                 return ["keys", "values", "entries", Symbol.iterator].forEach((i => {
                     e[i] = pn(i, !1, !1), n[i] = pn(i, !0, !1), t[i] = pn(i, !1, !0), r[i] = pn(i, !0, !0)
                 })), [e, n, t, r]
             }
-            var [vn, yn, mn, gn] = hn();
+            var [yn, vn, mn, gn] = hn();
 
             function xn(e, t) {
-                const n = t ? e ? gn : mn : e ? yn : vn;
+                const n = t ? e ? gn : mn : e ? vn : yn;
                 return (t, r, i) => "__v_isReactive" === r ? !e : "__v_isReadonly" === r ? e : "__v_raw" === r ? t : Reflect.get(gt(n, r) && r in t ? n : t, r, i)
             }
             var bn = {
                     get: xn(!1, !1)
                 },
                 wn = {
                     get: xn(!0, !1)
@@ -1935,31 +1936,31 @@
             function Ln(e) {
                 return e && Ln(e.__v_raw) || e
             }
 
             function $n(e) {
                 return Boolean(e && !0 === e.__v_isRef)
             }
-            ie("nextTick", (() => qe)), ie("dispatch", (e => y.bind(y, e))), ie("watch", ((e, {
+            ie("nextTick", (() => qe)), ie("dispatch", (e => v.bind(v, e))), ie("watch", ((e, {
                 evaluateLater: t,
                 cleanup: n
             }) => (e, r) => {
                 let i = t(e),
-                    o = v((() => {
+                    o = y((() => {
                         let e;
                         return i((t => e = t)), e
                     }), r);
                 n(o)
             })), ie("store", (function() {
                 return ct
             })), ie("data", (e => Z(e))), ie("root", (e => k(e))), ie("refs", (e => (e._x_refs_proxy || (e._x_refs_proxy = Y(function(e) {
-                let t = [],
-                    n = e;
-                for (; n;) n._x_refs && t.push(n._x_refs), n = n.parentNode;
-                return t
+                let t = [];
+                return j(e, (e => {
+                    e._x_refs && t.push(e._x_refs)
+                })), t
             }(e))), e._x_refs_proxy)));
             var Mn = {};
 
             function Nn(e) {
                 return Mn[e] || (Mn[e] = 0), ++Mn[e]
             }
 
@@ -2055,27 +2056,27 @@
 
             function qn(e) {
                 let t = Ze((() => document.querySelector(e)), (() => Rn))();
                 return t || g(`Cannot find x-teleport element for selector: "${e}"`), t
             }
             var In = () => {};
 
-            function zn(e, t, n, r) {
+            function Dn(e, t, n, r) {
                 let i = e,
                     o = e => r(e),
                     a = {},
                     s = (e, t) => n => t(e, n);
                 if (n.includes("dot") && (t = t.replace(/-/g, ".")), n.includes("camel") && (t = t.toLowerCase().replace(/-(\w)/g, ((e, t) => t.toUpperCase()))), n.includes("passive") && (a.passive = !0), n.includes("capture") && (a.capture = !0), n.includes("window") && (i = window), n.includes("document") && (i = document), n.includes("debounce")) {
                     let e = n[n.indexOf("debounce") + 1] || "invalid-wait",
-                        t = Bn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
+                        t = zn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
                     o = ot(o, t)
                 }
                 if (n.includes("throttle")) {
                     let e = n[n.indexOf("throttle") + 1] || "invalid-wait",
-                        t = Bn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
+                        t = zn(e.split("ms")[0]) ? Number(e.split("ms")[0]) : 250;
                     o = at(o, t)
                 }
                 return n.includes("prevent") && (o = s(o, ((e, t) => {
                     t.preventDefault(), e(t)
                 }))), n.includes("stop") && (o = s(o, ((e, t) => {
                     t.stopPropagation(), e(t)
                 }))), n.includes("self") && (o = s(o, ((t, n) => {
@@ -2087,35 +2088,35 @@
                 }))), o = s(o, ((e, r) => {
                     (function(e) {
                         return ["keydown", "keyup"].includes(e)
                     })(t) && function(e, t) {
                         let n = t.filter((e => !["window", "document", "prevent", "stop", "once", "capture"].includes(e)));
                         if (n.includes("debounce")) {
                             let e = n.indexOf("debounce");
-                            n.splice(e, Bn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
+                            n.splice(e, zn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
                         }
                         if (n.includes("throttle")) {
                             let e = n.indexOf("throttle");
-                            n.splice(e, Bn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
+                            n.splice(e, zn((n[e + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
                         }
                         if (0 === n.length) return !1;
-                        if (1 === n.length && Dn(e.key).includes(n[0])) return !1;
+                        if (1 === n.length && Bn(e.key).includes(n[0])) return !1;
                         const r = ["ctrl", "shift", "alt", "meta", "cmd", "super"].filter((e => n.includes(e)));
-                        return n = n.filter((e => !r.includes(e))), !(r.length > 0 && r.filter((t => ("cmd" !== t && "super" !== t || (t = "meta"), e[`${t}Key`]))).length === r.length && Dn(e.key).includes(n[0]))
+                        return n = n.filter((e => !r.includes(e))), !(r.length > 0 && r.filter((t => ("cmd" !== t && "super" !== t || (t = "meta"), e[`${t}Key`]))).length === r.length && Bn(e.key).includes(n[0]))
                     }(r, n) || e(r)
                 })), i.addEventListener(t, o, a), () => {
                     i.removeEventListener(t, o, a)
                 }
             }
 
-            function Bn(e) {
+            function zn(e) {
                 return !Array.isArray(e) && !isNaN(e)
             }
 
-            function Dn(e) {
+            function Bn(e) {
                 if (!e) return [];
                 var t;
                 e = [" ", "_"].includes(t = e) ? t : t.replace(/([a-z])([A-Z])/g, "$1-$2").replace(/[_\s]/, "-").toLowerCase();
                 let n = {
                     ctrl: "control",
                     slash: "/",
                     space: " ",
@@ -2132,21 +2133,39 @@
                     underscore: "_"
                 };
                 return n[e] = e, Object.keys(n).map((t => {
                     if (n[t] === e) return t
                 })).filter((e => e))
             }
 
-            function Fn(e) {
+            function Fn(e, t, n, r) {
+                return W((() => {
+                    if (n instanceof CustomEvent && void 0 !== n.detail) return null !== n.detail && void 0 !== n.detail ? n.detail : n.target.value;
+                    if ("checkbox" === e.type) {
+                        if (Array.isArray(r)) {
+                            let e = null;
+                            return e = t.includes("number") ? Hn(n.target.value) : t.includes("boolean") ? nt(n.target.value) : n.target.value, n.target.checked ? r.concat([e]) : r.filter((t => !(t == e)))
+                        }
+                        return n.target.checked
+                    }
+                    if ("select" === e.tagName.toLowerCase() && e.multiple) return t.includes("number") ? Array.from(n.target.selectedOptions).map((e => Hn(e.value || e.text))) : t.includes("boolean") ? Array.from(n.target.selectedOptions).map((e => nt(e.value || e.text))) : Array.from(n.target.selectedOptions).map((e => e.value || e.text));
+                    {
+                        let i;
+                        return i = "radio" === e.type ? n.target.checked ? n.target.value : r : n.target.value, t.includes("number") ? Hn(i) : t.includes("boolean") ? nt(i) : t.includes("trim") ? i.trim() : i
+                    }
+                }))
+            }
+
+            function Hn(e) {
                 let t = e ? parseFloat(e) : null;
                 return n = t, Array.isArray(n) || isNaN(n) ? e : t;
                 var n
             }
 
-            function Hn(e) {
+            function Wn(e) {
                 return null !== e && "object" == typeof e && "function" == typeof e.get && "function" == typeof e.set
             }
             In.inline = (e, {
                 modifiers: t
             }, {
                 cleanup: n
             }) => {
@@ -2168,45 +2187,35 @@
             }) => {
                 let o = e;
                 t.includes("parent") && (o = e.parentNode);
                 let a, s = fe(o, n);
                 a = "string" == typeof n ? fe(o, `${n} = __placeholder`) : "function" == typeof n && "string" == typeof n() ? fe(o, `${n()} = __placeholder`) : () => {};
                 let l = () => {
                         let e;
-                        return s((t => e = t)), Hn(e) ? e.get() : e
+                        return s((t => e = t)), Wn(e) ? e.get() : e
                     },
                     c = e => {
                         let t;
-                        s((e => t = e)), Hn(t) ? t.set(e) : a((() => {}), {
+                        s((e => t = e)), Wn(t) ? t.set(e) : a((() => {}), {
                             scope: {
                                 __placeholder: e
                             }
                         })
                     };
                 "string" == typeof n && "radio" === e.type && W((() => {
                     e.hasAttribute("name") || e.setAttribute("name", n)
                 }));
                 var u = "select" === e.tagName.toLowerCase() || ["checkbox", "radio"].includes(e.type) || t.includes("lazy") ? "change" : "input";
-                let f = Ke ? () => {} : zn(e, u, t, (n => {
-                    c(function(e, t, n, r) {
-                        return W((() => {
-                            if (n instanceof CustomEvent && void 0 !== n.detail) return null !== n.detail && void 0 !== n.detail ? n.detail : n.target.value;
-                            if ("checkbox" === e.type) {
-                                if (Array.isArray(r)) {
-                                    let e = null;
-                                    return e = t.includes("number") ? Fn(n.target.value) : t.includes("boolean") ? nt(n.target.value) : n.target.value, n.target.checked ? r.concat([e]) : r.filter((t => !(t == e)))
-                                }
-                                return n.target.checked
-                            }
-                            return "select" === e.tagName.toLowerCase() && e.multiple ? t.includes("number") ? Array.from(n.target.selectedOptions).map((e => Fn(e.value || e.text))) : t.includes("boolean") ? Array.from(n.target.selectedOptions).map((e => nt(e.value || e.text))) : Array.from(n.target.selectedOptions).map((e => e.value || e.text)) : t.includes("number") ? Fn(n.target.value) : t.includes("boolean") ? nt(n.target.value) : t.includes("trim") ? n.target.value.trim() : n.target.value
-                        }))
-                    }(e, t, n, l()))
+                let f = Ke ? () => {} : Dn(e, u, t, (n => {
+                    c(Fn(e, t, n, l()))
                 }));
-                if (t.includes("fill") && ([void 0, null, ""].includes(l()) || "checkbox" === e.type && Array.isArray(l())) && e.dispatchEvent(new Event(u, {})), e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = f, i((() => e._x_removeModelListeners.default())), e.form) {
-                    let t = zn(e.form, "reset", [], (t => {
+                if (t.includes("fill") && ([void 0, null, ""].includes(l()) || "checkbox" === e.type && Array.isArray(l())) && c(Fn(e, t, {
+                        target: e
+                    }, l())), e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = f, i((() => e._x_removeModelListeners.default())), e.form) {
+                    let t = Dn(e.form, "reset", [], (t => {
                         qe((() => e._x_model && e._x_model.set(e.value)))
                     }));
                     i((() => t()))
                 }
                 e._x_model = {
                     get() {
                         return l()
@@ -2216,15 +2225,15 @@
                     }
                 }, e._x_forceModelUpdate = t => {
                     void 0 === t && "string" == typeof n && n.match(/\./) && (t = ""), window.fromModel = !0, W((() => Qe(e, "value", t))), delete window.fromModel
                 }, r((() => {
                     let n = l();
                     t.includes("unintrusive") && document.activeElement.isSameNode(e) || e._x_forceModelUpdate(n)
                 }))
-            })), ge("cloak", (e => queueMicrotask((() => W((() => e.removeAttribute(ye("cloak")))))))), O((() => `[${ye("init")}]`)), ge("init", Ze(((e, {
+            })), ge("cloak", (e => queueMicrotask((() => W((() => e.removeAttribute(ve("cloak")))))))), O((() => `[${ve("init")}]`)), ge("init", Ze(((e, {
                 expression: t
             }, {
                 evaluate: n
             }) => "string" == typeof t ? !!t.trim() && n(t, {}, !1) : n(t, {}, !1)))), ge("text", ((e, {
                 expression: t
             }, {
                 effect: n,
@@ -2248,72 +2257,75 @@
                 n((() => {
                     i((t => {
                         W((() => {
                             e.innerHTML = t, e._x_ignoreSelf = !0, T(e), delete e._x_ignoreSelf
                         }))
                     }))
                 }))
-            })), Ce(Oe(":", ye("bind:")));
-            var Wn = (e, {
+            })), Ce(Oe(":", ve("bind:")));
+            var Vn = (e, {
                 value: t,
                 modifiers: n,
                 expression: r,
                 original: i
             }, {
-                effect: o
+                effect: o,
+                cleanup: a
             }) => {
                 if (!t) {
                     let t = {};
-                    return a = t, Object.entries(ft).forEach((([e, t]) => {
-                        Object.defineProperty(a, e, {
+                    return s = t, Object.entries(ft).forEach((([e, t]) => {
+                        Object.defineProperty(s, e, {
                             get() {
                                 return (...e) => t(...e)
                             }
                         })
                     })), void fe(e, r)((t => {
                         dt(e, t, i)
                     }), {
                         scope: t
                     })
                 }
-                var a;
+                var s;
                 if ("key" === t) return function(e, t) {
                     e._x_keyExpression = t
                 }(e, r);
                 if (e._x_inlineBindings && e._x_inlineBindings[t] && e._x_inlineBindings[t].extract) return;
-                let s = fe(e, r);
-                o((() => s((i => {
+                let l = fe(e, r);
+                o((() => l((i => {
                     void 0 === i && "string" == typeof r && r.match(/\./) && (i = ""), W((() => Qe(e, t, i, n)))
-                }))))
+                })))), a((() => {
+                    e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedStyles && e._x_undoAddedStyles()
+                }))
             };
 
-            function Vn(e, t, n, r) {
+            function Un(e, t, n, r) {
                 let i = {};
                 return /^\[.*\]$/.test(e.item) && Array.isArray(t) ? e.item.replace("[", "").replace("]", "").split(",").map((e => e.trim())).forEach(((e, n) => {
                     i[e] = t[n]
                 })) : /^\{.*\}$/.test(e.item) && !Array.isArray(t) && "object" == typeof t ? e.item.replace("{", "").replace("}", "").split(",").map((e => e.trim())).forEach((e => {
                     i[e] = t[e]
                 })) : i[e.item] = t, e.index && (i[e.index] = n), e.collection && (i[e.collection] = r), i
             }
 
-            function Un() {}
+            function Kn() {}
 
-            function Kn(e, t, n) {
+            function Zn(e, t, n) {
                 ge(t, (r => g(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${n}`, r)))
             }
-            Wn.inline = (e, {
+            Vn.inline = (e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }) => {
                 t && (e._x_inlineBindings || (e._x_inlineBindings = {}), e._x_inlineBindings[t] = {
                     expression: r,
                     extract: !1
                 })
-            }, ge("bind", Wn), A((() => `[${ye("data")}]`)), ge("data", ((e, {
+            }, ge("bind", Vn), A((() => `[${ve("data")}]`)), ge("data", ((e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
                 if (function(e) {
                         return !!Ke && (!!Ye || e.hasAttribute("data-has-alpine-state"))
                     }(e)) return;
@@ -2396,104 +2408,108 @@
                         var a;
                         a = n, !Array.isArray(a) && !isNaN(a) && n >= 0 && (n = Array.from(Array(n).keys(), (e => e + 1))), void 0 === n && (n = []);
                         let s = e._x_lookup,
                             l = e._x_prevKeys,
                             c = [],
                             u = [];
                         if ("object" != typeof(f = n) || Array.isArray(f))
-                            for (let e = 0; e < n.length; e++) {
-                                let i = Vn(t, n[e], e, n);
-                                r((e => u.push(e)), {
-                                    scope: {
-                                        index: e,
-                                        ...i
-                                    }
-                                }), c.push(i)
-                            } else n = Object.entries(n).map((([e, i]) => {
-                                let o = Vn(t, i, e, n);
-                                r((e => u.push(e)), {
+                            for (let i = 0; i < n.length; i++) {
+                                let o = Un(t, n[i], i, n);
+                                r((t => {
+                                    u.includes(t) && g("Duplicate key on x-for", e), u.push(t)
+                                }), {
                                     scope: {
-                                        index: e,
+                                        index: i,
                                         ...o
                                     }
                                 }), c.push(o)
+                            } else n = Object.entries(n).map((([i, o]) => {
+                                let a = Un(t, o, i, n);
+                                r((t => {
+                                    u.includes(t) && g("Duplicate key on x-for", e), u.push(t)
+                                }), {
+                                    scope: {
+                                        index: i,
+                                        ...a
+                                    }
+                                }), c.push(a)
                             }));
                         var f;
                         let p = [],
                             _ = [],
                             h = [],
-                            v = [];
+                            y = [];
                         for (let e = 0; e < l.length; e++) {
                             let t = l[e]; - 1 === u.indexOf(t) && h.push(t)
                         }
                         l = l.filter((e => !h.includes(e)));
-                        let y = "template";
+                        let v = "template";
                         for (let e = 0; e < u.length; e++) {
                             let t = u[e],
                                 n = l.indexOf(t);
-                            if (-1 === n) l.splice(e, 0, t), p.push([y, e]);
+                            if (-1 === n) l.splice(e, 0, t), p.push([v, e]);
                             else if (n !== e) {
                                 let t = l.splice(e, 1)[0],
                                     r = l.splice(n - 1, 1)[0];
                                 l.splice(e, 0, r), l.splice(n, 0, t), _.push([t, r])
-                            } else v.push(t);
-                            y = t
+                            } else y.push(t);
+                            v = t
                         }
                         for (let e = 0; e < h.length; e++) {
                             let t = h[e];
                             s[t]._x_effects && s[t]._x_effects.forEach(d), s[t].remove(), s[t] = null, delete s[t]
                         }
                         for (let e = 0; e < _.length; e++) {
                             let [t, n] = _[e], r = s[t], i = s[n], a = document.createElement("div");
                             W((() => {
-                                i || g('x-for ":key" is undefined or invalid', o), i.after(a), r.after(i), i._x_currentIfEl && i.after(i._x_currentIfEl), a.before(r), r._x_currentIfEl && r.after(r._x_currentIfEl), a.remove()
+                                i || g('x-for ":key" is undefined or invalid', o, n, s), i.after(a), r.after(i), i._x_currentIfEl && i.after(i._x_currentIfEl), a.before(r), r._x_currentIfEl && r.after(r._x_currentIfEl), a.remove()
                             })), i._x_refreshXForScope(c[u.indexOf(n)])
                         }
                         for (let e = 0; e < p.length; e++) {
                             let [t, n] = p[e], r = "template" === t ? o : s[t];
                             r._x_currentIfEl && (r = r._x_currentIfEl);
                             let a = c[n],
                                 l = u[n],
                                 f = document.importNode(o.content, !0).firstElementChild,
                                 d = i(a);
                             J(f, d, o), f._x_refreshXForScope = e => {
                                 Object.entries(e).forEach((([e, t]) => {
                                     d[e] = t
                                 }))
                             }, W((() => {
-                                r.after(f), T(f)
+                                r.after(f), Ze((() => T(f)))()
                             })), "object" == typeof l && g("x-for key cannot be an object, it must be a string or an integer", o), s[l] = f
                         }
-                        for (let e = 0; e < v.length; e++) s[v[e]]._x_refreshXForScope(c[u.indexOf(v[e])]);
+                        for (let e = 0; e < y.length; e++) s[y[e]]._x_refreshXForScope(c[u.indexOf(y[e])]);
                         o._x_prevKeys = u
                     }))
                 }(e, o, a, s))), r((() => {
                     Object.values(e._x_lookup).forEach((e => e.remove())), delete e._x_prevKeys, delete e._x_lookup
                 }))
-            })), Un.inline = (e, {
+            })), Kn.inline = (e, {
                 expression: t
             }, {
                 cleanup: n
             }) => {
                 let r = k(e);
                 r._x_refs || (r._x_refs = {}), r._x_refs[t] = e, n((() => delete r._x_refs[t]))
-            }, ge("ref", Un), ge("if", ((e, {
+            }, ge("ref", Kn), ge("if", ((e, {
                 expression: t
             }, {
                 effect: n,
                 cleanup: r
             }) => {
                 "template" !== e.tagName.toLowerCase() && g("x-if can only be used on a <template> tag", e);
                 let i = fe(e, t);
                 n((() => i((t => {
                     t ? (() => {
                         if (e._x_currentIfEl) return e._x_currentIfEl;
                         let t = e.content.cloneNode(!0).firstElementChild;
                         J(t, {}, e), W((() => {
-                            e.after(t), T(t)
+                            e.after(t), Ze((() => T(t)))()
                         })), e._x_currentIfEl = t, e._x_undoIf = () => {
                             m(t, (e => {
                                 e._x_effects && e._x_effects.forEach(d)
                             })), t.remove(), delete e._x_currentIfEl
                         }
                     })() : e._x_undoIf && (e._x_undoIf(), delete e._x_undoIf)
                 })))), r((() => e._x_undoIf && e._x_undoIf()))
@@ -2503,68 +2519,68 @@
                 evaluate: n
             }) => {
                 n(t).forEach((t => function(e, t) {
                     e._x_ids || (e._x_ids = {}), e._x_ids[t] || (e._x_ids[t] = Nn(t))
                 }(e, t)))
             })), Xe(((e, t) => {
                 e._x_ids && (t._x_ids = e._x_ids)
-            })), Ce(Oe("@", ye("on:"))), ge("on", Ze(((e, {
+            })), Ce(Oe("@", ve("on:"))), ge("on", Ze(((e, {
                 value: t,
                 modifiers: n,
                 expression: r
             }, {
                 cleanup: i
             }) => {
                 let o = r ? fe(e, r) : () => {};
                 "template" === e.tagName.toLowerCase() && (e._x_forwardEvents || (e._x_forwardEvents = []), e._x_forwardEvents.includes(t) || e._x_forwardEvents.push(t));
-                let a = zn(e, t, n, (e => {
+                let a = Dn(e, t, n, (e => {
                     o((() => {}), {
                         scope: {
                             $event: e
                         },
                         params: [e]
                     })
                 }));
                 i((() => a()))
-            }))), Kn("Collapse", "collapse", "collapse"), Kn("Intersect", "intersect", "intersect"), Kn("Focus", "trap", "focus"), Kn("Mask", "mask", "mask"), _t.setEvaluator(pe), _t.setReactivityEngine({
+            }))), Zn("Collapse", "collapse", "collapse"), Zn("Intersect", "intersect", "intersect"), Zn("Focus", "trap", "focus"), Zn("Mask", "mask", "mask"), _t.setEvaluator(pe), _t.setReactivityEngine({
                 reactive: jn,
-                effect: function(e, t = yt) {
+                effect: function(e, t = vt) {
                     (function(e) {
                         return e && !0 === e._isEffect
                     })(e) && (e = e.raw);
                     const n = function(e, t) {
                         const n = function() {
                             if (!n.active) return e();
                             if (!Nt.includes(n)) {
                                 It(n);
                                 try {
-                                    return Bt.push(zt), zt = !0, Nt.push(n), vt = n, e()
+                                    return zt.push(Dt), Dt = !0, Nt.push(n), yt = n, e()
                                 } finally {
-                                    Nt.pop(), Dt(), vt = Nt[Nt.length - 1]
+                                    Nt.pop(), Bt(), yt = Nt[Nt.length - 1]
                                 }
                             }
                         };
                         return n.id = qt++, n.allowRecurse = !!t.allowRecurse, n._isEffect = !0, n.active = !0, n.raw = e, n.deps = [], n.options = t, n
                     }(e, t);
                     return t.lazy || n(), n
                 },
                 release: function(e) {
                     e.active && (It(e), e.options.onStop && e.options.onStop(), e.active = !1)
                 },
                 raw: Ln
             });
-            var Zn = _t,
-                Jn = n(122),
-                Xn = n.n(Jn);
+            var Jn = _t,
+                Xn = n(122),
+                Yn = n.n(Xn);
 
-            function Yn(e, t) {
+            function Gn(e, t) {
                 e.classList.remove("scale-100"), t.classList.add("scale-100"), e.classList.add("scale-0"), t.classList.remove("scale-0")
             }
-            window.Alpine = Zn, Zn.plugin((function(t) {
-                t.directive("intersect", ((t, {
+            window.Alpine = Jn, Jn.plugin((function(t) {
+                t.directive("intersect", t.skipDuringClone(((t, {
                     value: n,
                     expression: i,
                     modifiers: o
                 }, {
                     evaluateLater: a,
                     cleanup: s
                 }) => {
@@ -2577,36 +2593,36 @@
                             e.forEach((e => {
                                 e.isIntersecting !== ("leave" === n) && (l(), o.includes("once") && u.disconnect())
                             }))
                         }), c);
                     u.observe(t), s((() => {
                         u.disconnect()
                     }))
-                }))
-            })), Zn.start(), window.addEventListener("DOMContentLoaded", (() => {
+                })))
+            })), Jn.start(), window.addEventListener("DOMContentLoaded", (() => {
                 ! function() {
                     const e = document.querySelectorAll(".highlight");
                     if (!e) return;
                     e.forEach((e => {
                         const t = e.querySelector("pre");
                         if (t) {
                             const e = '<button class="copy z-20 inline-flex h-6 w-6 items-center justify-center rounded-md border border-border bg-background opacity-0 focus:opacity-100 text-sm font-medium transition-all hover:bg-muted absolute right-4 top-4 tooltipped tooltipped-n" data-tooltip="Copy code" type="button"><span class="sr-only">Copy code</span><svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor" stroke="none" class="copy-icon h-[14px] w-[14px] transition-all transform scale-100 absolute"><path d="M200 976q-33 0-56.5-23.5T120 896V376q0-17 11.5-28.5T160 336q17 0 28.5 11.5T200 376v520h400q17 0 28.5 11.5T640 936q0 17-11.5 28.5T600 976H200Zm160-160q-33 0-56.5-23.5T280 736V256q0-33 23.5-56.5T360 176h360q33 0 56.5 23.5T800 256v480q0 33-23.5 56.5T720 816H360Zm0-80h360V256H360v480Zm0 0V256v480Z"/></svg><svg xmlns="http://www.w3.org/2000/svg" height="24" width="24" viewBox="0 96 960 960" fill="currentColor" stroke="none" class="copy-success-icon h-[14px] w-[14px] transition-all transform scale-0 absolute"><path d="M382 799q-8 0-15-2.5t-13-8.5L182 616q-11-11-10.5-28.5T183 559q11-11 28-11t28 11l143 143 339-339q11-11 28.5-11t28.5 11q11 11 11 28.5T778 420L410 788q-6 6-13 8.5t-15 2.5Z"/></svg></button>';
                             t.insertAdjacentHTML("beforeend", e)
                         }
                     }));
-                    const t = new(Xn())("button.copy", {
+                    const t = new(Yn())("button.copy", {
                         target: e => e.previousElementSibling
                     });
                     t.on("success", (({
                         trigger: e
                     }) => {
                         const t = e.getAttribute("data-tooltip"),
                             n = e.querySelector(".copy-icon"),
                             r = e.querySelector(".copy-success-icon");
-                        Yn(n, r), e.setAttribute("data-tooltip", "Copied!"), setTimeout((() => {
-                            Yn(r, n), e.setAttribute("data-tooltip", t)
+                        Gn(n, r), e.setAttribute("data-tooltip", "Copied!"), setTimeout((() => {
+                            Gn(r, n), e.setAttribute("data-tooltip", t)
                         }), 2e3)
                     }))
                 }()
             }))
         }()
 }();
```

### Comparing `sphinxawesome_theme-5.1.1/src/sphinxawesome_theme/toc.py` & `sphinxawesome_theme-5.1.2/src/sphinxawesome_theme/toc.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-5.1.1/PKG-INFO` & `sphinxawesome_theme-5.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 5.1.1
+Version: 5.1.2
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -82,10 +82,10 @@
 
 ### Better headerlinks
 
 Clicking the link icon after headers or captions automatically copies the URL to the clipboard.
 
 ### DocSearch
 
-This theme supports the [`sphinx-docsearch`](https://sphinx-docsearch.readthedocs.io/en/latest/)
+This theme supports the [`sphinx-docsearch`](https://sphinx-docsearch.readthedocs.io/en/latest/) extension
 to replace the built-in search with Algolia DocSearch.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.1 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.1.2 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
@@ -32,8 +32,8 @@
 If you load the bundled `sphinxawesome_theme.highlighting`, you can use these
 additional options in your `code-block` directives: - `emphasize-added`.
 Highlight lines that should be added - `emphasize-removed`. Highlight lines
 that should be removed - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code
 block ### Better headerlinks Clicking the link icon after headers or captions
 automatically copies the URL to the clipboard. ### DocSearch This theme
 supports the [`sphinx-docsearch`](https://sphinx-docsearch.readthedocs.io/en/
-latest/) to replace the built-in search with Algolia DocSearch.
+latest/) extension to replace the built-in search with Algolia DocSearch.
```

