# Comparing `tmp/macal-5.5.0a3.tar.gz` & `tmp/macal-5.5.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macal-5.5.0a3.tar", last modified: Tue Apr 16 21:59:08 2024, max compression
+gzip compressed data, was "macal-5.5.0a4.tar", last modified: Thu Apr 18 16:08:09 2024, max compression
```

## Comparing `macal-5.5.0a3.tar` & `macal-5.5.0a4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/.vscode/
--rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a3/.vscode/launch.json
--rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a3/.vscode/settings.json
--rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a3/LICENSE.txt
--rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a3/MANIFEST.in
--rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-16 21:59:08.076301 macal-5.5.0a3/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     4551 2024-04-16 13:27:36.000000 macal-5.5.0a3/README.md
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/documentation/
--rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a3/documentation/history.txt
--rw-r--r--   0 marco     (1000) marco     (1000)     1016 2024-04-16 21:58:56.000000 macal-5.5.0a3/pyproject.toml
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-16 21:59:08.076301 macal-5.5.0a3/setup.cfg
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/
--rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-15 16:33:22.000000 macal-5.5.0a3/src/macal/__about__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a3/src/macal/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/frontend/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a3/src/macal/frontend/__init__.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/frontend/ast/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a3/src/macal/frontend/ast/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a3/src/macal/frontend/ast/kind.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a3/src/macal/frontend/ast/metadata.py
--rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a3/src/macal/frontend/ast/node.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a3/src/macal/frontend/ast/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a3/src/macal/frontend/mlexer.py
--rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a3/src/macal/frontend/mparser.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a3/src/macal/frontend/mparserstate.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a3/src/macal/frontend/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     5713 2024-04-10 21:36:36.000000 macal-5.5.0a3/src/macal/macal.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a3/src/macal/mexceptions.py
--rw-r--r--   0 marco     (1000) marco     (1000)    11999 2024-04-16 21:53:55.000000 macal-5.5.0a3/src/macal/mrepl.py
--rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a3/src/macal/mrun.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a3/src/macal/py.typed
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/runtime/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a3/src/macal/runtime/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a3/src/macal/runtime/menvironment.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a3/src/macal/runtime/mimporter.py
--rw-r--r--   0 marco     (1000) marco     (1000)    77580 2024-04-15 14:47:24.000000 macal-5.5.0a3/src/macal/runtime/minterpreter.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal/runtime/native/
--rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a3/src/macal/runtime/native/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a3/src/macal/runtime/native/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a3/src/macal/runtime/native/system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a3/src/macal/runtime/native/time.py
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a3/src/macal/runtime/py.typed
--rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a3/src/macal/runtime/value_type.py
--rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a3/src/macal/runtime/values.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/src/macal.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-16 21:59:08.000000 macal-5.5.0a3/src/macal.egg-info/top_level.txt
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/tests/
--rw-r--r--   0 marco     (1000) marco     (1000)      980 2024-04-12 12:31:29.000000 macal-5.5.0a3/tests/agent.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-16 21:59:08.076301 macal-5.5.0a3/tests/lib/
--rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a3/tests/lib/csv.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_csv.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a3/tests/lib/ext_io.py
--rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_keyring.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_math.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a3/tests/lib/ext_strings.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_syslog.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a3/tests/lib/ext_system.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a3/tests/lib/ext_time.py
--rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a3/tests/lib/io.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a3/tests/lib/keyring.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a3/tests/lib/math.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a3/tests/lib/meraki_api_library_v1.py
--rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a3/tests/lib/meraki_v1.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a3/tests/lib/strings.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a3/tests/lib/syslog.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     2929 2024-04-10 19:31:44.000000 macal-5.5.0a3/tests/lib/system.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a3/tests/lib/time.mcl
--rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a3/tests/test.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/.vscode/
+-rw-r--r--   0 marco     (1000) marco     (1000)      540 2024-04-15 15:12:14.000000 macal-5.5.0a4/.vscode/launch.json
+-rw-r--r--   0 marco     (1000) marco     (1000)       51 2024-04-15 15:12:14.000000 macal-5.5.0a4/.vscode/settings.json
+-rw-r--r--   0 marco     (1000) marco     (1000)     1184 2024-03-22 12:04:18.000000 macal-5.5.0a4/LICENSE.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)      179 2024-04-16 17:31:53.000000 macal-5.5.0a4/MANIFEST.in
+-rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-18 16:08:09.928512 macal-5.5.0a4/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     4551 2024-04-16 13:27:36.000000 macal-5.5.0a4/README.md
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/documentation/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7076 2024-04-15 15:03:44.000000 macal-5.5.0a4/documentation/history.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)     1016 2024-04-16 21:58:56.000000 macal-5.5.0a4/pyproject.toml
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2024-04-18 16:08:09.928512 macal-5.5.0a4/setup.cfg
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/src/
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.918512 macal-5.5.0a4/src/macal/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1474 2024-04-18 13:46:47.000000 macal-5.5.0a4/src/macal/__about__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:11:34.000000 macal-5.5.0a4/src/macal/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/frontend/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:27.000000 macal-5.5.0a4/src/macal/frontend/__init__.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/frontend/ast/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:13:42.000000 macal-5.5.0a4/src/macal/frontend/ast/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2568 2024-04-08 13:40:36.000000 macal-5.5.0a4/src/macal/frontend/ast/kind.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1892 2024-04-08 20:08:54.000000 macal-5.5.0a4/src/macal/frontend/ast/metadata.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    32164 2024-04-09 13:34:29.000000 macal-5.5.0a4/src/macal/frontend/ast/node.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 23:39:28.000000 macal-5.5.0a4/src/macal/frontend/ast/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)    20787 2024-04-15 14:41:47.000000 macal-5.5.0a4/src/macal/frontend/mlexer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    49026 2024-04-16 21:09:39.000000 macal-5.5.0a4/src/macal/frontend/mparser.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5053 2024-04-16 15:52:59.000000 macal-5.5.0a4/src/macal/frontend/mparserstate.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:45.000000 macal-5.5.0a4/src/macal/frontend/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     5623 2024-04-18 13:45:52.000000 macal-5.5.0a4/src/macal/macal.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2172 2024-04-08 15:16:25.000000 macal-5.5.0a4/src/macal/mexceptions.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    15930 2024-04-18 16:03:02.000000 macal-5.5.0a4/src/macal/mrepl.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     7436 2024-04-15 17:26:42.000000 macal-5.5.0a4/src/macal/mrun.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-22 16:29:34.000000 macal-5.5.0a4/src/macal/py.typed
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/runtime/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-22 12:10:21.000000 macal-5.5.0a4/src/macal/runtime/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     9289 2024-04-16 15:54:17.000000 macal-5.5.0a4/src/macal/runtime/menvironment.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4011 2024-04-10 20:55:22.000000 macal-5.5.0a4/src/macal/runtime/mimporter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    72797 2024-04-18 13:35:19.000000 macal-5.5.0a4/src/macal/runtime/minterpreter.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal/runtime/native/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1285 2024-03-23 23:21:40.000000 macal-5.5.0a4/src/macal/runtime/native/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-24 20:22:17.000000 macal-5.5.0a4/src/macal/runtime/native/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     2129 2024-04-15 14:35:04.000000 macal-5.5.0a4/src/macal/runtime/native/system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1618 2024-03-24 06:01:49.000000 macal-5.5.0a4/src/macal/runtime/native/time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2024-03-23 18:22:52.000000 macal-5.5.0a4/src/macal/runtime/py.typed
+-rw-r--r--   0 marco     (1000) marco     (1000)     1705 2024-04-08 15:40:52.000000 macal-5.5.0a4/src/macal/runtime/value_type.py
+-rw-r--r--   0 marco     (1000) marco     (1000)    17433 2024-04-11 16:42:19.000000 macal-5.5.0a4/src/macal/runtime/values.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/src/macal.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     5367 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     1563 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       66 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       73 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        6 2024-04-18 16:08:09.000000 macal-5.5.0a4/src/macal.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/tests/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1030 2024-04-18 12:40:10.000000 macal-5.5.0a4/tests/agent.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2024-04-18 16:08:09.928512 macal-5.5.0a4/tests/lib/
+-rw-r--r--   0 marco     (1000) marco     (1000)      639 2023-11-17 02:10:51.000000 macal-5.5.0a4/tests/lib/csv.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      996 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_csv.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2135 2024-04-04 21:12:11.000000 macal-5.5.0a4/tests/lib/ext_io.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      873 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_keyring.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2265 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_math.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3810 2024-04-09 08:23:31.000000 macal-5.5.0a4/tests/lib/ext_strings.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4601 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_syslog.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4082 2024-04-10 19:30:13.000000 macal-5.5.0a4/tests/lib/ext_system.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1910 2023-11-17 14:12:28.000000 macal-5.5.0a4/tests/lib/ext_time.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      942 2024-04-04 21:00:01.000000 macal-5.5.0a4/tests/lib/io.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      808 2023-11-17 02:12:56.000000 macal-5.5.0a4/tests/lib/keyring.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     1329 2024-04-05 15:54:51.000000 macal-5.5.0a4/tests/lib/math.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)    34808 2024-04-10 20:24:42.000000 macal-5.5.0a4/tests/lib/meraki_api_library_v1.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     5577 2024-04-10 20:38:33.000000 macal-5.5.0a4/tests/lib/meraki_v1.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2047 2023-11-27 14:53:48.000000 macal-5.5.0a4/tests/lib/strings.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      661 2023-11-17 02:14:43.000000 macal-5.5.0a4/tests/lib/syslog.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     2923 2024-04-18 14:01:00.000000 macal-5.5.0a4/tests/lib/system.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)      991 2023-11-17 02:16:00.000000 macal-5.5.0a4/tests/lib/time.mcl
+-rw-r--r--   0 marco     (1000) marco     (1000)     5867 2024-04-09 23:07:14.000000 macal-5.5.0a4/tests/test.py
```

### Comparing `macal-5.5.0a3/.vscode/launch.json` & `macal-5.5.0a4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/LICENSE.txt` & `macal-5.5.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/PKG-INFO` & `macal-5.5.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macal
-Version: 5.5.0a3
+Version: 5.5.0a4
 Summary: Macal DSL is used for collecting and transforming data from various sources.
 Author-email: Marco Caspers <SamaDevTeam@westcon.com>
 Project-URL: Homepage, https://github.com/Sama-Developer/macal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `macal-5.5.0a3/README.md` & `macal-5.5.0a4/README.md`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/documentation/history.txt` & `macal-5.5.0a4/documentation/history.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/pyproject.toml` & `macal-5.5.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/__about__.py` & `macal-5.5.0a4/src/macal/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # SPDX-License-Identifier: MIT
 #
 
-__version__ = "5.5.0.alpha.3"
+__version__ = "5.5.0.alpha.4"
 __author__ = "Marco Caspers"
 __email__ = "samadevteam@westcon.com"
 __copyright__ = "Copyright 2024 Westcon Sama Development Team"
 __license__ = "MIT License"
```

### Comparing `macal-5.5.0a3/src/macal/__init__.py` & `macal-5.5.0a4/src/macal/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/__init__.py` & `macal-5.5.0a4/src/macal/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/ast/__init__.py` & `macal-5.5.0a4/src/macal/frontend/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/ast/kind.py` & `macal-5.5.0a4/src/macal/frontend/ast/kind.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/ast/metadata.py` & `macal-5.5.0a4/src/macal/frontend/ast/metadata.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/ast/node.py` & `macal-5.5.0a4/src/macal/frontend/ast/node.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/mlexer.py` & `macal-5.5.0a4/src/macal/frontend/mlexer.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/mparser.py` & `macal-5.5.0a4/src/macal/frontend/mparser.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/frontend/mparserstate.py` & `macal-5.5.0a4/src/macal/frontend/mparserstate.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/macal.py` & `macal-5.5.0a4/src/macal/macal.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,107 +49,104 @@
     ArrayObject,
     NodeMetadata,
     HaltValue,
 )
 
 
 class Macal:
-    def __init__(self, filename: str) -> None:
-        self.__filename: str = filename
+
+    def __init__(self, search_paths: list[str] = []) -> None:
         self.__environment: Env = Env.CreateGlobalEnv()
         self.__parser_state = ParserState(
-            name="global", parent=None, filename=filename
+            name="global", parent=None, filename=""
         )  # global environment state.
-        self.__paths: list[str] = []
-        self.__version__: str = __version__
+        self._search_paths: list[str] = search_paths
+        self._version: str = __version__
 
     @property
     def version(self) -> str:
-        return self.__version__
+        return self._version
 
     @property
     def paths(self) -> list[str]:
-        return self.__paths
+        return self._search_paths
 
-    def add_path(self, path: str) -> None:
-        self.__paths.append(path)
+    def AddPath(self, path: str) -> None:
+        self._search_paths.append(path)
 
-    def remove_path(self, path: str) -> None:
-        self.__paths.remove(path)
+    def RemovePath(self, path: str) -> None:
+        self._search_paths.remove(path)
 
-    def __convert(self, value: Any, env: Env) -> IRuntimeValue:
+    def _convert(self, value: Any, env: Env) -> IRuntimeValue:
         """Converts a Python value to a Macal value."""
         if value is None:
             return NilValue()
         if isinstance(value, bool):
             return BooleanValue(value)
         if isinstance(value, int):
             return IntegerValue(value)
         if isinstance(value, float):
             return FloatValue(value)
         if isinstance(value, str):
             return StringValue(value, NodeMetadata.new())
         if isinstance(value, dict):
             record = RecordObject(NodeMetadata.new())
             for key, val in value.items():
-                record.properties[key] = self.__convert(val, env)
+                record.properties[key] = self._convert(val, env)
             return record
         if isinstance(value, list):
             array = ArrayObject(NodeMetadata.new())
             for val in value:
-                array.append(self.__convert(val, env))
+                array.append(self._convert(val, env))
             return array
         raise RuntimeError(f"Unknown Python value type: {type(value)}")
 
-    def add_variable(self, name: str, value: Any) -> None:
+    def RegisterVariable(self, name: str, value: Any) -> None:
         """Add a variable to the global environment."""
         symbol = ParserSymbol(name, NodeMetadata.new(), is_global=True, is_const=False)
         self.__parser_state.symbols.append(symbol)
         self.__environment.DeclareVar(
-            name, value=self.__convert(value, env=self.__environment)
+            name, value=self._convert(value, env=self.__environment)
         )
 
-    def add_const(self, name: str, value: Any) -> None:
+    def RegisterConstant(self, name: str, value: Any) -> None:
         """Add a const to the global environment."""
         symbol = ParserSymbol(name, NodeMetadata.new(), is_global=True, is_const=True)
         self.__parser_state.symbols.append(symbol)
         self.__environment.DeclareVar(
-            name, value=self.__convert(value, env=self.__environment)
+            name, value=self._convert(value, env=self.__environment)
         )
 
-    def Run(self) -> None:
+    def AssignVariable(self, name: str, value: Any) -> None:
+        """Assign a value to a variable in the global environment."""
+
+        self.__environment.AssignVar(
+            name=name, value=self._convert(value, env=self.__environment), meta=None
+        )
+
+    def Run(self, filename: str) -> None:
         """Run a Macal file."""
         try:
-            with open(self.__filename, "r") as f:
-                source = f.read()
-            parser = Parser(self.__filename)
-            program = parser.ProduceAST(source, state=self.__parser_state)
-
-            interpreter = Interpreter()
-            for path in self.__paths:
-                interpreter.add_path(str(pathlib.Path(path).absolute()))
-            ret = interpreter.evaluate(program, self.__environment)
-            if isinstance(ret, HaltValue):
-                sys.exit(ret.value.value)
+            self.RunUnsafe(filename=filename, debug=False)
         except RuntimeErrorLC as e:
             print(f"{e}")
             sys.exit(1)
         except SyntaxError as e:
             print(f"{e}")
             sys.exit(1)
         except RuntimeError as e:
             print(f"{e}")
             sys.exit(1)
 
-    def RunDebug(self) -> None:
+    def RunUnsafe(self, filename: str, debug: bool = False) -> None:
         """Run a Macal file in debug mode, without any crash protections."""
-
-        with open(self.__filename, "r") as f:
+        with open(filename, "r") as f:
             source = f.read()
-        parser = Parser(self.__filename)
-        program = parser.ProduceAST(source, state=self.__parser_state, debug=True)
+        self.__parser_state.filename = filename
+        parser = Parser(filename)
+        program = parser.ProduceAST(source, state=self.__parser_state, debug=debug)
         interpreter = Interpreter()
-        for path in self.__paths:
+        for path in self._search_paths:
             interpreter.add_path(str(pathlib.Path(path).absolute()))
         ret = interpreter.evaluate(program, self.__environment)
         if isinstance(ret, HaltValue):
             sys.exit(ret.value.value)
```

### Comparing `macal-5.5.0a3/src/macal/mexceptions.py` & `macal-5.5.0a4/src/macal/mexceptions.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/mrun.py` & `macal-5.5.0a4/src/macal/mrun.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/__init__.py` & `macal-5.5.0a4/src/macal/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/menvironment.py` & `macal-5.5.0a4/src/macal/runtime/menvironment.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/mimporter.py` & `macal-5.5.0a4/src/macal/runtime/mimporter.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/minterpreter.py` & `macal-5.5.0a4/src/macal/runtime/minterpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,18 @@
         else:
             raise RuntimeError(
                 f"Unsupported binary operation '{op}' for value of type '{lhs.type}'."
             )
 
     def _eval_binary(self, expr: BinaryExpr, env: Env) -> IRuntimeValue:
         lhs = self.evaluate(expr.left, env)
+        if expr.operator in ["&&", "and", "&"] and lhs.value is False:
+            return BooleanValue(False)
+        if expr.operator in ["||", "or", "|"] and lhs.value is True:
+            return BooleanValue(True)
         rhs = self.evaluate(expr.right, env)
         return self._eval_binary_expr(lhs, rhs, expr.operator)
 
     def _eval_unary(self, expr: UnaryExpr, env: Env) -> IRuntimeValue:
         rhs = self.evaluate(expr.right, env)
         if expr.operator == "-":
             if isinstance(rhs, IntegerValue):
@@ -774,17 +778,15 @@
             raise RuntimeError(f"Invalid record literal {node}")
         if node.properties is None or len(node.properties) == 0:
             return RecordObject(node.metadata)
         obj = RecordObject(node.metadata)
         for prop in node.properties:
             if prop.key is None:
                 raise RuntimeErrorLC(
-                    f"Invalid record property {prop.key}",
-                    node.metadata.line,
-                    node.metadata.column,
+                    f"Invalid record property {prop.key}", node.metadata
                 )
             obj.properties[prop.key] = self.evaluate(prop, env)  #
         return obj
 
     def _eval_object(self, node: ObjectLiteral, env: Env) -> IRuntimeValue:
         if node.okind == ObjectKind.ARRAY:
             return self._eval_array(node, env)
@@ -1140,36 +1142,14 @@
         # When we get here we have to evaluate the default case if it exists
         if switch_stmt.default_case is not None and isinstance(
             switch_stmt.default_case, DefaultCaseStatement
         ):
             return self._run_matched_default_case(switch_stmt.default_case, env)
         return NilValue()
 
-    def _eval_where(
-        self, where_expr: IExpr, source_data: list[dict[str, Any]], env: Env
-    ):
-        scope = env.create_child_env(f"{env.name}_select_where")
-        for key in source_data[0].keys():
-            scope.DeclareVar(key, NilValue(), NodeMetadata.new(), True)
-        where_filtered_data: list[dict[str, Any]] = []
-        for row in source_data:
-            for key, val in row.items():
-                scope._set_var(key, self.__pconvert(val, env))
-            condition = self.evaluate(where_expr, scope)
-            if condition.type != ValueType.Boolean:
-                raise RuntimeErrorLC(
-                    "Where condition must be a boolean value.", where_expr.metadata
-                )
-            if condition.value is True:
-                where_filtered_data.append(row)
-        result_data: list[dict[str, Any]] = []
-        for row in where_filtered_data:
-            result_data.append({key: self.__mconvert(val) for key, val in row.items()})
-        return result_data
-
     def _eval_where_ex(self, where_expr: IExpr, source_data: ArrayObject, env: Env):
         scope = env.create_child_env(f"{env.name}_select_where")
         if isinstance(source_data.elements[0], RecordObject):
             sdr = source_data.elements[0]
             sdk = sdr.properties.keys()
         else:
             raise RuntimeErrorLC(
@@ -1192,22 +1172,14 @@
                     f"Where condition must be a boolean value {condition.type.name}",
                     where_expr.metadata,
                 )
             if condition.value is True:
                 where_filtered_data.append(row)
         return where_filtered_data
 
-    def _filter_fields(self, source: list[dict[str, Any]], fields: list[SelectField]):
-        if len(fields) == 1 and fields[0].field == "*":
-            return source
-        return [
-            {field.alias: row.get(field.field, None) for field in fields}
-            for row in source
-        ]
-
     def _filter_fields_ex(self, source: ArrayObject, fields: list[SelectField]):
         if len(fields) == 1 and fields[0].field == "*":
             return source
         source.Reset()  # reset the iterator.
         result: ArrayObject = ArrayObject(source.metadata)  # type: ignore
         while True:
             row = source.Next()
@@ -1311,104 +1283,14 @@
             return "array"
         if isinstance(value, dict):
             return "record"
         if isinstance(value, callable):  # type: ignore
             return "function"
         return "unknown"
 
-    def _eval_select(self, stmt: IStmt, env: Env) -> IRuntimeValue:
-        return self._eval_select_ex(stmt, env)
-        if not isinstance(stmt, SelectStatement):
-            raise RuntimeErrorLC("Invalid select statement", stmt.metadata)
-        destination_data: Union[list[dict[str, Any]], dict[str, Any]] = []
-
-        merge = stmt.merge
-        if merge is True:
-            dd = self.evaluate(stmt.into_expr, env)
-            if dd is None:
-                raise RuntimeErrorLC(
-                    "Into variable not found for select statement",
-                    stmt.into_expr.metadata,
-                )
-            destination_data = self.__mconvert(dd)
-            if isinstance(destination_data, dict):
-                destination_data = [destination_data]
-
-        sd = self.evaluate(stmt.from_expr, env)
-        source_data: list[dict[str, Any]]
-        if isinstance(sd, BooleanValue):
-            source_data = []
-        elif sd is None or isinstance(sd, NilValue) or sd == "nil":
-            source_data = []
-        else:
-            source_data = self.__mconvert(sd)
-
-        if not isinstance(source_data, list) and not isinstance(source_data, dict):
-            raise RuntimeErrorLC(
-                f"Invalid source data for select statement, expected record or array, got {self._python_type_to_macal_type(source_data)}",
-                stmt.from_expr.metadata,
-            )
-
-        if isinstance(source_data, dict):
-            source_data = [source_data]
-
-        if stmt.where_expr is not None and len(source_data) > 0:
-            source_data = self._eval_where(stmt.where_expr, source_data, env)
-
-        if len(source_data) >= 1:
-            source_data = self._filter_fields(source_data, stmt.fields)
-
-        # merge requires both datasets to be a list of dicts.
-        if len(destination_data) > 0 and isinstance(destination_data, dict):
-            destination_data = [destination_data]
-        elif (
-            len(destination_data) == 0
-            or destination_data is None
-            or destination_data is False
-            or isinstance(destination_data, NilValue)
-            or destination_data == "nil"
-        ):
-            destination_data = []
-
-        if len(source_data) > 0 and isinstance(source_data, dict):
-            source_data = [source_data]
-        elif (
-            len(source_data) == 0
-            or source_data is None
-            or source_data is False
-            or isinstance(source_data, NilValue)
-            or source_data == "nil"
-        ):
-            source_data = []
-
-        if merge is True:
-            destination_data = self._merge_data(source_data, destination_data)  # type: ignore
-            if len(destination_data) == 1 and isinstance(destination_data, list):
-                destination_data = destination_data[0]
-        else:
-            destination_data = source_data.copy()
-
-        if stmt.distinct is True:
-            if isinstance(destination_data, list) and len(destination_data) > 0:
-                destination_data = destination_data[0]
-            if isinstance(destination_data, dict) and len(destination_data) == 1:
-                destination_data = [v for _, v in destination_data.items()]
-                destination_data = destination_data[0]
-
-        if isinstance(destination_data, list) and (
-            (stmt.distinct is True and len(destination_data) > 0)
-            # or (len(destination_data) == 1)
-        ):
-            destination_data = destination_data[0]
-
-        self._set_select_into(
-            stmt.into_expr, self.__pconvert(destination_data, env), env
-        )
-        return NilValue()
-
     def _eval_select_ex(self, stmt: IStmt, env: Env) -> IRuntimeValue:
         if not isinstance(stmt, SelectStatement):
             raise RuntimeErrorLC("Invalid select statement", stmt.metadata)
         destination_data: Union[ArrayObject, RecordObject]
         merge = stmt.merge
         if merge is True:
             destination_data = self.evaluate(stmt.into_expr, env)  # type: ignore
@@ -1464,15 +1346,15 @@
                 destination_data = destination_data.elements[0]  # type: ignore
             if (
                 isinstance(destination_data, RecordObject)
                 and len(destination_data.columns) == 1
             ):
                 destination_data = destination_data.properties[
                     destination_data.columns[0]
-                ]
+                ]  # type: ignore
 
         if isinstance(destination_data, ArrayObject) and (
             (stmt.distinct is True and destination_data.length > 0)
             # or (destination_data.length == 1)
         ):
             destination_data = destination_data.elements[0]  # type: ignore
```

### Comparing `macal-5.5.0a3/src/macal/runtime/native/__init__.py` & `macal-5.5.0a4/src/macal/runtime/native/__init__.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/native/system.py` & `macal-5.5.0a4/src/macal/runtime/native/system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/native/time.py` & `macal-5.5.0a4/src/macal/runtime/native/time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/value_type.py` & `macal-5.5.0a4/src/macal/runtime/value_type.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal/runtime/values.py` & `macal-5.5.0a4/src/macal/runtime/values.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/src/macal.egg-info/PKG-INFO` & `macal-5.5.0a4/src/macal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macal
-Version: 5.5.0a3
+Version: 5.5.0a4
 Summary: Macal DSL is used for collecting and transforming data from various sources.
 Author-email: Marco Caspers <SamaDevTeam@westcon.com>
 Project-URL: Homepage, https://github.com/Sama-Developer/macal
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `macal-5.5.0a3/src/macal.egg-info/SOURCES.txt` & `macal-5.5.0a4/src/macal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/agent.py` & `macal-5.5.0a4/tests/agent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-from macal.macal import Macal
+from macal.macal import Macal  # type: ignore
 import json
 from dotenv import load_dotenv
 import os
 import sys
 
 sys.path.append("./meraki_scripts")
 
 
 def main() -> None:
     load_dotenv("./meraki_scripts/.env")
-    macal = Macal("./meraki_scripts/meraki_v11.mcl")
-    macal.add_path("./lib")
-    macal.add_path("./meraki_scripts")
+    search_paths = ["./lib", "./meraki_scripts"]
+    macal = Macal(search_paths=search_paths)
 
     with open("./meraki_scripts/meraki_api_agent_configuration.json") as f:
         config = json.load(f)
 
-    macal.add_const("configuration", config)
-    macal.add_variable("api_key", os.getenv("api_key"))
-    macal.add_variable("org_name", os.getenv("org_name"))
-    macal.add_variable("host_name", os.getenv("host_name"))
-    macal.add_variable("agent_version", "Meraki API Agent v10.1.0")
-    macal.add_variable("org_id", None)
+    macal.RegisterConstant("configuration", config)
+    macal.RegisterVariable("api_key", os.getenv("api_key"))
+    macal.RegisterVariable("org_name", os.getenv("org_name"))
+    macal.RegisterVariable("host_name", os.getenv("host_name"))
+    macal.RegisterVariable("agent_version", "Meraki API Agent v10.1.0")
+    macal.RegisterVariable("org_id", None)
     print()
     print("Running Meraki API Agent v10.1.0, please wait...")
     print()
-    macal.Run()
+    macal.Run("./meraki_scripts/meraki_v11.mcl")
     print()
     print("Meraki API Agent v10.1.0 has completed successfully.")
     print()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `macal-5.5.0a3/tests/lib/csv.mcl` & `macal-5.5.0a4/tests/lib/csv.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_csv.py` & `macal-5.5.0a4/tests/lib/ext_csv.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_io.py` & `macal-5.5.0a4/tests/lib/ext_io.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_keyring.py` & `macal-5.5.0a4/tests/lib/ext_keyring.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_math.py` & `macal-5.5.0a4/tests/lib/ext_math.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_strings.py` & `macal-5.5.0a4/tests/lib/ext_strings.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_syslog.py` & `macal-5.5.0a4/tests/lib/ext_syslog.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_system.py` & `macal-5.5.0a4/tests/lib/ext_system.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/ext_time.py` & `macal-5.5.0a4/tests/lib/ext_time.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/io.mcl` & `macal-5.5.0a4/tests/lib/io.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/keyring.mcl` & `macal-5.5.0a4/tests/lib/keyring.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/math.mcl` & `macal-5.5.0a4/tests/lib/math.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/meraki_api_library_v1.py` & `macal-5.5.0a4/tests/lib/meraki_api_library_v1.py`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/meraki_v1.mcl` & `macal-5.5.0a4/tests/lib/meraki_v1.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/strings.mcl` & `macal-5.5.0a4/tests/lib/strings.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/syslog.mcl` & `macal-5.5.0a4/tests/lib/syslog.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/lib/system.mcl` & `macal-5.5.0a4/tests/lib/system.mcl`

 * *Files 4% similar despite different names*

```diff
@@ -42,19 +42,19 @@
     Also added LoadEnv to make use of the dotenv library's capability to load system variables from a .env file.
     Path to the file is an optional argument.
 
 */
 
 const system = object {
     name: "system",
-    version: "5.5.0.alpha.1",
+    version: "5.5.0",
     author: "Marco Caspers",
     email: "SamaDevTeam@westcon.com",
     license: "MIT",
-    description: "This is the Macal DSL 6 System Library",
+    description: "This is the Macal DSL 5.5 System Library",
     external_module: "system.py"
 };
 
 Console => (params args) external 'ext_system', 'Console';
 Print => (params args) external 'ext_system', 'Console';
 
 Array => (params args) external 'ext_system', 'Array';
```

### Comparing `macal-5.5.0a3/tests/lib/time.mcl` & `macal-5.5.0a4/tests/lib/time.mcl`

 * *Files identical despite different names*

### Comparing `macal-5.5.0a3/tests/test.py` & `macal-5.5.0a4/tests/test.py`

 * *Files identical despite different names*

