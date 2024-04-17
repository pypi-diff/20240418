# Comparing `tmp/hdeps-1.2.0.tar.gz` & `tmp/hdeps-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdeps-1.2.0.tar", last modified: Tue Mar 19 20:51:15 2024, max compression
+gzip compressed data, was "hdeps-1.3.0.tar", last modified: Wed Apr 17 22:42:30 2024, max compression
```

## Comparing `hdeps-1.2.0.tar` & `hdeps-1.3.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.919011 hdeps-1.2.0/
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.852346 hdeps-1.2.0/.github/
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.859012 hdeps-1.2.0/.github/workflows/
--rw-r--r--   0 tim       (1000) tim       (1000)     1425 2024-02-22 00:00:21.000000 hdeps-1.2.0/.github/workflows/build.yml
--rw-r--r--   0 tim       (1000) tim       (1000)     1242 2024-02-22 00:00:21.000000 hdeps-1.2.0/.gitignore
--rw-r--r--   0 tim       (1000) tim       (1000)      257 2024-02-12 22:16:45.000000 hdeps-1.2.0/.vars.ini
--rw-r--r--   0 tim       (1000) tim       (1000)     1133 2024-02-22 00:00:21.000000 hdeps-1.2.0/LICENSE
--rw-r--r--   0 tim       (1000) tim       (1000)       51 2024-02-12 22:16:45.000000 hdeps-1.2.0/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)      992 2024-02-22 00:01:20.000000 hdeps-1.2.0/Makefile
--rw-r--r--   0 tim       (1000) tim       (1000)     1778 2024-03-19 20:51:15.919011 hdeps-1.2.0/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     1446 2024-02-22 00:00:21.000000 hdeps-1.2.0/README.md
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.889011 hdeps-1.2.0/hdeps/
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-12 22:16:45.000000 hdeps-1.2.0/hdeps/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1592 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/cache.py
--rw-r--r--   0 tim       (1000) tim       (1000)     6789 2024-03-19 20:50:30.000000 hdeps-1.2.0/hdeps/cli.py
--rw-r--r--   0 tim       (1000) tim       (1000)     4776 2024-03-19 20:50:30.000000 hdeps-1.2.0/hdeps/compatibility.py
--rw-r--r--   0 tim       (1000) tim       (1000)     2034 2024-02-15 00:30:20.000000 hdeps-1.2.0/hdeps/markers.py
--rw-r--r--   0 tim       (1000) tim       (1000)    10210 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/projects.py
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-12 22:16:45.000000 hdeps-1.2.0/hdeps/py.typed
--rw-r--r--   0 tim       (1000) tim       (1000)     1578 2024-02-14 22:11:07.000000 hdeps-1.2.0/hdeps/requirements.py
--rw-r--r--   0 tim       (1000) tim       (1000)    13700 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/resolution.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1474 2024-02-15 01:01:16.000000 hdeps-1.2.0/hdeps/session.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.899011 hdeps-1.2.0/hdeps/tests/
--rw-r--r--   0 tim       (1000) tim       (1000)      547 2024-03-19 20:50:30.000000 hdeps-1.2.0/hdeps/tests/__init__.py
--rw-r--r--   0 tim       (1000) tim       (1000)       97 2024-02-12 22:16:45.000000 hdeps-1.2.0/hdeps/tests/__main__.py
--rw-r--r--   0 tim       (1000) tim       (1000)     2481 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/_fake_session.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1620 2024-02-15 00:59:52.000000 hdeps-1.2.0/hdeps/tests/cache.py
--rw-r--r--   0 tim       (1000) tim       (1000)     3013 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/cli_scenarios.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1768 2024-03-19 20:50:30.000000 hdeps-1.2.0/hdeps/tests/compatibility.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.899011 hdeps-1.2.0/hdeps/tests/demo_project/
--rw-r--r--   0 tim       (1000) tim       (1000)      103 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/Makefile
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.902345 hdeps-1.2.0/hdeps/tests/demo_project/demo_project.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)      197 2024-02-20 05:05:32.000000 hdeps-1.2.0/hdeps/tests/demo_project/demo_project.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-02-20 05:05:32.000000 hdeps-1.2.0/hdeps/tests/demo_project/demo_project.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       74 2024-02-20 05:05:32.000000 hdeps-1.2.0/hdeps/tests/demo_project/demo_project.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-02-20 05:05:32.000000 hdeps-1.2.0/hdeps/tests/demo_project/demo_project.egg-info/top_level.txt
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.902345 hdeps-1.2.0/hdeps/tests/demo_project/dist/
--rw-r--r--   0 tim       (1000) tim       (1000)     1065 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0-py3-none-any.whl
--rw-r--r--   0 tim       (1000) tim       (1000)      824 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.bz2
--rw-r--r--   0 tim       (1000) tim       (1000)      782 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.gz
--rw-r--r--   0 tim       (1000) tim       (1000)      756 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.xz
--rw-r--r--   0 tim       (1000) tim       (1000)     2070 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.zip
--rw-r--r--   0 tim       (1000) tim       (1000)      191 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/demo_project/setup.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.909011 hdeps-1.2.0/hdeps/tests/fixtures/
--rw-r--r--   0 tim       (1000) tim       (1000)     1300 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/fixtures/CircularDependencyA-0.0.0.tar.gz
--rw-r--r--   0 tim       (1000) tim       (1000)     1304 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/fixtures/CircularDependencyB-0.0.0.tar.gz
--rw-r--r--   0 tim       (1000) tim       (1000)       39 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/batman-1.0-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/batman-2.0-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/fixtures/batman-2.1dev1234-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)      428 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/fixtures/batman.html
--rw-r--r--   0 tim       (1000) tim       (1000)       80 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/fixtures/circulardependencya.html
--rw-r--r--   0 tim       (1000) tim       (1000)       80 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/fixtures/circulardependencyb.html
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/pyver-3.10-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/pyver-3.6-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/pyver-3.7-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/pyver-3.8-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/pyver-3.9-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)      833 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/pyver.html
--rw-r--r--   0 tim       (1000) tim       (1000)       12 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/robin-1.0-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)       12 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/robin-2.0-py3-none-any.whl.metadata
--rw-r--r--   0 tim       (1000) tim       (1000)      273 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/fixtures/robin.html
--rw-r--r--   0 tim       (1000) tim       (1000)     1522 2024-02-14 20:55:17.000000 hdeps-1.2.0/hdeps/tests/markers.py
--rw-r--r--   0 tim       (1000) tim       (1000)     5294 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/tests/projects.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1411 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/requirements.py
--rw-r--r--   0 tim       (1000) tim       (1000)     2813 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/resolution.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.912344 hdeps-1.2.0/hdeps/tests/scenarios/
--rw-r--r--   0 tim       (1000) tim       (1000)      183 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_1.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      164 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_1_install_order.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      567 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_1_no_reuse.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      239 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_1_reuse.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      194 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_have_dep_nonpublic.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      159 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_have_nonpublic.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      233 2024-03-19 20:50:30.000000 hdeps-1.2.0/hdeps/tests/scenarios/batman_have_public.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      223 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/circular_dependency_sdist.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      367 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/color_conflict.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      451 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/color_legend.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      238 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/markers-in-feed.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      136 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/prerelease-dep.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      249 2024-03-12 22:19:14.000000 hdeps-1.2.0/hdeps/tests/scenarios/requires-python.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      446 2024-02-22 00:00:21.000000 hdeps-1.2.0/hdeps/tests/session.py
--rw-r--r--   0 tim       (1000) tim       (1000)     1016 2024-02-22 00:01:20.000000 hdeps-1.2.0/hdeps/types.py
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.892345 hdeps-1.2.0/hdeps.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     1778 2024-03-19 20:51:15.000000 hdeps-1.2.0/hdeps.egg-info/PKG-INFO
--rw-r--r--   0 tim       (1000) tim       (1000)     2875 2024-03-19 20:51:15.000000 hdeps-1.2.0/hdeps.egg-info/SOURCES.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-03-19 20:51:15.000000 hdeps-1.2.0/hdeps.egg-info/dependency_links.txt
--rw-r--r--   0 tim       (1000) tim       (1000)       41 2024-03-19 20:51:15.000000 hdeps-1.2.0/hdeps.egg-info/entry_points.txt
--rw-r--r--   0 tim       (1000) tim       (1000)      287 2024-03-19 20:51:15.000000 hdeps-1.2.0/hdeps.egg-info/requires.txt
--rw-r--r--   0 tim       (1000) tim       (1000)        6 2024-03-19 20:51:15.000000 hdeps-1.2.0/hdeps.egg-info/top_level.txt
-drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-03-19 20:51:15.912344 hdeps-1.2.0/scripts/
--rwxr-xr-x   0 tim       (1000) tim       (1000)     2286 2024-02-22 00:00:21.000000 hdeps-1.2.0/scripts/fixture-metadata-hashes
--rw-r--r--   0 tim       (1000) tim       (1000)     1603 2024-03-19 20:51:15.919011 hdeps-1.2.0/setup.cfg
--rw-r--r--   0 tim       (1000) tim       (1000)       58 2024-02-12 22:16:45.000000 hdeps-1.2.0/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.882372 hdeps-1.3.0/
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.872372 hdeps-1.3.0/.github/
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.875705 hdeps-1.3.0/.github/workflows/
+-rw-r--r--   0 tim       (1000) tim       (1000)     1425 2024-02-22 00:00:21.000000 hdeps-1.3.0/.github/workflows/build.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)     1242 2024-02-22 00:00:21.000000 hdeps-1.3.0/.gitignore
+-rw-r--r--   0 tim       (1000) tim       (1000)      257 2024-02-12 22:16:45.000000 hdeps-1.3.0/.vars.ini
+-rw-r--r--   0 tim       (1000) tim       (1000)     1133 2024-02-22 00:00:21.000000 hdeps-1.3.0/LICENSE
+-rw-r--r--   0 tim       (1000) tim       (1000)       51 2024-02-12 22:16:45.000000 hdeps-1.3.0/MANIFEST.in
+-rw-r--r--   0 tim       (1000) tim       (1000)      992 2024-02-22 00:01:20.000000 hdeps-1.3.0/Makefile
+-rw-r--r--   0 tim       (1000) tim       (1000)     1778 2024-04-17 22:42:30.882372 hdeps-1.3.0/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     1446 2024-02-22 00:00:21.000000 hdeps-1.3.0/README.md
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.875705 hdeps-1.3.0/hdeps/
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-12 22:16:45.000000 hdeps-1.3.0/hdeps/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1592 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/cache.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     6789 2024-03-19 20:50:30.000000 hdeps-1.3.0/hdeps/cli.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     4881 2024-04-17 22:42:07.000000 hdeps-1.3.0/hdeps/compatibility.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     2034 2024-02-15 00:30:20.000000 hdeps-1.3.0/hdeps/markers.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    10210 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/projects.py
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-12 22:16:45.000000 hdeps-1.3.0/hdeps/py.typed
+-rw-r--r--   0 tim       (1000) tim       (1000)     1578 2024-02-14 22:11:07.000000 hdeps-1.3.0/hdeps/requirements.py
+-rw-r--r--   0 tim       (1000) tim       (1000)    14178 2024-04-17 22:42:07.000000 hdeps-1.3.0/hdeps/resolution.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1474 2024-02-15 01:01:16.000000 hdeps-1.3.0/hdeps/session.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.879038 hdeps-1.3.0/hdeps/tests/
+-rw-r--r--   0 tim       (1000) tim       (1000)      547 2024-03-19 20:50:30.000000 hdeps-1.3.0/hdeps/tests/__init__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       97 2024-02-12 22:16:45.000000 hdeps-1.3.0/hdeps/tests/__main__.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     2481 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/_fake_session.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1620 2024-02-15 00:59:52.000000 hdeps-1.3.0/hdeps/tests/cache.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     3013 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/cli_scenarios.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1768 2024-03-19 20:50:30.000000 hdeps-1.3.0/hdeps/tests/compatibility.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.879038 hdeps-1.3.0/hdeps/tests/demo_project/
+-rw-r--r--   0 tim       (1000) tim       (1000)      103 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/Makefile
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.879038 hdeps-1.3.0/hdeps/tests/demo_project/demo_project.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)      197 2024-02-20 05:05:32.000000 hdeps-1.3.0/hdeps/tests/demo_project/demo_project.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-02-20 05:05:32.000000 hdeps-1.3.0/hdeps/tests/demo_project/demo_project.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       74 2024-02-20 05:05:32.000000 hdeps-1.3.0/hdeps/tests/demo_project/demo_project.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-02-20 05:05:32.000000 hdeps-1.3.0/hdeps/tests/demo_project/demo_project.egg-info/top_level.txt
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.879038 hdeps-1.3.0/hdeps/tests/demo_project/dist/
+-rw-r--r--   0 tim       (1000) tim       (1000)     1065 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0-py3-none-any.whl
+-rw-r--r--   0 tim       (1000) tim       (1000)      824 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.bz2
+-rw-r--r--   0 tim       (1000) tim       (1000)      782 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.gz
+-rw-r--r--   0 tim       (1000) tim       (1000)      756 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.xz
+-rw-r--r--   0 tim       (1000) tim       (1000)     2070 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.zip
+-rw-r--r--   0 tim       (1000) tim       (1000)      191 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/demo_project/setup.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.882372 hdeps-1.3.0/hdeps/tests/fixtures/
+-rw-r--r--   0 tim       (1000) tim       (1000)     1300 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/fixtures/CircularDependencyA-0.0.0.tar.gz
+-rw-r--r--   0 tim       (1000) tim       (1000)     1304 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/fixtures/CircularDependencyB-0.0.0.tar.gz
+-rw-r--r--   0 tim       (1000) tim       (1000)       39 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/batman-1.0-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/batman-2.0-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)       38 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/fixtures/batman-2.1dev1234-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)      428 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/fixtures/batman.html
+-rw-r--r--   0 tim       (1000) tim       (1000)       80 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/fixtures/circulardependencya.html
+-rw-r--r--   0 tim       (1000) tim       (1000)       80 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/fixtures/circulardependencyb.html
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/pyver-3.10-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/pyver-3.6-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/pyver-3.7-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/pyver-3.8-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)        0 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/pyver-3.9-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)      833 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/pyver.html
+-rw-r--r--   0 tim       (1000) tim       (1000)       12 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/robin-1.0-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)       12 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/robin-2.0-py3-none-any.whl.metadata
+-rw-r--r--   0 tim       (1000) tim       (1000)      273 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/fixtures/robin.html
+-rw-r--r--   0 tim       (1000) tim       (1000)     1522 2024-02-14 20:55:17.000000 hdeps-1.3.0/hdeps/tests/markers.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     5294 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/tests/projects.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1411 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/requirements.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     2813 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/resolution.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.882372 hdeps-1.3.0/hdeps/tests/scenarios/
+-rw-r--r--   0 tim       (1000) tim       (1000)      183 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_1.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      164 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_1_install_order.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      567 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_1_no_reuse.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      239 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_1_reuse.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      194 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_have_dep_nonpublic.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      159 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_have_nonpublic.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      233 2024-03-19 20:50:30.000000 hdeps-1.3.0/hdeps/tests/scenarios/batman_have_public.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      223 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/circular_dependency_sdist.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      367 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/color_conflict.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      451 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/color_legend.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      238 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/markers-in-feed.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      136 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/prerelease-dep.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      249 2024-03-12 22:19:14.000000 hdeps-1.3.0/hdeps/tests/scenarios/requires-python.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      446 2024-02-22 00:00:21.000000 hdeps-1.3.0/hdeps/tests/session.py
+-rw-r--r--   0 tim       (1000) tim       (1000)     1016 2024-02-22 00:01:20.000000 hdeps-1.3.0/hdeps/types.py
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.879038 hdeps-1.3.0/hdeps.egg-info/
+-rw-r--r--   0 tim       (1000) tim       (1000)     1778 2024-04-17 22:42:30.000000 hdeps-1.3.0/hdeps.egg-info/PKG-INFO
+-rw-r--r--   0 tim       (1000) tim       (1000)     2875 2024-04-17 22:42:30.000000 hdeps-1.3.0/hdeps.egg-info/SOURCES.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        1 2024-04-17 22:42:30.000000 hdeps-1.3.0/hdeps.egg-info/dependency_links.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)       41 2024-04-17 22:42:30.000000 hdeps-1.3.0/hdeps.egg-info/entry_points.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      287 2024-04-17 22:42:30.000000 hdeps-1.3.0/hdeps.egg-info/requires.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)        6 2024-04-17 22:42:30.000000 hdeps-1.3.0/hdeps.egg-info/top_level.txt
+drwxr-xr-x   0 tim       (1000) tim       (1000)        0 2024-04-17 22:42:30.882372 hdeps-1.3.0/scripts/
+-rwxr-xr-x   0 tim       (1000) tim       (1000)     2286 2024-02-22 00:00:21.000000 hdeps-1.3.0/scripts/fixture-metadata-hashes
+-rw-r--r--   0 tim       (1000) tim       (1000)     1603 2024-04-17 22:42:30.882372 hdeps-1.3.0/setup.cfg
+-rw-r--r--   0 tim       (1000) tim       (1000)       58 2024-02-12 22:16:45.000000 hdeps-1.3.0/setup.py
```

### Comparing `hdeps-1.2.0/.github/workflows/build.yml` & `hdeps-1.3.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/.gitignore` & `hdeps-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/LICENSE` & `hdeps-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/Makefile` & `hdeps-1.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/PKG-INFO` & `hdeps-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdeps
-Version: 1.2.0
+Version: 1.3.0
 Summary: Simple what-if dep resolution for python
 Home-page: https://github.com/hdeps/hdeps/
 Author: Tim Hatch
 Author-email: tim@timhatch.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hdeps-1.2.0/README.md` & `hdeps-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/cache.py` & `hdeps-1.3.0/hdeps/cache.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/cli.py` & `hdeps-1.3.0/hdeps/cli.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/compatibility.py` & `hdeps-1.3.0/hdeps/compatibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 from .markers import EnvironmentMarkers
 from .projects import Project
 from .types import VersionCallback
 
 LOG = logging.getLogger(__name__)
 
 
+class NoMatchingRelease(Exception):
+    pass
+
+
 def requires_python_match(
     project: Project, cache: Dict[str, bool], python_version: Version, v: Version
 ) -> bool:
     pv = project.versions[v]
     if not pv.requires_python:
         return True
     if (verdict := cache.get(pv.requires_python)) is not None:
@@ -89,36 +93,38 @@
     LOG.log(VLOG_2, "Callback %s -> %s", cur, cur_v)
 
     if already_chosen:
         possible.append(already_chosen)
 
     if not possible:
         if specifier_matched:
-            raise ValueError(
+            raise NoMatchingRelease(
                 f"{project.name} has no {python_version}-compatible release"
             )
         else:
-            raise ValueError(f"{project.name} has no release matching {req.specifier}")
+            raise NoMatchingRelease(
+                f"{project.name} has no release matching {req.specifier}"
+            )
 
     # The documentation for SepcifierSet.filter notes that it handles the logic
     # for whether to include prereleases, so we don't need that here.
     LOG.log(VLOG_1, "possible for %s: %s", req, possible)
     with kev("filter by specifier"):
         # This should only ever be ~3 items now!
         possible = list(req.specifier.filter(possible))
     if not possible:
         if not list(req.specifier.filter(project.versions.keys())):
             # Referencing the dragon above, if we had a current version and it was
             # unsuitable, then we still output a generic message.  Note that > does not
             # set the prerelease bit, but >= does.
-            raise ValueError(
+            raise NoMatchingRelease(
                 f"{project.name} has no release with constraint {req.specifier}"
             )
         else:
-            raise ValueError(
+            raise NoMatchingRelease(
                 f"{project.name} has no {python_version}-compatible release with constraint {req.specifier}"
             )
 
     # TODO: yanked support
 
     # The sort key is
     # ( matches_already_chosen: bool,
```

### Comparing `hdeps-1.2.0/hdeps/markers.py` & `hdeps-1.3.0/hdeps/markers.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/projects.py` & `hdeps-1.3.0/hdeps/projects.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/requirements.py` & `hdeps-1.3.0/hdeps/requirements.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/resolution.py` & `hdeps-1.3.0/hdeps/resolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 import click
 
 from keke import kev, ktrace
 
 from packaging.requirements import Requirement
 from packaging.utils import canonicalize_name
 from packaging.version import Version
-from pypi_simple import PyPISimple
+from pypi_simple import NoSuchProjectError, PyPISimple
 from requests.sessions import Session
 from vmodule import VLOG_1, VLOG_2
 
 # from tpe_prio import ThreadPoolExecutor
 
 from .cache import SimpleCache
 
-from .compatibility import find_best_compatible_version
+from .compatibility import find_best_compatible_version, NoMatchingRelease
 from .markers import EnvironmentMarkers
 from .projects import BasicMetadata, Project, ProjectVersion
 from .requirements import _iter_simple_requirements
 from .session import get_retry_session
 from .types import CanonicalName, Choice, ChoiceKeyType, Edge, VersionCallback
 
 LOG = logging.getLogger(__name__)
@@ -54,15 +54,15 @@
         self.pool = ThreadPoolExecutor(max_workers=parallelism)
         self.env_markers = env_markers
         self.pypi_simple = pypi_simple
         self.uncached_session = uncached_session or get_retry_session()
         self.extracted_metadata_cache = extracted_metadata_cache or SimpleCache()
         self.color = color
 
-        self.memo_fetch: Dict[CanonicalName, Future[Project]] = {}
+        self.memo_fetch: Dict[CanonicalName, Future[Optional[Project]]] = {}
         self.memo_fetch_lock = threading.Lock()
         self.memo_version_metadata: Dict[ProjectVersion, Future[BasicMetadata]] = {}
 
         self.queue: deque[
             Tuple[Choice, CanonicalName, Requirement, str, Set[ChoiceKeyType]]
         ] = deque()
         self.current_version_callback = current_version_callback
@@ -88,16 +88,21 @@
                     self._fetch_project, name, False
                 )
 
         empty_set: Set[ChoiceKeyType] = set()
         self.queue.append((self.root, name, req, source, empty_set))
 
     @ktrace("project_name", "proactive", shortname=True)
-    def _fetch_project(self, project_name: CanonicalName, proactive: bool) -> Project:
-        project_page = self.pypi_simple.get_project_page(project_name)
+    def _fetch_project(
+        self, project_name: CanonicalName, proactive: bool
+    ) -> Optional[Project]:
+        try:
+            project_page = self.pypi_simple.get_project_page(project_name)
+        except NoSuchProjectError:
+            return None
         project = Project.from_pypi_simple_project_page(project_page)
         # It's extremely likely that we will subsequently look up the deps of
         # the most recent version, so go ahead and schedule the metadata fetch.
         if project.versions:
             latest_version_key = max(project.versions)
             latest_version = project.versions[latest_version_key]
 
@@ -148,23 +153,31 @@
             )
             fut = self.memo_fetch[name]
             if hasattr(self.pool, "bump"):
                 self.pool.bump(fut)
             with kev("project result", project_name=name):
                 project = fut.result()
 
+            if project is None:
+                LOG.error("Missing dep processing %s", req, name)
+                continue
+
             cur = chosen.get(name)
             with kev("find_best_compatible_version", project_name=name, req=str(req)):
-                version = find_best_compatible_version(
-                    project,
-                    req,
-                    self.env_markers,
-                    cur,
-                    self.current_version_callback,
-                )
+                try:
+                    version = find_best_compatible_version(
+                        project,
+                        req,
+                        self.env_markers,
+                        cur,
+                        self.current_version_callback,
+                    )
+                except NoMatchingRelease:
+                    LOG.error("No matching version for %s processing %s", req, name)
+                    continue
             choice = Choice(name, version)
 
             edge = Edge(
                 choice, specifier=req.specifier, markers=req.marker, note=source
             )
             parent.deps.append(edge)
             if choice.key() in parent_keys:
```

### Comparing `hdeps-1.2.0/hdeps/session.py` & `hdeps-1.3.0/hdeps/session.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/__init__.py` & `hdeps-1.3.0/hdeps/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/_fake_session.py` & `hdeps-1.3.0/hdeps/tests/_fake_session.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/cache.py` & `hdeps-1.3.0/hdeps/tests/cache.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/cli_scenarios.py` & `hdeps-1.3.0/hdeps/tests/cli_scenarios.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/compatibility.py` & `hdeps-1.3.0/hdeps/tests/compatibility.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0-py3-none-any.whl` & `hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.bz2` & `hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.bz2`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.gz` & `hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.xz` & `hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.tar.xz`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.zip` & `hdeps-1.3.0/hdeps/tests/demo_project/dist/demo_project-0.0.0.zip`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/fixtures/CircularDependencyA-0.0.0.tar.gz` & `hdeps-1.3.0/hdeps/tests/fixtures/CircularDependencyA-0.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/fixtures/CircularDependencyB-0.0.0.tar.gz` & `hdeps-1.3.0/hdeps/tests/fixtures/CircularDependencyB-0.0.0.tar.gz`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/fixtures/pyver.html` & `hdeps-1.3.0/hdeps/tests/fixtures/pyver.html`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/markers.py` & `hdeps-1.3.0/hdeps/tests/markers.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/projects.py` & `hdeps-1.3.0/hdeps/tests/projects.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/requirements.py` & `hdeps-1.3.0/hdeps/tests/requirements.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/resolution.py` & `hdeps-1.3.0/hdeps/tests/resolution.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/tests/scenarios/batman_1_no_reuse.txt` & `hdeps-1.3.0/hdeps/tests/scenarios/batman_1_no_reuse.txt`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps/types.py` & `hdeps-1.3.0/hdeps/types.py`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/hdeps.egg-info/PKG-INFO` & `hdeps-1.3.0/hdeps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdeps
-Version: 1.2.0
+Version: 1.3.0
 Summary: Simple what-if dep resolution for python
 Home-page: https://github.com/hdeps/hdeps/
 Author: Tim Hatch
 Author-email: tim@timhatch.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `hdeps-1.2.0/hdeps.egg-info/SOURCES.txt` & `hdeps-1.3.0/hdeps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/scripts/fixture-metadata-hashes` & `hdeps-1.3.0/scripts/fixture-metadata-hashes`

 * *Files identical despite different names*

### Comparing `hdeps-1.2.0/setup.cfg` & `hdeps-1.3.0/setup.cfg`

 * *Files identical despite different names*

