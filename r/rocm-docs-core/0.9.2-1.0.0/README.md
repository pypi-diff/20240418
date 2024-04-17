# Comparing `tmp/rocm-docs-core-0.9.2.tar.gz` & `tmp/rocm_docs_core-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocm-docs-core-0.9.2.tar", last modified: Fri May  5 19:34:34 2023, max compression
+gzip compressed data, was "rocm_docs_core-1.0.0.tar", last modified: Wed Apr 17 23:05:33 2024, max compression
```

## Comparing `rocm-docs-core-0.9.2.tar` & `rocm_docs_core-1.0.0.tar`

### file list

```diff
@@ -1,102 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.284805 rocm-docs-core-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    17097 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 19:34:34.284805 rocm-docs-core-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:34:34.284805 rocm-docs-core-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.256803 rocm-docs-core-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.260804 rocm-docs-core-0.9.2/src/rocm_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12249 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.252803 rocm-docs-core-0.9.2/src/rocm_docs/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.260804 rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/
--rw-r--r--   0 runner    (1001) docker     (123)    72387 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/extra_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/header.html
--rw-r--r--   0 runner    (1001) docker     (123)    37264 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/doxygen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.260804 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.264804 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/components/article-info.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/components/social-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.264804 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/sections/header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.268804 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.256803 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.280805 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20756 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16748 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21924 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17872 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20780 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16808 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21876 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17876 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20672 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16756 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21820 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17780 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20172 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16372 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21248 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17384 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20664 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16696 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21520 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17544 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27552 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22132 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29388 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23712 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27592 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22184 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29392 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23824 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27456 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22212 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29224 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23676 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    26652 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    21516 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    28292 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22904 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27376 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22040 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23168 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    29304 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    23704 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    27520 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    22084 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    21856 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    17820 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    20712 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    16740 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts.css
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.284805 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)      924 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    10074 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-05 19:34:19.000000 rocm-docs-core-0.9.2/src/rocm_docs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:34:34.284805 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 19:34:34.000000 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-05 19:34:34.000000 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:34:34.000000 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 19:34:34.000000 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-05 19:34:34.000000 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 19:34:34.000000 rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.837326 rocm_docs_core-1.0.0/
+-rwxrwxrwx   0 root         (0) root         (0)    17095 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3966 2024-04-17 23:05:33.829329 rocm_docs_core-1.0.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2347 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/README.md
+-rwxrwxrwx   0 root         (0) root         (0)     3592 2024-04-17 23:04:15.000000 rocm_docs_core-1.0.0/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-17 23:05:33.838539 rocm_docs_core-1.0.0/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.056692 rocm_docs_core-1.0.0/src/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.245573 rocm_docs_core-1.0.0/src/rocm_docs/
+-rwxrwxrwx   0 root         (0) root         (0)     2663 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    11121 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.291377 rocm_docs_core-1.0.0/src/rocm_docs/data/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.401984 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/
+-rwxrwxrwx   0 root         (0) root         (0)    72476 2024-04-17 22:44:44.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css
+-rwxrwxrwx   0 root         (0) root         (0)      112 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/footer.html
+-rwxrwxrwx   0 root         (0) root         (0)     1428 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/header.html
+-rwxrwxrwx   0 root         (0) root         (0)    37255 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/stylesheet.css
+-rwxrwxrwx   0 root         (0) root         (0)     2940 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/projects.schema.json
+-rwxrwxrwx   0 root         (0) root         (0)     4222 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/data/projects.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     8600 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/doxygen.py
+-rwxrwxrwx   0 root         (0) root         (0)     4663 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/formatting.py
+-rwxrwxrwx   0 root         (0) root         (0)    17085 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/projects.py
+-rwxrwxrwx   0 root         (0) root         (0)       59 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.472070 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/
+-rwxrwxrwx   0 root         (0) root         (0)      185 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/404.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.562229 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/
+-rwxrwxrwx   0 root         (0) root         (0)     1931 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/article-info.html
+-rwxrwxrwx   0 root         (0) root         (0)      215 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
+-rwxrwxrwx   0 root         (0) root         (0)      217 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.017452 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.666545 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/
+-rwxrwxrwx   0 root         (0) root         (0)      149 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
+-rwxrwxrwx   0 root         (0) root         (0)     1424 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
+-rwxrwxrwx   0 root         (0) root         (0)       67 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.767980 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/
+-rwxrwxrwx   0 root         (0) root         (0)       45 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
+-rwxrwxrwx   0 root         (0) root         (0)      703 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
+-rwxrwxrwx   0 root         (0) root         (0)       75 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.899227 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/
+-rwxrwxrwx   0 root         (0) root         (0)      149 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
+-rwxrwxrwx   0 root         (0) root         (0)     1424 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
+-rwxrwxrwx   0 root         (0) root         (0)       70 2024-03-13 19:55:26.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
+-rwxrwxrwx   0 root         (0) root         (0)      344 2024-04-17 22:44:51.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/layout.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:31.005508 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/
+-rwxrwxrwx   0 root         (0) root         (0)      318 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/footer-content.html
+-rwxrwxrwx   0 root         (0) root         (0)     2137 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/footer.html
+-rwxrwxrwx   0 root         (0) root         (0)     2267 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/header.html
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:31.358365 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/
+-rwxrwxrwx   0 root         (0) root         (0)      831 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
+-rwxrwxrwx   0 root         (0) root         (0)     3984 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/custom.css
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:30.045367 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.425927 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/
+-rwxrwxrwx   0 root         (0) root         (0)    20756 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
+-rwxrwxrwx   0 root         (0) root         (0)    16748 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    21924 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    17872 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    20780 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
+-rwxrwxrwx   0 root         (0) root         (0)    16808 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    21876 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    17876 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    20672 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff
+-rwxrwxrwx   0 root         (0) root         (0)    16756 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    21820 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    17780 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    20172 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff
+-rwxrwxrwx   0 root         (0) root         (0)    16372 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    21248 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    17384 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    20664 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff
+-rwxrwxrwx   0 root         (0) root         (0)    16696 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    21520 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    17544 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    27552 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff
+-rwxrwxrwx   0 root         (0) root         (0)    22132 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    29388 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    23712 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    27592 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff
+-rwxrwxrwx   0 root         (0) root         (0)    22184 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    29392 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    23824 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    27456 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff
+-rwxrwxrwx   0 root         (0) root         (0)    22212 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    29224 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    23676 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    26652 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff
+-rwxrwxrwx   0 root         (0) root         (0)    21516 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    28292 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    22904 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    27376 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff
+-rwxrwxrwx   0 root         (0) root         (0)    22040 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    28704 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    23168 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    29304 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    23704 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    27520 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff
+-rwxrwxrwx   0 root         (0) root         (0)    22084 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    21856 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff
+-rwxrwxrwx   0 root         (0) root         (0)    17820 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2
+-rwxrwxrwx   0 root         (0) root         (0)    20712 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff
+-rwxrwxrwx   0 root         (0) root         (0)    16740 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2
+-rwxrwxrwx   0 root         (0) root         (0)     9931 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css
+-rwxrwxrwx   0 root         (0) root         (0)     3502 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map
+-rwxrwxrwx   0 root         (0) root         (0)     1503 2024-01-12 23:06:42.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.573687 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/
+-rwxrwxrwx   0 root         (0) root         (0)     1611 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg
+-rwxrwxrwx   0 root         (0) root         (0)      925 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg
+-rwxrwxrwx   0 root         (0) root         (0)     1760 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
+-rwxrwxrwx   0 root         (0) root         (0)    10074 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
+-rwxrwxrwx   0 root         (0) root         (0)     3426 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
+-rwxrwxrwx   0 root         (0) root         (0)      780 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
+-rwxrwxrwx   0 root         (0) root         (0)     1260 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
+-rwxrwxrwx   0 root         (0) root         (0)    19276 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+-rwxrwxrwx   0 root         (0) root         (0)      596 2024-01-12 23:06:43.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
+-rwxrwxrwx   0 root         (0) root         (0)      243 2024-04-17 22:44:44.000000 rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/theme.conf
+-rwxrwxrwx   0 root         (0) root         (0)     5279 2024-04-17 22:59:16.000000 rocm_docs_core-1.0.0/src/rocm_docs/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     5975 2024-04-17 22:59:13.000000 rocm_docs_core-1.0.0/src/rocm_docs/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.814071 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3966 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     6839 2024-04-17 23:05:29.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       55 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)      485 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-17 23:05:28.000000 rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-17 23:05:33.784843 rocm_docs_core-1.0.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     2637 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/tests/test_doxygen.py
+-rwxrwxrwx   0 root         (0) root         (0)     1272 2024-02-21 19:55:38.000000 rocm_docs_core-1.0.0/tests/test_meta.py
+-rwxrwxrwx   0 root         (0) root         (0)     5682 2024-04-17 22:59:17.000000 rocm_docs_core-1.0.0/tests/test_projects.py
+-rwxrwxrwx   0 root         (0) root         (0)     1854 2024-04-17 22:59:17.000000 rocm_docs_core-1.0.0/tests/test_sites.py
```

### Comparing `rocm-docs-core-0.9.2/LICENSE.txt` & `rocm_docs_core-1.0.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Copyright (c) 2023 Advanced Micro Devices, Inc.
 
 ===========================================================================
 
-All files exclusive of files in src/rocm_docs/data/_images are governed by 
+All files exclusive of files in src/rocm_docs/data/_images are governed by
 the following terms:
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
@@ -21,15 +21,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 
 ===========================================================================
 
-Files in src/rocm_docs/data/_images and its subdirectories are governed by 
+Files in src/rocm_docs/data/_images and its subdirectories are governed by
 the following terms:
 
 Creative Commons Attribution 4.0 International Public License
 
 By exercising the Licensed Rights (defined below), You accept and agree
 to be bound by the terms and conditions of this Creative Commons
 Attribution 4.0 International Public License ("Public License"). To the
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/__init__.py` & `rocm_docs_core-1.0.0/src/rocm_docs/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-"""Set up variables for documentation of ROCm projects using RTD."""
+"""Defines the ROCmDocs package.
+
+Set up variables for documentation of ROCm projects
+that are using Read the Docs.
+"""
+
+from __future__ import annotations
+
+from typing import ClassVar, TypeAlias
 
 import os
-import subprocess
-from typing import Dict, List, Optional, Union
 
 from rocm_docs.core import setup
 
-MaybePath = Union[str, os.PathLike, None]
+MaybePath: TypeAlias = str | os.PathLike[str] | None
 
 
 # Intentionally disabling the too-many-instance-attributes check in pylint
 # as this class is intended to contain all necessary Sphinx config variables
 # pylint: disable=too-many-instance-attributes
 class ROCmDocs:
-    """A class to contain all of the Sphinx variables"""
+    """A class to contain all of the Sphinx variables."""
 
-    SPHINX_VARS = [
+    SPHINX_VARS: ClassVar = [
         "extensions",
         "html_title",
         "html_theme",
         "html_theme_options",
         "doxygen_root",
         "doxygen_project",
         "doxyfile",
         "doxysphinx_enabled",
     ]
 
     def __init__(
         self,
         project_name: str,
-        version_string : str = None,
-        _: MaybePath = None,
+        _: str | None = None,
+        __: MaybePath = None,
     ) -> None:
+        """Intialize ROCmDocs."""
         self._project_name: str = project_name
-        self._version_string: str = version_string
-        self.extensions: List[str] = []
+        self.extensions: list[str] = []
         self.html_title: str
         self.html_theme: str
-        self.html_theme_options: Dict[str, Union[str, bool, List[str]]] = {}
+        self.html_theme_options: dict[str, str | (bool | list[str])] = {}
         self.doxygen_root: MaybePath = None
-        self.doxygen_project: Dict[str, Union[Optional[str], MaybePath]] = {
+        self.doxygen_project: dict[str, str | None | MaybePath] = {
             "name": None,
             "path": None,
         }
         self.doxyfile: MaybePath = None
         self.doxysphinx_enabled: bool = False
 
     @property
@@ -51,16 +57,17 @@
         """Sphinx project variable."""
         return self._project_name
 
     def run_doxygen(
         self,
         doxygen_root: MaybePath = None,
         doxygen_path: MaybePath = None,
-        doxygen_file: Optional[str] = None,
+        doxygen_file: str | None = None,
     ) -> None:
+        """Run doxygen as part of Sphinx by adding rocm_docs.doxygen."""
         if "rocm_docs.doxygen" not in self.extensions:
             self.extensions.append("rocm_docs.doxygen")
 
         self.doxygen_root = doxygen_root
         self.doxygen_project = {
             "name": self._project_name,
             "path": doxygen_path,
@@ -71,23 +78,15 @@
         """Enable embedding the doxygen generated api."""
         if "rocm_docs.doxygen" not in self.extensions:
             self.extensions.append("rocm_docs.doxygen")
 
         self.doxysphinx_enabled = True
 
     def setup(self) -> None:
-        """Sets up default RTD variables."""
+        """Set up default RTD variables."""
         self.extensions.append("rocm_docs")
         full_project_name = self._project_name
-        if self._version_string is None and os.path.exists("../CMakeLists.txt"):
-            getVersionString = r'sed -n -e "s/^.*VERSION_STRING.* \"\([0-9\.]\{1,\}\).*/\1/p" ../CMakeLists.txt'
-            self._version_string = subprocess.getoutput(getVersionString)
-        if self._version_string is not None and len(self._version_string) > 0:
-            full_project_name += f" {self._version_string}"
         self.html_title = full_project_name
         self.html_theme = "rocm_docs_theme"
 
-    def disable_main_doc_link(self) -> None:
-        self.html_theme_options["link_main_doc"] = False
-
 
 __all__ = ["setup", "ROCmDocs"]
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/core.py` & `rocm_docs_core-1.0.0/src/rocm_docs/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,353 +1,342 @@
-"""Core rocm_docs extension that enables a core set of sphinx extensions and
-provides good defaults for settings. Provides a consistent common
-base environment for the rocm documentation projects."""
+"""Core rocm_docs extension.
 
+It enables a core set of sphinx extensions and provides good defaults for
+settings. The environment provided is meant as consistent common base for
+ROCm documentation projects.
+"""
+
+from __future__ import annotations
+
+from typing import Any, Generic, TypeVar, cast
+
+import importlib.resources
 import inspect
 import os
-import re
-import subprocess
-import sys
-import types
+import urllib.parse
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import Any, Callable, Dict, Generic, List, Set, Type, TypeVar
 
 import bs4
-from pydata_sphinx_theme.utils import config_provided_by_user
+import git.repo
+from pydata_sphinx_theme.utils import (  # type: ignore[import-untyped]
+    config_provided_by_user,
+)
 from sphinx.application import Sphinx
 from sphinx.config import Config
 
-import rocm_docs.util as util
-
-# based on doxygen.py
-if sys.version_info < (3, 9):
-    import importlib_resources
-else:
-    import importlib.resources as importlib_resources
-
-
 T = TypeVar("T")
 
 
 class _ConfigUpdater(Generic[T], ABC):
     def __init__(self, default: T) -> None:
         super().__init__()
         self.default = default
 
     @abstractmethod
     def __call__(self, key: str, app: Sphinx) -> None:
         pass
 
 
-def _config_updater(
-    f: Callable[[str, Sphinx, T], None]
-) -> Type[_ConfigUpdater]:
-    def __call__(self: _ConfigUpdater[T], key: str, app: Sphinx) -> None:
-        f(key, app, self.default)
-
-    def update_body(body: Dict[str, Any]) -> None:
-        body["__call__"] = __call__
-
-    return types.new_class(
-        f.__name__, bases=[_ConfigUpdater[T]], exec_body=update_body
-    )
-
-
-@_config_updater
-def _ConfigExtend(key: str, app: Sphinx, default: T) -> None:
-    getattr(app.config, key).extend(default)
-
-
-@_config_updater
-def _ConfigUnion(key: str, app: Sphinx, default: Set[T]) -> None:
-    getattr(app.config, key).update(default)
+class _ConfigExtend(_ConfigUpdater[list[T]]):
+    def __call__(self, key: str, app: Sphinx) -> None:
+        getattr(app.config, key).extend(self.default)
 
 
-@_config_updater
-def _ConfigDefault(key: str, app: Sphinx, default: T) -> None:
-    if not config_provided_by_user(app, key):
-        setattr(app.config, key, default)
+class _ConfigDefault(_ConfigUpdater[T]):
+    def __call__(self, key: str, app: Sphinx) -> None:
+        if not config_provided_by_user(app, key):
+            setattr(app.config, key, self.default)
 
 
-@_config_updater
-def _ConfigOverride(key: str, app: Sphinx, value: T) -> None:
-    setattr(app.config, key, value)
+class _ConfigUnion(_ConfigUpdater[set[T]]):
+    def __call__(self, key: str, app: Sphinx) -> None:
+        getattr(app.config, key).update(self.default)
 
 
-@_config_updater
-def _ConfigMerge(key: str, app: Sphinx, default: Dict[str, Any]) -> None:
-    setting: Dict[str, Any] = getattr(app.config, key)
-    for key, value in default.items():
-        setting.setdefault(key, value)
+class _ConfigMerge(_ConfigUpdater[dict[str, Any]]):
+    def __call__(self, key: str, app: Sphinx) -> None:
+        current_setting: dict[str, Any] = getattr(app.config, key)
+        for item in self.default.items():
+            current_setting.setdefault(item[0], item[1])
 
 
 class _DefaultSettings:
     author = _ConfigDefault(
         'Advanced Micro Devices <a href="https://">Disclaimer and'
         " Licensing Info</a>"
     )
     # pylint: disable=redefined-builtin
     copyright = _ConfigDefault("2022-2023, Advanced Micro Devices Ltd")
     # pylint: enable=redefined-builtin
     myst_enable_extensions = _ConfigUnion(
-        {"colon_fence", "fieldlist", "linkify", "replacements", "substitution"}
-    )
-    myst_heading_anchors = _ConfigDefault(3)
-    external_toc_path = _ConfigOverride("./.sphinx/_toc.yml")
-    external_toc_exclude_missing = _ConfigDefault(False)
-    intersphinx_mapping = _ConfigMerge(
         {
-            "rtd": ("https://docs.readthedocs.io/en/stable/", None),
-            "python": ("https://docs.python.org/3/", None),
-            "sphinx": ("https://www.sphinx-doc.org/en/master/", None),
+            "colon_fence",
+            "dollarmath",
+            "fieldlist",
+            "html_image",
+            "replacements",
+            "substitution",
         }
     )
-    intersphinx_disabled_domains = _ConfigDefault(["std"])
+    myst_heading_anchors = _ConfigDefault(3)
+    external_toc_exclude_missing = _ConfigDefault(False)
     epub_show_urls = _ConfigDefault("footnote")
     exclude_patterns = _ConfigExtend(["_build", "Thumbs.db", ".DS_Store"])
     numfig = _ConfigDefault(True)
     linkcheck_timeout = _ConfigDefault(10)
     linkcheck_request_headers = _ConfigMerge(
         {
-            r'https://docs.github.com/': {'User-Agent': 'Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:112.0) \
-                Gecko/20100101 Firefox/112.0'}
+            r"https://docs.github.com/": {
+                "User-Agent": (
+                    "Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:112.0)          "
+                    "       Gecko/20100101 Firefox/112.0"
+                )
+            }
         }
     )
 
     @classmethod
     def update_config(cls, app: Sphinx, _: Config) -> None:
+        """Update the Sphinx configuration from the default settings."""
         for name, attr in inspect.getmembers(cls):
             if isinstance(attr, _ConfigUpdater):
                 attr(name, app)
 
 
-def _format_toc_file(app: Sphinx, config: Config) -> None:
-    toc_in_path = Path(app.srcdir) / "./.sphinx/_toc.yml.in"
-    if not (toc_in_path.exists() and toc_in_path.is_file()):
-        raise FileNotFoundError(
-            f"Expected input toc file {toc_in_path} to exist and be"
-            " readable."
-        )
-    util.format_toc(
-        toc_path=app.srcdir,
-        repo_path=app.srcdir,
-        input_name="./.sphinx/_toc.yml.in",
-        output_name=config.external_toc_path,
-    )
-
-
 def _force_notfound_prefix(app: Sphinx, _: Config) -> None:
-    if not "READTHEDOCS" in os.environ:
+    if "READTHEDOCS" not in os.environ:
         return
 
-    if not config_provided_by_user(app, "notfound_urls_prefix"):
+    if config_provided_by_user(app, "notfound_urls_prefix"):
         return
 
-    current_version = app.config["html_context"].get("current_version", "")
-    if current_version != "":
-        current_version += "/"
-    abs_path = re.sub(
-        r"^(?:.*://)?[^/]*/(.*)/[^/]*/$",
-        r"/\1/" + current_version,
-        app.config.html_baseurl,
-    )
-    app.config.notfound_urls_prefix = abs_path
+    components = urllib.parse.urlparse(os.environ["READTHEDOCS_CANONICAL_URL"])
+    app.config.notfound_urls_prefix = components.path  # type: ignore[attr-defined]
+
 
 def _set_article_info(app: Sphinx, _: Config) -> None:
-    """Add article info headers to HTML pages"""
-    if app.config.setting_all_article_info is False and len(app.config.article_pages) == 0:
+    """Add article info headers to HTML pages."""
+    if (
+        app.config.setting_all_article_info is False
+        and len(app.config.article_pages) == 0
+    ):
         return
 
-    rocm_docs_package = importlib_resources.files("rocm_docs")
-    article_info_path = os.path.join(rocm_docs_package, "rocm_docs_theme/components/article-info.html")
-    with open(article_info_path, "r") as file:
-        article_info = file.read()
+    article_info = (
+        importlib.resources.files("rocm_docs")
+        .joinpath("rocm_docs_theme/components/article-info.html")
+        .read_text(encoding="utf-8")
+    )
 
-    specific_pages = []
+    specific_pages: list[str] = []
 
     _set_page_article_info(app, article_info, specific_pages)
 
     if app.config.setting_all_article_info is True:
         _set_all_article_info(app, article_info, specific_pages)
 
 
 def _set_page_article_info(
-    app: Sphinx, 
-    article_info: str, 
-    specific_pages: List[str]
+    app: Sphinx, article_info: str, specific_pages: list[str]
 ) -> None:
+    """Add article info headers to the configured HTML pages.
+
+    The pages can be set in "article_pages" of the Sphinx configuration.
     """
-    Add article info headers to specific HTML pages
-    mentioned in app.config.article_pages
-    """
+    repo = git.repo.Repo(app.srcdir, search_parent_directories=True)
     for page in app.config.article_pages:
-        path_html = os.path.join(app.config.html_output_directory, page["file"]) + ".html"
-        path_source = page["file"] + ".rst"
-        if os.path.isfile(path_source) is False:
-            path_source = page["file"] + ".md"
+        path_rel = app.project.doc2path(page["file"], basedir=False)
+        path_html = Path(app.outdir, path_rel).with_suffix(".html")
+        path_source = Path(app.srcdir, path_rel)
+
+        # FIXME: This will silently skip all files when not building the default
+        # `html` format (e.g `htmlzip`, `epub` or `pdf`)
+        if not path_html.is_file():
+            continue
 
-        font_awesome_os = ""
-        if "os" not in page.keys():
+        article_os_info = ""
+        if "os" not in page:
             page["os"] = app.config.all_article_info_os
         if "linux" in page["os"]:
-            font_awesome_os += '<i class="fa-brands fa-linux fa-2xl fa-fw"></i>'
+            article_os_info += "Linux"
         if "windows" in page["os"]:
-            font_awesome_os += '<i class="fa-brands fa-windows fa-2xl fa-fw"></i>'
-        modified_info = article_info.replace("<!--osicons-->", font_awesome_os)
+            if len(article_os_info) > 0:
+                article_os_info += " and "
+            article_os_info += "Windows"
+        modified_info = article_info.replace("<!--os-info-->", article_os_info)
 
         author = app.config.all_article_info_author
-        if "author" in page.keys():
+        if "author" in page:
             author = page["author"]
         modified_info = modified_info.replace("AMD", author)
 
-        date_info = _get_time_last_modified(path_source)
-        if "date" in page.keys():
+        date_info: str | None = None
+        if "date" in page:
             date_info = page["date"]
+        else:
+            date_info = _get_time_last_modified(repo, path_source)
+
+        if not date_info:
+            date_info = cast(str, app.config.all_article_info_date)
+
         modified_info = modified_info.replace("2023", date_info)
 
-        if "read-time" in page.keys():
+        if "read-time" in page:
             read_time = page["read-time"]
         else:
             read_time = _estimate_read_time(path_html)
         modified_info = modified_info.replace("5 min read", read_time)
 
-        specific_pages.append(path_html)
+        specific_pages.append(page["file"])
         _write_article_info(path_html, modified_info)
 
 
 def _set_all_article_info(
-    app: Sphinx, 
-    article_info: str, 
-    specific_pages: List[str]
+    app: Sphinx, article_info: str, specific_pages: list[str]
 ) -> None:
-    """
-    Add article info headers with general settings to all HTML pages
-    except those in app.config.article_pages
-    """
-    (html_pages, source_map) = _get_all_pages(app.config.html_output_directory)
+    """Add article info headers with general settings to all HTML pages.
 
-    for page in html_pages:
+    Pages that have specific settings (configured by "article_pages") are
+    skipped.
+    """
+    repo = git.repo.Repo(app.srcdir, search_parent_directories=True)
+    for docname in app.project.docnames:
         # skip pages with specific settings
-        if page in specific_pages:
+        if docname in specific_pages:
             continue
 
-        font_awesome_os = ""
-        if "linux" in app.config.all_article_info_os:
-            font_awesome_os += '<i class="fa-brands fa-linux fa-2xl fa-fw"></i>'
-        if "windows" in app.config.all_article_info_os:
-            font_awesome_os += '<i class="fa-brands fa-windows fa-2xl fa-fw"></i>'
+        page_rel = app.project.doc2path(docname, basedir=False)
+        page = Path(app.outdir, page_rel).with_suffix(".html")
 
-        page_key = Path(page).stem
-        if page_key in source_map.keys():
-            modified_path = source_map[page_key]
-        else:
-            modified_path = page
-        date_info = _get_time_last_modified(modified_path)
-        if len(date_info) == 0:
-            date_info = app.config.all_article_info_date
+        # FIXME: This will silently skip all files when not building the default
+        # `html` format (e.g `htmlzip`, `epub` or `pdf`)
+        if not page.is_file():
+            continue
 
-        modified_info = article_info.replace("<!--osicons-->", font_awesome_os)
-        modified_info = modified_info.replace("AMD", app.config.all_article_info_author)
+        article_os_info = ""
+        if "linux" in app.config.all_article_info_os:
+            article_os_info += "Linux"
+        if "windows" in app.config.all_article_info_os:
+            if len(article_os_info) > 0:
+                article_os_info += " and "
+            article_os_info += "Windows"
+
+        date_info = _get_time_last_modified(repo, Path(app.srcdir, page_rel))
+        if not date_info:
+            date_info = cast(str, app.config.all_article_info_date)
+
+        modified_info = article_info.replace("<!--os-info-->", article_os_info)
+        modified_info = modified_info.replace(
+            "AMD", app.config.all_article_info_author
+        )
         modified_info = modified_info.replace("2023", date_info)
-        modified_info = modified_info.replace("5 min read", _estimate_read_time(page))
-        
-        _write_article_info(page, modified_info)
-
-
-def _get_all_pages(output_directory: str):
-    html_pages = list()
-    source_map = dict()
-
-    for root, _, files in os.walk(output_directory):
-        for file in files:
-            if file.endswith(".html"):
-                html_pages.append(os.path.join(root, file))
+        modified_info = modified_info.replace(
+            "5 min read", _estimate_read_time(page)
+        )
 
-    for root, _, files in os.walk("."):
-        for file in files:
-            if file.endswith(".rst") or file.endswith(".md"):
-                file_key = Path(file).stem
-                source_map[file_key] = os.path.join(root, file)
-    
-    return (html_pages, source_map)
+        _write_article_info(page, modified_info)
 
 
-def _get_time_last_modified(path: str) -> str:
-    return subprocess.getoutput(f"git log -1 --pretty=format:%cd --date=short {path}")
+def _get_time_last_modified(repo: git.repo.Repo, path: Path) -> str | None:
+    try:
+        time = next(
+            repo.iter_commits(paths=path, max_count=1)
+        ).committed_datetime
+        return time.strftime("%Y-%m-%d")
+    except StopIteration:
+        return None
 
 
-def _estimate_read_time(file_name: str) -> str:
+def _estimate_read_time(file_name: Path) -> str:
     def is_visible(element):
-        if element.parent.name in ['style', 'script', '[document]', 'head', 'title']:
+        if element.parent.name in [
+            "style",
+            "script",
+            "[document]",
+            "head",
+            "title",
+        ]:
             return False
-        elif isinstance(element, bs4.element.Comment):
+        if isinstance(element, bs4.element.Comment):
             return False
-        elif element.string == "\n":
+        if element.string == "\n":
             return False
         return True
-    
-    def count_words(text, avg_word_len):
-        words = 0
-        for line in text:
-            words += len(line)/avg_word_len
-        return words
-
-    WORDS_PER_MIN = 200
-    AVG_WORD_LEN = 5
-
-    file = open(file_name, "r")
-    html = file.read()
-    soup = bs4.BeautifulSoup(html, 'html.parser')
+
+    words_per_minute = 200
+    average_word_length = 5
+
+    with open(file_name, encoding="utf-8") as file:
+        html = file.read()
+    soup = bs4.BeautifulSoup(html, "html.parser")
     page_text = soup.findAll(text=True)
     visible_page_text = filter(is_visible, page_text)
-    average_word_count = count_words(visible_page_text, AVG_WORD_LEN)
-    time_minutes = max(1, int(average_word_count // WORDS_PER_MIN))
+    average_word_count = (
+        sum(len(line) for line in visible_page_text) / average_word_length
+    )
+    time_minutes = int(max(1, round(average_word_count / words_per_minute)))
     return f"{time_minutes} min read time"
 
 
-def _write_article_info(path: str, article_info: str) -> None:
-    with open(path, "r+") as file:
+def _write_article_info(path: os.PathLike[Any], article_info: str) -> None:
+    with open(path, "r+", encoding="utf8") as file:
         page_html = file.read()
-        soup = bs4.BeautifulSoup(page_html, 'html.parser')
+        soup = bs4.BeautifulSoup(page_html, "html.parser")
 
         has_article_info = soup.find("div", id="rocm-docs-core-article-info")
-        if has_article_info is not None or soup.article is None or soup.article.h1 is None:
+        if (
+            has_article_info is not None
+            or soup.article is None
+            or soup.article.h1 is None
+        ):
             return
-            
-        soup.article.h1.insert_after(bs4.BeautifulSoup(article_info, 'html.parser'))
+
+        soup.article.h1.insert_after(
+            bs4.BeautifulSoup(article_info, "html.parser")
+        )
         file.seek(0)
         file.truncate(0)
         file.write(str(soup))
-        
 
-def setup(app: Sphinx) -> Dict[str, Any]:
+
+def setup(app: Sphinx) -> dict[str, Any]:
+    """Set up rocm_docs.core as a Sphinx extension."""
     required_extensions = [
         "myst_parser",
         "notfound.extension",
+        "rocm_docs.projects",
         "sphinx_copybutton",
         "sphinx_design",
-        "sphinx_external_toc",
         "sphinx.ext.autodoc",
         "sphinx.ext.autosummary",
         "sphinx.ext.doctest",
         "sphinx.ext.duration",
-        "sphinx.ext.intersphinx",
     ]
     for ext in required_extensions:
         app.setup_extension(ext)
 
-    app.add_config_value("html_output_directory", default="_build/html/", rebuild="html", types=str)
-    app.add_config_value("setting_all_article_info", default=False, rebuild="html", types=Any)
-    app.add_config_value("all_article_info_os", default=["linux", "windows"], rebuild="html", types=Any)
-    app.add_config_value("all_article_info_author", default="", rebuild="html", types=Any)
-    app.add_config_value("all_article_info_date", default="2023", rebuild="html", types=Any)
-    app.add_config_value("all_article_info_read_time", default="", rebuild="html", types=Any)
+    app.add_config_value(
+        "setting_all_article_info", default=False, rebuild="html", types=str
+    )
+    app.add_config_value(
+        "all_article_info_os",
+        default=["linux", "windows"],
+        rebuild="html",
+        types=str,
+    )
+    app.add_config_value(
+        "all_article_info_author", default="", rebuild="html", types=str
+    )
+    app.add_config_value(
+        "all_article_info_date", default="2023", rebuild="html", types=str
+    )
+    app.add_config_value(
+        "all_article_info_read_time", default="", rebuild="html", types=str
+    )
     app.add_config_value("article_pages", default=[], rebuild="html", types=Any)
 
     # Run before notfound.extension sees the config (default priority(=500))
     app.connect("config-inited", _force_notfound_prefix, priority=400)
     app.connect("config-inited", _DefaultSettings.update_config)
-    # This needs to happen before external-tocs's config-inited (priority=900)
-    app.connect("config-inited", _format_toc_file)
     app.connect("build-finished", _set_article_info, priority=1000)
     return {"parallel_read_safe": True, "parallel_write_safe": True}
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/extra_stylesheet.css` & `rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/extra_stylesheet.css`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         --page-secondary-foreground-color: #859399;
         --separator-color: #38393b;
         --side-nav-background: #252628;
 
         --code-background: #2a2c2f;
 
         --tablehead-background: #2a2c2f;
-    
+
         --blockquote-background: #222325;
         --blockquote-foreground: #7e8c92;
 
         --warning-color: #2e1917;
         --warning-color-dark: #ad2617;
         --warning-color-darker: #f5b1aa;
         --note-color: #3b2e04;
@@ -884,15 +884,15 @@
     .doxygen-content #doc-content > div > div.contents,
     .doxygen-content .PageDoc > div.contents {
         display: flex;
         flex-direction: row-reverse;
         flex-wrap: nowrap;
         align-items: flex-start;
     }
-    
+
     .doxygen-content div.contents .textblock {
         min-width: 200px;
         flex-grow: 1;
     }
 }
 
 .doxygen-content div.contents, .doxygen-content div.header .title, .doxygen-content div.header .summary {
@@ -1141,16 +1141,16 @@
         margin: 0;
         padding: var(--spacing-large) 0;
         display: block;
     }
 
     .doxygen-content div.contents .toc.interactive > h3::before {
         content: "";
-        width: 0; 
-        height: 0; 
+        width: 0;
+        height: 0;
         border-left: 4px solid transparent;
         border-right: 4px solid transparent;
         border-top: 5px solid var(--primary-color);
         display: inline-block;
         margin-right: var(--spacing-small);
         margin-bottom: calc(var(--navigation-font-size) / 4);
         transform: rotate(-90deg);
@@ -1833,16 +1833,16 @@
     color: var(--page-secondary-foreground-color);
 }
 
 .doxygen-content table.memberdecls img[src="closed.png"],
 .doxygen-content table.memberdecls img[src="open.png"],
 .doxygen-content div.dynheader img[src="open.png"],
 .doxygen-content div.dynheader img[src="closed.png"] {
-    width: 0; 
-    height: 0; 
+    width: 0;
+    height: 0;
     border-left: 4px solid transparent;
     border-right: 4px solid transparent;
     border-top: 5px solid var(--primary-color);
     margin-top: 8px;
     display: block;
     float: left;
     margin-left: -10px;
@@ -1852,15 +1852,15 @@
 .doxygen-content table.memberdecls img {
     margin-right: 10px;
 }
 
 .doxygen-content table.memberdecls img[src="closed.png"],
 .doxygen-content div.dynheader img[src="closed.png"] {
     transform: rotate(-90deg);
-    
+
 }
 
 .doxygen-content .compoundTemplParams {
     font-family: var(--font-family-monospace);
     color: var(--primary-dark-color);
     font-size: var(--code-font-size);
 }
@@ -1895,15 +1895,15 @@
         padding-top: 0;
     }
 
     .doxygen-content table.memberdecls .mdescLeft {
         margin-bottom: calc(0px - var(--page-font-size));
     }
 
-    .doxygen-content table.memberdecls .memItemRight, 
+    .doxygen-content table.memberdecls .memItemRight,
     .doxygen-content table.memberdecls .mdescRight,
     .doxygen-content table.memberdecls .memTemplItemRight {
         border-top: 0;
         padding-top: 0;
         padding-right: var(--spacing-large);
         overflow-x: auto;
     }
@@ -2074,16 +2074,16 @@
     border-radius: var(--border-radius-small);
 }
 
 .doxygen-content .classindex dl.even {
     background-color: transparent;
 }
 
-/* 
- Class Index Doxygen 1.8 
+/*
+ Class Index Doxygen 1.8
 */
 
 .doxygen-content table.classindex {
     margin-left: 0;
     margin-right: 0;
     width: 100%;
 }
@@ -2220,15 +2220,15 @@
 .doxygen-content .contents table:not(.memberdecls):not(.mlabels):not(.fieldtable):not(.memname) tbody::-webkit-scrollbar-thumb,
 .doxygen-content div.contents .toc::-webkit-scrollbar-thumb,
 .doxygen-content .contents .dotgraph::-webkit-scrollbar-thumb,
 .doxygen-content .contents .tabs-overview-container::-webkit-scrollbar-thumb {
     background-color: transparent;
     border: var(--webkit-scrollbar-padding) solid transparent;
     border-radius: calc(var(--webkit-scrollbar-padding) + var(--webkit-scrollbar-padding));
-    background-clip: padding-box;  
+    background-clip: padding-box;
 }
 
 .doxygen-content #nav-tree:hover::-webkit-scrollbar-thumb,
 .doxygen-content div.fragment:hover::-webkit-scrollbar-thumb,
 .doxygen-content pre.fragment:hover::-webkit-scrollbar-thumb,
 .doxygen-content div.memproto:hover::-webkit-scrollbar-thumb,
 .doxygen-content .contents center:hover::-webkit-scrollbar-thumb,
@@ -2491,8 +2491,15 @@
     html:not([data-theme=light]) .doxygen-content .tabs-overview button.tab-button:hover .tab-title {
         color: var(--page-foreground-color);
     }
 }
 
 html[data-theme=dark] .doxygen-content .tabs-overview button.tab-button:hover .tab-title {
     color: var(--page-foreground-color);
-}
+}
+
+/*
+ Alignment for Doxygen tables (eg: Modules)
+*/
+.doxygen-content .contents {
+    justify-content: left;
+}
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/header.html` & `rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/header.html`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/data/_doxygen/stylesheet.css` & `rocm_docs_core-1.0.0/src/rocm_docs/data/_doxygen/stylesheet.css`

 * *Files 0% similar despite different names*

```diff
@@ -418,17 +418,15 @@
 .doxygen-content img.dark-mode-visible {
 	display: none;
 }
 .doxygen-content img.light-mode-visible {
 	display: none;
 }
 
-.doxygen-content img.formulaDsp {
-	
-}
+.doxygen-content img.formulaDsp {}
 
 .doxygen-content img.formulaInl, .doxygen-content img.inline {
 	vertical-align: middle;
 }
 
 .doxygen-content div.center {
 	text-align: center;
@@ -484,27 +482,27 @@
 	color: #002080;
 }
 
 .doxygen-content span.charliteral {
 	color: #008080;
 }
 
-.doxygen-content span.vhdldigit { 
+.doxygen-content span.vhdldigit {
 	color: #FF00FF;
 }
 
-.doxygen-content span.vhdlchar { 
+.doxygen-content span.vhdlchar {
 	color: #000000;
 }
 
-.doxygen-content span.vhdlkeyword { 
+.doxygen-content span.vhdlkeyword {
 	color: #700070;
 }
 
-.doxygen-content span.vhdllogic { 
+.doxygen-content span.vhdllogic {
 	color: #FF0000;
 }
 
 .doxygen-content blockquote {
         background-color: #F7F8FB;
         border-left: 2px solid #9CAFD4;
         margin: 0 24px 0 4px;
@@ -1226,20 +1224,20 @@
 
 .doxygen-content #projectlogo
 {
 	text-align: center;
 	vertical-align: bottom;
 	border-collapse: separate;
 }
- 
+
 .doxygen-content #projectlogo img
-{ 
+{
 	border: 0px none;
 }
- 
+
 .doxygen-content #projectalign
 {
         vertical-align: middle;
         padding-left: 0.5em;
 }
 
 .doxygen-content #projectname
@@ -1668,8 +1666,8 @@
     content: "▼";
     padding-right:4px;
     font-size: 80%;
 }
 
 .doxygen-content .contents .doxysphinx-inline-parent p {
 	display: inline;
-}
+}
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/components/article-info.html` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/components/article-info.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div id="rocm-docs-core-article-info" class="sd-container-fluid sd-sphinx-override sd-p-0 sd-mt-2 sd-mb-4 sd-p-2 sd-rounded-1 docutils">
 <div class="sd-row sd-row-cols-2 sd-gx-2 sd-gy-1 docutils">
 <div class="sd-col sd-col-auto sd-d-flex-row sd-align-minor-center docutils" style="color:gray;">
-    OS: <!--osicons-->
+    Applies to <!--os-info-->
 </div>
 <div class="sd-col sd-d-flex-row sd-align-minor-center docutils">
 <div class="sd-container-fluid sd-sphinx-override docutils">
 <div class="sd-row sd-row-cols-2 sd-row-cols-xs-2 sd-row-cols-sm-3 sd-row-cols-md-3 sd-row-cols-lg-3 sd-gx-3 sd-gy-1 docutils">
 <div class="sd-col sd-col-auto sd-d-flex-row sd-align-minor-center docutils">
     <p class="sd-p-0 sd-m-0" style="color:gray;">AMD</p>
 </div>
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/sections/footer.html` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/sections/footer.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,39 @@
-<div class="rocm-footer">
-    {%- include "components/social-links.html" with context -%}
-    <div class="rocm-footer-links">
-        <ul>
-            <li><a href="https://www.amd.com/en/corporate/copyright" target="_blank">Terms and Conditions</a></li>
-            <li><a href="https://rocm.docs.amd.com/en/latest/release/licensing.html">ROCm Licenses and Disclaimers</a></li>
-            <li><a href="https://www.amd.com/en/corporate/privacy" target="_blank">Privacy</a></li>
-            <li><a href="https://www.amd.com/en/corporate/trademarks" target="_blank">Trademarks</a></li>
-            <li><a href="https://www.amd.com/system/files/documents/statement-human-trafficking-forced-labor.pdf" target="_blank">Statement on Forced Labor</a></li>
-            <li><a href="https://www.amd.com/en/corporate/competition" target="_blank">Fair and Open Competition</a></li>
-            <li><a href="https://www.amd.com/system/files/documents/amd-uk-tax-strategy.pdf" target="_blank">UK Tax Strategy</a></li>
-            <li><a href="https://www.amd.com/en/corporate/cookies" target="_blank">Cookie Policy</a></li>
-            <!-- OneTrust Cookies Settings button start -->
-            <li><a href="#cookie-settings" id="ot-sdk-btn" class="ot-sdk-show-settings">Cookie Settings</a></li>
-            <!-- OneTrust Cookies Settings button end -->        
-        </ul>
+{%
+from "flavors/" ~ theme_flavor ~ "/footer.jinja" import
+    license_link
+with context
+%}
+<footer class="rocm-footer">
+    <div class="container-lg">
+        <section class="bottom-menu menu py-45">
+            <div class="row d-flex align-items-center">
+                <div class="col-12 text-center">
+                    <ul>
+                        <li><a href="https://www.amd.com/en/corporate/copyright" target="_blank">Terms and Conditions</a></li>
+                        {{ license_link() }}
+                        <li><a href="https://www.amd.com/en/corporate/privacy" target="_blank">Privacy</a></li>
+                        <li><a href="https://www.amd.com/en/corporate/trademarks" target="_blank">Trademarks</a></li>
+                        <li><a href="https://www.amd.com/system/files/documents/statement-human-trafficking-forced-labor.pdf" target="_blank">Statement on Forced Labor</a></li>
+                        <li><a href="https://www.amd.com/en/corporate/competition" target="_blank">Fair and Open Competition</a></li>
+                        <li><a href="https://www.amd.com/system/files/documents/amd-uk-tax-strategy.pdf" target="_blank">UK Tax Strategy</a></li>
+                        <li><a href="https://www.amd.com/en/corporate/cookies" target="_blank">Cookie Policy</a></li>
+                        <!-- OneTrust Cookies Settings button start -->
+                        <li><a href="#cookie-settings" id="ot-sdk-btn" class="ot-sdk-show-settings">Cookie Settings</a></li>
+                        <!-- OneTrust Cookies Settings button end -->
+                    </ul>
+                </div>
+            </div>
+            <div class="row d-flex align-items-center">
+                <div class="col-12 text-center">
+                    <div>
+                        <span class="copyright">© 2023 Advanced Micro Devices, Inc</span>
+                    </div>
+                </div>
+            </div>
+        </section>
     </div>
-    {% include 'components/copyright.html' %}
-</div>
+</footer>
 
 <!-- <div id="rdc-watermark-container">
     <img id="rdc-watermark" src="{{ pathto('_static/images/alpha-watermark.svg',1) }}" alt="DRAFT watermark"/>
 </div> -->
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-{%- include "components/social-links.html" with context -%}
+{% from "flavors/" ~ theme_flavor ~ "/footer.jinja" import license_link with
+context %}
     * _T_e_r_m_s_ _a_n_d_ _C_o_n_d_i_t_i_o_n_s
-    * _R_O_C_m_ _L_i_c_e_n_s_e_s_ _a_n_d_ _D_i_s_c_l_a_i_m_e_r_s
+    * {{ license_link() }}
     * _P_r_i_v_a_c_y
     * _T_r_a_d_e_m_a_r_k_s
     * _S_t_a_t_e_m_e_n_t_ _o_n_ _F_o_r_c_e_d_ _L_a_b_o_r
     * _F_a_i_r_ _a_n_d_ _O_p_e_n_ _C_o_m_p_e_t_i_t_i_o_n
     * _U_K_ _T_a_x_ _S_t_r_a_t_e_g_y
     * _C_o_o_k_i_e_ _P_o_l_i_c_y
     * _C_o_o_k_i_e_ _S_e_t_t_i_n_g_s
-{% include 'components/copyright.html' %}
+Â© 2023 Advanced Micro Devices, Inc
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-500italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-600italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-800italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts.css` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts.css.map` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.css.map`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/fonts.scss` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/fonts.scss`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/alpha-watermark.svg`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/amd-header-logo.svg`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 00000320: 6c79 676f 6e20 636c 6173 733d 2263 6c73  lygon class="cls
 00000330: 2d31 2220 706f 696e 7473 3d22 3131 352e  -1" points="115.
 00000340: 3734 2032 332e 3938 2031 3135 2e37 3420  74 23.98 115.74 
 00000350: 3130 2e39 2031 3036 2e34 2032 302e 3234  10.9 106.4 20.24
 00000360: 2031 3036 2e34 2033 332e 3333 2031 3139   106.4 33.33 119
 00000370: 2e34 3820 3333 2e33 3320 3132 382e 3832  .48 33.33 128.82
 00000380: 2032 332e 3938 2031 3135 2e37 3420 3233   23.98 115.74 23
-00000390: 2e39 3822 2f3e 3c2f 7376 673e            .98"/></svg>
+00000390: 2e39 3822 2f3e 3c2f 7376 673e 0a         .98"/></svg>.
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg`

 * *Files 0% similar despite different names*

```diff
@@ -103,8 +103,8 @@
 00000660: 2d33 3233 2039 202d 3838 2031 3820 2d31  -323 9 -88 18 -1
 00000670: 3933 2032 3220 2d32 3333 206c 3620 2d37  93 22 -233 l6 -7
 00000680: 3320 2d38 3420 3320 2d38 3420 3320 3320  3 -84 3 -84 3 3 
 00000690: 3630 2063 3220 3536 2033 3320 3333 3720  60 c2 56 33 337 
 000006a0: 3532 2034 3835 2032 3720 3231 3020 3333  52 485 27 210 33
 000006b0: 2032 3530 2033 3720 3234 3620 3320 2d33   250 37 246 3 -3
 000006c0: 2031 3120 2d37 3820 3139 202d 3136 387a   11 -78 19 -168z
-000006d0: 222f 3e0a 3c2f 673e 0a3c 2f73 7667 3e    "/>.</g>.</svg>
+000006d0: 222f 3e0a 3c2f 673e 0a3c 2f73 7667 3e0a  "/>.</g>.</svg>.
```

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png` & `rocm_docs_core-1.0.0/src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png`

 * *Files identical despite different names*

### Comparing `rocm-docs-core-0.9.2/src/rocm_docs_core.egg-info/SOURCES.txt` & `rocm_docs_core-1.0.0/src/rocm_docs_core.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/rocm_docs/__init__.py
 src/rocm_docs/core.py
 src/rocm_docs/doxygen.py
+src/rocm_docs/formatting.py
+src/rocm_docs/projects.py
+src/rocm_docs/py.typed
 src/rocm_docs/theme.py
 src/rocm_docs/util.py
+src/rocm_docs/data/projects.schema.json
+src/rocm_docs/data/projects.yaml
 src/rocm_docs/data/_doxygen/extra_stylesheet.css
 src/rocm_docs/data/_doxygen/footer.html
 src/rocm_docs/data/_doxygen/header.html
 src/rocm_docs/data/_doxygen/stylesheet.css
+src/rocm_docs/rocm_docs_theme/404.html
 src/rocm_docs/rocm_docs_theme/layout.html
 src/rocm_docs/rocm_docs_theme/theme.conf
 src/rocm_docs/rocm_docs_theme/components/article-info.html
-src/rocm_docs/rocm_docs_theme/components/copyright.html
 src/rocm_docs/rocm_docs_theme/components/left-side-menu.html
-src/rocm_docs/rocm_docs_theme/components/social-links.html
+src/rocm_docs/rocm_docs_theme/components/toggle-primary-sidebar.html
+src/rocm_docs/rocm_docs_theme/flavors/rocm/footer.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm/header.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm/left-side-menu.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/footer.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/header.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm-blogs/left-side-menu.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/footer.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/header.jinja
+src/rocm_docs/rocm_docs_theme/flavors/rocm-docs-home/left-side-menu.jinja
 src/rocm_docs/rocm_docs_theme/sections/footer-content.html
 src/rocm_docs/rocm_docs_theme/sections/footer.html
 src/rocm_docs/rocm_docs_theme/sections/header.html
 src/rocm_docs/rocm_docs_theme/static/code_word_breaks.js
 src/rocm_docs/rocm_docs_theme/static/custom.css
 src/rocm_docs/rocm_docs_theme/static/fonts.css
 src/rocm_docs/rocm_docs_theme/static/fonts.css.map
 src/rocm_docs/rocm_docs_theme/static/fonts.scss
+src/rocm_docs/rocm_docs_theme/static/rdcMisc.js
 src/rocm_docs/rocm_docs_theme/static/renameVersionLinks.js
 src/rocm_docs/rocm_docs_theme/static/rocm_footer.css
 src/rocm_docs/rocm_docs_theme/static/rocm_header.css
+src/rocm_docs/rocm_docs_theme/static/theme_mode_captions.js
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300.woff2
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-300italic.woff2
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500.woff2
 src/rocm_docs/rocm_docs_theme/static/fonts/open-sans/open-sans-v34-latin-500italic.woff
@@ -80,8 +96,12 @@
 src/rocm_docs/rocm_docs_theme/static/images/beta-watermark.svg
 src/rocm_docs/rocm_docs_theme/static/images/rocm-logo.png
 src/rocm_docs_core.egg-info/PKG-INFO
 src/rocm_docs_core.egg-info/SOURCES.txt
 src/rocm_docs_core.egg-info/dependency_links.txt
 src/rocm_docs_core.egg-info/entry_points.txt
 src/rocm_docs_core.egg-info/requires.txt
-src/rocm_docs_core.egg-info/top_level.txt
+src/rocm_docs_core.egg-info/top_level.txt
+tests/test_doxygen.py
+tests/test_meta.py
+tests/test_projects.py
+tests/test_sites.py
```

