# Comparing `tmp/mkdocs_publisher-1.2.0.tar.gz` & `tmp/mkdocs_publisher-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_publisher-1.2.0.tar", max compression
+gzip compressed data, was "mkdocs_publisher-1.3.0.tar", max compression
```

## Comparing `mkdocs_publisher-1.2.0.tar` & `mkdocs_publisher-1.3.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0     1098 2023-10-02 21:12:38.574444 mkdocs_publisher-1.2.0/LICENSE
--rw-r--r--   0        0        0     4245 2023-10-17 16:56:53.922567 mkdocs_publisher-1.2.0/README.md
--rw-r--r--   0        0        0     1984 2023-10-10 11:40:00.321915 mkdocs_publisher-1.2.0/mkdocs_publisher/_cli/plugins/dev.py
--rw-r--r--   0        0        0     3493 2023-10-10 11:40:00.322168 mkdocs_publisher-1.2.0/mkdocs_publisher/_cli/plugins/md_tools.py
--rw-r--r--   0        0        0     1911 2023-10-10 11:40:00.322463 mkdocs_publisher-1.2.0/mkdocs_publisher/_cli/publisher.py
--rw-r--r--   0        0        0     1136 2023-10-10 11:40:00.322595 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/__init__.py
--rw-r--r--   0        0        0     1136 2023-10-10 11:40:00.322687 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py
--rw-r--r--   0        0        0     2016 2023-10-10 11:40:00.322840 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css
--rw-r--r--   0        0        0      689 2023-10-02 21:12:38.595155 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css
--rw-r--r--   0        0        0     2471 2023-10-10 11:40:00.323066 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map
--rw-r--r--   0        0        0     3348 2023-10-10 11:40:00.323176 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css
--rw-r--r--   0        0        0     1861 2023-10-02 21:12:38.595338 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css
--rw-r--r--   0        0        0     3852 2023-10-10 11:40:00.323283 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map
--rw-r--r--   0        0        0     1136 2023-10-10 11:40:00.323387 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/templates/__init__.py
--rw-r--r--   0        0        0     1443 2023-10-10 11:40:00.323674 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/templates/backlinks.html
--rw-r--r--   0        0        0     1892 2023-10-10 11:40:00.323954 mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/templates/posts-list.html
--rw-r--r--   0        0        0     2801 2023-10-17 16:56:53.923007 mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/file_utils.py
--rw-r--r--   0        0        0     2181 2023-10-10 11:40:00.324395 mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/html_modifiers.py
--rw-r--r--   0        0        0     8900 2023-10-17 16:56:53.923303 mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/links.py
--rw-r--r--   0        0        0     2012 2023-10-10 11:40:00.324881 mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/mkdocs_utils.py
--rw-r--r--   0        0        0     3626 2023-10-10 11:40:00.325303 mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/resources.py
--rw-r--r--   0        0        0     1474 2023-10-10 11:40:00.325424 mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/urls.py
--rw-r--r--   0        0        0     3027 2023-10-10 11:40:00.325730 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/config.py
--rw-r--r--   0        0        0     8636 2023-10-10 11:40:00.326098 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/creators.py
--rw-r--r--   0        0        0     1136 2023-10-10 11:40:00.326182 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/lang/__init__.py
--rw-r--r--   0        0        0      355 2023-10-02 21:12:38.596205 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/lang/en.yaml
--rw-r--r--   0        0        0      368 2023-10-02 21:12:38.596253 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/lang/pl.yaml
--rw-r--r--   0        0        0     4411 2023-10-10 11:40:00.326305 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/modifiers.py
--rw-r--r--   0        0        0     8596 2023-10-10 11:40:00.326568 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/parsers.py
--rw-r--r--   0        0        0     6619 2023-10-10 12:08:40.413927 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/plugin.py
--rw-r--r--   0        0        0     4011 2023-10-10 11:40:00.326907 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/structures.py
--rw-r--r--   0        0        0     2988 2023-10-10 11:40:00.327017 mkdocs_publisher-1.2.0/mkdocs_publisher/blog/translate.py
--rw-r--r--   0        0        0     2726 2023-10-10 11:40:00.327149 mkdocs_publisher-1.2.0/mkdocs_publisher/debugger/config.py
--rw-r--r--   0        0        0     4354 2023-10-10 11:40:00.327241 mkdocs_publisher-1.2.0/mkdocs_publisher/debugger/loggers.py
--rw-r--r--   0        0        0     6321 2023-10-10 11:40:00.327457 mkdocs_publisher-1.2.0/mkdocs_publisher/debugger/plugin.py
--rw-r--r--   0        0        0     2377 2023-10-10 11:40:00.327696 mkdocs_publisher-1.2.0/mkdocs_publisher/meta/config.py
--rw-r--r--   0        0        0    17209 2023-10-10 12:08:40.414363 mkdocs_publisher-1.2.0/mkdocs_publisher/meta/plugin.py
--rw-r--r--   0        0        0     7711 2023-10-17 16:59:53.419870 mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/base.py
--rw-r--r--   0        0        0     5195 2023-10-17 16:56:53.923617 mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/config.py
--rw-r--r--   0        0        0    11938 2023-10-17 16:56:53.923786 mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/minifiers.py
--rw-r--r--   0        0        0     5296 2023-10-10 11:40:00.328630 mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/plugin.py
--rw-r--r--   0        0        0     6891 2023-10-10 11:40:00.328903 mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/backlinks.py
--rw-r--r--   0        0        0     6025 2023-10-10 11:40:00.329019 mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/callouts.py
--rw-r--r--   0        0        0     2659 2023-10-17 16:56:53.924078 mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/config.py
--rw-r--r--   0        0        0     4602 2023-10-10 11:40:00.329363 mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/md_links.py
--rw-r--r--   0        0        0     8664 2023-10-17 16:56:53.924506 mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/plugin.py
--rw-r--r--   0        0        0     4203 2023-10-10 11:40:00.329739 mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/vega.py
--rw-r--r--   0        0        0     2035 2023-10-10 11:40:00.329831 mkdocs_publisher-1.2.0/mkdocs_publisher/social/config.py
--rw-r--r--   0        0        0     5155 2023-10-10 11:40:00.329999 mkdocs_publisher-1.2.0/mkdocs_publisher/social/plugin.py
--rw-r--r--   0        0        0     3569 2023-10-17 16:56:53.927850 mkdocs_publisher-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 mkdocs_publisher-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1103 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/LICENSE
+-rw-r--r--   0        0        0     4858 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/README.md
+-rw-r--r--   0        0        0     3625 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/dev.py
+-rw-r--r--   0        0        0     3492 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/md_tools.py
+-rw-r--r--   0        0        0     2107 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/publisher.py
+-rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/__init__.py
+-rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css
+-rw-r--r--   0        0        0      689 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css
+-rw-r--r--   0        0        0     2471 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map
+-rw-r--r--   0        0        0     3353 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css
+-rw-r--r--   0        0        0     1861 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css
+-rw-r--r--   0        0        0     3852 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map
+-rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/__init__.py
+-rw-r--r--   0        0        0     1448 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/backlinks.html
+-rw-r--r--   0        0        0     1897 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/posts-list.html
+-rw-r--r--   0        0        0     2941 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/file_utils.py
+-rw-r--r--   0        0        0     2186 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/html_modifiers.py
+-rw-r--r--   0        0        0     9763 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/links.py
+-rw-r--r--   0        0        0     3699 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/mkdocs_utils.py
+-rw-r--r--   0        0        0     2741 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/publisher_utils.py
+-rw-r--r--   0        0        0     3632 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/resources.py
+-rw-r--r--   0        0        0     2580 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/urls.py
+-rw-r--r--   0        0        0     3032 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/config.py
+-rw-r--r--   0        0        0     8617 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/creators.py
+-rw-r--r--   0        0        0     1141 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/__init__.py
+-rw-r--r--   0        0        0      355 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/en.yaml
+-rw-r--r--   0        0        0      368 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/pl.yaml
+-rw-r--r--   0        0        0     4416 2024-04-18 13:43:52.373277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/modifiers.py
+-rw-r--r--   0        0        0     8421 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/parsers.py
+-rw-r--r--   0        0        0     6491 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/plugin.py
+-rw-r--r--   0        0        0     3990 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/structures.py
+-rw-r--r--   0        0        0     2993 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/blog/translate.py
+-rw-r--r--   0        0        0     2796 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/config.py
+-rw-r--r--   0        0        0     4950 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/loggers.py
+-rw-r--r--   0        0        0     6416 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/plugin.py
+-rw-r--r--   0        0        0     3945 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/config.py
+-rw-r--r--   0        0        0    15338 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/meta_files.py
+-rw-r--r--   0        0        0     5605 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/nav.py
+-rw-r--r--   0        0        0     5609 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/meta/plugin.py
+-rw-r--r--   0        0        0     7668 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/base.py
+-rw-r--r--   0        0        0     5200 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/config.py
+-rw-r--r--   0        0        0    11943 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/minifiers.py
+-rw-r--r--   0        0        0     5271 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/plugin.py
+-rw-r--r--   0        0        0     5423 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/backlinks.py
+-rw-r--r--   0        0        0     6030 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/callouts.py
+-rw-r--r--   0        0        0     2784 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/config.py
+-rw-r--r--   0        0        0     5062 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/md_links.py
+-rw-r--r--   0        0        0     8579 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/plugin.py
+-rw-r--r--   0        0        0     4207 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/vega.py
+-rw-r--r--   0        0        0     2040 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/social/config.py
+-rw-r--r--   0        0        0     5160 2024-04-18 13:43:52.377277 mkdocs_publisher-1.3.0/mkdocs_publisher/social/plugin.py
+-rw-r--r--   0        0        0     3516 2024-04-18 13:43:52.445277 mkdocs_publisher-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6740 1970-01-01 00:00:00.000000 mkdocs_publisher-1.3.0/PKG-INFO
```

### Comparing `mkdocs_publisher-1.2.0/LICENSE` & `mkdocs_publisher-1.3.0/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/README.md` & `mkdocs_publisher-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
----
-date: 2023-10-02 23:12:38
-update: 2023-10-10 13:18:32
----
 # Publisher for MkDocs
 
-[![PyPI version](https://img.shields.io/pypi/v/mkdocs-publisher?logo=pypi&style=plastic)](https://pypi.org/project/mkdocs-publisher/)
-[![License type](https://img.shields.io/pypi/l/mkdocs-publisher?logo=pypi&style=plastic)](https://opensource.org/license/mit/)
-[![PyPI Downloads last month](https://img.shields.io/pypi/dm/mkdocs-publisher?logo=pypi&style=plastic)](https://pypistats.org/search/mkdocs-publisher)
-[![Python versions](https://img.shields.io/pypi/pyversions/mkdocs-publisher?logo=python&style=plastic)](https://www.python.org)
-[![GitHub last commit](https://img.shields.io/github/last-commit/mkusz/mkdocs-publisher?logo=github&style=plastic)](https://github.com/mkusz/mkdocs-publisher/commits/main)
+[![License type](https://img.shields.io/github/license/mkusz/mkdocs-publisher?logo=pypi&logoColor=white&style=plastic&label=License)](https://opensource.org/license/mit/)
+[![PyPI version](https://img.shields.io/pypi/v/mkdocs-publisher?logo=pypi&logoColor=white&style=plastic&label=PyPi)](https://pypi.org/project/mkdocs-publisher/)
+[![PyPI - Python Version](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmkusz%2Fmkdocs-publisher%2Fmain%2Fpyproject.toml&query=%24.tool.poetry.dependencies.python&logo=python&logoColor=white&style=plastic&label=Python)](https://www.python.org)
+[![PyPI Downloads last month](https://img.shields.io/pypi/dm/mkdocs-publisher?logo=pypi&logoColor=white&style=plastic&label=Downloads)](https://pypistats.org/search/mkdocs-publisher)
+[![GitHub last commit](https://img.shields.io/github/last-commit/mkusz/mkdocs-publisher?logo=github&logoColor=white&style=plastic&label=Last%20commit)](https://github.com/mkusz/mkdocs-publisher/commits/main)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=plastic&label=Pre-commit)](https://github.com/pre-commit/pre-commit)
+![Code Coverage](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmkusz%2Fmkdocs-publisher%2Fmain%2Fcov.json&query=%24.percent_covered_display&suffix=%25&color=green&style=plastic&label=Code%20coverage)
 
 Publisher for [MkDocs](https://www.mkdocs.org/) is a set of plugins that helps with content creation and publication.
 
 ## Features
 
 - [pub-meta](https://mkusz.github.io/mkdocs-publisher/setup/general/pub-meta/) – support for:
 	- automatic [document navigation](https://www.mkdocs.org/user-guide/configuration/#nav) creation based on file names order,
@@ -50,21 +48,21 @@
 
 ```yaml
 theme: material
 
 plugins:
   - search  # Material for MkDocs search plugin
   - pub-debugger
-  - pub-obsidian  # blog is a directory with all blog posts
+  - pub-blog
   - pub-obsidian
   - pub-social
   - pub-meta
   - pub-minifier
 ```
 
 ## Planned features
 
-A full list of planned developments can be found on [this documentation page](https://mkusz.github.io/mkdocs-publisher/development/other/backlog/). I'm planning to move it to the project [GitHub issues](https://github.com/mkusz/mkdocs-publisher/issues) with proper badges and longer descriptions, but it's time-consuming and at this stage I'd rather spend it to develop a project.
+A full list of planned developments can be found on [this documentation page](https://mkusz.github.io/mkdocs-publisher/development/other/backlog/). I'm planning to move it to the project [GitHub issues](https://github.com/mkusz/mkdocs-publisher/issues) with proper badges and longer descriptions, but it's time-consuming and at this stage I'd rather spend it developing a project.
 
 ## Version history
 
 The entire version history can be found in the project [version history](https://mkusz.github.io/mkdocs-publisher/development/changelog/) document and inside [releases](https://github.com/mkusz/mkdocs-publisher/releases).
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_cli/plugins/dev.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/publisher.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,40 +16,40 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import importlib
+import logging
 import pathlib
 
 import click
 
-from mkdocs_publisher._shared import file_utils
-
 
 @click.group
-def app():
-    """Development tools"""
-    pass
-
-
-@app.command()
-def css_min():
-    """Minify project CSS files"""
-    project_dir = pathlib.Path.cwd() / "mkdocs_publisher"
-    for input_css_file in project_dir.rglob("*.css"):
-        if ".min" not in input_css_file.suffixes:
-            output_css_file = input_css_file.parent / f"{input_css_file.stem}.min.css"
-            print(output_css_file)
-            cmd = [
-                "postcss",
-                str(input_css_file),
-                "-m",
-                "--verbose",
-                "-u",
-                "cssnano",
-                "postcss-svgo",
-                "-o",
-                str(output_css_file),
-            ]
-            file_utils.run_subprocess(cmd, capture_output=False)
+@click.option("--debug", is_flag=True, default=False, help="Show debug messages")
+def app(debug):
+    """Publisher plugin for MkDocs (by Maciej 'maQ' Kusz).
+
+    More information can be fount at: https://github.com/mkusz/mkdocs-publisher
+    """
+    log_level = logging.DEBUG if debug else logging.INFO
+    logging.basicConfig(level=log_level)
+
+
+def build_app(app: click.group):  # type: ignore
+    plugins_path = pathlib.Path(__file__).parent.resolve() / "plugins"
+    for plugin_file_name in pathlib.Path(plugins_path).rglob("*.py"):
+        plugin_name = pathlib.PurePath(plugin_file_name).stem
+        plugin_module = importlib.import_module(f"mkdocs_publisher._cli.plugins.{plugin_name}")
+        app.add_command(
+            cmd=getattr(plugin_module, "app", plugin_name), name=str(plugin_name.replace("_", "-"))
+        )
+
+
+build_app(app=app)
+
+
+if __name__ == "__main__":
+    app()
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_cli/plugins/md_tools.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_cli/plugins/md_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -32,15 +32,15 @@
 from mkdocs_publisher.obsidian.plugin import ObsidianPlugin
 
 log = logging.getLogger("mkdocs.plugins.publisher.cli.md_tools")
 
 
 @click.group
 def app():
-    """Markdown tools"""
+    """Markdown tools."""
     pass
 
 
 @app.command()
 def key_rename():
     mkdocs_config = mkdocs_utils.get_mkdocs_config()
     obsidian_plugin = ObsidianPlugin()
@@ -72,12 +72,12 @@
                     post_meta.pop(key, None)
                 elif key in [old_key_name, new_key_name] and old_key_name in post_meta:
                     yaml_text_dump = yaml.safe_dump(
                         {new_key_name: post_meta[old_key_name]}, indent=2
                     )
                     output = f"{output}{yaml_text_dump}"
                     post_meta.pop(old_key_name, None)
-            for key in post_meta.keys():
+            for key in post_meta:
                 output = f"{output}{yaml.safe_dump({key: post_meta[key]}, indent=2)}"
             output = f"{output}---\n\n{content}"
             md_file.seek(0)
             md_file.write(output)
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_cli/publisher.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/translate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,37 +16,59 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import importlib
-import pathlib
+import importlib.resources
+import logging
+from dataclasses import fields
+from pathlib import Path
+from typing import cast
 
-import click
+import yaml
 
+from mkdocs_publisher.blog import lang as lang_path
+from mkdocs_publisher.blog.config import BlogPluginConfig
+from mkdocs_publisher.blog.structures import Translation
 
-@click.group
-def app():
-    """Publisher plugin for MkDocs (by Maciej 'maQ' Kusz).
+log = logging.getLogger("mkdocs.plugins.publisher.blog.translate")
 
-    More information can be fount at: https://github.com/mkusz/mkdocs-publisher
-    """
-    pass
 
+class Translate:
+    def __init__(self, config: BlogPluginConfig):
+        self._config: BlogPluginConfig = config
+        self._translation: Translation = cast(Translation, None)
 
-def build_app(app: click.group):  # type: ignore
-    plugins_path = pathlib.Path(__file__).parent.resolve() / "plugins"
-    for plugin_file_name in pathlib.Path(plugins_path).rglob("*.py"):
-        plugin_name = pathlib.PurePath(plugin_file_name).stem
-        plugin_module = importlib.import_module(f"mkdocs_publisher._cli.plugins.{plugin_name}")
-        app.add_command(
-            cmd=getattr(plugin_module, "app", plugin_name), name=str(plugin_name.replace("_", "-"))
-        )
-
-
-build_app(app=app)
+        self._read_lang()
 
-
-if __name__ == "__main__":
-    app()
+    def _read_lang(self):
+        lang_yaml_oath = Path(
+            str(importlib.resources.files(lang_path).joinpath(f"{self._config.lang}.yaml"))
+        )
+        if not lang_yaml_oath.exists():
+            log.warning(
+                f"There is no translation for '{self._config.lang}' language, "
+                f"so default language ('{BlogPluginConfig.lang.default}') will be used"
+            )
+            lang_yaml_oath = str(
+                importlib.resources.files(lang_path).joinpath(
+                    f"{BlogPluginConfig.lang.default}.yaml"
+                )
+            )
+        with open(lang_yaml_oath) as lang_yaml:
+            translation_yaml_data = yaml.safe_load(lang_yaml)
+        translation_keys = [f.name for f in fields(Translation)]
+        translation_data = {
+            k: v for k, v in translation_yaml_data.items() if k in translation_keys
+        }
+        # Inject overrides from mkdocs.yml config
+        for key in translation_keys:
+            value = self._config.translation.get(key, None)
+            if value is not None:
+                translation_data[key] = value
+        self._translation = Translation(**translation_data)
+
+    @property
+    def translation(self) -> Translation:
+        return self._translation
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/__init__.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MIT License
  *
- * Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+ * Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/blog.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MIT License
  *
- * Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+ * Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
  *
  * Permission is hereby granted, free of charge, to any person obtaining a copy
  * of this software and associated documentation files (the "Software"), to deal
  * in the Software without restriction, including without limitation the rights
  * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  * copies of the Software, and to permit persons to whom the Software is
  * furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/stylesheets/obsidian.min.css.map`

 * *Files identical despite different names*

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/templates/__init__.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/templates/backlinks.html` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/backlinks.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 <!--
   ~ MIT License
   ~
-  ~ Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+  ~ Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
   ~
   ~ Permission is hereby granted, free of charge, to any person obtaining a copy
   ~ of this software and associated documentation files (the "Software"), to deal
   ~ in the Software without restriction, including without limitation the rights
   ~ to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
   ~ copies of the Software, and to permit persons to whom the Software is
   ~ furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_extra/assets/templates/posts-list.html` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_extra/assets/templates/posts-list.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--
   ~ MIT License
   ~
-  ~ Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+  ~ Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
   ~
   ~ Permission is hereby granted, free of charge, to any person obtaining a copy
   ~ of this software and associated documentation files (the "Software"), to deal
   ~ in the Software without restriction, including without limitation the rights
   ~ to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
   ~ copies of the Software, and to permit persons to whom the Software is
   ~ furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/file_utils.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/file_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,15 +20,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 import subprocess
 from hashlib import md5
 from pathlib import Path
-from typing import List
+from typing import Optional
 from uuid import uuid4
 
 log = logging.getLogger("mkdocs.plugins.publisher._shared.file_utils")
 
 
 def run_subprocess(cmd, capture_output: bool = True) -> subprocess.CompletedProcess:
     cmd = [arg for arg in cmd if arg is not None]
@@ -51,26 +51,28 @@
         while chunk := binary_file.read(block_size):
             file_hash.update(chunk)
         return file_hash.hexdigest()
 
 
 def list_files(
     directory: Path,
-    extensions: List[str] = [],
-    exclude: List[str] = [],
-) -> List[Path]:
-    temp_files_list: List[Path] = []
+    extensions: Optional[list[str]] = None,
+    exclude: Optional[list[str]] = None,
+) -> list[Path]:
+    temp_files_list: list[Path] = []
+    extensions = [] if extensions is None else extensions
+    exclude = [] if exclude is None else exclude
     for ext in extensions:
         for file in directory.glob(f"**/*{ext}"):
             temp_files_list.append(file.relative_to(directory))
 
-    excluded_files_list: List[Path] = []
+    excluded_files_list: list[Path] = []
     for exc in exclude:
         for file in directory.rglob(exc):
             excluded_files_list.append(file.relative_to(directory))
 
-    files_list: List[Path] = [file for file in temp_files_list if file not in excluded_files_list]
+    files_list: list[Path] = [file for file in temp_files_list if file not in excluded_files_list]
     return files_list
 
 
 def get_hashed_file_name(file: Path) -> Path:
     return Path(file.with_name(f"{str(uuid4()).replace('-', '')}{str(file.suffix).lower()}").name)
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/html_modifiers.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/html_modifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/mkdocs_utils.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/publisher_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,32 +17,53 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
+from pathlib import Path
+from typing import Optional
+from typing import Union
 from typing import cast
 
 from mkdocs.config.defaults import MkDocsConfig
 
-log = logging.getLogger("mkdocs.plugins.publisher._shared.mkdosc_utils")
+from mkdocs_publisher._shared import mkdocs_utils
+from mkdocs_publisher.blog.config import BlogPluginConfig
+from mkdocs_publisher.obsidian.config import ObsidianPluginConfig
+
+log = logging.getLogger("mkdocs.plugins.publisher._shared.publisher_utils")
+
+
+def get_blog_dir(mkdocs_config: MkDocsConfig) -> Optional[Path]:
+    blog_config: Optional[Union[BlogPluginConfig, Path]] = cast(
+        BlogPluginConfig,
+        mkdocs_utils.get_plugin_config(
+            mkdocs_config=mkdocs_config,
+            plugin_name="pub-blog",
+        ),
+    )
+    if blog_config is not None:
+        blog_config = Path(mkdocs_config.docs_dir).joinpath(blog_config.blog_dir)
+
+    return blog_config
+
+
+def get_obsidian_dirs(mkdocs_config: MkDocsConfig) -> tuple[list[Path], Optional[Path]]:
+    ignored_dirs: list[Path] = []
+    attachments_dir: Optional[Path] = None
+    docs_dir = Path(mkdocs_config.docs_dir)
+
+    obsidian_config: Optional[ObsidianPluginConfig] = cast(
+        ObsidianPluginConfig,
+        mkdocs_utils.get_plugin_config(
+            mkdocs_config=mkdocs_config,
+            plugin_name="pub-obsidian",
+        ),
+    )
+    if obsidian_config is not None:
+        ignored_dirs.append(docs_dir.joinpath(obsidian_config.obsidian_dir))
+        ignored_dirs.append(docs_dir.joinpath(obsidian_config.templates_dir))
+        attachments_dir = docs_dir.joinpath(obsidian_config.attachments_dir)
 
-
-def get_plugin_config(mkdocs_config: MkDocsConfig, plugin_name: str) -> dict:
-    plugins = mkdocs_config.plugins
-    if isinstance(plugins, list):
-        for plugin in plugins:
-            if isinstance(plugin, dict) and list(plugin.keys())[0] == plugin_name:
-                return plugin[list(plugin.keys())[0]]
-            elif isinstance(plugin, str) and plugin == plugin_name:
-                return {}
-        raise SystemError("Break")
-    else:
-        return mkdocs_config.plugins[plugin_name].config
-
-
-def get_mkdocs_config() -> MkDocsConfig:
-    config = MkDocsConfig()
-    with open("mkdocs.yml", mode="r") as mkdocs_yml:
-        config.load_file(mkdocs_yml)
-    return cast(MkDocsConfig, config)
+    return ignored_dirs, attachments_dir
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/_shared/resources.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/_shared/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -88,10 +88,11 @@
             config_extra_files=config.extra_css,
             files=files,
         )
 
 
 def read_template_file(template_file_name: str) -> str:
     """Read and return content of template file"""
+
     resource_file_path = importlib.resources.files(templates).joinpath(template_file_name)
     with importlib.resources.as_file(resource_file_path) as template_file:
         return template_file.read_text(encoding="utf-8")
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/config.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/creators.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/creators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,15 +20,14 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 from collections import OrderedDict
 from datetime import datetime
 from pathlib import Path
-from typing import Dict
 from typing import cast
 
 import jinja2
 import yaml
 from mkdocs.structure.files import File
 from mkdocs.structure.files import Files
 
@@ -63,18 +62,18 @@
     start_page: bool,
     blog_config: BlogConfig,
     config_nav: OrderedDict,
 ) -> None:
     """Create blog posts index files."""
 
     log.info("Creating blog posts index files")
-    posts_chunks: Dict[str, list] = {}
-    archive_chunks: Dict[str, list] = {}
-    categories_chunks: Dict[str, list] = {}
-    tags_chunks: Dict[str, list] = {}
+    posts_chunks: dict[str, list] = {}
+    archive_chunks: dict[str, list] = {}
+    categories_chunks: dict[str, list] = {}
+    tags_chunks: dict[str, list] = {}
 
     # Build post index pages
     for index, date in enumerate(sorted(blog_config.blog_posts, reverse=True)):
         index = (
             "index"
             if start_page and index < blog_config.plugin_config.posts_per_page
             else f"index-{str(index//blog_config.plugin_config.posts_per_page)}"
@@ -159,15 +158,15 @@
             )
         }
     )
 
 
 def _create_pages(
     blog_config: BlogConfig,
-    posts_chunks: Dict[str, list],
+    posts_chunks: dict[str, list],
     sub_dir: Path,
     page_title: str,
 ) -> list[dict[str, str]]:
     config_nav = []
 
     blog_temp_dir = blog_config.temp_dir / blog_config.plugin_config.blog_dir
     blog_temp_dir.mkdir(exist_ok=True)
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/lang/__init__.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/lang/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/modifiers.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/modifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/parsers.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -72,29 +72,30 @@
     on_serve: bool = False,
 ):
     """Parse all markdown files and extract blog posts from `blog_dir` (default: 'posts').
     BlogPost object is created and filled with content and metadata of the post.
     """
     log.info(f"Parsing blog posts from '{blog_config.blog_dir}' directory")
     for file_path in blog_config.docs_dir.glob("**/*.md"):
-        if blog_config.meta_config is not None:
-            if file_path.parts[-1] == blog_config.meta_config.dir_meta_file:
-                continue
+        if (
+            blog_config.meta_config is not None
+            and file_path.parts[-1] == blog_config.meta_config.dir_meta_file
+        ):
+            continue
         file_path = Path(file_path)
         path = Path(file_path).relative_to(blog_config.docs_dir)
         if path.is_relative_to(blog_config.blog_dir):
             parents = list(path.parents)[:-1]
             with file_path.open(encoding="utf-8-sig", errors="strict") as md_file:
                 content, post_meta = meta_parser.get_data(md_file.read())
                 if not parents:
                     for line in content.split("\n"):
                         if line.startswith("# "):
                             config_nav[line[2:]] = str(path)
                 elif str(parents[0]) == str(blog_config.blog_dir):
-
                     if "publish" not in post_meta:
                         # TODO: read default value from meta config
                         log.info(
                             f"File: {file_path} - missing 1 required positional argument: "
                             f"'publish' (setting to default: draft)"
                         )
                         post_meta["publish"] = "draft"
@@ -136,23 +137,20 @@
                     post_data["path"] = str(path)
                     if (
                         "slug" in post_meta
                         and post_meta["slug"] is not None
                         and post_meta["slug"].strip() != ""
                     ):
                         post_data["slug"] = post_meta["slug"]
-                    # try:
+
                     blog_post: BlogPost = BlogPost(**post_data)
 
                     # Add new post to blog posts collection
                     blog_config.blog_posts[blog_post.date] = blog_post
                     log.debug(f"New blog posts: {blog_post.title}")
-                    # except TypeError as e:
-                    #     msg = str(e).replace("__init__()", f"File: {file_path} -")
-                    #     log.warning(msg)
 
                     # TODO: add reading time
                     # print(f"{file_path} - {count_words(post.content) / 265 * 60}")
 
 
 def create_blog_post_teaser(blog_config: BlogConfig):
     """Extracting beginning of a blog content as a teaser. End of a teaser is determined by
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/plugin.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,19 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import contextlib
 import logging
 from collections import OrderedDict
 from pathlib import Path
 from typing import Any
-from typing import Dict
 from typing import Literal
 from typing import Optional
 from typing import cast
 
 from mkdocs.config import Config
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
@@ -59,15 +59,14 @@
         self._on_serve: bool = False
 
     def on_startup(self, *, command: Literal["build", "gh-deploy", "serve"], dirty: bool) -> None:
         if command == "serve":
             self._on_serve = True
 
     def on_config(self, config: MkDocsConfig) -> Config:
-
         # Initialization of all the values
         self.blog_config.parse_configs(mkdocs_config=config, plugin_config=self.config)
 
         # Modify nav section
         if config.nav is None:
             config.nav = [{str(self.blog_config.blog_dir): str(self.blog_config.blog_dir)}]
 
@@ -109,34 +108,31 @@
             else:
                 new_nav.append(nav_item)
         config.nav = new_nav
 
         return config
 
     def on_nav(self, nav: Navigation, config: MkDocsConfig, files: Files) -> Navigation:
-
         modifiers.blog_post_nav_remove(
             start_page=self._start_page, blog_config=self.blog_config, nav=nav
         )
 
         return nav
 
     def on_files(self, files: Files, config: MkDocsConfig) -> Files:
-
         creators.create_blog_files(blog_config=self.blog_config, files=files)
 
         resources.add_extra_css(stylesheet_file_name="blog.min.css", config=config, files=files)
 
         return files
 
     @event_priority(-100)  # Run after all other plugins
     def on_page_context(
-        self, context: Dict[str, Any], *, page: Page, config: MkDocsConfig, nav: Navigation
-    ) -> Optional[Dict[str, Any]]:
-
+        self, context: dict[str, Any], *, page: Page, config: MkDocsConfig, nav: Navigation
+    ) -> Optional[dict[str, Any]]:
         if Path(page.file.src_path).parts[0] == self.config.blog_dir:
             page.meta[self.config.comments.key_name] = self.config.comments.enabled
 
         # Temporary created files cannot be edited
         if page.file.src_uri in self.blog_config.temp_files_list:
             page.edit_url = None
 
@@ -145,33 +141,26 @@
         )
         return context
 
     @event_priority(-100)  # Run after all other plugins
     def on_page_markdown(
         self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files
     ) -> Optional[str]:
-
         obsidian_plugin: Optional[ObsidianPluginConfig] = mkdocs_utils.get_plugin_config(
             mkdocs_config=config, plugin_name="pub-obsidian"
         )  # type: ignore
         if obsidian_plugin is not None:
             md_links = MarkdownLinks(mkdocs_config=config)
             markdown = md_links.normalize_relative_links(
                 markdown=markdown, current_file_path=page.file.src_path
             )
         return markdown
 
     @event_priority(-100)  # Run after all other plugins
     def on_build_error(self, error: Exception) -> None:
-
-        try:
+        with contextlib.suppress(AttributeError):
             file_utils.remove_dir(directory=self.blog_config.temp_dir)
-        except AttributeError:
-            pass  # TODO: remove this when rebuilding blog plugin
 
     @event_priority(-100)  # Run after all other plugins
     def on_shutdown(self) -> None:
-
-        try:
+        with contextlib.suppress(AttributeError):
             file_utils.remove_dir(directory=self.blog_config.temp_dir)
-        except AttributeError:
-            pass  # TODO: remove this when rebuilding blog plugin
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/blog/structures.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/blog/structures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,16 +21,14 @@
 # SOFTWARE.
 
 from dataclasses import asdict
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import datetime
 from pathlib import Path
-from typing import Dict
-from typing import List
 from typing import Optional
 
 from mkdocs.config.defaults import MkDocsConfig
 
 # noinspection PyProtectedMember
 from mkdocs_publisher._shared import mkdocs_utils
 from mkdocs_publisher.blog.config import BlogPluginConfig
@@ -41,16 +39,16 @@
 class BlogPost:
     """Single blog post data container"""
 
     title: str
     date: datetime
     path: Optional[str]
     content: Optional[str]
-    tags: Optional[List[str]]
-    categories: Optional[List[str]]
+    tags: Optional[list[str]]
+    categories: Optional[list[str]]
     slug: Optional[str] = None
     teaser: str = ""
     is_teaser: bool = False
 
     @property
     def as_dict(self) -> dict:
         return asdict(self)
@@ -82,31 +80,32 @@
     plugin_config: BlogPluginConfig = field(init=False)
     meta_config: Optional[MetaPluginConfig] = field(init=False, default=None)
     translation: Translation = field(init=False)
     temp_dir: Path = field(init=False)
     docs_dir: Path = field(init=False)
     blog_dir: Path = field(init=False)
     site_dir: Path = field(init=False)
-    blog_posts: Dict[datetime, BlogPost] = field(init=False, default_factory=lambda: dict())
-    temp_files: Dict[str, Path] = field(init=False, default_factory=lambda: dict())
+    blog_posts: dict[datetime, BlogPost] = field(init=False, default_factory=lambda: dict())
+    temp_files: dict[str, Path] = field(init=False, default_factory=lambda: dict())
 
     @property
-    def temp_files_list(self) -> List[str]:
+    def temp_files_list(self) -> list[str]:
         temp_files = []
         for path in self.temp_files.values():
             temp_files.append(str(path.relative_to(self.temp_dir)))
         return temp_files
 
     def parse_configs(self, mkdocs_config: MkDocsConfig, plugin_config: BlogPluginConfig):
         from mkdocs_publisher.blog.translate import Translate
 
         self.mkdocs_config = mkdocs_config
         self.plugin_config = plugin_config
-        self.meta_config: Optional[MetaPluginConfig] = mkdocs_utils.get_plugin_config(
-            mkdocs_config=mkdocs_config, plugin_name="pub-meta"
+        self.meta_config: Optional[MetaPluginConfig] = (
+            mkdocs_utils.get_plugin_config(mkdocs_config=mkdocs_config, plugin_name="pub-meta")
+            or None
         )  # type: ignore
         self.temp_dir = Path(plugin_config.temp_dir)
         self.docs_dir = Path(mkdocs_config.docs_dir)
         self.blog_dir = Path(plugin_config.blog_dir)
         self.site_dir = Path(mkdocs_config.site_dir)
         self.translation = Translate(config=plugin_config).translation
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/debugger/config.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -29,14 +29,15 @@
 class _DebuggerConsoleConfig(Config):
     enabled = option.Type(bool, default=True)
     # noinspection PyUnresolvedReferences,PyProtectedMember
     log_level = option.Choice(choices=logging._nameToLevel.keys(), default="INFO")
     show_code_link = option.Type(bool, default=False)
     show_logger_name = option.Type(bool, default=True)
     show_entry_time = option.Type(bool, default=True)
+    show_deprecation_warnings = option.Type(bool, default=False)
     entry_time_format = option.Type(str, default="%H:%M:%S.%f")
     filter_logger_names = option.Type(list, default=[])
 
 
 class _DebuggerFileConfig(Config):
     enabled = option.Type(bool, default=True)
     # noinspection PyUnresolvedReferences,PyProtectedMember
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/debugger/loggers.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/loggers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,25 +17,28 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
+import re
 import site
 from datetime import datetime
 from pathlib import Path
 
 import colorama
 
 from mkdocs_publisher.debugger.config import _DebuggerConsoleConfig
 from mkdocs_publisher.debugger.config import _DebuggerFileConfig
 
 colorama.init()
 
+LIVERELOAD_MSG_RE = re.compile(r"(?P<time>\[\d{,2}:\d{1,2}:\d{,2}] )?(?P<text>.*)")
+DEPRECATION_MSG_RE = re.compile(r"^(?P<deprecation>DeprecationWarning:)")
 SITE_PACKAGES_DIR = Path(site.getsitepackages()[0])
 LOG_LEVEL_COLOR_MAPPING = {
     logging.DEBUG: colorama.Fore.BLUE,
     logging.INFO: colorama.Fore.GREEN,
     logging.WARNING: colorama.Fore.YELLOW,
     logging.ERROR: colorama.Fore.RED,
     logging.CRITICAL: colorama.Fore.RED,
@@ -51,14 +54,18 @@
 
 class ProjectPathStreamFormatter(logging.Formatter):
     def __init__(self, console_config: _DebuggerConsoleConfig):
         self._console_config: _DebuggerConsoleConfig = console_config
 
         super().__init__()
 
+    @staticmethod
+    def _livereload_msg_strip_time(match: re.Match) -> str:
+        return match.groupdict()["text"]
+
     def format(self, record: logging.LogRecord) -> str:
         path = Path(record.pathname)
         try:
             record.project_path = str(path.relative_to(path.cwd()))
         except ValueError:
             record.project_path = str(path)
 
@@ -76,14 +83,17 @@
             fmt = f"{fmt} {colorama.Fore.CYAN}[%(name)s]{colorama.Fore.RESET}"
 
         self._style._fmt = fmt
         self.datefmt = str(self._console_config.entry_time_format).replace(
             "%f", str(record.msecs)[0:3]
         )
 
+        if self._console_config.show_entry_time:
+            record.msg = re.sub(LIVERELOAD_MSG_RE, self._livereload_msg_strip_time, record.msg)
+
         return super().format(record=record)
 
 
 class ProjectPathFileFormatter(logging.Formatter):
     def format(self, record: logging.LogRecord) -> str:
         project_file_path = Path(record.pathname)
         try:
@@ -92,23 +102,28 @@
                     SITE_PACKAGES_DIR
                     if "site-packages" in str(project_file_path)
                     else project_file_path.cwd()
                 )
             )
         except ValueError:
             record.project_path = str(project_file_path)
+
         return super().format(record=record)
 
 
 class ProjectPathConsoleFilter(logging.Filter):
     def __init__(self, console_config: _DebuggerConsoleConfig):
         self._console_config: _DebuggerConsoleConfig = console_config
         super().__init__()
 
     def filter(self, record):
+        if not self._console_config.show_deprecation_warnings and re.findall(
+            DEPRECATION_MSG_RE, record.msg
+        ):
+            return None
         return record if record.name not in self._console_config.filter_logger_names else None
 
 
 class ProjectPathFileFilter(logging.Filter):
     def __init__(self, file_config: _DebuggerFileConfig):
         self._file_config: _DebuggerFileConfig = file_config
         super().__init__()
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/debugger/plugin.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/debugger/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,14 +21,15 @@
 # SOFTWARE.
 
 import logging
 import platform
 import sys
 from io import BytesIO
 from pathlib import Path
+from typing import cast
 from zipfile import ZIP_DEFLATED
 from zipfile import ZipFile
 
 from mkdocs.plugins import BasePlugin
 from mkdocs.plugins import event_priority
 
 # noinspection PyProtectedMember
@@ -60,16 +61,19 @@
             filename=f"%Y%m%d_%H%M%S{LOG_FILENAME_SUFFIX}"
         )
 
         self._mkdocs_log_file: str = str(Path(self._mkdocs_log_file_handler.baseFilename).name)
         self._mkdocs_log_date: str = self._mkdocs_log_file.replace(LOG_FILENAME_SUFFIX, "")
 
         self.load_config(
-            options=mkdocs_utils.get_plugin_config(
-                mkdocs_config=mkdocs_utils.get_mkdocs_config(), plugin_name="pub-debugger"
+            options=cast(
+                dict,
+                mkdocs_utils.get_plugin_config(
+                    mkdocs_config=mkdocs_utils.get_mkdocs_config(), plugin_name="pub-debugger"
+                ),
             ),
             config_file_path=mkdocs_utils.get_mkdocs_config().config_file_path,
         )
 
         if self.config.console_log.enabled:
             self._mkdocs_log_stream_handler.setFormatter(
                 loggers.ProjectPathStreamFormatter(console_config=self.config.console_log)
@@ -119,15 +123,14 @@
             if self.config.zip_log.remove_old_files:
                 for log_file in Path(".").rglob(f"*{ZIP_FILENAME_SUFFIX}"):
                     if str(log_file) != zip_file_name:
                         log_file.unlink(missing_ok=True)
 
             archive = BytesIO()
             with ZipFile(archive, "a", ZIP_DEFLATED, False) as archive_file:
-
                 # Zip files from list
                 for file_to_zip in FILES_TO_ZIP_LIST:
                     if Path(file_to_zip).exists():
                         log.debug(f"File: {file_to_zip} added to archive")
                         archive_file.write(filename=file_to_zip, arcname=file_to_zip)
                     else:
                         log.debug(f"File: {file_to_zip} doesn't exists and not added to archive")
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/meta/config.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/social/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -20,37 +20,28 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from mkdocs.config import config_options as option
 from mkdocs.config.base import Config
 
 
-class _MetaSlugConfig(Config):
+class _SocialOpenGraphConfig(Config):
     enabled = option.Type(bool, default=True)
-    warn_on_missing = option.Type(bool, default=True)
-    key_name = option.Type(str, default="slug")
+    locale = option.Type(str, default="en_US")
 
 
-class _MetaPublishConfig(Config):
-    search_in_hidden = option.Type(bool, default=False)
-    search_in_draft = option.Type(bool, default=False)
-    file_default = option.Choice(
-        choices=["draft", "hidden", "published", True, False], default=False
-    )
-    file_warn_on_missing = option.Type(bool, default=True)
-    dir_default = option.Choice(
-        choices=["draft", "hidden", "published", True, False], default=True
-    )
-    dir_warn_on_missing = option.Type(bool, default=False)
-    key_name = option.Type(str, default="publish")
-
-
-class _MetaTitleConfig(Config):
-    key_name = option.Type(str, default="title")
-
-
-class MetaPluginConfig(Config):
-    dir_meta_file = option.Type(str, default="README.md")
-
-    slug: _MetaSlugConfig = option.SubConfig(_MetaSlugConfig)  # type: ignore
-    publish: _MetaPublishConfig = option.SubConfig(_MetaPublishConfig)  # type: ignore
-    title: _MetaTitleConfig = option.SubConfig(_MetaTitleConfig)  # type: ignore
+class _SocialTwitterConfig(Config):
+    enabled = option.Type(bool, default=True)
+    website = option.Type(str, default="")
+    author = option.Type(str, default="")
+
+
+class _SocialMetaKeysConfig(Config):
+    title_key = option.Type(str, default="title")
+    description_key = option.Type(str, default="description")
+    image_key = option.Type(str, default="image")
+
+
+class SocialConfig(Config):
+    twitter: _SocialTwitterConfig = option.SubConfig(_SocialTwitterConfig)  # type: ignore
+    og: _SocialOpenGraphConfig = option.SubConfig(_SocialOpenGraphConfig)  # type: ignore
+    meta_keys: _SocialMetaKeysConfig = option.SubConfig(_SocialMetaKeysConfig)  # type: ignore
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/meta/plugin.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/meta/meta_files.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -17,357 +17,343 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
-from datetime import datetime
+import re
+from collections import UserDict
+from collections.abc import Generator
+from dataclasses import dataclass
+from dataclasses import field
 from pathlib import Path
-from typing import Literal
+from typing import Any
 from typing import Optional
-from typing import cast
 from urllib.parse import quote
 
-from mkdocs.config import Config
 from mkdocs.config.defaults import MkDocsConfig
-from mkdocs.plugins import BasePlugin
-from mkdocs.plugins import event_priority
+from mkdocs.structure.files import File
 from mkdocs.structure.files import Files
-from mkdocs.structure.nav import Link
-from mkdocs.structure.nav import Navigation
-from mkdocs.structure.nav import Section
-from mkdocs.structure.pages import Page
 from mkdocs.utils import meta as meta_parser
 
 # noinspection PyProtectedMember
-from mkdocs_publisher._shared import mkdocs_utils
-from mkdocs_publisher.blog.config import BlogPluginConfig
+from mkdocs_publisher._shared.urls import create_slug
 from mkdocs_publisher.meta.config import MetaPluginConfig
-from mkdocs_publisher.meta.config import _MetaPublishConfig
-from mkdocs_publisher.obsidian.config import ObsidianPluginConfig
+from mkdocs_publisher.meta.config import OverviewChoiceEnum
+from mkdocs_publisher.meta.config import PublishChoiceEnum
+from mkdocs_publisher.meta.config import TitleChoiceEnum
 
-log = logging.getLogger("mkdocs.plugins.publisher.meta.plugin")
-INDEX_FILE_NAME = "index.md"
+log = logging.getLogger("mkdocs.plugins.publisher._shared.meta_files")
 
 
-class MetaPlugin(BasePlugin[MetaPluginConfig]):
-    def __init__(self):
-        """
-        TODO: SEO optimizations
-        Useful links for sitemap.xml manipulation etc.:
-        - https://octamedia.pl/blog/mapa-strony-xml/
-        - https://octamedia.pl/blog/linkowanie-wewnetrzne/ (useful for obsidian backlinks)
-        """
-        self._blog_config: Optional[BlogPluginConfig] = None
-        self._dirs_slugs: dict = {}
-        self._dirs_titles: dict = {}
-        self._draft_dirs: list = []
-        self._hidden_dirs: list = []
-        self._draft_files: list = []
-        self._hidden_files: list = []
-        self._not_other_files: list = []
-        self._on_serve = False
-
-    def _build_config_nav(self, directory: Path, relative_to: Path) -> list:
-        nav = list()
-        sorted_files = sorted([f for f in directory.glob("*")])
-
-        # Make index.md a first file in given directory
-        other_files = [f for f in sorted_files if f.name not in self._not_other_files]
-        sorted_files = [f for f in sorted_files if f.name == "index.md"]
-        sorted_files.extend(other_files)
-
-        for file in sorted_files:
-            if not any([d for d in self._draft_dirs if file.is_relative_to(d)]):
-                if file.is_dir():
-                    title = self._dirs_titles.get(file, file.stem)
-                    dir_nav = self._build_config_nav(directory=file, relative_to=relative_to)
-                    if isinstance(dir_nav, list) and len(dir_nav) > 0:  # Skip empty directories
-                        nav.append({title: dir_nav})
-                elif file.is_file() and file.suffix == ".md":
-                    with file.open(encoding="utf-8-sig", errors="strict") as md_file:
-                        markdown, meta = meta_parser.get_data(md_file.read())
-                        title = meta.get(self.config.title.key_name, file.stem)
-
-                        # Read document publication status
-                        publish = meta.get(self.config.publish.key_name)
-                        if publish is None:
-                            log_message = (
-                                f'Missing "{self.config.publish.key_name}" value in '
-                                f'file "{file.relative_to(relative_to)}". Setting to '
-                                f'default value: "{self.config.publish.file_default}".'
-                            )
-                            if self.config.publish.file_warn_on_missing:
-                                log.warning(log_message)
-                            else:
-                                log.debug(log_message)
-                            publish = self.config.publish.file_default
-
-                        # TODO: make it configurable
-                        if publish in ["draft", "false", False] and self._on_serve:
-                            publish = "published"
-
-                        # Add file to variables used in nav cleanup based on publication status
-                        if publish in ["draft", "false", False]:
-                            self._draft_files.append(str(file.relative_to(relative_to)))
-                        elif publish == "hidden":
-                            self._hidden_files.append(str(file.relative_to(relative_to)))
-
-                        # Add not draft file to navigation (hidden will be removed in nav cleanup)
-                        if publish not in ["draft", "false", False]:
-                            nav.append({title: str(file.relative_to(relative_to))})
-            elif (
-                file.is_dir()
-                and self._blog_config is not None
-                and str(file.relative_to(relative_to)) == self._blog_config.blog_dir
-            ):
-                nav.append({file.stem: str(file.relative_to(relative_to))})
-        return nav
+HEADINGS_RE = re.compile(r"^#+ (?P<title>[^|#\r\n\t\f\v]+)$")
+
+
+@dataclass
+class MetaFile:
+    path: Path
+    abs_path: Path
+    is_dir: bool
+    is_overview: bool = field(default=False)
+    is_hidden: bool = field(default=False)
+    is_draft: Optional[bool] = field(default=None)
+    title: Optional[str] = field(default=None)
+    slug: Optional[str] = field(default=None)
+    file: Optional[File] = field(default=None)
 
-    def _nav_cleanup(self, items: list, elements_to_remove: list) -> list:
+    @property
+    def name(self) -> str:
+        return self.path.name
 
-        nav = []
-        for item in items:
-            if isinstance(item, Page) and Path(item.file.abs_src_path) not in elements_to_remove:
-                nav.append(item)
-            elif isinstance(item, Link):
-                nav.append(item)
-            elif isinstance(item, Section):
-                item.children = self._nav_cleanup(
-                    items=item.children, elements_to_remove=elements_to_remove
+    @property
+    def parent(self) -> Optional[Path]:
+        parent = self.path.parent
+        if str(parent) == ".":
+            parent = None
+        return parent
+
+
+class MetaFiles(UserDict):
+    def __init__(self):
+        self._on_serve: bool = False
+        self._mkdocs_config: Optional[MkDocsConfig] = None
+        self._meta_plugin_config: Optional[MetaPluginConfig] = None
+        self._hidden_paths: list[Path] = []
+        super().__init__()
+
+    @property
+    def meta_file(self) -> str:
+        return self._meta_plugin_config.dir_meta_file
+
+    @property
+    def on_serve(self) -> bool:
+        return self._on_serve
+
+    @on_serve.setter
+    def on_serve(self, on_serve: bool):
+        self._on_serve = on_serve
+
+    def add_hidden_path(self, hidden_path: Optional[Path]):
+        if hidden_path is not None:
+            self._hidden_paths.append(hidden_path.relative_to(self._mkdocs_config.docs_dir))
+
+    def set_configs(self, mkdocs_config: MkDocsConfig, meta_plugin_config: MetaPluginConfig):
+        self._mkdocs_config = mkdocs_config
+        self._meta_plugin_config = meta_plugin_config
+
+    @staticmethod
+    def _read_md_file(meta_file_path: Path) -> tuple[str, dict[str, Any]]:  # pragma: no cover
+        with meta_file_path.open(encoding="utf-8-sig", errors="strict") as md_file:
+            # Add empty line at the end of file and read all data
+            return meta_parser.get_data(f"{md_file.read()}\n")
+
+    def _get_title(self, meta_file: MetaFile, meta: dict[str, Any], markdown: str):
+        title: Optional[str] = None
+        mode = self._meta_plugin_config.title.mode
+
+        if mode == TitleChoiceEnum.META:
+            title = meta.get(self._meta_plugin_config.title.key_name)
+            if title is None and self._meta_plugin_config.title.warn_on_missing_meta:
+                log.warning(
+                    f'Title value from "{self._meta_plugin_config.title.key_name}" meta data '
+                    f'is missing for file: "{str(meta_file.path)}"'
                 )
-                if len(item.children) > 0:  # Skip empty Sections
-                    nav.append(item)
 
-        return nav
+        if title is None and (mode == TitleChoiceEnum.META or mode == TitleChoiceEnum.HEAD):
+            headings = re.findall(HEADINGS_RE, markdown)
+            title = str(headings[0]).strip() if len(headings) > 0 else None
+            if title is None and self._meta_plugin_config.title.warn_on_missing_header:
+                log.warning(
+                    f'Title value from first heading is missing for file: "{str(meta_file.path)}"'
+                )
 
-    def on_startup(self, *, command: Literal["build", "gh-deploy", "serve"], dirty: bool) -> None:
-        if command == "serve":
-            self._on_serve = True
-
-    @event_priority(100)  # Run before any other plugins
-    def on_config(self, config: MkDocsConfig) -> Optional[Config]:
-
-        # Setup some default values
-        self._not_other_files = [INDEX_FILE_NAME, self.config.dir_meta_file]
-
-        log.info(f'Reading meta data from "{self.config.dir_meta_file}" files')
-        for meta_file in Path(config.docs_dir).glob(f"**/{self.config.dir_meta_file}"):
-            with meta_file.open(encoding="utf-8-sig", errors="strict") as md_file:
-
-                # Add empty line at the end of file and read all data
-                markdown, meta = meta_parser.get_data(f"{md_file.read()}\n")
-
-                # Read slug for directories
-                slug = meta.get(self.config.slug.key_name)
-                if slug is not None:
-                    self._dirs_slugs[meta_file.parent] = slug
-
-                # Read title for directory
-                title = meta.get(self.config.title.key_name)
-                if title is not None:
-                    self._dirs_titles[meta_file.parent] = title
-
-                # Read directories publication status
-                publish = meta.get(str(self.config.publish.key_name))
-                if publish is None:
-                    if self.config.publish.dir_warn_on_missing:
-                        log.warning(
-                            f'Missing "{self.config.publish.key_name}" value in '
-                            f'file "{meta_file.relative_to(config.docs_dir)}". Setting to '
-                            f'default value: "{self.config.publish.dir_default}".'
-                        )
-                    publish = self.config.publish.dir_default
-                dir_path = str(meta_file.parent.relative_to(config.docs_dir))
+        if title is None and (mode == TitleChoiceEnum.META or mode == TitleChoiceEnum.FILE):
+            title = str(meta_file.path.stem).replace("_", " ").title()
 
-                if publish in ["draft", "false", False] and self._on_serve:
-                    publish = "published"
+        meta_file.title = title
 
-                if publish in ["draft", "false", False]:
-                    self._draft_dirs.append(dir_path)
-                elif publish == "hidden":
-                    self._hidden_dirs.append(dir_path)
-                elif publish not in _MetaPublishConfig.dir_default.choices:  # type: ignore
+    def _get_slug(self, meta_file: MetaFile, meta: dict[str, Any]):
+        meta_file.slug = create_slug(  # pragma: no cover
+            file_name=meta_file.path.stem,
+            slug_mode=self._meta_plugin_config.slug.mode,
+            slug=meta.get(self._meta_plugin_config.slug.key_name),
+            title=meta_file.title,
+            warn_on_missing=self._meta_plugin_config.slug.warn_on_missing,
+        )
+
+    def _get_overview(self, meta_file: MetaFile, meta: dict[str, Any], markdown: str):
+        """Overview works only for metafiles ("README.md", "index.md") that are detected as dir"""
+        if not meta_file.is_dir:
+            meta_file.is_overview = False
+        else:
+            is_overview = meta.get(
+                self._meta_plugin_config.overview.key_name,
+                self._meta_plugin_config.overview.default,
+            )
+            if is_overview == OverviewChoiceEnum.AUTO:
+                meta_file.is_overview = bool(len(markdown.strip()))
+            else:
+                meta_file.is_overview = is_overview
+
+    def _get_publish_status(self, meta_file: MetaFile, meta: dict[str, Any]):
+        publish = meta.get(str(self._meta_plugin_config.publish.key_name), None)
+
+        # Get default values if publish status is not specified
+        if publish is None:
+            if meta_file.is_dir:
+                publish = self._meta_plugin_config.publish.dir_default
+                if self._meta_plugin_config.publish.dir_warn_on_missing:
                     log.warning(
-                        f'Wrong key "{self.config.publish.key_name}" value '
-                        f'in file "{meta_file.relative_to(config.docs_dir)}" (only '
-                        f"{_MetaPublishConfig.dir_default.choices} are possible)"  # type: ignore
+                        f'Missing "{self._meta_plugin_config.publish.key_name}" value in '
+                        f'file "{meta_file.path}". Setting to '
+                        f'default value: "{self._meta_plugin_config.publish.dir_default}".'
+                    )
+            else:
+                publish = self._meta_plugin_config.publish.file_default
+                if self._meta_plugin_config.publish.file_warn_on_missing:
+                    log.warning(
+                        f'Missing "{self._meta_plugin_config.publish.key_name}" value in '
+                        f'file "{meta_file.path}". Setting to '
+                        f'default value: "{self._meta_plugin_config.publish.file_default}".'
                     )
 
-                log.debug(
-                    f"Title: {title}, publish: {publish}, "
-                    f"slug: {slug} "
-                    f'(directory: "{dir_path}")'
+        # Override some values inherited from parent
+        if meta_file.parent is not None:
+            meta_file_parent: MetaFile = self[str(meta_file.parent)]
+
+            if meta_file_parent.is_draft:
+                publish = False
+            if meta_file_parent.is_hidden:
+                publish = PublishChoiceEnum.HIDDEN
+
+        # When live preview is running, all pages are visible
+        if self._on_serve:
+            publish = True
+
+        if publish not in PublishChoiceEnum.choices():
+            publish = self._meta_plugin_config.publish.file_default
+            log.warning(
+                f'Wrong key "{self._meta_plugin_config.publish.key_name}" value '
+                f'({publish}) in file "{meta_file.path}" (only '
+                f"{PublishChoiceEnum.choices()} are possible)"
+            )
+
+        # Set values depends on publish status
+        if meta_file.path in self._hidden_paths or publish == PublishChoiceEnum.HIDDEN:
+            meta_file.is_hidden = True
+            meta_file.is_draft = False
+        elif publish in PublishChoiceEnum.drafts():
+            meta_file.is_hidden = False
+            meta_file.is_draft = True
+        elif publish in PublishChoiceEnum.published():
+            meta_file.is_hidden = False
+            meta_file.is_draft = False
+
+    def _get_metadata(self, meta_file: MetaFile, meta_file_path: Path):  # pragma: no cover
+        """Read all metadata values for given file"""
+        # Order of method execution is crucial for reading all values.
+        markdown, meta = self._read_md_file(meta_file_path=meta_file_path)
+
+        self._get_title(meta_file=meta_file, meta=meta, markdown=markdown)
+        self._get_slug(meta_file=meta_file, meta=meta)
+        if self._meta_plugin_config.overview.enabled:
+            self._get_overview(meta_file=meta_file, meta=meta, markdown=markdown)
+        self._get_publish_status(meta_file=meta_file, meta=meta)
+
+        log.debug(meta_file)
+
+    def __setitem__(self, path: str, meta_file: MetaFile):
+        if meta_file.is_dir:
+            meta_file_exists = False
+
+            # Calculate properties based on meta file metadata
+            meta_file_path = meta_file.abs_path.joinpath(self._meta_plugin_config.dir_meta_file)
+            if meta_file_path.exists():
+                meta_file_exists = True
+                self._get_metadata(meta_file=meta_file, meta_file_path=meta_file_path)
+
+            if not meta_file_exists:
+                meta_file.title = str(meta_file.path.stem)
+                meta_file.slug = create_slug(
+                    file_name=str(meta_file.name),
+                    slug_mode=self._meta_plugin_config.slug.mode,
+                    slug=meta_file.path.stem,
+                    title=meta_file.title,
+                    warn_on_missing=self._meta_plugin_config.slug.warn_on_missing,
                 )
+                meta_file.is_draft = not self._meta_plugin_config.publish.dir_default
+        else:
+            self._get_metadata(meta_file=meta_file, meta_file_path=meta_file.abs_path)
+
+        super().__setitem__(path, meta_file)
+
+    def drafts(self, files: bool = False, dirs: bool = False) -> dict[str, MetaFile]:
+        draft_files = {}
+        for path, meta_file in self.items():
+            if meta_file.is_draft and (
+                (files and not dirs and not meta_file.is_dir)
+                or (not files and dirs and meta_file.is_dir)
+                or (not files and not dirs)
+            ):
+                draft_files[path] = meta_file
+        return draft_files
 
-        # Add blog dir to one that will be skipped (blog has its own file resolution order)
-        self._blog_config: Optional[BlogPluginConfig] = mkdocs_utils.get_plugin_config(
-            mkdocs_config=config,
-            plugin_name="pub-blog",
-        )  # type: ignore
-        if self._blog_config is not None:
-            blog_dir = cast(BlogPluginConfig, self._blog_config).blog_dir
-            # TODO: cleanup mess with short directory names in self._draft_dirs
-            if (
-                blog_dir not in self._draft_dirs
-                and Path(config.docs_dir) / blog_dir not in self._draft_dirs
-            ):  # type: ignore
-                self._draft_dirs.append(blog_dir)
-
-        # Add obsidian dirs to ones that will be skipped
-        obsidian_config: Optional[ObsidianPluginConfig] = mkdocs_utils.get_plugin_config(
-            mkdocs_config=config,
-            plugin_name="pub-obsidian",
-        )  # type: ignore
-        if obsidian_config is not None:
-            # TODO: cleanup mess with short directory names in self._draft_dirs
-            if (
-                obsidian_config.obsidian_dir != ""
-                and obsidian_config.obsidian_dir not in self._draft_dirs
-                and Path(config.docs_dir) / obsidian_config.obsidian_dir not in self._draft_dirs
+    def hidden(self, files: bool = False, dirs: bool = False) -> dict[str, MetaFile]:
+        hidden_files = {}
+        for path, meta_file in self.items():
+            if meta_file.is_hidden and (
+                (files and not dirs and not meta_file.is_dir)
+                or (not files and dirs and meta_file.is_dir)
+                or (not files and not dirs)
             ):
-                self._draft_dirs.append(obsidian_config.obsidian_dir)
-            if (
-                obsidian_config.templates_dir != ""
-                and obsidian_config.templates_dir not in self._draft_dirs
-                and Path(config.docs_dir) / obsidian_config.templates_dir not in self._draft_dirs
+                hidden_files[path] = meta_file
+        return hidden_files
+
+    def add_meta_files(self, ignored_dirs: list[Path]):
+        """Iterate over all files and directories in docs directory"""
+        for docs_file in sorted(Path(self._mkdocs_config.docs_dir).rglob("*")):
+            meta_link: Optional[MetaFile] = None
+            is_ignored = any(
+                [docs_file.is_relative_to(ignored_dir) for ignored_dir in ignored_dirs]
+            )
+
+            if not is_ignored and docs_file.is_dir():
+                meta_link = MetaFile(
+                    path=docs_file.relative_to(self._mkdocs_config.docs_dir),
+                    abs_path=docs_file,
+                    is_dir=True,
+                )
+            elif (
+                not is_ignored
+                and docs_file.suffix == ".md"
+                and docs_file.name != self._meta_plugin_config.dir_meta_file
             ):
-                self._draft_dirs.append(obsidian_config.templates_dir)
-        self._draft_dirs = [Path(config.docs_dir) / d for d in self._draft_dirs]
-        self._hidden_dirs = [Path(config.docs_dir) / f for f in self._hidden_dirs]
-        for draft_dir in self._draft_dirs:
-            if not draft_dir.exists():
-                log.warning(
-                    f'Directory "{draft_dir.relative_to(config.docs_dir)}" doesn\'t exists'
+                meta_link = MetaFile(
+                    path=docs_file.relative_to(self._mkdocs_config.docs_dir),
+                    abs_path=docs_file,
+                    is_dir=False,
                 )
-        config.nav = self._build_config_nav(
-            directory=Path(config.docs_dir), relative_to=Path(config.docs_dir)
-        )
-        log.info(
-            f"Draft directories: "
-            f"{[str(d.relative_to(config.docs_dir)) for d in self._draft_dirs]}"
-        )
-        log.info(
-            f"Hidden directories: "
-            f"{[str(d.relative_to(config.docs_dir)) for d in self._hidden_dirs]}"
-        )
-        draft_files_list = [
-            str(f.relative_to(config.docs_dir)) if isinstance(f, Path) else f
-            for f in self._draft_files
-        ]
-        log.info(f"Draft files: {draft_files_list}")
-        hidden_files_list = [
-            str(f.relative_to(config.docs_dir)) if isinstance(f, Path) else f
-            for f in self._hidden_files
-        ]
-        log.info(f"Hidden files: {hidden_files_list}")
-
-        return config
-
-    @event_priority(-100)
-    def on_files(self, files: Files, *, config: MkDocsConfig) -> Optional[Files]:
-
-        relative_draft_dirs = [str(f.relative_to(config.docs_dir)) for f in self._draft_dirs]
-        if self._blog_config is not None:
-            relative_draft_dirs.remove(self._blog_config.blog_dir)
+
+            if meta_link is not None:
+                self[str(meta_link.path)] = meta_link
+
+    def change_files_slug(self, files: Files, ignored_dirs: list[Path]) -> Files:
+        draft_files = self.drafts(files=True).keys()
+        hidden_files = self.hidden(files=True)
+
+        ignored_dirs.extend([d.abs_path for d in self.drafts(dirs=True).values()])
 
         new_files = Files(files=[])
         for file in files:
-
-            file_path = Path(file.abs_src_path)
-            if file_path.suffix == ".md":
-                if (
-                    any([d for d in self._draft_dirs if file_path.is_relative_to(d)])
-                    and Path(file_path) not in self._draft_files
-                ):
-                    self._draft_files.append(file_path)
-                elif (
-                    any([d for d in self._hidden_dirs if file_path.is_relative_to(d)])
-                    and Path(file_path) not in self._hidden_files
-                ):
-                    self._hidden_files.append(file_path)
+            file: File
+            file_path: Path = Path(file.src_path)
 
             if (
-                not any([file.src_uri.startswith(draft_dir) for draft_dir in relative_draft_dirs])
-                and str(Path(file.src_uri).name) != self.config.dir_meta_file
-                and str(file.src_uri) not in self._draft_files
+                not any([Path(file.abs_src_path).is_relative_to(d) for d in ignored_dirs])
+                and file.src_path not in draft_files
+                and file.src_path not in hidden_files
+                and str(file_path.name) != self._meta_plugin_config.dir_meta_file
+            ) or (
+                str(file_path.name) == self._meta_plugin_config.dir_meta_file
+                and str(file_path.parent) in self
+                and self[str(file_path.parent)].is_overview
             ):
-                new_files.append(file)
-
-                if file.is_documentation_page():
-
-                    meta_file = Path(file.abs_src_path)
-                    with meta_file.open(encoding="utf-8-sig", errors="strict") as md_file:
-                        markdown, meta = meta_parser.get_data(md_file.read())
-
-                        # Read slug
-                        slug = meta.get(self.config.slug.key_name)
-                        # TODO: add slugify and config
-                        if slug is None and self.config.slug.warn_on_missing:
-                            log.warning(
-                                f'File "{file.src_path}" has no '
-                                f'"{self.config.slug.key_name}" meta data'
-                            )
-
-                        # Get URL parts
-                        if file.url.endswith("/"):
-                            file.url = file.url[0:-1]
-                        url_parts = file.url.split("/")
-
-                        # Get abs file parts
-                        path_parts: list[Path] = []
-                        for path_part in file.src_path.split("/"):
-                            if not path_parts:
-                                path_parts.append(Path(config.docs_dir) / path_part)
-                            else:
-                                path_parts.append(path_parts[-1] / path_part)
-
-                        # Replace URL parts that have slug defined
-                        for position, path_part in enumerate(path_parts):
-                            if path_part in self._dirs_slugs:
-                                url_parts[position] = self._dirs_slugs[path_part]
-
-                        # Replace last URL part with current file slug if exists
-                        if slug is not None and self.config.slug.enabled:
-                            url_parts[-1] = slug
-
-                        # Recreate file params based on URL with replaced parts
-                        if file.url != ".":  # Do not modify main index page
-                            file.url = quote(f"{'/'.join(url_parts)}/")
-                            url_parts.append(file.dest_uri.split("/")[-1])
-                            file.dest_uri = quote("/".join(url_parts))
-                            file.abs_dest_path = str(Path(config.site_dir) / file.dest_uri)
+                if self._meta_plugin_config.slug.enabled:
+                    # Get URL parts
+                    if file.url.endswith("/"):
+                        file.url = file.url[0:-1]
+                    url_parts = file.url.split("/")
+
+                    # Get abs file parts
+                    path_parts: list[Path] = []
+                    for path_part in file_path.parts:
+                        if not path_parts:
+                            path_parts.append(Path(path_part))
+                        else:
+                            path_parts.append(path_parts[-1] / path_part)
+
+                    # Replace URL parts that have slug defined
+                    for position, path_part in enumerate(path_parts):
+                        meta_file: Optional[MetaFile] = self.get(str(path_part), None)
+                        if meta_file is not None:
+                            url_parts[position] = meta_file.slug
+
+                    # Recreate file params based on URL with replaced parts
+                    if file.url != ".":  # Do not modify main index page
+                        file.url = quote(f"{'/'.join(url_parts)}/")
+                        url_parts.append(file.dest_uri.split("/")[-1])
+                        if len(url_parts) >= 2 and url_parts[-1] == url_parts[-2]:
+                            url_parts.pop(-1)
+                        file.dest_uri = quote("/".join(url_parts))
+                        file.abs_dest_path = str(
+                            Path(self._mkdocs_config.site_dir) / file.dest_uri
+                        )
 
+                new_files.append(file)
         return new_files
 
-    def on_nav(
-        self, nav: Navigation, *, config: MkDocsConfig, files: Files
-    ) -> Optional[Navigation]:
-
-        elements_to_remove = []
-        elements_to_remove.extend(self._draft_files)
-        elements_to_remove.extend(self._hidden_files)
-
-        nav.items = self._nav_cleanup(items=nav.items, elements_to_remove=elements_to_remove)
-
-        return nav
-
-    @event_priority(-100)  # Run after all other plugins
-    def on_page_markdown(self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files):
-
-        # Modify page update date
-        # TODO: move date format to config
-        # TODO: warn on missing in config
-        update_date: datetime = page.meta.get(
-            "update", page.meta.get("date", datetime.strptime(page.update_date, "%Y-%m-%d"))
-        )
-        try:
-            page.update_date = update_date.strftime("%Y-%m-%d")
-        except AttributeError:
-            # TODO: add format fallback
-            pass
-
-        if (
-            page.file.src_uri in self._hidden_files and not self.config.publish.search_in_hidden
-        ) or (page.file.src_uri in self._draft_files and not self.config.publish.search_in_draft):
-            page.meta["search"] = {"exclude": True}
+    def files_gen(self) -> Generator[MetaFile, Any, None]:
+        for meta_file in self.values():
+            meta_file: MetaFile
+            if not meta_file.is_draft and not meta_file.is_hidden:
+                yield meta_file
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/base.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -23,16 +23,14 @@
 import logging
 from dataclasses import asdict
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 from threading import Semaphore
 from threading import Thread
-from typing import Dict
-from typing import List
 from typing import Optional
 
 from mkdocs.config.defaults import MkDocsConfig
 
 # noinspection PyProtectedMember
 from mkdocs_publisher._shared import file_utils
 from mkdocs_publisher.minifier.config import MinifierConfig
@@ -68,22 +66,22 @@
 
 
 class BaseMinifier:
     def __init__(
         self,
         plugin_config: MinifierConfig,
         mkdocs_config: MkDocsConfig,
-        cached_files: Dict[str, CachedFile],
+        cached_files: dict[str, CachedFile],
     ):
         self._plugin_config: MinifierConfig = plugin_config
         self._mkdocs_config: MkDocsConfig = mkdocs_config
         self._minify_options: Optional[_MinifierCommonConfig] = None
-        self._cached_files: Dict[str, CachedFile] = cached_files
+        self._cached_files: dict[str, CachedFile] = cached_files
         self._cache_enabled: bool = self._plugin_config.cache_enabled
-        self._exclude: List = self._plugin_config.exclude[:]
+        self._exclude: list = self._plugin_config.exclude[:]
 
     def minifier(self, cached_file: CachedFile) -> Optional[CachedFile]:
         raise NotImplementedError
 
     def __call__(self):
         minifier_name = self.__class__.__name__.replace("Minifier", "").upper()
         self._cache_enabled = self._minify_options.cache_enabled if self._cache_enabled else False
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/config.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/minifiers.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/minifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/minifier/plugin.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/minifier/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,15 +19,14 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 from multiprocessing import cpu_count
 from pathlib import Path
-from typing import Dict
 from typing import Literal
 from typing import cast
 
 import yaml
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.plugins import event_priority
@@ -45,31 +44,30 @@
 
     def on_startup(self, *, command: Literal["build", "gh-deploy", "serve"], dirty: bool) -> None:
         if command == "serve":
             self._on_serve = True
 
     @event_priority(-100)  # Run after all other plugins
     def on_post_build(self, *, config: MkDocsConfig) -> None:
-
         Path(self.config.cache_dir).mkdir(exist_ok=True)
 
         # TODO: Add path to tools checker
-        cached_files: Dict[str, CachedFile] = {}
+        cached_files: dict[str, CachedFile] = {}
 
         if self.config.threads == 0:
             self.config.threads = int(cpu_count())
         if self.config.threads < 1:
             log.info('Number of "threads" cannot be smaller than 1 (changing to minimal 1)')
             self.config.threads = 1
         log.info(f"Threads used for minifiers: {self.config.threads}")
 
         cached_files_list: Path = Path(self.config.cache_dir) / self.config.cache_file
         if cached_files_list.exists():
             try:
-                with open(cached_files_list, "r") as yaml_file:
+                with open(cached_files_list) as yaml_file:
                     cached_files = yaml.safe_load(yaml_file)
                     for file_path, cached_file in cached_files.items():
                         cached_files[file_path] = CachedFile(**cast(dict, cached_file))
             except (yaml.YAMLError, AttributeError) as e:
                 log.warning(f"File '{cached_files_list}' corrupted. Rebuilding cache.")
                 log.debug(e)
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/backlinks.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/backlinks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,145 +19,113 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import logging
 import re
 from dataclasses import dataclass
-
-# from hashlib import md5
-from typing import Dict
-from typing import List
-from typing import Optional
 from typing import cast
 
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.structure.pages import Page
 
-from mkdocs_publisher._shared import links
-
 # noinspection PyProtectedMember
-from mkdocs_publisher._shared.urls import slugify
+from mkdocs_publisher._shared import links
 from mkdocs_publisher.blog.plugin import BlogPlugin
 
 log = logging.getLogger("mkdocs.plugins.publisher.obsidian.backlinks")
 
-HTTP_LINK_RE = re.compile(r"\[([^][\r\n]+)]\((https?://[^][)(\s]+)(#[\w\-.]+)?\)")
-
 
-@dataclass()
+@dataclass
 class Link:
     text: str
     destination: str
     title: str
     source: str
 
 
 class BacklinkLinks:
     def __init__(
         self,
         mkdocs_config: MkDocsConfig,
-        backlinks: Dict[str, List[Link]],
+        backlinks: dict[str, list[Link]],
     ):
         self._mkdocs_config: MkDocsConfig = mkdocs_config
-        self._backlinks: Dict[str, List[Link]] = backlinks
-
-    @staticmethod
-    def _build_anchor_link(backlink: str, anchor_link: Optional[str]) -> str:
-        """Create backlink anchor link"""
-
-        anchor_link = f"{backlink}{anchor_link}"
-        # log.warning(anchor_link)
-        for r in (("../", ""), (".md", ""), ("#", ""), ("/", ""), ("_", "-")):
-            anchor_link = anchor_link.replace(*r)
-        anchor_link = slugify(text=anchor_link)
-        # log.error(anchor_link)
-        return anchor_link
+        self._backlinks: dict[str, list[Link]] = backlinks
 
     @staticmethod
     def _other_link_to_text(match: re.Match) -> str:
         """Return only a text from a link (http or markdown)"""
-        return match.group(1)
+        return match.groupdict()["link"]
 
-    def _create_anchor_link(self, match: re.Match):
-        """Create a backlink with an additional anchor link"""
-        anchor_link = match.group(3) if match.group(3) is not None else ""
-        backlink = match.group(2)
-        backlink_anchor_link = self._build_anchor_link(backlink=backlink, anchor_link=anchor_link)
-        # TODO: create anchor link using slug from meta
-        link = f"[{match.group(1)}]({backlink}{anchor_link}){{#{backlink_anchor_link}}}"
-        # link_md5 = md5(f"[{match.group(1)}]({backlink}{anchor_link})".encode()).hexdigest()
-        # log.error(f"{link_md5} = {link}")
-        return link
+    @staticmethod
+    def _create_backlink(match: re.Match):
+        link = links.LinkMatch(**match.groupdict())
+        return link.as_backlink
 
     def _parse_markdown_link(self, match: re.Match, page: Page, line: str):
         """Parse markdown link"""
-        anchor_link = match.group(3) if match.group(3) is not None else ""
-        original_link_destination = match.group(2)
-        original_link_text = f"[{match.group(1)}]({original_link_destination}{anchor_link})"
-        anchor_link = self._build_anchor_link(
-            backlink=original_link_destination, anchor_link=anchor_link
-        )
-        backlink_link = f"{self._mkdocs_config.site_url}{page.url}#{anchor_link}"
+        original_link = links.LinkMatch(**match.groupdict())
+        backlink_link = f"{self._mkdocs_config.site_url}{page.url}{original_link.backlink_anchor}"
 
         # Convert document link into backlink
-        link_replacement = f'<a href="{backlink_link}">{match.group(1)}</a>'
-        backlink_text = line.replace(original_link_text, link_replacement)
+        link_replacement = f'<a href="{backlink_link}">{original_link.text}</a>'
+        backlink_text = line.replace(str(original_link), link_replacement)
 
         # Convert other links into text
         backlink_text = re.sub(links.MD_LINK_RE, self._other_link_to_text, backlink_text)
-        backlink_text = re.sub(HTTP_LINK_RE, self._other_link_to_text, backlink_text)
+        backlink_text = re.sub(links.HTTP_LINK_RE, self._other_link_to_text, backlink_text)
 
         # Create a backlink with context
         backlink_text = f'<p class="obsidian_backlink">{backlink_text}</p>'
 
         # Convert relative backlinks into absolute backlinks inside document directory
         original_link_source = page.file.src_uri
-        if len(original_link_destination.split("/")) == 1:
+        if len(original_link.link.split("/")) == 1:
             destination_pre = original_link_source.split("/")[:-1]
-            destination_pre.append(original_link_destination)
-            original_link_destination = "/".join(destination_pre)
-        original_link_destination = original_link_destination.replace("../", "")
+            destination_pre.append(str(original_link.link))
+            original_link.link = "/".join(destination_pre)
+        original_link.link = original_link.link.replace("../", "")
 
-        link = Link(
+        new_link = Link(
             text=backlink_text,
             destination=backlink_link,
-            source=original_link_destination,
+            source=original_link.link,
             title=str(page.title),
         )
 
         # Get blog temporary files
         temp_blog_files = []
         if "pub-blog" in self._mkdocs_config.plugins:
             blog_plugin: BlogPlugin = cast(BlogPlugin, self._mkdocs_config.plugins["pub-blog"])
             temp_blog_files = blog_plugin.blog_config.temp_files_list
 
         # Do not add backlink if backlinks points to the same document
         if (
-            original_link_source != original_link_destination
+            original_link_source != original_link.link
             and original_link_source not in temp_blog_files
         ):
             log.debug(
-                f"Found backlink to: {match.group(2)}"
-                f"{match.group(3) if match.group(3) is not None else ''}"
+                f"Found backlink to: {original_link.link}"
+                f"{original_link.anchor if original_link.anchor is not None else ''}"
             )
-            if original_link_destination not in self._backlinks:
-                self._backlinks[original_link_destination] = [link]
+            if original_link.link not in self._backlinks:
+                self._backlinks[original_link.link] = [new_link]
             else:
                 link_found = False
-                for existing_link in self._backlinks[original_link_destination]:
+                for existing_link in self._backlinks[original_link.link]:
                     # Add backlink to an existing one
-                    if existing_link.title == link.title:
+                    if existing_link.title == new_link.title:
                         link_found = True
-                        existing_link.text = f"{existing_link.text}<hr>{link.text}"
+                        existing_link.text = f"{existing_link.text}<hr>{new_link.text}"
                 if not link_found:
-                    self._backlinks[original_link_destination].append(link)
+                    self._backlinks[original_link.link].append(new_link)
 
     def find_markdown_links(self, markdown: str, page: Page):
         # """Find all markdown backlinks"""
         for line in markdown.split("\n"):
             for match in re.finditer(links.MD_LINK_RE, line):
                 self._parse_markdown_link(match=match, page=page, line=line)
 
-    def convert_to_anchor_link(self, markdown: str) -> str:
+    def convert_to_backlink(self, markdown: str) -> str:
         """Convert backlink to link with an anchor for direct navigation after clicking on it"""
-        return re.sub(links.MD_LINK_RE, self._create_anchor_link, markdown)
+        return re.sub(links.MD_LINK_RE, self._create_backlink, markdown)
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/callouts.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/callouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/config.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -46,15 +46,17 @@
 
 class _ObsidianLinksConfig(Config):
     wikilinks_enabled = option.Type(bool, default=True)
     img_lazy_loading = option.Type(bool, default=True)
 
 
 class ObsidianPluginConfig(Config):
+    # TODO: read those values from Obsidian config files
     obsidian_dir = option.Type(str, default=".obsidian")
     templates_dir = option.Type(str, default="_templates")
+    attachments_dir = option.Type(str, default="_attachments")
 
     backlinks: _ObsidianBacklinksConfig = option.SubConfig(_ObsidianBacklinksConfig)  # type: ignore
     callouts: _ObsidianCalloutsConfig = option.SubConfig(_ObsidianCalloutsConfig)  # type: ignore
     comments: _ObsidianCommentsConfig = option.SubConfig(_ObsidianCommentsConfig)  # type: ignore
     vega: _ObsidianVegaConfig = option.SubConfig(_ObsidianVegaConfig)  # type: ignore
     links: _ObsidianLinksConfig = option.SubConfig(_ObsidianLinksConfig)  # type: ignore
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/md_links.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/md_links.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -70,33 +70,43 @@
         md_embed_link_obj.is_loading_lazy = self._links_config.img_lazy_loading
         md_embed_link = str(md_embed_link_obj)
         log.debug(f"Normalizing md embed link: {match.group(0)} > {md_embed_link}")
         return md_embed_link
 
     @staticmethod
     def _normalize_md_links(match: re.Match) -> str:
-        md_link = str(links.LinkMatch(**match.groupdict()))
+        md_link_obj = links.LinkMatch(**match.groupdict())
+        md_link = str(md_link_obj)
         log.debug(f"Normalizing md link: {match.group(0)} > {md_link}")
         return md_link
 
+    @staticmethod
+    def _normalize_anchor_links(match: re.Match) -> str:
+        anchor_link_obj = links.LinkMatch(**match.groupdict())
+        anchor_link = str(anchor_link_obj)
+        log.debug(f"Normalizing anchor link: {match.group(0)} > {anchor_link}")
+        return anchor_link
+
     def normalize_links(self, markdown: str, current_file_path: str) -> str:
         self._current_file_path = current_file_path
         if self._links_config.wikilinks_enabled:
             markdown = re.sub(links.WIKI_LINK_RE, self._normalize_wiki_link, markdown)
             markdown = re.sub(links.WIKI_EMBED_LINK_RE, self._normalize_wiki_embed_link, markdown)
+            markdown = re.sub(links.ANCHOR_LINK_RE, self._normalize_anchor_links, markdown)
         markdown = re.sub(links.MD_EMBED_LINK_RE, self._normalize_md_embed_link, markdown)
         markdown = re.sub(links.MD_LINK_RE, self._normalize_md_links, markdown)
         return markdown
 
     def _normalize_relative_link(self, match: re.Match) -> str:
         md_link_obj = links.RelativeLinkMatch(**match.groupdict())
         md_link_obj.relative_path_finder = links.RelativePathFinder(
             current_file_path=Path(cast(str, self._current_file_path)),
             docs_dir=Path(self._mkdocs_config.docs_dir),
             relative_path=Path(cast(str, self._blog_config.blog_dir)),
         )
+        # log.warning(str(md_link_obj))
         return str(md_link_obj)
 
     def normalize_relative_links(self, markdown: str, current_file_path: str) -> str:
         self._current_file_path = current_file_path
         markdown = re.sub(links.RELATIVE_LINK_RE, self._normalize_relative_link, markdown)
         return markdown
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/plugin.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -21,16 +21,14 @@
 # SOFTWARE.
 
 import logging
 import re
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Callable
-from typing import Dict
-from typing import List
 from typing import Optional
 
 import jinja2
 import watchdog.events
 from mkdocs.config import Config
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.livereload import LiveReloadServer
@@ -66,43 +64,50 @@
     def __repr__(self):
         return f"<!--{self.comment}-->" if self.is_html_comment else ""
 
 
 class ObsidianPlugin(BasePlugin[ObsidianPluginConfig]):
     def __init__(self):
         self._backlink_links: Optional[BacklinkLinks] = None
-        self._backlinks: Dict[str, List[Link]] = {}
+        self._backlinks: dict[str, list[Link]] = {}
         self._md_links: Optional[MarkdownLinks] = None
-        self._vega_pages: List[Page] = list()
+        self._vega_pages: list[Page] = list()
 
     def _normalize_comments(self, match: re.Match) -> str:
         comment = Comment(**match.groupdict())
         comment.is_html_comment = self.config.comments.inject_as_html
         return str(comment)
 
     def on_config(self, config: MkDocsConfig) -> Optional[Config]:
         self._backlink_links = BacklinkLinks(mkdocs_config=config, backlinks=self._backlinks)
         self._md_links = MarkdownLinks(mkdocs_config=config)
         return config
 
+    def on_files(self, files: Files, *, config: MkDocsConfig) -> Optional[Files]:
+        if self.config.vega.enabled:
+            resources.add_extra_css(
+                stylesheet_file_name="obsidian.min.css",
+                config=config,
+                files=files,
+            )
+        return files
+
     def on_nav(
         self, nav: Navigation, *, config: MkDocsConfig, files: Files
     ) -> Optional[Navigation]:
-
         if self.config.backlinks.enabled:
             log.info("Parsing backlinks")
             for file in files:
                 if file.page is not None:
                     log.debug(f"Parsing backlinks in file '{file.src_path}'")
                     with open(file.abs_src_path, encoding="utf-8-sig", errors="strict") as md_file:
-                        markdown, meta = meta_parser.get_data(md_file.read())
+                        markdown, _ = meta_parser.get_data(md_file.read())
                         markdown = self._md_links.normalize_links(
                             markdown=markdown, current_file_path=str(file.src_uri)
                         )
-
                         self._backlink_links.find_markdown_links(markdown=markdown, page=file.page)
         return nav
 
     @event_priority(100)  # Run before all other plugins
     def on_page_markdown(
         self, markdown: str, *, page: Page, config: MkDocsConfig, files: Files
     ) -> Optional[str]:
@@ -124,15 +129,15 @@
             # TODO: add verification if all things are enabled in .obsidian config
             vega_charts = VegaCharts(vega_config=self.config.vega)
             markdown = vega_charts.generate_charts(markdown=markdown)
             if vega_charts.is_vega:
                 self._vega_pages.append(page)
 
         if self.config.backlinks.enabled:
-            markdown = self._backlink_links.convert_to_anchor_link(markdown=markdown)
+            markdown = self._backlink_links.convert_to_backlink(markdown=markdown)
             page_backlinks = self._backlinks.get(f"{page.file.src_uri}", None)
             if page_backlinks is not None:
                 log.debug(f"Adding backlinks to '{page.file.src_uri}'")
                 backlink_template = resources.read_template_file(
                     template_file_name="backlinks.html"
                 )
                 context = {
@@ -141,25 +146,15 @@
                 }
                 template = jinja2.Environment(loader=jinja2.BaseLoader()).from_string(
                     backlink_template
                 )
                 markdown = f"{markdown}{template.render(context)}"
         return markdown
 
-    def on_files(self, files: Files, *, config: MkDocsConfig) -> Optional[Files]:
-        if self.config.vega.enabled:
-            resources.add_extra_css(
-                stylesheet_file_name="obsidian.min.css",
-                config=config,
-                files=files,
-            )
-        return files
-
     def on_post_page(self, output: str, *, page: Page, config: MkDocsConfig) -> Optional[str]:
-
         if self.config.vega.enabled and page in self._vega_pages:
             # TODO: embed scripts to assets and give possibility to serve from site_dir
             html_modifier = HTMLModifier(markup=output)
             html_modifier.add_head_script(src="https://cdn.jsdelivr.net/npm/vega@5.22.1")
             html_modifier.add_head_script(src="https://cdn.jsdelivr.net/npm/vega-lite@5.6.1")
             html_modifier.add_head_script(src="https://cdn.jsdelivr.net/npm/vega-embed@6.21.2")
             output = str(html_modifier)
@@ -179,15 +174,15 @@
             """Watcher implementation that skips .obsidian directory"""
             if (
                 isinstance(event, watchdog.events.FileModifiedEvent)
                 and any([str(event.src_path).startswith(d) for d in docs_dirs_to_skip])
                 or event.is_directory
             ):
                 return
-            log.debug(str(event))
+
             with server._rebuild_cond:
                 # noinspection PyProtectedMember
                 server._to_rebuild[server.builder] = True
                 server._rebuild_cond.notify_all()
 
         handler = watchdog.events.FileSystemEventHandler()
         handler.on_any_event = no_obsidian_callback
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/obsidian/vega.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/obsidian/vega.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -69,15 +69,14 @@
             vega_start_match = re.match(VEGA_BLOCK_START, line)
             if not in_vega_block and vega_start_match:
                 in_vega_block = True
                 vega_schema = self._vega_schema_mapping[vega_start_match.group(2)]
             elif in_vega_block:
                 vega_stop_match = re.match(VEGA_BLOCK_STOP, line)
                 if vega_stop_match:
-
                     # Create chart data as JSON
                     vega_chart_json = json.loads("\n".join(vega_block_lines))
                     if "$schema" not in vega_chart_json:
                         vega_chart_json["$schema"] = vega_schema
 
                     # Render chart
                     self._vega_chart_id += 1
```

### Comparing `mkdocs_publisher-1.2.0/mkdocs_publisher/social/plugin.py` & `mkdocs_publisher-1.3.0/mkdocs_publisher/social/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2023 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
+# Copyright (c) 2023-2024 Maciej 'maQ' Kusz <maciej.kusz@gmail.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `mkdocs_publisher-1.2.0/pyproject.toml` & `mkdocs_publisher-1.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mkdocs-publisher"
-version = "1.2.0"
+version = "1.3.0"
 description = "Publisher for MkDocs - set of plugins for content creators"
 authors = ["Maciej 'maQ' Kusz <maciej.kusz@gmail.com>"]
-license = "BSD"
+license = "MIT License"
 readme = "README.md"
 keywords = [
     "mkdocs",
     "mkdocs-plugin",
     "blog",
     "categories",
     "debugger",
@@ -18,15 +18,15 @@
     "minifier",
     "navigation",
     "obsidian",
     "publisher",
     "tags",
 ]
 packages = [
-    {include = "mkdocs_publisher"},
+    {include = "mkdocs_publisher"}
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Environment :: Web Environment",
     "Intended Audience :: Education",
     "Intended Audience :: Developers",
@@ -36,66 +36,51 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: 3.13",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Documentation",
     "Topic :: Text Editors :: Documentation",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: Markdown",
     "Topic :: Utilities",
 ]
-homepage = "https://github.com/mkusz/mkdocs-publisher"
+homepage = "https://mkusz.github.io/mkdocs-publisher"
 repository = "https://github.com/mkusz/mkdocs-publisher"
 documentation = "https://mkusz.github.io/mkdocs-publisher"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/mkusz/mkdocs-publisher/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 mkdocs = "^1.5.3"
-pymdown-extensions = "^10.3"
-beautifulsoup4 = "^4.12.2"
-mkdocs-material = "^9.4.4"
+pymdown-extensions = "^10.7"
+beautifulsoup4 = "^4.12.3"
+mkdocs-material = "^9.5.18"
 
 [tool.poetry.group.dev.dependencies]
-isort = "^5.12.0"
-black = "^22.12.0"
-yamllint = "^1.29.0"
-pyright = "1.1.323"
-ruff = "^0.0.292"
+yamllint = "^1.35.1"
+pyright = "1.1.359"
+ruff = "^0.3.7"
 
 [tool.poetry.group.test.dependencies]
-coverage = "^7.3.2"
-pytest = "^7.4.2"
+coverage = "^7.4.4"
+pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
+pytest-check = "^2.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.black]
-line-length = 99
-
-[tool.isort]
-py_version=39
-profile = "black"
-line_length = 99
-force_single_line = true
-src_paths = [
-    "mkdocs_publisher",
-    "tests",
-]
-
 [tool.pyright]
 extraPaths = [
     "mkdocs_publisher",
 ]
 include = [
     "mkdocs_publisher",
     "tests",
@@ -106,37 +91,45 @@
 ]
 reportMissingImports = false
 reportMissingTypeStubs = false
 reportOptionalMemberAccess = false
 typeCheckingMode = "basic"
 
 [tool.pytest.ini_options]
-addopts = "--tb=short --log-level=DEBUG --cov-report=html --cov=mkdocs_publisher"
+addopts = "--tb=short --log-level=DEBUG --cov-report=html --cov-report=json --cov=mkdocs_publisher"
 markers = [
     "deprecated: Tests no longer used",
     ]
 testpaths = [
     "tests",
 ]
 
 [tool.ruff]
 target-version = "py39"
 line-length = 99
 
-[tool.ruff.mccabe]
+[tool.ruff.lint]
+select = ["B", "E", "F", "I", "UP", "SIM"]
+
+[tool.ruff.lint.isort]
+force-single-line = true
+
+[tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 include_namespace_packages = true
 skip_empty = true
-skip_covered = false
+skip_covered = true
 
+[tool.coverage.json]
+pretty_print = true
 
 [tool.poetry.plugins."mkdocs.plugins"]
 pub-blog = "mkdocs_publisher.blog.plugin:BlogPlugin"
 pub-debugger = "mkdocs_publisher.debugger.plugin:DebuggerPlugin"
 pub-meta = "mkdocs_publisher.meta.plugin:MetaPlugin"
 pub-minifier = "mkdocs_publisher.minifier.plugin:MinifierPlugin"
 pub-obsidian = "mkdocs_publisher.obsidian.plugin:ObsidianPlugin"
```

### Comparing `mkdocs_publisher-1.2.0/PKG-INFO` & `mkdocs_publisher-1.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,57 @@
 Metadata-Version: 2.1
 Name: mkdocs-publisher
-Version: 1.2.0
+Version: 1.3.0
 Summary: Publisher for MkDocs - set of plugins for content creators
-Home-page: https://github.com/mkusz/mkdocs-publisher
-License: BSD
+Home-page: https://mkusz.github.io/mkdocs-publisher
+License: MIT
 Keywords: mkdocs,mkdocs-plugin,blog,categories,debugger,docs,documentation,frontmatter,markdown,minifier,navigation,obsidian,publisher,tags
 Author: Maciej 'maQ' Kusz
 Author-email: maciej.kusz@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation
 Classifier: Topic :: Text Editors :: Documentation
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Utilities
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: mkdocs (>=1.5.3,<2.0.0)
-Requires-Dist: mkdocs-material (>=9.4.4,<10.0.0)
-Requires-Dist: pymdown-extensions (>=10.3,<11.0)
+Requires-Dist: mkdocs-material (>=9.5.18,<10.0.0)
+Requires-Dist: pymdown-extensions (>=10.7,<11.0)
 Project-URL: Bug Tracker, https://github.com/mkusz/mkdocs-publisher/issues
 Project-URL: Documentation, https://mkusz.github.io/mkdocs-publisher
 Project-URL: Repository, https://github.com/mkusz/mkdocs-publisher
 Description-Content-Type: text/markdown
 
----
-date: 2023-10-02 23:12:38
-update: 2023-10-10 13:18:32
----
 # Publisher for MkDocs
 
-[![PyPI version](https://img.shields.io/pypi/v/mkdocs-publisher?logo=pypi&style=plastic)](https://pypi.org/project/mkdocs-publisher/)
-[![License type](https://img.shields.io/pypi/l/mkdocs-publisher?logo=pypi&style=plastic)](https://opensource.org/license/mit/)
-[![PyPI Downloads last month](https://img.shields.io/pypi/dm/mkdocs-publisher?logo=pypi&style=plastic)](https://pypistats.org/search/mkdocs-publisher)
-[![Python versions](https://img.shields.io/pypi/pyversions/mkdocs-publisher?logo=python&style=plastic)](https://www.python.org)
-[![GitHub last commit](https://img.shields.io/github/last-commit/mkusz/mkdocs-publisher?logo=github&style=plastic)](https://github.com/mkusz/mkdocs-publisher/commits/main)
+[![License type](https://img.shields.io/github/license/mkusz/mkdocs-publisher?logo=pypi&logoColor=white&style=plastic&label=License)](https://opensource.org/license/mit/)
+[![PyPI version](https://img.shields.io/pypi/v/mkdocs-publisher?logo=pypi&logoColor=white&style=plastic&label=PyPi)](https://pypi.org/project/mkdocs-publisher/)
+[![PyPI - Python Version](https://img.shields.io/badge/dynamic/toml?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmkusz%2Fmkdocs-publisher%2Fmain%2Fpyproject.toml&query=%24.tool.poetry.dependencies.python&logo=python&logoColor=white&style=plastic&label=Python)](https://www.python.org)
+[![PyPI Downloads last month](https://img.shields.io/pypi/dm/mkdocs-publisher?logo=pypi&logoColor=white&style=plastic&label=Downloads)](https://pypistats.org/search/mkdocs-publisher)
+[![GitHub last commit](https://img.shields.io/github/last-commit/mkusz/mkdocs-publisher?logo=github&logoColor=white&style=plastic&label=Last%20commit)](https://github.com/mkusz/mkdocs-publisher/commits/main)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=plastic&label=Pre-commit)](https://github.com/pre-commit/pre-commit)
+![Code Coverage](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fraw.githubusercontent.com%2Fmkusz%2Fmkdocs-publisher%2Fmain%2Fcov.json&query=%24.percent_covered_display&suffix=%25&color=green&style=plastic&label=Code%20coverage)
 
 Publisher for [MkDocs](https://www.mkdocs.org/) is a set of plugins that helps with content creation and publication.
 
 ## Features
 
 - [pub-meta](https://mkusz.github.io/mkdocs-publisher/setup/general/pub-meta/) – support for:
 	- automatic [document navigation](https://www.mkdocs.org/user-guide/configuration/#nav) creation based on file names order,
@@ -93,22 +89,22 @@
 
 ```yaml
 theme: material
 
 plugins:
   - search  # Material for MkDocs search plugin
   - pub-debugger
-  - pub-obsidian  # blog is a directory with all blog posts
+  - pub-blog
   - pub-obsidian
   - pub-social
   - pub-meta
   - pub-minifier
 ```
 
 ## Planned features
 
-A full list of planned developments can be found on [this documentation page](https://mkusz.github.io/mkdocs-publisher/development/other/backlog/). I'm planning to move it to the project [GitHub issues](https://github.com/mkusz/mkdocs-publisher/issues) with proper badges and longer descriptions, but it's time-consuming and at this stage I'd rather spend it to develop a project.
+A full list of planned developments can be found on [this documentation page](https://mkusz.github.io/mkdocs-publisher/development/other/backlog/). I'm planning to move it to the project [GitHub issues](https://github.com/mkusz/mkdocs-publisher/issues) with proper badges and longer descriptions, but it's time-consuming and at this stage I'd rather spend it developing a project.
 
 ## Version history
 
 The entire version history can be found in the project [version history](https://mkusz.github.io/mkdocs-publisher/development/changelog/) document and inside [releases](https://github.com/mkusz/mkdocs-publisher/releases).
```

