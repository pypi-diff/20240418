# Comparing `tmp/sphinx_external_toc_strict-1.1.2.tar.gz` & `tmp/sphinx_external_toc_strict-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_external_toc_strict-1.1.2.tar", last modified: Thu Apr 18 11:39:54 2024, max compression
+gzip compressed data, was "sphinx_external_toc_strict-1.1.3.tar", last modified: Thu Apr 18 12:31:38 2024, max compression
```

## Comparing `sphinx_external_toc_strict-1.1.2.tar` & `sphinx_external_toc_strict-1.1.3.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.316089 sphinx_external_toc_strict-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.264090 sphinx_external_toc_strict-1.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.268090 sphinx_external_toc_strict-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/kit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/python-nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/quality.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/test-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.github/workflows/testsuite.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-04-18 11:39:54.316089 sphinx_external_toc_strict-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.268090 sphinx_external_toc_strict-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.272090 sphinx_external_toc_strict-1.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/_static/toc-graphic.png
--rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/_static/toc_tree.pptx
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.272090 sphinx_external_toc_strict-1.1.2/docs/code/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/compat.rst
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/constrants.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/events.rst
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/filename_suffix.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/parsing_shared.rst
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/parsing_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/pep518_read.rst
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/tools_strictyaml.rst
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/code/version_semantic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.272090 sphinx_external_toc_strict-1.1.2/docs/example/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.272090 sphinx_external_toc_strict-1.1.2/docs/example/globfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/example/globfolder/page1.rst
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/example/globfolder/page2.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/example/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.272090 sphinx_external_toc_strict-1.1.2/docs/example/subfolder/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/example/subfolder/page.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-black.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-docutils-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-python.txt
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-sphinx-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-strictyaml-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-strictyaml-source.txt
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/objects-toc-strict.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/requirements.pip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.272090 sphinx_external_toc_strict-1.1.2/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/user_guide/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/user_guide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/user_guide/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/docs/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/howto.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/igor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.276090 sphinx_external_toc_strict-1.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/dev.pip
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/kit.in
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/kit.pip
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/manage.in
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/manage.pip
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/mypy.in
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/mypy.pip
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/pins.pip
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/pip-tools.pip
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/pip.pip
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/prod.in
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/prod.pip
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/requirements/tox.pip
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:39:54.316089 sphinx_external_toc_strict-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.260090 sphinx_external_toc_strict-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.280089 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/filename_suffix.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/filename_suffix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_shared.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/pep518_read.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/pep518_read.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/tools_strictyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/tools_strictyaml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/version_semantic.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.292089 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29500 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 11:39:54.000000 sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.280089 sphinx_external_toc_strict-1.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.284089 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/bad_option_value.yml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/bad_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/doc_multiple_times.yml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/doc_validation_fail.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/empty_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/empty_subtrees.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/entry_not_a_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/entry_unknown_link_type.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/file_and_glob_present.yml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/item_then_subtrees_key.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/items_in_glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/items_in_url.yml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/list.yml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/no_root.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/subtree_with_no_items.yml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/unknown_keys.yml
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/unknown_keys_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_bad_toc_files/unknown_usecase.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.284089 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/jb_docs_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/list_and_nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/numbered_chapters.yml
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/numbered_depth.yml
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/numbered_parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/parts.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/simple_dict.yml
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/simple_list.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.288089 sphinx_external_toc_strict-1.1.2/tests/_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/basic.yml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/basic_compressed.yml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/caption_not_entries.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/exclude_missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/glob.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/glob_md.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/nested.yml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_toc_files/tableofcontents.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.288089 sphinx_external_toc_strict-1.1.2/tests/_warning_toc_files/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_warning_toc_files/contains_toctree.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_warning_toc_files/file_not_in_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_warning_toc_files/multiple_tableofcontents.yml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_warning_toc_files/no_glob_match.yml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/_warning_toc_files/tableofcontents_no_toc.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.288089 sphinx_external_toc_strict-1.1.2/tests/test_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_cli/test_create_toc.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_filename_suffix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.288089 sphinx_external_toc_strict-1.1.2/tests/test_parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_pep518_read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.292089 sphinx_external_toc_strict-1.1.2/tests/test_sphinx/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_sphinx/test_success_basic_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_sphinx/test_success_basic_compressed_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_sphinx/test_success_caption_not_entries_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_sphinx/test_success_glob_md_.xml
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_sphinx/test_success_tableofcontents_.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_sphinx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:39:54.292089 sphinx_external_toc_strict-1.1.2/tests/test_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_create_site_map_from_path.yml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_basic_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_basic_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_glob_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_glob_md_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_list_and_nested_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_numbered_depth_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_numbered_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_parts_.yml
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_simple_dict_.yml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_simple_list_.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tests/test_version_semantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-18 11:39:46.000000 sphinx_external_toc_strict-1.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.852928 sphinx_external_toc_strict-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.804927 sphinx_external_toc_strict-1.1.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.804927 sphinx_external_toc_strict-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10381 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/kit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/python-nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/quality.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/test-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.github/workflows/testsuite.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31271 2024-04-18 12:31:38.852928 sphinx_external_toc_strict-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.808927 sphinx_external_toc_strict-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5730 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.808927 sphinx_external_toc_strict-1.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)   147326 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/_static/toc-graphic.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49736 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/_static/toc_tree.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/code/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/compat.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/constrants.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/events.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/filename_suffix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/parsing_shared.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/parsing_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/pep518_read.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/tools_strictyaml.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/code/version_semantic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/example/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/example/globfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/globfolder/page1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/globfolder/page2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/example/subfolder/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/example/subfolder/page.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-black.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-docutils-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1111839 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-python.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-sphinx-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-source.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/objects-toc-strict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/requirements.pip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/sphinx.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/docs/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/howto.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17383 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/igor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.812928 sphinx_external_toc_strict-1.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/dev.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/kit.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/kit.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/manage.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/manage.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/mypy.in
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/mypy.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pins.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip-tools.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/pip.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/prod.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/prod.pip
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/requirements/tox.pip
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 12:31:38.852928 sphinx_external_toc_strict-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.800927 sphinx_external_toc_strict-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.816928 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12354 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19082 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19183 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9252 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/version_semantic.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.832928 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    31271 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7733 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 12:31:38.000000 sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.820927 sphinx_external_toc_strict-1.1.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/bad_option_value.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/bad_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/doc_multiple_times.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/doc_validation_fail.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/empty_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/empty_subtrees.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/entry_not_a_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/entry_unknown_link_type.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/file_and_glob_present.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/item_then_subtrees_key.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/items_in_glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/items_in_url.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/list.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/no_root.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/subtree_with_no_items.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/unknown_keys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/unknown_keys_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_bad_toc_files/unknown_usecase.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/jb_docs_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/list_and_nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_chapters.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_depth.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_depth_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/numbered_parts_subset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/parts.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/simple_dict.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/simple_list.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/basic.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/basic_compressed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/caption_not_entries.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/exclude_missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/glob.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/glob_md.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/nested.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_toc_files/tableofcontents.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/contains_toctree.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/file_not_in_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/multiple_tableofcontents.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/no_glob_match.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/_warning_toc_files/tableofcontents_no_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.824928 sphinx_external_toc_strict-1.1.3/tests/test_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_cli/test_create_toc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_filename_suffix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.828928 sphinx_external_toc_strict-1.1.3/tests/test_parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_pep518_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.828928 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_basic_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_basic_compressed_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_caption_not_entries_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_glob_md_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_tableofcontents_.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_sphinx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:31:38.832928 sphinx_external_toc_strict-1.1.3/tests/test_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_create_site_map_from_path.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_basic_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_basic_compressed_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_basic_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_caption_not_entries_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_exclude_missing_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_glob_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_glob_md_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_file_to_sitemap_tableofcontents_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_list_and_nested_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_chapters_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_depth_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_depth_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_numbered_parts_subset_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_parts_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_simple_dict_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_simple_list_.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9140 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tests/test_version_semantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-18 12:31:31.000000 sphinx_external_toc_strict-1.1.3/tox.ini
```

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/codeql-analysis.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/dependency-review.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/kit.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/kit.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/python-nightly.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/python-nightly.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/quality.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/quality.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/release.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/test-coverage.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/test-coverage.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.github/workflows/testsuite.yml` & `sphinx_external_toc_strict-1.1.3/.github/workflows/testsuite.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.gitignore` & `sphinx_external_toc_strict-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/.pre-commit-config.yaml` & `sphinx_external_toc_strict-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/CHANGELOG.md` & `sphinx_external_toc_strict-1.1.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/CHANGES.rst` & `sphinx_external_toc_strict-1.1.3/CHANGES.rst`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,24 @@
    1. Dropped support for hidden document files
 
    Commit items for NEXT VERSION
    ..............................
 
 .. scriv-start-here
 
+.. _changes_1-1-3:
+
+Version 1.1.3 — 2024-04-18
+--------------------------
+
+- ci(.readthedocs.yml): python.install.requirements list rather than dict
+- style(pyproject.toml): configure project.urls
+- docs(README.rst): github-ci badge use workflow release
+- docs(README.rst): add badges
+
 .. _changes_1-1-2:
 
 Version 1.1.2 — 2024-04-18
 --------------------------
 
 - ci(test-coverage.yml): bump version codecov/codecov-action
 - ci(release.yml): bump version sigstore/gh-action-sigstore-python
```

### Comparing `sphinx_external_toc_strict-1.1.2/CONTRIBUTING.md` & `sphinx_external_toc_strict-1.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/LICENSE` & `sphinx_external_toc_strict-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/Makefile` & `sphinx_external_toc_strict-1.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/NOTICE.txt` & `sphinx_external_toc_strict-1.1.3/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/PKG-INFO` & `sphinx_external_toc_strict-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.2
+Version: 1.1.3
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,19 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/msftcangoblowm/sphinx-external-toc-strict
-Project-URL: Documentation, https://sphinx-external-toc-strict.readthedocs.io/intro.html
+Project-URL: Documentation, https://sphinx-external-toc-strict.readthedocs.io
+Project-URL: Changes, https://raw.githubusercontent.com/msftcangoblowm/sphinx-external-toc-strict/main/CHANGES.rst
+Project-URL: PyPI Releases, https://pypi.org/project/sphinx-external-toc-strict
+Project-URL: Source code, https://github.com/msftcangoblowm/sphinx-external-toc-strict
+Project-URL: Issue tracker, https://github.com/msftcangoblowm/sphinx-external-toc-strict/issues
 Project-URL: Chat, https://mastodon.social/@msftcangoblowme
 Keywords: sphinx,extension,toc,strictyaml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -248,18 +251,17 @@
 .. For details: https://github.com/msftcangoblowm/sphinx-external-toc-strict/blob/master/NOTICE.txt
 
 sphinx-external-toc-strict
 ===========================
 
 A sphinx extension that allows the documentation site-map (a.k.a Table of Contents) to be defined external to the documentation files.
 
-| Github-CI |github-ci|
-| Coverage Status |codecov|
-| Code style: black |black|
-| PyPI |pypi|
+|  |kit| |license| |versions|
+|  |test-status| |codecov| |quality-status| |docs| |black|
+|  |stars| |mastodon-msftcangoblowm|
 
 In normal Sphinx documentation, the documentation site-map is defined
 *via* a bottom-up approach - adding
 `toctree directives <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#table-of-contents>`_
 within pages of the documentation.
 
 This extension facilitates a **top-down** approach to defining the
@@ -804,17 +806,36 @@
 - test against orphan file
 - `sphinx-book-theme#304 <https://github.com/executablebooks/sphinx-book-theme/pull/304>`_
 - CLI command to generate toc from existing documentation ``toctrees`` (and then remove toctree directives)
 - test rebuild on toc changes (and document how rebuilds are controlled when toc changes)
 - some jupyter-book issues point to potential changes in numbering, based on where the ``toctree`` is in the document.
   So could look into placing it e.g. under the first heading/title
 
-.. |github-ci| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/workflows/continuous-integration/badge.svg?branch=main
-   :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict
-   :alt: Source code
-.. |codecov| image:: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict
-   :alt: coverage
+.. |test-status| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/testsuite.yml/badge.svg?branch=main&event=push
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/testsuite.yml
+    :alt: Test suite status
+.. |quality-status| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/quality.yml/badge.svg?branch=main&event=push
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/quality.yml
+    :alt: Quality check status
+.. |docs| image:: https://readthedocs.org/projects/sphinx-external-toc-strict/badge/?version=latest&style=flat
+    :target: https://sphinx-external-toc-strict.readthedocs.io/
+    :alt: Documentation
+.. |kit| image:: https://img.shields.io/pypi/v/sphinx-external-toc-strict
+    :target: https://pypi.org/project/sphinx-external-toc-strict/
+    :alt: PyPI status
+.. |versions| image:: https://img.shields.io/pypi/pyversions/sphinx-external-toc-strict.svg?logo=python&logoColor=FBE072
+    :target: https://pypi.org/project/sphinx-external-toc-strict/
+    :alt: Python versions supported
+.. |license| image:: https://img.shields.io/github/license/msftcangoblowm/sphinx-external-toc-strict
+    :target: https://pypi.org/project/sphinx-external-toc-strict/blob/master/LICENSE.txt
+    :alt: License
+.. |stars| image:: https://img.shields.io/github/stars/msftcangoblowm/sphinx-external-toc-strict.svg?logo=github
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/stargazers
+    :alt: GitHub stars
+.. |mastodon-msftcangoblowm| image:: https://img.shields.io/mastodon/follow/112019041247183249
+    :target: https://mastodon.social/@msftcangoblowme
+    :alt: msftcangoblowme on Mastodon
+.. |codecov| image:: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict/branch/main/graph/badge.svg?token=HCBC74IABR
+    :target: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict
+    :alt: sphinx-external-toc-strict coverage percentage
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
-.. |pypi| image:: https://img.shields.io/pypi/v/sphinx-external-toc-strict.svg
-   :alt: https://pypi.org/project/sphinx-external-toc-strict
```

### Comparing `sphinx_external_toc_strict-1.1.2/README.rst` & `sphinx_external_toc_strict-1.1.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 .. For details: https://github.com/msftcangoblowm/sphinx-external-toc-strict/blob/master/NOTICE.txt
 
 sphinx-external-toc-strict
 ===========================
 
 A sphinx extension that allows the documentation site-map (a.k.a Table of Contents) to be defined external to the documentation files.
 
-| Github-CI |github-ci|
-| Coverage Status |codecov|
-| Code style: black |black|
-| PyPI |pypi|
+|  |kit| |license| |versions|
+|  |test-status| |codecov| |quality-status| |docs| |black|
+|  |stars| |mastodon-msftcangoblowm|
 
 In normal Sphinx documentation, the documentation site-map is defined
 *via* a bottom-up approach - adding
 `toctree directives <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#table-of-contents>`_
 within pages of the documentation.
 
 This extension facilitates a **top-down** approach to defining the
@@ -558,17 +557,36 @@
 - test against orphan file
 - `sphinx-book-theme#304 <https://github.com/executablebooks/sphinx-book-theme/pull/304>`_
 - CLI command to generate toc from existing documentation ``toctrees`` (and then remove toctree directives)
 - test rebuild on toc changes (and document how rebuilds are controlled when toc changes)
 - some jupyter-book issues point to potential changes in numbering, based on where the ``toctree`` is in the document.
   So could look into placing it e.g. under the first heading/title
 
-.. |github-ci| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/workflows/continuous-integration/badge.svg?branch=main
-   :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict
-   :alt: Source code
-.. |codecov| image:: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict
-   :alt: coverage
+.. |test-status| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/testsuite.yml/badge.svg?branch=main&event=push
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/testsuite.yml
+    :alt: Test suite status
+.. |quality-status| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/quality.yml/badge.svg?branch=main&event=push
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/quality.yml
+    :alt: Quality check status
+.. |docs| image:: https://readthedocs.org/projects/sphinx-external-toc-strict/badge/?version=latest&style=flat
+    :target: https://sphinx-external-toc-strict.readthedocs.io/
+    :alt: Documentation
+.. |kit| image:: https://img.shields.io/pypi/v/sphinx-external-toc-strict
+    :target: https://pypi.org/project/sphinx-external-toc-strict/
+    :alt: PyPI status
+.. |versions| image:: https://img.shields.io/pypi/pyversions/sphinx-external-toc-strict.svg?logo=python&logoColor=FBE072
+    :target: https://pypi.org/project/sphinx-external-toc-strict/
+    :alt: Python versions supported
+.. |license| image:: https://img.shields.io/github/license/msftcangoblowm/sphinx-external-toc-strict
+    :target: https://pypi.org/project/sphinx-external-toc-strict/blob/master/LICENSE.txt
+    :alt: License
+.. |stars| image:: https://img.shields.io/github/stars/msftcangoblowm/sphinx-external-toc-strict.svg?logo=github
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/stargazers
+    :alt: GitHub stars
+.. |mastodon-msftcangoblowm| image:: https://img.shields.io/mastodon/follow/112019041247183249
+    :target: https://mastodon.social/@msftcangoblowme
+    :alt: msftcangoblowme on Mastodon
+.. |codecov| image:: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict/branch/main/graph/badge.svg?token=HCBC74IABR
+    :target: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict
+    :alt: sphinx-external-toc-strict coverage percentage
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
-.. |pypi| image:: https://img.shields.io/pypi/v/sphinx-external-toc-strict.svg
-   :alt: https://pypi.org/project/sphinx-external-toc-strict
```

### Comparing `sphinx_external_toc_strict-1.1.2/docs/Makefile` & `sphinx_external_toc_strict-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/_static/toc-graphic.png` & `sphinx_external_toc_strict-1.1.3/docs/_static/toc-graphic.png`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/_static/toc_tree.pptx` & `sphinx_external_toc_strict-1.1.3/docs/_static/toc_tree.pptx`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/_toc.yml` & `sphinx_external_toc_strict-1.1.3/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/code/cli.rst` & `sphinx_external_toc_strict-1.1.3/docs/code/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/conf.py` & `sphinx_external_toc_strict-1.1.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 
 # Original author Chris Sewell <chrisj_sewell@hotmail.com>
 # copyright = "2021, Executable Book Project"
 
 # @@@ editable
 copyright = "2023–2024, Dave Faulkmore"
 # The short X.Y.Z version.
-version = "1.1.2"
+version = "1.1.3"
 # The full version, including alpha/beta/rc tags.
-release = "1.1.2"
+release = "1.1.3"
 # The date of release, in "monthname day, year" format.
 release_date = "April 18, 2024"
 # @@@ end
 
 v = parse(release)
 version_short = f"{v.major}.{v.minor}"
 # version_xyz = f"{v.major}.{v.minor}.{v.micro}"
```

### Comparing `sphinx_external_toc_strict-1.1.2/docs/intro.rst` & `sphinx_external_toc_strict-1.1.3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/objects-python.txt` & `sphinx_external_toc_strict-1.1.3/docs/objects-python.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/objects-sphinx-docs.txt` & `sphinx_external_toc_strict-1.1.3/docs/objects-sphinx-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/objects-strictyaml-docs.txt` & `sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-docs.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/objects-strictyaml-source.txt` & `sphinx_external_toc_strict-1.1.3/docs/objects-strictyaml-source.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/requirements.pip` & `sphinx_external_toc_strict-1.1.3/docs/requirements.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/user_guide/api.rst` & `sphinx_external_toc_strict-1.1.3/docs/user_guide/api.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/user_guide/cli.rst` & `sphinx_external_toc_strict-1.1.3/docs/user_guide/cli.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/user_guide/sphinx.rst` & `sphinx_external_toc_strict-1.1.3/docs/user_guide/sphinx.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/docs/user_guide/why.rst` & `sphinx_external_toc_strict-1.1.3/docs/user_guide/why.rst`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/howto.txt` & `sphinx_external_toc_strict-1.1.3/howto.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/igor.py` & `sphinx_external_toc_strict-1.1.3/igor.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/pyproject.toml` & `sphinx_external_toc_strict-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,16 +30,19 @@
 ]
 # author sphinx-external-toc {name = "Chris Sewell", email = "chrisj_sewell@hotmail.com"},
 authors = [  # Contact by mastodon please
     {name = "Dave Faulkmore", email = "faulkmore@protonmail.com"},
 ]
 
 [project.urls]
-Homepage = "https://github.com/msftcangoblowm/sphinx-external-toc-strict"
-Documentation = "https://sphinx-external-toc-strict.readthedocs.io/intro.html"
+Documentation = "https://sphinx-external-toc-strict.readthedocs.io"
+Changes = "https://raw.githubusercontent.com/msftcangoblowm/sphinx-external-toc-strict/main/CHANGES.rst"
+"PyPI Releases" = "https://pypi.org/project/sphinx-external-toc-strict"
+"Source code" = "https://github.com/msftcangoblowm/sphinx-external-toc-strict"
+"Issue tracker" = "https://github.com/msftcangoblowm/sphinx-external-toc-strict/issues"
 Chat = "https://mastodon.social/@msftcangoblowme"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["sphinx_external_toc_strict*"]
 
 [tool.setuptools.dynamic]
```

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/dev.pip` & `sphinx_external_toc_strict-1.1.3/requirements/dev.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/kit.in` & `sphinx_external_toc_strict-1.1.3/requirements/kit.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/kit.pip` & `sphinx_external_toc_strict-1.1.3/requirements/kit.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/manage.pip` & `sphinx_external_toc_strict-1.1.3/requirements/manage.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/pip-tools.pip` & `sphinx_external_toc_strict-1.1.3/requirements/pip-tools.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/prod.pip` & `sphinx_external_toc_strict-1.1.3/requirements/prod.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/tox.in` & `sphinx_external_toc_strict-1.1.3/requirements/tox.in`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/requirements/tox.pip` & `sphinx_external_toc_strict-1.1.3/requirements/tox.pip`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/setup.py` & `sphinx_external_toc_strict-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/__init__.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/_compat.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/_compat.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/api.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/api.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/api.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/cli.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/constants.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/constants.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/constants.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/events.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/events.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/events.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/filename_suffix.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/filename_suffix.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/filename_suffix.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_shared.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_shared.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_shared.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_strictyaml.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/parsing_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/parsing_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/pep518_read.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/pep518_read.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/pep518_read.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/tools_strictyaml.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/tools_strictyaml.pyi` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/tools_strictyaml.pyi`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict/version_semantic.py` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict/version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/PKG-INFO` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-external-toc-strict
-Version: 1.1.2
+Version: 1.1.3
 Summary: A sphinx extension that allows the site-map to be defined in a single YAML file.
 Author-email: Dave Faulkmore <faulkmore@protonmail.com>
 License: MIT License
         
         Copyright (c) 2021 Executable Books
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,16 +21,19 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/msftcangoblowm/sphinx-external-toc-strict
-Project-URL: Documentation, https://sphinx-external-toc-strict.readthedocs.io/intro.html
+Project-URL: Documentation, https://sphinx-external-toc-strict.readthedocs.io
+Project-URL: Changes, https://raw.githubusercontent.com/msftcangoblowm/sphinx-external-toc-strict/main/CHANGES.rst
+Project-URL: PyPI Releases, https://pypi.org/project/sphinx-external-toc-strict
+Project-URL: Source code, https://github.com/msftcangoblowm/sphinx-external-toc-strict
+Project-URL: Issue tracker, https://github.com/msftcangoblowm/sphinx-external-toc-strict/issues
 Project-URL: Chat, https://mastodon.social/@msftcangoblowme
 Keywords: sphinx,extension,toc,strictyaml
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -248,18 +251,17 @@
 .. For details: https://github.com/msftcangoblowm/sphinx-external-toc-strict/blob/master/NOTICE.txt
 
 sphinx-external-toc-strict
 ===========================
 
 A sphinx extension that allows the documentation site-map (a.k.a Table of Contents) to be defined external to the documentation files.
 
-| Github-CI |github-ci|
-| Coverage Status |codecov|
-| Code style: black |black|
-| PyPI |pypi|
+|  |kit| |license| |versions|
+|  |test-status| |codecov| |quality-status| |docs| |black|
+|  |stars| |mastodon-msftcangoblowm|
 
 In normal Sphinx documentation, the documentation site-map is defined
 *via* a bottom-up approach - adding
 `toctree directives <https://www.sphinx-doc.org/en/master/usage/restructuredtext/directives.html#table-of-contents>`_
 within pages of the documentation.
 
 This extension facilitates a **top-down** approach to defining the
@@ -804,17 +806,36 @@
 - test against orphan file
 - `sphinx-book-theme#304 <https://github.com/executablebooks/sphinx-book-theme/pull/304>`_
 - CLI command to generate toc from existing documentation ``toctrees`` (and then remove toctree directives)
 - test rebuild on toc changes (and document how rebuilds are controlled when toc changes)
 - some jupyter-book issues point to potential changes in numbering, based on where the ``toctree`` is in the document.
   So could look into placing it e.g. under the first heading/title
 
-.. |github-ci| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/workflows/continuous-integration/badge.svg?branch=main
-   :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict
-   :alt: Source code
-.. |codecov| image:: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict
-   :alt: coverage
+.. |test-status| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/testsuite.yml/badge.svg?branch=main&event=push
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/testsuite.yml
+    :alt: Test suite status
+.. |quality-status| image:: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/quality.yml/badge.svg?branch=main&event=push
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/actions/workflows/quality.yml
+    :alt: Quality check status
+.. |docs| image:: https://readthedocs.org/projects/sphinx-external-toc-strict/badge/?version=latest&style=flat
+    :target: https://sphinx-external-toc-strict.readthedocs.io/
+    :alt: Documentation
+.. |kit| image:: https://img.shields.io/pypi/v/sphinx-external-toc-strict
+    :target: https://pypi.org/project/sphinx-external-toc-strict/
+    :alt: PyPI status
+.. |versions| image:: https://img.shields.io/pypi/pyversions/sphinx-external-toc-strict.svg?logo=python&logoColor=FBE072
+    :target: https://pypi.org/project/sphinx-external-toc-strict/
+    :alt: Python versions supported
+.. |license| image:: https://img.shields.io/github/license/msftcangoblowm/sphinx-external-toc-strict
+    :target: https://pypi.org/project/sphinx-external-toc-strict/blob/master/LICENSE.txt
+    :alt: License
+.. |stars| image:: https://img.shields.io/github/stars/msftcangoblowm/sphinx-external-toc-strict.svg?logo=github
+    :target: https://github.com/msftcangoblowm/sphinx-external-toc-strict/stargazers
+    :alt: GitHub stars
+.. |mastodon-msftcangoblowm| image:: https://img.shields.io/mastodon/follow/112019041247183249
+    :target: https://mastodon.social/@msftcangoblowme
+    :alt: msftcangoblowme on Mastodon
+.. |codecov| image:: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict/branch/main/graph/badge.svg?token=HCBC74IABR
+    :target: https://codecov.io/gh/msftcangoblowm/sphinx-external-toc-strict
+    :alt: sphinx-external-toc-strict coverage percentage
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/ambv/black
-.. |pypi| image:: https://img.shields.io/pypi/v/sphinx-external-toc-strict.svg
-   :alt: https://pypi.org/project/sphinx-external-toc-strict
```

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/SOURCES.txt` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/src/sphinx_external_toc_strict.egg-info/requires.txt` & `sphinx_external_toc_strict-1.1.3/src/sphinx_external_toc_strict.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/chapters.yml` & `sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/chapters.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/jb_docs_toc.yml` & `sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/jb_docs_toc.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/_jb_migrate_toc_files/parts.yml` & `sphinx_external_toc_strict-1.1.3/tests/_jb_migrate_toc_files/parts.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/_toc_files/glob_md.yml` & `sphinx_external_toc_strict-1.1.3/tests/_toc_files/glob_md.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/conftest.py` & `sphinx_external_toc_strict-1.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_api.py` & `sphinx_external_toc_strict-1.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_cli/test_create_toc.txt` & `sphinx_external_toc_strict-1.1.3/tests/test_cli/test_create_toc.txt`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_cli.py` & `sphinx_external_toc_strict-1.1.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_filename_suffix.py` & `sphinx_external_toc_strict-1.1.3/tests/test_filename_suffix.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_create_toc_dict_glob_md_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_create_toc_dict_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_basic_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_basic_compressed_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_glob_md_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_glob_md_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_nested_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_nested_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing/test_file_to_sitemap_tableofcontents_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_parsing.py` & `sphinx_external_toc_strict-1.1.3/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_pep518_read.py` & `sphinx_external_toc_strict-1.1.3/tests/test_pep518_read.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_sphinx/test_success_tableofcontents_.xml` & `sphinx_external_toc_strict-1.1.3/tests/test_sphinx/test_success_tableofcontents_.xml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_sphinx.py` & `sphinx_external_toc_strict-1.1.3/tests/test_sphinx.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_tools/test_create_site_map_from_path.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_create_site_map_from_path.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_chapters_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_chapters_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_jb_docs_toc_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_tools/test_migrate_jb_parts_.yml` & `sphinx_external_toc_strict-1.1.3/tests/test_tools/test_migrate_jb_parts_.yml`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_tools.py` & `sphinx_external_toc_strict-1.1.3/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tests/test_version_semantic.py` & `sphinx_external_toc_strict-1.1.3/tests/test_version_semantic.py`

 * *Files identical despite different names*

### Comparing `sphinx_external_toc_strict-1.1.2/tox.ini` & `sphinx_external_toc_strict-1.1.3/tox.ini`

 * *Files identical despite different names*

