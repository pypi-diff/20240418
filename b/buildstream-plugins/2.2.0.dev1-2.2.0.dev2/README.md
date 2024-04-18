# Comparing `tmp/buildstream-plugins-2.2.0.dev1.tar.gz` & `tmp/buildstream-plugins-2.2.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildstream-plugins-2.2.0.dev1.tar", last modified: Wed Apr 17 10:05:12 2024, max compression
+gzip compressed data, was "buildstream-plugins-2.2.0.dev2.tar", last modified: Thu Apr 18 16:24:30 2024, max compression
```

## Comparing `buildstream-plugins-2.2.0.dev1.tar` & `buildstream-plugins-2.2.0.dev2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      797 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/.asf.yaml
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4135 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/projectconfig.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2966 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/userconfig.yaml
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1505 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/compose.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1517 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/filter.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      995 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/import.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      964 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/manual.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1485 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/script.yaml
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3675 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/autotools.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1927 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/cmake.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1438 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/make.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2098 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/meson.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1255 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/pip.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1363 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/setuptools.yaml
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2446 2024-04-17 09:10:06.000000 buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/markdown_it/port.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1350 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/COMMITTERS.rst
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    11358 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/LICENSE
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      152 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/MANIFEST.in
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2183 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/NEWS
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      167 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/NOTICE
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1742 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/PKG-INFO
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      443 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/README.rst
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      985 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/project.conf
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      989 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/pyproject.toml
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/requirements/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       79 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/requirements/mypy-requirements.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      177 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/requirements/plugin-requirements.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      163 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/requirements/test-requirements.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      561 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/setup.cfg
--rwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4076 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/setup.py
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/src/
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.141885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      654 2024-04-17 09:07:37.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/__init__.py
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/__init__.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2297 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3675 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2259 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1927 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1775 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1438 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2114 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2098 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1566 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1255 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.yaml
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1675 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1363 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.yaml
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/__init__.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4261 2024-04-17 09:06:46.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/_utils.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     8486 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/bzr.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    15309 2024-04-17 09:06:46.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/cargo.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    23204 2024-04-07 14:36:16.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/docker.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    39482 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/git.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3510 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/patch.py
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     9290 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/pip.py
-drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-17 10:05:12.145885 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1742 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/PKG-INFO
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2579 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        1 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      612 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/entry_points.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        1 2024-04-04 13:11:50.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/not-zip-safe
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       48 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/requires.txt
--rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       20 2024-04-17 10:05:12.000000 buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/top_level.txt
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.978535 buildstream-plugins-2.2.0.dev2/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      797 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/.asf.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.974535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/data/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4135 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/data/projectconfig.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2966 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/data/userconfig.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.974535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1505 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/compose.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1517 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/filter.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      995 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/import.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      964 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/manual.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1485 2024-04-04 13:12:42.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/script.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.974535 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3675 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/autotools.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1927 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/cmake.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1438 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/make.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2098 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/meson.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1255 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/pip.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1363 2024-04-07 17:21:50.000000 buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/setuptools.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/release/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/release/lib/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/release/lib/python3.11/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/.tox/release/lib/python3.11/site-packages/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.974535 buildstream-plugins-2.2.0.dev2/.tox/release/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2446 2024-04-17 09:10:06.000000 buildstream-plugins-2.2.0.dev2/.tox/release/lib/python3.11/site-packages/markdown_it/port.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1350 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/COMMITTERS.rst
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    11358 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/LICENSE
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      152 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/MANIFEST.in
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2537 2024-04-18 08:39:29.000000 buildstream-plugins-2.2.0.dev2/NEWS
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      167 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/NOTICE
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1742 2024-04-18 16:24:30.978535 buildstream-plugins-2.2.0.dev2/PKG-INFO
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      443 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/README.rst
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      985 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/project.conf
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      989 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/pyproject.toml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.974535 buildstream-plugins-2.2.0.dev2/requirements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       79 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/requirements/mypy-requirements.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      177 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/requirements/plugin-requirements.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      163 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/requirements/test-requirements.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      561 2024-04-18 16:24:30.982535 buildstream-plugins-2.2.0.dev2/setup.cfg
+-rwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4076 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/setup.py
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.970535 buildstream-plugins-2.2.0.dev2/src/
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.978535 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      654 2024-04-18 14:01:01.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/__init__.py
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.978535 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/__init__.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2297 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/autotools.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3675 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/autotools.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2259 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/cmake.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1927 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/cmake.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1775 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/make.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1438 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/make.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2114 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/meson.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2098 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/meson.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1566 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/pip.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1255 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/pip.yaml
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1675 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/setuptools.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1363 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/setuptools.yaml
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.978535 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/__init__.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     4261 2024-04-17 09:06:46.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/_utils.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     8486 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/bzr.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    15309 2024-04-17 09:06:46.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/cargo.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    23204 2024-04-07 14:36:16.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/docker.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)    39482 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/git.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     3510 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/patch.py
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     9290 2023-10-16 16:49:42.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/pip.py
+drwxr-xr-x   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        0 2024-04-18 16:24:30.978535 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     1742 2024-04-18 16:24:30.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)     2579 2024-04-18 16:24:30.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        1 2024-04-18 16:24:30.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)      612 2024-04-18 16:24:30.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)        1 2024-04-04 13:11:50.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/not-zip-safe
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       48 2024-04-18 16:24:30.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/requires.txt
+-rw-r--r--   0 abderrahimkitouni  (1001) abderrahimkitouni  (1001)       20 2024-04-18 16:24:30.000000 buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/top_level.txt
```

### Comparing `buildstream-plugins-2.2.0.dev1/.asf.yaml` & `buildstream-plugins-2.2.0.dev2/.asf.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/projectconfig.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/data/projectconfig.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/data/userconfig.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/data/userconfig.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/compose.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/compose.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/filter.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/filter.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/import.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/import.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/manual.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/manual.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/script.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream/plugins/elements/script.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/autotools.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/autotools.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/cmake.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/cmake.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/make.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/make.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/meson.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/meson.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/pip.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/pip.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/setuptools.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/lint/lib/python3.11/site-packages/buildstream_plugins/elements/setuptools.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/.tox/release/lib/python3.11/site-packages/markdown_it/port.yaml` & `buildstream-plugins-2.2.0.dev2/.tox/release/lib/python3.11/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/COMMITTERS.rst` & `buildstream-plugins-2.2.0.dev2/COMMITTERS.rst`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/LICENSE` & `buildstream-plugins-2.2.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/NEWS` & `buildstream-plugins-2.2.0.dev2/NEWS`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,22 @@
 =========================
+buildstream-plugins 2.2.0
+=========================
+
+ o cargo: Fix mirroring (#55)
+
+ o cargo: Support authentication using .netrc (#57)
+
+ o docker: Fix authentication when using .netrc (#59)
+
+ o docker: Improve flexibility for mirroring (#58)
+
+ o cargo: Add support for source mirrors and bearer http authentication (#60, #64)
+
+=========================
 buildstream-plugins 2.1.0
 =========================
 
  o Guard against malformed URIs in cargo crates (#52)
 
 =========================
 buildstream-plugins 2.0.1
```

### Comparing `buildstream-plugins-2.2.0.dev1/PKG-INFO` & `buildstream-plugins-2.2.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildstream-plugins
-Version: 2.2.0.dev1
+Version: 2.2.0.dev2
 Summary: A collection of plugins for BuildStream.
 Home-page: https://buildstream.build
 Author: The Apache Software Foundation
 Author-email: dev@buildstream.apache.org
 License: Apache License Version 2.0
 Project-URL: Documentation, https://apache.github.io/buildstream-plugins/
 Project-URL: Source, https://github.com/apache/buildstream-plugins/
```

### Comparing `buildstream-plugins-2.2.0.dev1/project.conf` & `buildstream-plugins-2.2.0.dev2/project.conf`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/pyproject.toml` & `buildstream-plugins-2.2.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/setup.cfg` & `buildstream-plugins-2.2.0.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/setup.py` & `buildstream-plugins-2.2.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/__init__.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
 #
 # Remember to adjust this version number before tagging releases
 #
-__version__ = "2.2.0.dev1"
+__version__ = "2.2.0.dev2"
```

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/autotools.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/autotools.yaml` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/autotools.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/cmake.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/cmake.yaml` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/cmake.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/make.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/make.yaml` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/make.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/meson.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/meson.yaml` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/meson.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/pip.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/pip.yaml` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/pip.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/setuptools.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/elements/setuptools.yaml` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/elements/setuptools.yaml`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/_utils.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/_utils.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/bzr.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/bzr.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/cargo.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/cargo.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/docker.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/docker.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/git.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/git.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/patch.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/patch.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins/sources/pip.py` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins/sources/pip.py`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/PKG-INFO` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildstream-plugins
-Version: 2.2.0.dev1
+Version: 2.2.0.dev2
 Summary: A collection of plugins for BuildStream.
 Home-page: https://buildstream.build
 Author: The Apache Software Foundation
 Author-email: dev@buildstream.apache.org
 License: Apache License Version 2.0
 Project-URL: Documentation, https://apache.github.io/buildstream-plugins/
 Project-URL: Source, https://github.com/apache/buildstream-plugins/
```

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/SOURCES.txt` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildstream-plugins-2.2.0.dev1/src/buildstream_plugins.egg-info/entry_points.txt` & `buildstream-plugins-2.2.0.dev2/src/buildstream_plugins.egg-info/entry_points.txt`

 * *Files identical despite different names*

