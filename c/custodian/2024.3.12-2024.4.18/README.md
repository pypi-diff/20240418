# Comparing `tmp/custodian-2024.3.12.tar.gz` & `tmp/custodian-2024.4.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodian-2024.3.12.tar", last modified: Tue Mar 12 19:08:46 2024, max compression
+gzip compressed data, was "custodian-2024.4.18.tar", last modified: Thu Apr 18 14:11:14 2024, max compression
```

## Comparing `custodian-2024.3.12.tar` & `custodian-2024.4.18.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.505059 custodian-2024.3.12/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-12 19:08:37.000000 custodian-2024.3.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-03-12 19:08:46.501059 custodian-2024.3.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-03-12 19:08:37.000000 custodian-2024.3.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.493059 custodian-2024.3.12/custodian/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.497059 custodian-2024.3.12/custodian/ansible/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10819 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/ansible/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/ansible/interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.497059 custodian-2024.3.12/custodian/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cli/converge_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cli/converge_kpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cli/cstdn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cli/run_nwchem.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cli/run_vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.497059 custodian-2024.3.12/custodian/cp2k/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cp2k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45079 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cp2k/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cp2k/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13913 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cp2k/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cp2k/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/cp2k/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    38908 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.497059 custodian-2024.3.12/custodian/feff/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/feff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/feff/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/feff/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/feff/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.501059 custodian-2024.3.12/custodian/lobster/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/lobster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/lobster/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/lobster/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.501059 custodian-2024.3.12/custodian/nwchem/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/nwchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/nwchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/nwchem/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.501059 custodian-2024.3.12/custodian/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/qchem/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    33116 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/qchem/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/qchem/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.501059 custodian-2024.3.12/custodian/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84270 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/vasp/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/vasp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    41833 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-03-12 19:08:37.000000 custodian-2024.3.12/custodian/vasp/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.501059 custodian-2024.3.12/custodian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-03-12 19:08:46.000000 custodian-2024.3.12/custodian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-12 19:08:46.000000 custodian-2024.3.12/custodian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:08:46.000000 custodian-2024.3.12/custodian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-12 19:08:46.000000 custodian-2024.3.12/custodian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-12 19:08:46.000000 custodian-2024.3.12/custodian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 19:08:46.000000 custodian-2024.3.12/custodian.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-03-12 19:08:37.000000 custodian-2024.3.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 19:08:46.505059 custodian-2024.3.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:08:46.501059 custodian-2024.3.12/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9791 2024-03-12 19:08:38.000000 custodian-2024.3.12/tests/test_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-12 19:08:38.000000 custodian-2024.3.12/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.005005 custodian-2024.4.18/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-18 14:11:03.000000 custodian-2024.4.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-04-18 14:11:14.005005 custodian-2024.4.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4923 2024-04-18 14:11:03.000000 custodian-2024.4.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:13.997005 custodian-2024.4.18/custodian/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.001005 custodian-2024.4.18/custodian/ansible/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11303 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/ansible/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/ansible/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.001005 custodian-2024.4.18/custodian/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cli/converge_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cli/converge_kpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cli/cstdn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cli/run_nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cli/run_vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.001005 custodian-2024.4.18/custodian/cp2k/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cp2k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45023 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cp2k/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cp2k/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13945 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cp2k/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cp2k/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/cp2k/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38975 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.001005 custodian-2024.4.18/custodian/feff/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/feff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/feff/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/feff/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/feff/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.001005 custodian-2024.4.18/custodian/lobster/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/lobster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/lobster/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/lobster/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.001005 custodian-2024.4.18/custodian/nwchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/nwchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/nwchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/nwchem/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.005005 custodian-2024.4.18/custodian/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20860 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/qchem/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33140 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/qchem/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/qchem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.005005 custodian-2024.4.18/custodian/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84473 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/vasp/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/vasp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41899 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-04-18 14:11:03.000000 custodian-2024.4.18/custodian/vasp/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.005005 custodian-2024.4.18/custodian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8113 2024-04-18 14:11:13.000000 custodian-2024.4.18/custodian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-18 14:11:13.000000 custodian-2024.4.18/custodian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:11:13.000000 custodian-2024.4.18/custodian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-18 14:11:13.000000 custodian-2024.4.18/custodian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-18 14:11:13.000000 custodian-2024.4.18/custodian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-18 14:11:13.000000 custodian-2024.4.18/custodian.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-18 14:11:03.000000 custodian-2024.4.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:11:14.005005 custodian-2024.4.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:11:14.005005 custodian-2024.4.18/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-04-18 14:11:04.000000 custodian-2024.4.18/tests/test_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-18 14:11:04.000000 custodian-2024.4.18/tests/test_utils.py
```

### Comparing `custodian-2024.3.12/LICENSE` & `custodian-2024.4.18/LICENSE`

 * *Files identical despite different names*

### Comparing `custodian-2024.3.12/PKG-INFO` & `custodian-2024.4.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2024.3.12
+Version: 2024.4.18
 Summary: A simple JIT job management framework in Python.
 Author: Matthew Horton, Samuel M. Blau, Stephen Dacek, William Davidson Richards, Xiaohui Qu
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>, Shyue Ping Ong <ongsp@ucsd.edu>
 Maintainer: Janosh Riebesell, Shyue Ping Ong
 License: The MIT License (MIT)
         Copyright (c) 2011-2012 MIT & LBNL
```

### Comparing `custodian-2024.3.12/README.md` & `custodian-2024.4.18/README.md`

 * *Files identical despite different names*

### Comparing `custodian-2024.3.12/custodian/ansible/actions.py` & `custodian-2024.4.18/custodian/ansible/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 import os
 import shutil
 
 
 def get_nested_dict(input_dict, key):
     """Helper function to interpret a nested dict input."""
     current = input_dict
-    toks = key.split("->")
-    n = len(toks)
-    for i, tok in enumerate(toks):
+    tokens = key.split("->")
+    n = len(tokens)
+    for i, tok in enumerate(tokens):
         if tok not in current and i < n - 1:
             current[tok] = {}
         elif i == n - 1:
-            return current, toks[-1]
+            return current, tokens[-1]
         current = current[tok]
     return None
 
 
 class DictActions:
     """Class to implement the supported mongo-like modifications on a dict.
 
@@ -42,60 +42,60 @@
     However, note that "_set" does not support modification of nested dicts
     using the mongo {"a.b":1} notation. This is because mongo does not allow
     keys with "." to be inserted. Instead, nested dict modification is
     supported using a special "->" keyword, e.g. {"a->b": 1}
     """
 
     @staticmethod
-    def set(input_dict, settings, directory=None):
+    def set(input_dict, settings, directory=None) -> None:
         """
         Sets a value using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
-        for k, v in settings.items():
-            (d, key) = get_nested_dict(input_dict, k)
-            d[key] = v
+        for key, val in settings.items():
+            dct, sub_key = get_nested_dict(input_dict, key)
+            dct[sub_key] = val
 
     @staticmethod
-    def unset(input_dict, settings, directory=None):
+    def unset(input_dict, settings, directory=None) -> None:
         """
         Unset a value using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
         for key in settings:
             dct, inner_key = get_nested_dict(input_dict, key)
             del dct[inner_key]
 
     @staticmethod
-    def push(input_dict, settings, directory=None):
+    def push(input_dict, settings, directory=None) -> None:
         """
         Push to a list using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
-        for k, v in settings.items():
-            (d, key) = get_nested_dict(input_dict, k)
-            if key in d:
-                d[key].append(v)
+        for key, val in settings.items():
+            dct, sub_key = get_nested_dict(input_dict, key)
+            if sub_key in dct:
+                dct[sub_key].append(val)
             else:
-                d[key] = [v]
+                dct[sub_key] = [val]
 
     @staticmethod
-    def push_all(input_dict, settings, directory=None):
+    def push_all(input_dict, settings, directory=None) -> None:
         """
         Push multiple items to a list using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
@@ -104,65 +104,65 @@
             dct, k2 = get_nested_dict(input_dict, k1)
             if k2 in dct:
                 dct[k2] += val
             else:
                 dct[k2] = val
 
     @staticmethod
-    def inc(input_dict, settings, directory=None):
+    def inc(input_dict, settings, directory=None) -> None:
         """
-        Increment a value using MongdoDB syntax.
+        Increment a value using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
-        for k, v in settings.items():
-            (d, key) = get_nested_dict(input_dict, k)
-            if key in d:
-                d[key] += v
+        for key, val in settings.items():
+            dct, sub_key = get_nested_dict(input_dict, key)
+            if sub_key in dct:
+                dct[sub_key] += val
             else:
-                d[key] = v
+                dct[sub_key] = val
 
     @staticmethod
-    def rename(input_dict, settings, directory=None):
+    def rename(input_dict, settings, directory=None) -> None:
         """
         Rename a key using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
-        for key, v in settings.items():
-            if val := input_dict.pop(key, None):
-                input_dict[v] = val
+        for key, val in settings.items():
+            if input_val := input_dict.pop(key, None):
+                input_dict[val] = input_val
 
     @staticmethod
-    def add_to_set(input_dict, settings, directory=None):
+    def add_to_set(input_dict, settings, directory=None) -> None:
         """
         Add to set using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
-        for k, v in settings.items():
-            (d, key) = get_nested_dict(input_dict, k)
-            if key in d and (not isinstance(d[key], list)):
-                raise ValueError(f"Keyword {k} does not refer to an array.")
-            if key in d and v not in d[key]:
-                d[key].append(v)
-            elif key not in d:
-                d[key] = v
+        for key, val in settings.items():
+            dct, sub_key = get_nested_dict(input_dict, key)
+            if sub_key in dct and (not isinstance(dct[sub_key], list)):
+                raise ValueError(f"Keyword {key} does not refer to an array.")
+            if sub_key in dct and val not in dct[sub_key]:
+                dct[sub_key].append(val)
+            elif sub_key not in dct:
+                dct[sub_key] = val
 
     @staticmethod
-    def pull(input_dict, settings, directory=None):
+    def pull(input_dict, settings, directory=None) -> None:
         """
         Pull an item using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
@@ -171,15 +171,15 @@
             dct, k2 = get_nested_dict(input_dict, k1)
             if k2 in dct and (not isinstance(dct[k2], list)):
                 raise ValueError(f"Keyword {k1} does not refer to an array.")
             if k2 in dct:
                 dct[k2] = [itm for itm in dct[k2] if itm != val]
 
     @staticmethod
-    def pull_all(input_dict, settings, directory=None):
+    def pull_all(input_dict, settings, directory=None) -> None:
         """
         Pull multiple items to a list using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
@@ -187,118 +187,119 @@
         for key, val in settings.items():
             if key in input_dict and (not isinstance(input_dict[key], list)):
                 raise ValueError(f"Keyword {key} does not refer to an array.")
             for itm in val:
                 DictActions.pull(input_dict, {key: itm})
 
     @staticmethod
-    def pop(input_dict, settings, directory=None):
+    def pop(input_dict, settings, directory=None) -> None:
         """
         Pop item from a list using MongoDB syntax.
 
         Args:
             input_dict (dict): The input dictionary to be modified.
             settings (dict): The specification of the modification to be made.
             directory (None): dummy parameter for compatibility with FileActions
         """
-        for k, v in settings.items():
-            (d, key) = get_nested_dict(input_dict, k)
-            if key in d and (not isinstance(d[key], list)):
-                raise ValueError(f"Keyword {k} does not refer to an array.")
-            if v == 1:
-                d[key].pop()
-            elif v == -1:
-                d[key].pop(0)
+        for key, val in settings.items():
+            dct, sub_key = get_nested_dict(input_dict, key)
+            if sub_key in dct and (not isinstance(dct[sub_key], list)):
+                raise ValueError(f"Keyword {key} does not refer to an array.")
+            if val == 1:
+                dct[sub_key].pop()
+            elif val == -1:
+                dct[sub_key].pop(0)
 
 
 class FileActions:
     """
     Class of supported file actions. For FileActions, the modder class takes in
     a filename as a string. The filename should preferably be a full path to
     avoid ambiguity.
     """
 
     @staticmethod
-    def file_create(filename, settings, directory):
+    def file_create(filename, settings, directory) -> None:
         """
         Creates a file.
 
         Args:
             filename (str): Filename.
             settings (dict): Must be {"content": actual_content}
             directory (str): Directory to create file in
         """
         if len(settings) != 1:
             raise ValueError("Settings must only contain one item with key 'content'.")
-        for k, v in settings.items():
-            if k == "content":
+        for key, val in settings.items():
+            if key == "content":
                 with open(filename, "w") as file:
-                    file.write(v)
+                    file.write(val)
 
     @staticmethod
-    def file_move(filename, settings, directory):
+    def file_move(filename, settings, directory) -> None:
         """
         Moves a file. {'_file_move': {'dest': 'new_file_name'}}.
 
         Args:
             filename (str): Filename.
             settings (dict): Must be {"dest": path of new file}
             directory (str): Directory to move file from and to
         """
         if len(settings) != 1:
             raise ValueError("Settings must only contain one item with key 'dest'.")
-        for k, v in settings.items():
-            if k == "dest":
-                shutil.move(os.path.join(directory, filename), os.path.join(directory, v))
+        for key, val in settings.items():
+            if key == "dest":
+                shutil.move(os.path.join(directory, filename), os.path.join(directory, val))
 
     @staticmethod
-    def file_delete(filename, settings, directory):
+    def file_delete(filename, settings, directory) -> None:
         """
         Deletes a file. {'_file_delete': {'mode': "actual"}}.
 
         Args:
             filename (str): Filename.
             settings (dict): Must be {"mode": actual/simulated}. Simulated
                 mode only prints the action without performing it.
             directory (str): Directory to delete file in
         """
         if len(settings) != 1:
             raise ValueError("Settings must only contain one item with key 'mode'.")
-        for k, v in settings.items():
-            if k == "mode" and v == "actual":
+        for key, val in settings.items():
+            if key == "mode" and val == "actual":
                 try:
                     os.remove(os.path.join(directory, filename))
                 except OSError:
                     # Skip file not found error.
                     pass
-            elif k == "mode" and v == "simulated":
+            elif key == "mode" and val == "simulated":
                 print(f"Simulated removal of {filename}")
 
     @staticmethod
-    def file_copy(filename, settings, directory):
+    def file_copy(filename, settings, directory) -> None:
         """
         Copies a file. {'_file_copy': {'dest': 'new_file_name'}}.
 
         Args:
             filename (str): Filename.
             settings (dict): Must be {"dest": path of new file}
             directory (str): Directory to copy file to/from
         """
-        for k, v in settings.items():
-            if k.startswith("dest"):
-                shutil.copyfile(os.path.join(directory, filename), os.path.join(directory, v))
+        for key, val in settings.items():
+            if key.startswith("dest"):
+                shutil.copyfile(os.path.join(directory, filename), os.path.join(directory, val))
 
     @staticmethod
-    def file_modify(filename, settings, directory):
+    def file_modify(filename, settings, directory) -> None:
         """
         Modifies file access.
 
         Args:
             filename (str): Filename.
             settings (dict): Can be "mode" or "owners"
             directory (str): Directory to modify file in
         """
-        for k, v in settings.items():
-            if k == "mode":
-                os.chmod(os.path.join(directory, filename), v)
-            if k == "owners":
-                os.chown(os.path.join(directory, filename), v)
+        for key, val in settings.items():
+            if key == "mode":
+                os.chmod(os.path.join(directory, filename), val)
+            if key == "owners":
+                # TODO fix this mypy error, missing 3rd positional argument to chown
+                os.chown(os.path.join(directory, filename), val)  # type: ignore[call-arg]
```

### Comparing `custodian-2024.3.12/custodian/ansible/interpreter.py` & `custodian-2024.4.18/custodian/ansible/interpreter.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     >>> modder.modify(mod, dct)
     >>> dct['Bye']
     'World'
     >>> dct['Hello']
     'Universe'
     """
 
-    def __init__(self, actions=None, strict=True, directory="./"):
+    def __init__(self, actions=None, strict=True, directory="./") -> None:
         """Initialize a Modder from a list of supported actions.
 
         Args:
             actions ([Action]): A sequence of supported actions. See
                 :mod:`custodian.ansible.actions`. Default is None,
                 which means only DictActions are supported.
             strict (bool): Indicating whether to use strict mode. In non-strict
@@ -47,15 +47,15 @@
         for action in actions:
             for attr in dir(action):
                 if (not re.match(r"__\w+__", attr)) and callable(getattr(action, attr)):
                     self.supported_actions[f"_{attr}"] = getattr(action, attr)
         self.strict = strict
         self.directory = directory
 
-    def modify(self, modification, obj):
+    def modify(self, modification, obj) -> None:
         """
         Note that modify makes actual in-place modifications. It does not
         return a copy.
 
         Args:
             modification (dict): Modification must be {action_keyword :
                 settings}. E.g., {'_set': {'Hello':'Universe', 'Bye': 'World'}}
```

### Comparing `custodian-2024.3.12/custodian/cli/converge_geometry.py` & `custodian-2024.4.18/custodian/cli/converge_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             final=converged,
             backup=backup,
             suffix=suffix,
             settings_override=settings,
         )
 
 
-def do_run(args):
+def do_run(args) -> None:
     """Perform the run."""
     handlers = [
         VaspErrorHandler(),
         MeshSymmetryErrorHandler(),
         UnconvergedErrorHandler(),
         NonConvergingErrorHandler(),
         PotimErrorHandler(),
```

### Comparing `custodian-2024.3.12/custodian/cli/converge_kpoints.py` & `custodian-2024.4.18/custodian/cli/converge_kpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             final=False,
             backup=backup,
             suffix=f".kpoints.{'x'.join(map(str, m))}",
             settings_override=settings,
         )
 
 
-def do_run(args):
+def do_run(args) -> None:
     """Perform the run."""
     handlers = [VaspErrorHandler(), UnconvergedErrorHandler()]
     c = Custodian(
         handlers,
         get_runs(
             vasp_command=args.command.split(),
             target=args.target,
@@ -61,15 +61,15 @@
             max_steps=args.max_steps,
         ),
         max_errors=10,
     )
     c.run()
 
 
-def main():
+def main() -> None:
     """Main method."""
     import argparse
 
     parser = argparse.ArgumentParser(
         description="""
     converge_kpoints perform a KPOINTS convergence. What this script will do
     is to run a particular VASP run with increasing multiples of the initial
```

### Comparing `custodian-2024.3.12/custodian/cli/cstdn.py` & `custodian-2024.4.18/custodian/cli/cstdn.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,30 +69,30 @@
   max_errors: 10
   scratch_dir: /tmp
   gzipped_output: True
   checkpoint: True
 """
 
 
-def run(args):
+def run(args) -> None:
     """Perform a single run."""
     FORMAT = "%(asctime)s %(message)s"
     logging.basicConfig(format=FORMAT, level=logging.INFO, filename="run.log")
     logging.info(f"Spec file is {args.spec_file}")
     dct = loadfn(args.spec_file[0])
     c = Custodian.from_spec(dct)
     c.run()
 
 
-def print_example(args):
+def print_example(args) -> None:
     """Print the example_yaml."""
     print(example_yaml)
 
 
-def main():
+def main() -> None:
     """Main method."""
     parser = argparse.ArgumentParser(
         description="""
     cstdn is a convenient script to run custodian style jobs using a
     simple YAML spec.""",
         epilog="""Author: Shyue Ping Ong""",
     )
```

### Comparing `custodian-2024.3.12/custodian/cli/run_nwchem.py` & `custodian-2024.4.18/custodian/cli/run_nwchem.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 
 from custodian.custodian import Custodian
 from custodian.nwchem.handlers import NwchemErrorHandler
 from custodian.nwchem.jobs import NwchemJob
 
 
-def do_run(args):
+def do_run(args) -> None:
     """Do the run."""
     logging.basicConfig(format="%(asctime)s %(message)s", level=logging.INFO, filename="run.log")
     job = NwchemJob(
         nwchem_cmd=args.command.split(),
         input_file=args.infile,
         output_file=args.outfile,
     )
@@ -22,15 +22,15 @@
         scratch_dir=args.scratch,
         gzipped_output=args.gzipped,
         checkpoint=True,
     )
     c.run()
 
 
-def main():
+def main() -> None:
     """Main method."""
     import argparse
 
     parser = argparse.ArgumentParser(
         description="""
     run_nwchem is a master script to perform various kinds of Nwchem runs.
     """,
```

### Comparing `custodian-2024.3.12/custodian/cli/run_vasp.py` & `custodian-2024.4.18/custodian/cli/run_vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,15 +192,15 @@
                 backup=backup,
                 settings_override=settings,
                 copy_magmom=copy_magmom,
                 auto_npar=auto_npar,
             )
 
 
-def do_run(args):
+def do_run(args) -> None:
     """Do the run."""
     FORMAT = "%(asctime)s %(message)s"
     logging.basicConfig(format=FORMAT, level=logging.INFO, filename="run.log")
     logging.info(f"Handlers used are {args.handlers}")
     handlers = [load_class("custodian.vasp.handlers", handler) for handler in args.handlers]
     validators = [load_class("custodian.vasp.validators", validator) for validator in args.validators]
 
@@ -212,15 +212,15 @@
         scratch_dir=args.scratch,
         gzipped_output=args.gzip,
         checkpoint=True,
     )
     c.run()
 
 
-def main():
+def main() -> None:
     """Main method."""
     import argparse
 
     parser = argparse.ArgumentParser(
         description="run_vasp is a master script to perform various kinds of VASP runs.",
         epilog="Author: Shyue Ping Ong",
     )
```

### Comparing `custodian-2024.3.12/custodian/cp2k/handlers.py` & `custodian-2024.4.18/custodian/cp2k/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,25 +54,25 @@
     """
 
     is_monitor = True
     raises_runtime_error = False
 
     error_msgs = {"seg_fault": ["SIGSEGV"], "out_of_memory": ["insufficient virtual memory"], "abort": ["SIGABRT"]}
 
-    def __init__(self, std_err="std_err.txt"):
+    def __init__(self, std_err="std_err.txt") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             std_err (str): This is the file where the stderr for cp2k
                 is being redirected. The error messages that are checked are
                 present in the stderr. Defaults to "std_err.txt", which is the
                 default redirect used by :class:`custodian.cp2k.jobs.Cp2kJob`.
         """
         self.std_err = std_err
-        self.errors = set()
+        self.errors: set[str] = set()
 
     def check(self, directory="./"):
         """Check for error in std_err file."""
         self.errors = set()
         with open(self.std_err) as file:
             for line in file:
                 line = line.strip()
@@ -129,15 +129,15 @@
     (3) Pseudo-diagonalization (Not implemented)
 
     (4) Purification methods (Not implemented)
     """
 
     is_monitor = True
 
-    def __init__(self, input_file="cp2k.inp", output_file="cp2k.out"):
+    def __init__(self, input_file="cp2k.inp", output_file="cp2k.out") -> None:
         """Initialize the error handler from a set of input and output files.
 
         Args:
             input_file (str): Name of the CP2K input file.
             output_file (str): Name of the CP2K output file.
         """
         self.input_file = input_file
@@ -156,17 +156,15 @@
         self.is_ot = ci.check("FORCE_EVAL/DFT/SCF/OT")
         if out.filenames.get("restart"):
             self.restart = out.filenames["restart"][-1]
 
         # General catch for SCF not converged
         # TODO: should not-static runs allow for some unconverged scf? Leads to issues in my experience
         scf = out.data["scf_converged"] or [True]
-        if not scf[0]:
-            return True
-        return False
+        return bool(not scf[0])
 
     def correct(self, directory="./"):
         """Apply corrections to aid convergence if possible."""
         ci = Cp2kInput.from_file(os.path.join(directory, self.input_file))
 
         actions = self.__correct_ot(ci=ci) if self.is_ot else self.__correct_diag(ci=ci)
 
@@ -397,15 +395,15 @@
     FORCE_EVAL/DFT/PRINT/CONDITION_OVERLAP) can diverge if the precision
     is set to a normal value. So, this error handler will bump up the precision
     in an attempt to remedy the problem.
     """
 
     is_monitor = True
 
-    def __init__(self, output_file="cp2k.out", input_file="cp2k.inp"):
+    def __init__(self, output_file="cp2k.out", input_file="cp2k.inp") -> None:
         """Initializes the error handler from an output files.
 
         Args:
             output_file (str): Name of the CP2K output file.
             input_file (str): Name of the CP2K input file.
         """
         self.output_file = output_file
@@ -459,15 +457,15 @@
             as some sub-routines, like the HFX module, can take a long time to
             update the output file.
 
     """
 
     is_monitor = True
 
-    def __init__(self, input_file="cp2k.inp", output_file="cp2k.out", timeout=3600):
+    def __init__(self, input_file="cp2k.inp", output_file="cp2k.out", timeout=3600) -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             input_file (str): Name of the input file to modify if needed
             output_file (str): Name of the output file to monitor
             timeout (int): The time in seconds between checks where if there
                 is no activity on the output file, the run is considered
@@ -484,17 +482,15 @@
     def check(self, directory="./"):
         """Check for frozen jobs."""
         st = os.stat(os.path.join(directory, self.output_file))
         out = Cp2kOutput(os.path.join(directory, self.output_file), auto_load=False, verbose=False)
         try:
             out.ran_successfully()
             # If job finished, then hung, don't need to wait very long to confirm frozen
-            if time.time() - st.st_mtime > 300:
-                return True
-            return False
+            return time.time() - st.st_mtime > 300
         except ValueError:
             pass
 
         t = tail(self.output_file, 2)
         if time.time() - st.st_mtime > self.timeout:
             if t[0].split() == ["Step", "Update", "method", "Time", "Convergence", "Total", "energy", "Change"]:
                 self.frozen_preconditioner = True
@@ -600,31 +596,31 @@
         (2) Cholesky decomposition error from SCF diagonalization. If found, the
             handler will try switching from the restore algorithm to inverse cholesky
     """
 
     is_monitor = False
     is_terminating = True
 
-    def __init__(self, input_file="cp2k.inp", output_file="cp2k.out"):
+    def __init__(self, input_file="cp2k.inp", output_file="cp2k.out") -> None:
         """
         Initialize handler for CP2K abort messages.
 
         Args:
             input_file: (str) name of the input file
             output_file: (str) name of the output file
         """
         self.input_file = input_file
         self.output_file = output_file
         self.messages = {
             "cholesky": r"(Cholesky decomposition failed. Matrix ill conditioned ?)",
             "cholesky_scf": r"(Cholesky decompose failed: the matrix is not positive definite or)",
         }
-        self.responses = []
+        self.responses: list[str] = []
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for abort messages."""
         matches = regrep(
             os.path.join(directory, self.output_file),
             patterns=self.messages,
             reverse=True,
             terminate_on_match=True,
             postprocess=str,
@@ -786,15 +782,15 @@
         self,
         input_file="cp2k.inp",
         output_file="cp2k.out",
         max_same=5,
         pgf_orb_strict=1e-20,
         eps_default_strict=1e-12,
         eps_gvg_strict=1e-10,
-    ):
+    ) -> None:
         """
         Initialize the error handler.
 
         Args:
             input_file (str): name of the input file to modify (if needed)
             output_file (str): name of the output file to monitor
             max_same (int): maximum number of SCF convergence loops with the same
@@ -821,17 +817,15 @@
         self.eps_default_strict = eps_default_strict
         self.eps_gvg_strict = eps_gvg_strict
 
     def check(self, directory="./"):
         """Check for stuck SCF convergence."""
         conv = get_conv(os.path.join(directory, self.output_file))
         counts = [len([*group]) for _k, group in itertools.groupby(conv)]
-        if any(cnt > self.max_same for cnt in counts):
-            return True
-        return False
+        return bool(any(cnt > self.max_same for cnt in counts))
 
     def correct(self, directory="/."):
         """Correct issue if possible."""
         ci = Cp2kInput.from_file(os.path.join(directory, self.input_file))
         actions = []
 
         if ci.check("FORCE_EVAL/DFT/XC/HF"):  # Hybrid has special considerations
@@ -944,15 +938,15 @@
     def __init__(
         self,
         input_file="cp2k.inp",
         output_file="cp2k.out",
         max_iter=20,
         max_total_iter=200,
         optimizers=("BFGS", "CG", "BFGS", "CG"),
-    ):
+    ) -> None:
         """
         Initialize the error handler.
 
         Args:
             input_file: name of the input file
             output_file: name of the output file
             max_iter: Max iter for an "inner loop", i.e. max iterations for one optimizer before
@@ -970,17 +964,15 @@
         self.optimizers = optimizers
         self.optimizer_id = 0
 
     def check(self, directory="./"):
         """Check for unconverged geometry optimization."""
         o = Cp2kOutput(os.path.join(directory, self.output_file))
         o.convergence()
-        if o.data.get("geo_opt_not_converged"):
-            return True
-        return False
+        return bool(o.data.get("geo_opt_not_converged"))
 
     def correct(self, directory):
         """Correct issue if possible."""
         ci = Cp2kInput.from_file(os.path.join(directory, self.input_file))
         actions = []
 
         max_iter = ci["motion"]["geo_opt"].get("MAX_ITER", Keyword("", 200)).values[0]
@@ -1030,34 +1022,34 @@
     (see Custodian), and simply creates checkpoint.json.
     """
 
     is_monitor = False
     raises_runtime_error = False
     is_terminating = False
 
-    def __init__(self, output_file="cp2k.out", enable_checkpointing=True):
+    def __init__(self, output_file="cp2k.out", enable_checkpointing=True) -> None:
         """
         Args:
             output_file (str): name of the cp2k output file
             enable_checkpointing (bool): whether or not to enable checkpointing when
                 the walltime is reached by dumping checkpoint.json.
         """
         self.output_file = output_file
         self.enable_checkpointing = enable_checkpointing
 
     def check(self, directory="./"):
         """Check if internal CP2K walltime handler was tripped."""
-        if regrep(
-            filename=os.path.join(directory, self.output_file),
-            patterns={"walltime": r"(exceeded requested execution time)"},
-            reverse=True,
-            terminate_on_match=True,
-            postprocess=bool,
-        ).get("walltime"):
-            return True
-        return False
+        return bool(
+            regrep(
+                filename=os.path.join(directory, self.output_file),
+                patterns={"walltime": "(exceeded requested execution time)"},
+                reverse=True,
+                terminate_on_match=True,
+                postprocess=bool,
+            ).get("walltime")
+        )
 
     def correct(self, directory="./"):
         """Dump checkpoint info if requested."""
         if self.enable_checkpointing:
             dumpfn({"_path": directory}, fn=(os.path.join(directory, "checkpoint.json")))
         return {"errors": ["Walltime error"], "actions": []}
```

### Comparing `custodian-2024.3.12/custodian/cp2k/interpreter.py` & `custodian-2024.4.18/custodian/cp2k/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class Cp2kModder(Modder):
     """
     Cp2kModder is a lightweight class for applying modifications to cp2k input files. It
     also supports modifications that are file operations (e.g. copying).
     """
 
-    def __init__(self, filename="cp2k.inp", actions=None, strict=True, ci=None, directory="./"):
+    def __init__(self, filename="cp2k.inp", actions=None, strict=True, ci=None, directory="./") -> None:
         """Initialize a Modder for Cp2kInput sets.
 
         Args:
             filename (str): name of cp2k input file to modify. This file will be overwritten
                 if actions are applied.
             actions ([Action]): A sequence of supported actions. See
                 :mod:`custodian.ansible.actions`. Default is None,
@@ -39,15 +39,15 @@
         """
         self.directory = directory
         self.ci = ci or Cp2kInput.from_file(os.path.join(self.directory, filename))
         self.filename = filename
         actions = actions or [FileActions, DictActions]
         super().__init__(actions, strict)
 
-    def apply_actions(self, actions):
+    def apply_actions(self, actions) -> None:
         """
         Applies a list of actions to the CP2K Input Set and rewrites modified
         files.
 
         Args:
             actions (dict): A list of actions of the form {'file': filename,
                 'action': moddermodification} or {'dict': cp2k_key,
@@ -64,15 +64,15 @@
                 self.ci = Cp2kInput.from_file(os.path.join(self.directory, self.filename))
             else:
                 raise ValueError(f"Unrecognized format: {action}")
         cleanup_input(self.ci)
         self.ci.write_file(os.path.join(self.directory, self.filename))
 
     @staticmethod
-    def _modify(modification, obj):
+    def _modify(modification, obj) -> None:
         """
         Note that modify makes actual in-place modifications. It does not
         return a copy.
 
         Args:
             modification (dict): Modification must be {action_keyword :
                 settings}. E.g., {'_set': {'Hello':'Universe', 'Bye': 'World'}}
```

### Comparing `custodian-2024.3.12/custodian/cp2k/jobs.py` & `custodian-2024.4.18/custodian/cp2k/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         output_file="cp2k.out",
         stderr_file="std_err.txt",
         suffix="",
         final=True,
         backup=True,
         settings_override=None,
         restart=False,
-    ):
+    ) -> None:
         """
         This constructor is necessarily complex due to the need for
         flexibility. For standard kinds of runs, it's often better to use one
         of the static constructors. The defaults are usually fine too.
 
         Args:
             cp2k_cmd (list): Command to run cp2k as a list of args. For example,
@@ -76,15 +76,15 @@
         self.stderr_file = stderr_file
         self.final = final
         self.backup = backup
         self.suffix = suffix
         self.settings_override = settings_override if settings_override else []
         self.restart = restart
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         """
         Performs initial setup for Cp2k in three stages. First, if custodian is running in restart mode, then
         the restart function will copy the restart file to self.input_file, and remove any previous WFN initialization
         if present. Second, any additional user specified settings will be applied. Lastly, a backup of the input
         file will be made for reference.
         """
         decompress_dir(directory)
@@ -124,15 +124,15 @@
             open(os.path.join(directory, self.stderr_file), "w", buffering=1) as f_err,
         ):
             # use line buffering for stderr
             return subprocess.Popen(cmd, cwd=directory, stdout=f_std, stderr=f_err, shell=False)
 
     # TODO double jobs, file manipulations, etc. should be done in atomate in the future
     # and custodian should only run the job itself
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """Postprocessing includes renaming and gzipping where necessary."""
         files = os.listdir(directory)
         if os.path.isfile(self.output_file) and self.suffix != "":
             os.mkdir(f"run{self.suffix}")
             for file in files:
                 if "json" in file:
                     continue
@@ -143,15 +143,15 @@
                         shutil.copy(os.path.join(directory, file), os.path.join(directory, f"run{self.suffix}/{file}"))
 
         # Remove continuation so if a subsequent job is run in
         # the same directory, will not restart this job.
         if os.path.isfile(os.path.join(directory, "continue.json")):
             os.remove(os.path.join(directory, "continue.json"))
 
-    def terminate(self, directory="./"):
+    def terminate(self, directory="./") -> None:
         """Terminate cp2k."""
         for cmd in self.cp2k_cmd:
             if "cp2k" in cmd:
                 try:
                     os.system(f"killall {cmd}")
                 except Exception:
                     pass
```

### Comparing `custodian-2024.3.12/custodian/cp2k/utils.py` & `custodian-2024.4.18/custodian/cp2k/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from collections import deque
 
 from pymatgen.io.cp2k.inputs import Cp2kInput
 from pymatgen.io.cp2k.outputs import Cp2kOutput
 
 
-def restart(actions, output_file, input_file, no_actions_needed=False):
+def restart(actions, output_file, input_file, no_actions_needed=False) -> None:
     """
     Helper function. To discard old restart if convergence is already good, and copy
     the restart file to the input file. Restart also supports switching back and forth
     between OT and diagonalization as needed based on convergence behavior. If OT is not
     being used and a band gap exists, then OT will be activated.
 
     Args:
@@ -47,15 +47,15 @@
                     "file": os.path.abspath(restart_file),
                     "action": {"_file_copy": {"dest": os.path.abspath(input_file)}},
                 },
             )
 
 
 # TODO Not sure I like this solution
-def cleanup_input(ci):
+def cleanup_input(ci) -> None:
     """
     Intention is to use this to remove problematic parts of the input file.
 
         (1) The "POTENTIAL" section within KIND cannot be empty, but the number
             sequences used inside do not play nice with the input parser
 
     """
@@ -63,15 +63,15 @@
         return
     if any(k.upper() == "POTENTIAL" for k in ci.subsections):
         ci.subsections.pop("POTENTIAL")
     for val in ci.subsections.values():
         cleanup_input(val)
 
 
-def activate_ot(actions, ci):
+def activate_ot(actions, ci) -> None:
     """
     Activate OT scheme.
 
     actions (list):
         list of actions that are being applied. Will be modified in-place
 
     ci (Cp2kInput):
@@ -114,15 +114,15 @@
                 )
             ],
         },
     ]
     actions += ot_actions
 
 
-def activate_diag(actions):
+def activate_diag(actions) -> None:
     """
     Activate diagonalization.
 
     actions (list):
         list of actions that are being applied. Will be modified in-place
     """
     diag_actions = [
@@ -160,22 +160,20 @@
 
     Args:
         output (Cp2kOutput): cp2k output object for determining band gap
         ci (Cp2kInput): cp2k input object for determining if OT is already active
         minimum_band_gap (float): the minimum band gap for OT
     """
     output.parse_dos()
-    if (
+    return bool(
         not ci.check("FORCE_EVAL/DFT/SCF/OT")
         and not ci.check("FORCE_EVAL/DFT/KPOINTS")
         and output.band_gap
         and output.band_gap > minimum_band_gap
-    ):
-        return True
-    return False
+    )
 
 
 def tail(filename, n=10):
     """Returns the last n lines of a file as a list (including empty lines)."""
     with open(filename) as file:
         t = deque(file, n)
         if t:
```

### Comparing `custodian-2024.3.12/custodian/cp2k/validators.py` & `custodian-2024.4.18/custodian/cp2k/validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Validators for CP2K calculations."""
 
+from __future__ import annotations
+
 import os
 from abc import abstractmethod, abstractproperty
 
 from pymatgen.io.cp2k.outputs import Cp2kOutput
 
 from custodian.custodian import Validator
 
@@ -35,23 +37,23 @@
     def no_children(self, directory="./"):
         """Job should not have children."""
 
 
 class Cp2kOutputValidator(Cp2kValidator):
     """Checks that a valid cp2k output file was generated."""
 
-    def __init__(self, output_file="cp2k.out"):
+    def __init__(self, output_file="cp2k.out") -> None:
         """
         Args:
             output_file (str): cp2k output file to analyze.
         """
         self.output_file = output_file
         self._check = False
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool | None:
         """
         Check for valid output. Checks that the end of the
         program was reached, and that convergence was
         achieved.
         """
         try:
             o = Cp2kOutput(os.path.join(directory, self.output_file))
@@ -68,20 +70,20 @@
             self._check = True
             return True
         except Exception:
             self._check = True
             return True
 
     @property
-    def kill(self, directory="./"):
+    def kill(self, directory="./") -> bool:
         """Kill the job with raise error."""
         return True
 
     @property
-    def exit(self, directory="./"):
+    def exit(self, directory="./") -> bool:
         """Don't raise error, but exit the job."""
         return True
 
     @property
-    def no_children(self, directory="./"):
+    def no_children(self, directory="./") -> bool:
         """Job should not have children."""
         return True
```

### Comparing `custodian-2024.3.12/custodian/custodian.py` & `custodian-2024.4.18/custodian/custodian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 This module implements the main Custodian class, which manages a list of jobs
 given a set of error handlers, the abstract base classes for the
 ErrorHandlers and Jobs.
 """
 
+from __future__ import annotations
+
 import datetime
 import logging
 import os
 import subprocess
 import sys
 import tarfile
 import time
@@ -120,15 +122,15 @@
         scratch_dir=None,
         gzipped_output=False,
         checkpoint=False,
         terminate_func=None,
         terminate_on_nonzero_returncode=True,
         directory=None,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize a Custodian from a list of jobs and error handlers.
 
         Args:
             handlers ([ErrorHandler]): Error handlers. In order of priority of
                 fixing.
             jobs ([Job]): Sequence of Jobs to be run. Note that this can be
                 any sequence or even a generator yielding jobs.
@@ -221,35 +223,35 @@
                     abs_directory = os.path.abspath(directory)
                     abs_target = os.path.abspath(target)
 
                     prefix = os.path.commonprefix([abs_directory, abs_target])
 
                     return prefix == abs_directory
 
-                def safe_extract(tar, path=directory, members=None, *, numeric_owner=False):
+                def safe_extract(tar, path=directory, members=None, *, numeric_owner=False) -> None:
                     for member in tar.getmembers():
                         member_path = os.path.join(path, member.name)
                         if not is_within_directory(path, member_path):
                             raise Exception("Attempted Path Traversal in Tar File")
 
                     tar.extractall(path, members, numeric_owner=numeric_owner)
 
                 safe_extract(file, directory)
             # Log the corrections to a json file.
             run_log = loadfn(os.path.join(directory, Custodian.LOG_FILE), cls=MontyDecoder)
 
         return restart, run_log
 
     @staticmethod
-    def _delete_checkpoints(directory):
+    def _delete_checkpoints(directory) -> None:
         for file in glob(os.path.join(directory, "custodian.chk.*.tar.gz")):
             os.remove(file)
 
     @staticmethod
-    def _save_checkpoint(directory, index):
+    def _save_checkpoint(directory, index) -> None:
         try:
             Custodian._delete_checkpoints(directory)
             n = os.path.join(directory, f"custodian.chk.{index}.tar.gz")
             with tarfile.open(n, mode="w:gz", compresslevel=3) as file:
                 file.add(directory, arcname=".")
             logger.info(f"Checkpoint written to {n}")
         except Exception:
@@ -404,15 +406,15 @@
                     gzip_dir(".")
 
             # Cleanup checkpoint files (if any) if run is successful.
             Custodian._delete_checkpoints(self.directory)
 
         return self.run_log
 
-    def _run_job(self, job_n, job):
+    def _run_job(self, job_n, job) -> None:
         """
         Runs a single job.
 
         Args:
             job_n: job number (1 index)
             job: Custodian job
 
@@ -649,24 +651,22 @@
         for handler in handlers:
             try:
                 if handler.check(directory=self.directory):
                     if (
                         handler.max_num_corrections is not None
                         and handler.n_applied_corrections >= handler.max_num_corrections
                     ):
-                        msg = (
-                            f"Maximum number of corrections {handler.max_num_corrections} reached for handler {handler}"
-                        )
+                        msg = f"Maximum number of corrections {handler.max_num_corrections} reached for {handler=}"
                         if handler.raise_on_max:
                             self.run_log[-1]["handler"] = handler
                             self.run_log[-1]["max_errors_per_handler"] = True
                             raise MaxCorrectionsPerHandlerError(
                                 msg, raises=True, max_errors_per_handler=handler.max_num_corrections, handler=handler
                             )
-                        logger.warning(msg + " Correction not applied.")
+                        logger.warning(f"{msg} Correction not applied.")
                         continue
                     if terminate_func is not None and handler.is_terminating:
                         logger.info("Terminating job")
                         terminate_func(directory=self.directory)
                         # make sure we don't terminate twice
                         terminate_func = None
                     dct = handler.correct(directory=self.directory)
@@ -675,17 +675,17 @@
                     corrections.append(dct)
                     handler.n_applied_corrections += 1
             except Exception:
                 if not self.skip_over_errors:
                     raise
                 import traceback
 
-                logger.error(f"Bad handler {handler}")
+                logger.error(f"Bad {handler=}")
                 logger.error(traceback.format_exc())
-                corrections.append({"errors": [f"Bad handler {handler}"], "actions": []})
+                corrections.append({"errors": [f"Bad {handler=}"], "actions": []})
         self.total_errors += len(corrections)
         self.errors_current_job += len(corrections)
         self.run_log[-1]["corrections"] += corrections
         # We do a dump of the run log after each check.
         dumpfn(self.run_log, os.path.join(self.directory, Custodian.LOG_FILE), cls=MontyEncoder, indent=4)
         # Clear all the cached values to avoid reusing them in a subsequent check
         tracked_lru_cache.tracked_cache_clear()
@@ -713,15 +713,15 @@
     def postprocess(self, directory="./"):
         """
         This method is called at the end of a job, *after* error detection.
         This allows post-processing, such as cleanup, analysis of results,
         etc.
         """
 
-    def terminate(self, directory="./"):
+    def terminate(self, directory="./") -> None:
         """Implement termination function."""
         return
 
     @property
     def name(self):
         """A nice string name for the job."""
         return type(self).__name__
@@ -756,15 +756,15 @@
     raises_runtime_error = True
     """
     Whether this handler causes custodian to raise a runtime error if it cannot
     handle the error (i.e. if correct returns a dict with "actions":None, or
     "actions":[])
     """
 
-    max_num_corrections = None
+    max_num_corrections: int | None = None
     raise_on_max = False
     """
     Whether corrections from this specific handler should be applied only a
     fixed maximum number of times on a single job (i.e. the counter is reset
     at the beginning of each job). If the maximum number is reached the code
     will either raise a MaxCorrectionsPerHandlerError (raise_on_max==True) or stops
     considering the correction (raise_on_max==False). If max_num_corrections
@@ -809,15 +809,15 @@
         try:
             return self._num_applied_corrections
         except AttributeError:
             self._num_applied_corrections = 0
             return self._num_applied_corrections
 
     @n_applied_corrections.setter
-    def n_applied_corrections(self, value):
+    def n_applied_corrections(self, value) -> None:
         """
         Setter for the number of corrections applied.
 
         Args:
              value(int): the number of corrections applied
         """
         self._num_applied_corrections = value
@@ -840,44 +840,44 @@
             (bool) Indicating if errors are detected.
         """
 
 
 class CustodianError(RuntimeError):
     """Exception class for Custodian errors."""
 
-    def __init__(self, message, raises=False):
+    def __init__(self, message, raises=False) -> None:
         """Initialize the error with a message.
 
         Args:
             message (str): Message passed to Exception
             raises (bool): Whether this should be raised outside custodian
         """
         super().__init__(message)
         self.raises = raises
         self.message = message
 
 
 class ValidationError(CustodianError):
     """Error raised when a validator does not pass the check."""
 
-    def __init__(self, message, raises, validator):
+    def __init__(self, message, raises, validator) -> None:
         """
         Args:
             message (str): Message passed to Exception
             raises (bool): Whether this should be raised outside custodian
             validator (Validator): Validator that caused the exception.
         """
         super().__init__(message, raises)
         self.validator = validator
 
 
 class NonRecoverableError(CustodianError):
     """Error raised when a handler found an error but could not fix it."""
 
-    def __init__(self, message, raises, handler):
+    def __init__(self, message, raises, handler) -> None:
         """
         Args:
             message (str): Message passed to Exception
             raises (bool): Whether this should be raised outside custodian
             handler (Handler): Handler that caused the exception.
         """
         super().__init__(message, raises)
@@ -887,29 +887,29 @@
 class ReturnCodeError(CustodianError):
     """Error raised when the process gave non zero return code."""
 
 
 class MaxCorrectionsError(CustodianError):
     """Error raised when the maximum allowed number of errors is reached."""
 
-    def __init__(self, message, raises, max_errors):
+    def __init__(self, message, raises, max_errors) -> None:
         """
         Args:
             message (str): Message passed to Exception
             raises (bool): Whether this should be raised outside custodian
             max_errors (int): the number of errors reached.
         """
         super().__init__(message, raises)
         self.max_errors = max_errors
 
 
 class MaxCorrectionsPerJobError(CustodianError):
     """Error raised when the maximum allowed number of errors per job is reached."""
 
-    def __init__(self, message, raises, max_errors_per_job, job):
+    def __init__(self, message, raises, max_errors_per_job, job) -> None:
         """
         Args:
             message (str): Message passed to Exception
             raises (bool): Whether this should be raised outside custodian
             max_errors_per_job (int): the number of errors per job reached
             job (Job): the job that was stopped.
         """
```

### Comparing `custodian-2024.3.12/custodian/feff/handlers.py` & `custodian-2024.4.18/custodian/feff/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module implements specific error handler for FEFF runs."""
 
+from __future__ import annotations
+
 import logging
 import os
 import re
 
 from pymatgen.io.feff.sets import FEFFDictSet
 
 from custodian.custodian import ErrorHandler
@@ -31,15 +33,15 @@
 
 
 class UnconvergedErrorHandler(ErrorHandler):
     """Correct the unconverged error of FEFF's SCF calculation."""
 
     is_monitor = False
 
-    def __init__(self, output_filename="log1.dat"):
+    def __init__(self, output_filename="log1.dat") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): Filename for the log1.dat file. log1.dat file
                 contains the SCF calculation convergence information. Change this only
                 if it is different from the default (unlikely).
         """
@@ -48,15 +50,15 @@
     def check(self, directory="./"):
         """
         If the FEFF run does not converge, the check will return
         "TRUE".
         """
         return self._notconverge_check(directory)
 
-    def _notconverge_check(self, directory):
+    def _notconverge_check(self, directory) -> bool | None:
         # Process the output file and get converge information
         not_converge_pattern = re.compile("Convergence not reached.*")
         converge_pattern = re.compile("Convergence reached.*")
         with open(os.path.join(directory, self.output_filename)) as file:
             for line in file:
                 if len(not_converge_pattern.findall(line)) > 0:
                     return True
```

### Comparing `custodian-2024.3.12/custodian/feff/interpreter.py` & `custodian-2024.4.18/custodian/feff/interpreter.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from custodian.ansible.actions import DictActions, FileActions
 from custodian.ansible.interpreter import Modder
 
 
 class FeffModder(Modder):
     """A Modder for FeffInput sets."""
 
-    def __init__(self, actions=None, strict=True, feffinp=None, directory="./"):
-        """
+    def __init__(self, actions=None, strict=True, feffinp=None, directory="./") -> None:
+        """Initialize a FeffModder.
+
         Args:
             actions ([Action]): A sequence of supported actions. See
             actions ([Action]): A sequence of supported actions. See
                 :mod:`custodian.ansible.actions`. Default is None,
                 which means DictActions and FileActions are supported.
             strict (bool): Indicating whether to use strict mode. In non-strict
                 mode, unsupported actions are simply ignored without any
@@ -29,38 +30,38 @@
         """
         self.directory = directory
         self.feffinp = feffinp or FEFFDictSet.from_directory(self.directory)
         self.feffinp = self.feffinp.all_input()
         actions = actions or [FileActions, DictActions]
         super().__init__(actions, strict)
 
-    def apply_actions(self, actions):
+    def apply_actions(self, actions) -> None:
         """
         Applies a list of actions to the FEFF Input Set and rewrites modified
         files.
 
         Args:
             actions (dict): A list of actions of the form {'file': filename,
                 'action': moddermodification} or {'dict': feffinput_key,
                 'action': moddermodification}
         """
         modified = []
         for action in actions:
             if "dict" in action:
-                k = action["dict"]
-                modified.append(k)
-                self.feffinp[k] = self.modify_object(action["action"], self.feffinp[k])
+                key = action["dict"]
+                modified.append(key)
+                self.feffinp[key] = self.modify_object(action["action"], self.feffinp[key])
             elif "file" in action:
                 self.modify(action["action"], action["file"])
             else:
                 raise ValueError(f"Unrecognized format: {action}")
         if modified:
             feff = self.feffinp
             feff_input = "\n\n".join(
                 str(feff[key]) for key in ("HEADER", "PARAMETERS", "POTENTIALS", "ATOMS") if key in feff
             )
-            for k, v in feff.items():
-                with open(os.path.join(self.directory, k), "w") as file:
-                    file.write(str(v))
+            for key, val in feff.items():
+                with open(os.path.join(self.directory, key), "w") as file:
+                    file.write(str(val))
 
             with open(os.path.join(self.directory, "feff.inp"), "w") as file:
                 file.write(feff_input)
```

### Comparing `custodian-2024.3.12/custodian/feff/jobs.py` & `custodian-2024.4.18/custodian/feff/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self,
         feff_cmd,
         output_file="feff.out",
         stderr_file="std_feff_err.txt",
         backup=True,
         gzipped=False,
         gzipped_prefix="feff_out",
-    ):
+    ) -> None:
         """
         This constructor is used for a standard FEFF initialization.
 
         Args:
             feff_cmd (str): the name of the full executable for running FEFF
             output_file (str): Name of file to direct standard out to.
                 Defaults to "feff.out".
@@ -81,11 +81,11 @@
             open(os.path.join(directory, self.output_file), "w") as f_std,
             open(os.path.join(directory, self.stderr_file), "w", buffering=1) as f_err,
         ):
             # Use line buffering for stderr
             # On TSCC, need to run shell command
             return subprocess.Popen(self.feff_cmd, cwd=directory, stdout=f_std, stderr=f_err, shell=True)  # pylint: disable=R1732
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """Renaming or gzipping all the output as needed."""
         if self.gzipped:
             backup("*", directory=directory, prefix=self.gzipped_prefix)
```

### Comparing `custodian-2024.3.12/custodian/lobster/handlers.py` & `custodian-2024.4.18/custodian/lobster/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 __email__ = "janine.george@uclouvain.be"
 __date__ = "April 27, 2020"
 
 
 class EnoughBandsValidator(Validator):
     """validates if enough bands for COHP calculation are available."""
 
-    def __init__(self, output_filename: str = "lobsterout"):
+    def __init__(self, output_filename: str = "lobsterout") -> None:
         """
 
         Args:
             output_filename: filename of output file, usually lobsterout.
         """
         self.output_filename = output_filename
 
@@ -43,15 +43,15 @@
 class LobsterFilesValidator(Validator):
     """
     Check for existence of some of the files that lobster
         normally create upon running.
     Check if lobster terminated normally by looking for finished.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Dummy init."""
 
     def check(self, directory: str = "./") -> bool:
         """Check for errors."""
         for filename in ("lobsterout",):
             if not os.path.isfile(os.path.join(directory, filename)):
                 return True
@@ -59,15 +59,15 @@
             data = file.read()
         return "finished" not in data
 
 
 class ChargeSpillingValidator(Validator):
     """Check if spilling is below certain threshold!"""
 
-    def __init__(self, output_filename: str = "lobsterout", charge_spilling_limit: float = 0.05):
+    def __init__(self, output_filename: str = "lobsterout", charge_spilling_limit: float = 0.05) -> None:
         """
 
         Args:
             output_filename: filename of the output file of lobster, usually lobsterout
             charge_spilling_limit: limit of the charge spilling that will be considered okay.
         """
         self.output_filename = output_filename
@@ -75,11 +75,11 @@
 
     def check(self, directory: str = "./") -> bool:
         """Open lobsterout and find charge spilling."""
         if os.path.isfile(os.path.join(directory, self.output_filename)):
             lobsterout = Lobsterout(os.path.join(directory, self.output_filename))
             if lobsterout.charge_spilling[0] > self.charge_spilling_limit:
                 return True
-            if len(lobsterout.charge_spilling) > 1 and lobsterout.charge_spilling[1] > self.charge_spilling_limit:
-                return True
-            return False
+            return bool(
+                len(lobsterout.charge_spilling) > 1 and lobsterout.charge_spilling[1] > self.charge_spilling_limit
+            )
         return False
```

### Comparing `custodian-2024.3.12/custodian/lobster/jobs.py` & `custodian-2024.4.18/custodian/lobster/jobs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module implements jobs for Lobster runs."""
 
 import logging
 import os
+import shlex
 import shutil
 import subprocess
 
 from monty.io import zopen
 from monty.shutil import compress_file
 
 from custodian.custodian import Job
@@ -48,15 +49,15 @@
         self,
         lobster_cmd: str,
         output_file: str = "lobsterout",
         stderr_file: str = "std_err_lobster.txt",
         gzipped: bool = True,
         add_files_to_gzip=(),
         backup: bool = True,
-    ):
+    ) -> None:
         """
 
         Args:
             lobster_cmd: command to run lobster
             output_file: usually lobsterout
             stderr_file: standard output
             gzipped: if True, Lobster files and add_files_to_gzip will be gzipped
@@ -66,34 +67,35 @@
         self.lobster_cmd = lobster_cmd
         self.output_file = output_file
         self.stderr_file = stderr_file
         self.gzipped = gzipped
         self.add_files_to_gzip = add_files_to_gzip
         self.backup = backup
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         """Will backup lobster input files."""
         if self.backup:
             for file in LOBSTERINPUT_FILES:
                 shutil.copy(os.path.join(directory, file), os.path.join(directory, f"{file}.orig"))
 
     def run(self, directory="./"):
         """Runs the job."""
-        cmd = self.lobster_cmd
+        # join split commands (e.g. from atomate and atomate2)
+        cmd = self.lobster_cmd if isinstance(self.lobster_cmd, str) else shlex.join(self.lobster_cmd)
 
-        logger.info(f"Running {' '.join(cmd)}")
+        logger.info(f"Running {cmd}")
 
         with (
             zopen(os.path.join(directory, self.output_file), "w") as f_std,
+            # use line buffering for stderr
             zopen(os.path.join(directory, self.stderr_file), "w", buffering=1) as f_err,
         ):
-            # use line buffering for stderr
-            return subprocess.Popen(cmd, cwd=directory, stdout=f_std, stderr=f_err)  # pylint: disable=R1732
+            return subprocess.run(cmd, stdout=f_std, stderr=f_err, shell=True, check=False)
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """Will gzip relevant files (won't gzip custodian.json and other output files from the cluster)."""
         if self.gzipped:
             for file in LOBSTEROUTPUT_FILES:
                 if os.path.isfile(os.path.join(directory, file)):
                     compress_file(os.path.join(directory, file), compression="gz")
             for file in LOBSTERINPUT_FILES:
                 if os.path.isfile(os.path.join(directory, file)):
```

### Comparing `custodian-2024.3.12/custodian/nwchem/handlers.py` & `custodian-2024.4.18/custodian/nwchem/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class NwchemErrorHandler(ErrorHandler):
     """
     Error handler for Nwchem Jobs. Currently tested only for B3LYP DFT jobs
     generated by pymatgen.
     """
 
-    def __init__(self, output_filename="mol.nwout"):
+    def __init__(self, output_filename="mol.nwout") -> None:
         """Initialize with an output file name.
 
         Args:
             output_filename (str): This is the file where the stdout for nwchem
                 is being redirected. The error messages that are checked are
                 present in the stdout. Defaults to "mol.nwout", which is the
                 default redirect used by :class:`custodian.nwchem.jobs
@@ -69,9 +69,9 @@
 
         m = Modder(directory=directory)
         for action in actions:
             nwi = m.modify_object(action, nwi)
         nwi.write_file(self.input_file)
         return {"errors": self.errors, "actions": actions}
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "NwchemErrorHandler"
```

### Comparing `custodian-2024.3.12/custodian/nwchem/jobs.py` & `custodian-2024.4.18/custodian/nwchem/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self,
         nwchem_cmd,
         input_file="mol.nw",
         output_file="mol.nwout",
         gzipped=False,
         backup=True,
         settings_override=None,
-    ):
+    ) -> None:
         """Initialize a basic NwChem job.
 
         Args:
             nwchem_cmd ([str]): Command to run Nwchem as a list of args. For
                 example, ["nwchem"].
             input_file (str): Input file to run. Defaults to "mol.nw".
             output_file (str): Name of file to direct standard out to.
@@ -49,21 +49,21 @@
         self.nwchem_cmd = nwchem_cmd
         self.input_file = input_file
         self.output_file = output_file
         self.backup = backup
         self.gzipped = gzipped
         self.settings_override = settings_override
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         """Performs backup if necessary."""
         if self.backup:
             shutil.copy(os.path.join(directory, self.input_file), os.path.join(directory, f"{self.input_file}.orig"))
 
     def run(self, directory="./"):
         """Performs actual nwchem run."""
         with zopen(self.output_file, "w") as fout:
             return subprocess.Popen([*self.nwchem_cmd, self.input_file], cwd=directory, stdout=fout)  # pylint: disable=R1732
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """Renaming or gzipping as needed."""
         if self.gzipped:
             gzip_dir(directory)
```

### Comparing `custodian-2024.3.12/custodian/qchem/handlers.py` & `custodian-2024.4.18/custodian/qchem/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,31 +33,31 @@
 
     def __init__(
         self,
         input_file="mol.qin",
         output_file="mol.qout",
         scf_max_cycles=100,
         geom_max_cycles=200,
-    ):
+    ) -> None:
         """Initialize the error handler from a set of input and output files.
 
         Args:
             input_file (str): Name of the QChem input file.
             output_file (str): Name of the QChem output file.
             scf_max_cycles (int): The max iterations to set to fix SCF failure.
             geom_max_cycles (int): The max iterations to set to fix geometry
                 optimization failure.
         """
         self.input_file = input_file
         self.output_file = output_file
         self.scf_max_cycles = scf_max_cycles
         self.geom_max_cycles = geom_max_cycles
         self.outdata = None
-        self.errors = []
-        self.opt_error_history = []
+        self.errors: list[str] = []
+        self.opt_error_history: list[str] = []
 
     def check(self, directory="./"):
         """Checks output file for errors."""
         self._output_path = os.path.join(directory, self.output_file)
         self.outdata = QCOutput(self._output_path).data
         self.errors = self.outdata.get("errors")
         self.warnings = self.outdata.get("warnings")
```

### Comparing `custodian-2024.3.12/custodian/qchem/jobs.py` & `custodian-2024.4.18/custodian/qchem/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         output_file="mol.qout",
         qclog_file="mol.qclog",
         suffix="",
         calc_loc=None,
         nboexe=None,
         save_scratch=False,
         backup=True,
-    ):
+    ) -> None:
         """
         Args:
             qchem_command (str): Command to run QChem.
             max_cores (int): Maximum number of cores to parallelize over.
             multimode (str): Parallelization scheme, either openmp or mpi.
             input_file (str): Name of the QChem input file.
             output_file (str): Name of the QChem output file.
@@ -116,15 +116,15 @@
         multi = {"openmp": "-nt", "mpi": "-np"}
         if self.multimode not in multi:
             raise RuntimeError("ERROR: Multimode should only be set to openmp or mpi")
         command = [multi[self.multimode], str(self.max_cores), self._input_path, self._output_path, "scratch"]
         command = self.qchem_command + command
         return " ".join(command)
 
-    def setup(self, directory: str | Path = "./"):
+    def setup(self, directory: str | Path = "./") -> None:
         """Sets up environment variables necessary to efficiently run QChem.
 
         Args:
             directory (str): The directory to run in. Defaults to "./".
         """
         self._input_path = os.path.join(directory, self.input_file)
         if self.backup:
@@ -141,15 +141,15 @@
             or qcinp.rem.get("nbo_external", "none").lower() == "true"
         ):
             os.environ["KMP_INIT_AT_FORK"] = "FALSE"
             if self.nboexe is None:
                 raise RuntimeError("Trying to run NBO7 without providing NBOEXE in fworker! Exiting...")
             os.environ["NBOEXE"] = self.nboexe
 
-    def postprocess(self, directory: str | Path = "./"):
+    def postprocess(self, directory: str | Path = "./") -> None:
         """Renames and removes scratch files after running QChem.
 
         Args:
             directory (str): The directory to run in. Defaults to "./".
         """
         self._input_path = os.path.join(directory, self.input_file)
         self._output_path = os.path.join(directory, self.output_file)
```

### Comparing `custodian-2024.3.12/custodian/qchem/utils.py` & `custodian-2024.4.18/custodian/qchem/utils.py`

 * *Files identical despite different names*

### Comparing `custodian-2024.3.12/custodian/utils.py` & `custodian-2024.4.18/custodian/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import functools
 import logging
 import os
 import tarfile
 from glob import glob
 
 
-def backup(filenames, prefix="error", directory="./"):
+def backup(filenames, prefix="error", directory="./") -> None:
     """
     Backup files to a tar.gz file. Used, for example, in backing up the
     files of an errored run before performing corrections.
 
     Args:
         filenames ([str]): List of files to backup. Supports wildcards, e.g.,
             *.*.
@@ -58,15 +58,15 @@
     Used to cache the parsed outputs in handlers/validators, to avoid
     multiple parsing of the same file.
     Allows Custodian to clear the cache after all the checks have been performed.
     """
 
     cached_functions: set = set()
 
-    def __init__(self, func):
+    def __init__(self, func) -> None:
         """
         Args:
             func: function to be decorated.
         """
         self.func = functools.lru_cache(func)
         functools.update_wrapper(self, func)
 
@@ -77,12 +77,12 @@
     def __call__(self, *args, **kwargs):
         """Call the decorated function."""
         result = self.func(*args, **kwargs)
         self.cached_functions.add(self.func)
         return result
 
     @classmethod
-    def tracked_cache_clear(cls):
+    def tracked_cache_clear(cls) -> None:
         """Clear the cache of all the decorated functions."""
         while cls.cached_functions:
             f = cls.cached_functions.pop()
             f.cache_clear()
```

### Comparing `custodian-2024.3.12/custodian/vasp/handlers.py` & `custodian-2024.4.18/custodian/vasp/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
     def __init__(
         self,
         output_filename="vasp.out",
         errors_subset_to_catch=None,
         vtst_fixes=False,
         **kwargs,
-    ):
+    ) -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
                 present in the stdout. Defaults to "vasp.out", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
@@ -151,16 +151,16 @@
                 ```
             vtst_fixes (bool): Whether to consider VTST optimizers. Defaults to
                 False for compatibility purposes, but if you have VTST, you
                 would likely benefit from setting this to True.
             **kwargs: Ignored. Added to increase signature flexibility.
         """
         self.output_filename = output_filename
-        self.errors = set()
-        self.error_count = Counter()
+        self.errors: set[str] = set()
+        self.error_count: Counter[str] = Counter()
         self.errors_subset_to_catch = errors_subset_to_catch or list(VaspErrorHandler.error_msgs)
         self.vtst_fixes = vtst_fixes
         self.logger = logging.getLogger(type(self).__name__)
 
     def check(self, directory="./"):
         """Check for error."""
         incar = Incar.from_file(os.path.join(directory, "INCAR"))
@@ -689,15 +689,15 @@
     default due to numerical evaluation of derivatives.
     """
 
     is_monitor = True
 
     error_msgs = {"lrf_comm": ["LRF_COMMUTATOR internal error"]}
 
-    def __init__(self, output_filename: str = "std_err.txt"):
+    def __init__(self, output_filename: str = "std_err.txt") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stderr for vasp
                 is being redirected. The error messages that are checked are
                 present in the stderr. Defaults to "std_err.txt", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
@@ -745,15 +745,15 @@
     is_monitor = True
 
     error_msgs = {
         "kpoints_trans": ["internal error in GENERATE_KPOINTS_TRANS: number of G-vector changed in star"],
         "out_of_memory": ["Allocation would exceed memory limit"],
     }
 
-    def __init__(self, output_filename: str = "std_err.txt"):
+    def __init__(self, output_filename: str = "std_err.txt") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stderr for vasp
                 is being redirected. The error messages that are checked are
                 present in the stderr. Defaults to "std_err.txt", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
@@ -805,15 +805,15 @@
     is_monitor = True
 
     error_msgs = {
         "aliasing": ["WARNING: small aliasing (wrap around) errors must be expected"],
         "aliasing_incar": ["Your FFT grids (NGX,NGY,NGZ) are not sufficient for an accurate"],
     }
 
-    def __init__(self, output_filename: str = "vasp.out"):
+    def __init__(self, output_filename: str = "vasp.out") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
                 present in the stdout. Defaults to "vasp.out", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
@@ -886,15 +886,15 @@
         VaspModder(vi=vi, directory=directory).apply_actions(actions)
         return {"errors": list(self.errors), "actions": actions}
 
 
 class DriftErrorHandler(ErrorHandler):
     """Corrects for total drift exceeding the force convergence criteria."""
 
-    def __init__(self, max_drift=None, to_average=3, enaug_multiply=2):
+    def __init__(self, max_drift=None, to_average=3, enaug_multiply=2) -> None:
         """Initialize the handler with max drift
         Args:
             max_drift (float): This defines the max drift. Leaving this at the default of None gets the max_drift from
                 EDFIFFG.
         """
         self.max_drift = max_drift
         self.to_average = int(to_average)
@@ -966,29 +966,29 @@
     Corrects the mesh symmetry error in VASP. This error is sometimes
     non-fatal. So this error handler only checks at the end of the run,
     and if the run has converged, no error is recorded.
     """
 
     is_monitor = False
 
-    def __init__(self, output_filename: str = "vasp.out", output_vasprun="vasprun.xml"):
+    def __init__(self, output_filename: str = "vasp.out", output_vasprun="vasprun.xml") -> None:
         """Initialize the handler with the output files to check.
 
         Args:
             output_filename (str): This is the file where the stdout for vasp
                 is being redirected. The error messages that are checked are
                 present in the stdout. Defaults to "vasp.out", which is the
                 default redirect used by :class:`custodian.vasp.jobs.VaspJob`.
             output_vasprun (str): Filename for the vasprun.xml file. Change
                 this only if it is different from the default (unlikely).
         """
         self.output_filename = output_filename
         self.output_vasprun = output_vasprun
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         msg = "Reciprocal lattice and k-lattice belong to different class of lattices."
 
         vi = VaspInput.from_directory(directory)
         # disregard this error if KSPACING is set and no KPOINTS file is generated
         if vi["INCAR"].get("KSPACING", False):
             return False
@@ -1028,24 +1028,24 @@
 
 
 class UnconvergedErrorHandler(ErrorHandler):
     """Check if a run is converged."""
 
     is_monitor = False
 
-    def __init__(self, output_filename: str = "vasprun.xml"):
+    def __init__(self, output_filename: str = "vasprun.xml") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): Filename for the vasprun.xml file. Change
                 this only if it is different from the default (unlikely).
         """
         self.output_filename = output_filename
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         try:
             v = load_vasprun(os.path.join(directory, self.output_filename))
             if not v.converged:
                 return True
         except Exception:
             pass
@@ -1151,24 +1151,24 @@
     ISMEAR=-5, and is not a static calculation, which is only appropriate for
     semiconductors. If this occurs, this handler will rerun the calculation
     using the smearing settings appropriate for metals (ISMEAR=2, SIGMA=0.2).
     """
 
     is_monitor = False
 
-    def __init__(self, output_filename: str = "vasprun.xml"):
+    def __init__(self, output_filename: str = "vasprun.xml") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): Filename for the vasprun.xml file. Change
                 this only if it is different from the default (unlikely).
         """
         self.output_filename = output_filename
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         try:
             v = load_vasprun(os.path.join(directory, self.output_filename))
             # check whether bandgap is zero, tetrahedron smearing was used
             # and relaxation is performed.
             if v.eigenvalue_band_properties[0] == 0 and v.incar.get("ISMEAR", 1) < -3 and v.incar.get("NSW", 0) > 1:
                 return True
@@ -1197,24 +1197,24 @@
     will rerun the calculation using the KSPACING setting appropriate for metals
     (KSPACING=0.22). Note that this handler depends on values set by set_kspacing
     logic in MPScanRelaxSet.
     """
 
     is_monitor = False
 
-    def __init__(self, output_filename: str = "vasprun.xml"):
+    def __init__(self, output_filename: str = "vasprun.xml") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): Filename for the vasprun.xml file. Change
                 this only if it is different from the default (unlikely).
         """
         self.output_filename = output_filename
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         try:
             v = load_vasprun(os.path.join(directory, self.output_filename))
             # check whether bandgap is zero and KSPACING is too large
             # using 0 as fallback value for KSPACING so that this handler does not trigger if KSPACING is not set
             if v.eigenvalue_band_properties[0] == 0 and v.incar.get("KSPACING", 0) > 0.22:
                 return True
@@ -1271,18 +1271,18 @@
     When ISMEAR > 0 (Methfessel-Paxton), monitor the magnitude of the entropy
     term T*S in the OUTCAR file. If the entropy term is larger than 1 meV/atom, reduce the
     value of SIGMA. See VASP documentation for ISMEAR.
     """
 
     is_monitor = True
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initializes the handler with a buffer time."""
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         incar = Incar.from_file(os.path.join(directory, "INCAR"))
         try:
             outcar = load_outcar(os.path.join(directory, "OUTCAR"))
         except Exception:
             # Can't perform check if Outcar not valid
             return False
@@ -1339,30 +1339,30 @@
     This is typically caused by too large a POTIM. Runs typically
     end up crashing with some other error (e.g. BRMIX) as the geometry
     gets progressively worse.
     """
 
     is_monitor = True
 
-    def __init__(self, input_filename="POSCAR", output_filename="OSZICAR", dE_threshold=1):
+    def __init__(self, input_filename="POSCAR", output_filename="OSZICAR", dE_threshold=1) -> None:
         """Initialize the handler with the input and output files to check.
 
         Args:
             input_filename (str): This is the POSCAR file that the run
                 started from. Defaults to "POSCAR". Change
                 this only if it is different from the default (unlikely).
             output_filename (str): This is the OSZICAR file. Change
                 this only if it is different from the default (unlikely).
             dE_threshold (float): The threshold energy change. Defaults to 1eV.
         """
         self.input_filename = input_filename
         self.output_filename = output_filename
         self.dE_threshold = dE_threshold
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool | None:
         """Check for error."""
         try:
             oszicar = Oszicar(os.path.join(directory, self.output_filename))
             n = len(Poscar.from_file(self.input_filename).structure)
             max_dE = max(s["dE"] for s in oszicar.ionic_steps[1:]) / n
             if max_dE > self.dE_threshold:
                 return True
@@ -1406,15 +1406,15 @@
             timeout (int): The time in seconds between checks where if there
                 is no activity on the output file, the run is considered
                 frozen. Defaults to 3600 seconds, i.e., 1 hour.
         """
         self.output_filename = output_filename
         self.timeout = timeout
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool | None:
         """Check for error."""
         st = os.stat(os.path.join(directory, self.output_filename))
         if time.time() - st.st_mtime > self.timeout:
             return True
         return None
 
     def correct(self, directory="./"):
@@ -1438,15 +1438,15 @@
     Check if a run is hitting the maximum number of electronic steps at the
     last nionic_steps ionic steps (default=10). If so, change ALGO using a
     multi-step ladder scheme or kill the job.
     """
 
     is_monitor = True
 
-    def __init__(self, output_filename: str = "OSZICAR", nionic_steps=10):
+    def __init__(self, output_filename: str = "OSZICAR", nionic_steps=10) -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): This is the OSZICAR file. Change
                 this only if it is different from the default (unlikely).
             nionic_steps (int): The threshold number of ionic steps that
                 needs to hit the maximum number of electronic steps for the
@@ -1574,15 +1574,15 @@
     # itself naturally with the STOPCAR.
     is_terminating = False
 
     # This handler will be unrecoverable, but custodian shouldn't raise an
     # error
     raises_runtime_error = False
 
-    def __init__(self, wall_time=None, buffer_time=300, electronic_step_stop=False):
+    def __init__(self, wall_time=None, buffer_time=300, electronic_step_stop=False) -> None:
         """Initialize the handler with a buffer time.
 
         Args:
             wall_time (int): Total walltime in seconds. If this is None and
                 the job is running on a PBS system, the handler will attempt to
                 determine the walltime from the PBS_WALLTIME environment
                 variable. If the wall time cannot be determined or is not
@@ -1626,15 +1626,15 @@
                 self.start_time, "%a %b %d %H:%M:%S UTC %Y"
             )
 
         self.electronic_step_stop = electronic_step_stop
         self.electronic_steps_timings = [0]
         self.prev_check_time = self.start_time
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         if self.wall_time:
             run_time = datetime.datetime.now() - self.start_time
             total_secs = run_time.total_seconds()
             outcar = load_outcar(os.path.join(directory, "OUTCAR"))
             if not self.electronic_step_stop:
                 # Determine max time per ionic step.
@@ -1679,32 +1679,30 @@
 
     is_monitor = True
 
     # The CheckpointHandler should not terminate as we want VASP to terminate
     # itself naturally with the STOPCAR.
     is_terminating = False
 
-    def __init__(self, interval=3600):
+    def __init__(self, interval=3600) -> None:
         """Initialize the handler with an interval.
 
         Args:
             interval (int): Interval at which to checkpoint in seconds.
             Defaults to 3600 (1 hr).
         """
         self.interval = interval
         self.start_time = datetime.datetime.now()
         self.chk_counter = 0
 
     def check(self, directory="./"):
         """Check for error."""
         run_time = datetime.datetime.now() - self.start_time
         total_secs = run_time.seconds + run_time.days * 3600 * 24
-        if total_secs > self.interval:
-            return True
-        return False
+        return total_secs > self.interval
 
     def correct(self, directory="./"):
         """Perform corrections."""
         content = "LSTOP = .TRUE."
         chkpt_content = f'Index: {self.chk_counter}\nTime: "{datetime.datetime.now()}"'
         self.chk_counter += 1
 
@@ -1722,15 +1720,15 @@
             modder.modify(action["action"], action["file"])
 
         # Reset the clock.
         self.start_time = datetime.datetime.now()
 
         return {"errors": ["Checkpoint reached"], "actions": actions}
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"CheckpointHandler with interval {self.interval}"
 
 
 class StoppedRunHandler(ErrorHandler):
     """
     This is not an error handler per se, but rather a checkpointer. What this
     does is that every X seconds, a STOPCAR will be written. This forces VASP to
@@ -1744,15 +1742,15 @@
 
     is_monitor = False
 
     # The CheckpointHandler should not terminate as we want VASP to terminate
     # itself naturally with the STOPCAR.
     is_terminating = False
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Dummy init."""
 
     def check(self, directory="./"):
         """Check for error."""
         return os.path.isfile(os.path.join(directory, "chkpt.yaml"))
 
     def correct(self, directory="./"):
@@ -1776,24 +1774,24 @@
     """
     Check if a run has positive absolute energy.
     If so, change ALGO from Fast to Normal or kill the job.
     """
 
     is_monitor = True
 
-    def __init__(self, output_filename: str = "OSZICAR"):
+    def __init__(self, output_filename: str = "OSZICAR") -> None:
         """Initialize the handler with the output file to check.
 
         Args:
             output_filename (str): This is the OSZICAR file. Change
                 this only if it is different from the default (unlikely).
         """
         self.output_filename = output_filename
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for error."""
         try:
             oszicar = Oszicar(os.path.join(directory, self.output_filename))
             if oszicar.final_energy > 0:
                 return True
         except Exception:
             pass
```

### Comparing `custodian-2024.3.12/custodian/vasp/interpreter.py` & `custodian-2024.4.18/custodian/vasp/interpreter.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from custodian.ansible.actions import DictActions, FileActions
 from custodian.ansible.interpreter import Modder
 
 
 class VaspModder(Modder):
     """A Modder for VaspInputSets."""
 
-    def __init__(self, actions=None, strict=True, vi=None, directory="./"):
+    def __init__(self, actions=None, strict=True, vi=None, directory="./") -> None:
         """Initialize a Modder for VaspInput sets.
 
         Args:
             actions ([Action]): A sequence of supported actions. See
                 :mod:`custodian.ansible.actions`. Default is None,
                 which means DictActions and FileActions are supported.
             strict (bool): Indicating whether to use strict mode. In non-strict
@@ -27,15 +27,15 @@
                 avoid having to reparse the directory).
         """
         self.vi = vi or VaspInput.from_directory(directory)
         self.directory = directory
         actions = actions or [FileActions, DictActions]
         super().__init__(actions, strict)
 
-    def apply_actions(self, actions):
+    def apply_actions(self, actions) -> None:
         """
         Applies a list of actions to the Vasp Input Set and rewrites modified
         files.
 
         Args:
             actions (dict): A list of actions of the form {'file': filename,
                 'action': moddermodification} or {'dict': vaspinput_key,
```

### Comparing `custodian-2024.3.12/custodian/vasp/io.py` & `custodian-2024.4.18/custodian/vasp/io.py`

 * *Files identical despite different names*

### Comparing `custodian-2024.3.12/custodian/vasp/jobs.py` & `custodian-2024.4.18/custodian/vasp/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         backup=True,
         auto_npar=False,
         auto_gamma=True,
         settings_override=None,
         gamma_vasp_cmd=None,
         copy_magmom=False,
         auto_continue=False,
-    ):
+    ) -> None:
         """
         This constructor is necessarily complex due to the need for
         flexibility. For standard kinds of runs, it's often better to use one
         of the static constructors. The defaults are usually fine too.
 
         Args:
             vasp_cmd (str): Command to run vasp as a list of args. For example,
@@ -162,15 +162,15 @@
                         vasp_path = which(vasp_cmd[-1])
                     scope.set_tag("vasp_path", vasp_path)
                     scope.set_tag("vasp_cmd", vasp_cmd)
                 except Exception:
                     logger.exception(f"Failed to detect VASP path: {vasp_cmd}")
                     scope.set_tag("vasp_cmd", vasp_cmd)
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         """
         Performs initial setup for VaspJob, including overriding any settings
         and backing up.
         """
         decompress_dir(directory)
 
         if self.backup:
@@ -251,15 +251,15 @@
         with (
             open(os.path.join(directory, self.output_file), "w") as f_std,
             open(os.path.join(directory, self.stderr_file), "w", buffering=1) as f_err,
         ):
             # use line buffering for stderr
             return subprocess.Popen(cmd, cwd=directory, stdout=f_std, stderr=f_err, start_new_session=True)  # pylint: disable=R1732
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """
         Postprocessing includes renaming and gzipping where necessary.
         Also copies the magmom to the incar if necessary.
         """
         for file in (*VASP_OUTPUT_FILES, self.output_file):
             file = os.path.join(directory, file)
             if os.path.isfile(file):
@@ -567,15 +567,15 @@
         """
         nsw = 99 if atom_relax else 0
 
         incar = Incar.from_file(os.path.join(directory, "INCAR"))
 
         # Set the energy convergence criteria as the EDIFFG (if present) or
         # 10 x EDIFF (which itself defaults to 1e-4 if not present).
-        etol = incar["EDIFFG"] if incar.get("EDIFFG") and incar.get("EDIFFG") > 0 else incar.get("EDIFF", 0.0001) * 10
+        e_tol = incar["EDIFFG"] if incar.get("EDIFFG") and incar.get("EDIFFG") > 0 else incar.get("EDIFF", 0.0001) * 10
 
         if lattice_direction == "a":
             lattice_index = 0
         elif lattice_direction == "b":
             lattice_index = 1
         else:
             lattice_index = 2
@@ -608,15 +608,15 @@
                     ind = sorted_x.index(min_x)
                     if ind == 0:
                         other = ind + 1
                     elif ind == len(sorted_x) - 1:
                         other = ind - 1
                     else:
                         other = ind + 1 if energies[sorted_x[ind + 1]] < energies[sorted_x[ind - 1]] else ind - 1
-                    if abs(energies[min_x] - energies[sorted_x[other]]) < etol:
+                    if abs(energies[min_x] - energies[sorted_x[other]]) < e_tol:
                         logger.info(f"Stopping optimization! Final {lattice_direction} = {min_x}")
                         break
 
                     if ind == 0 and len(sorted_x) > 2:
                         # Lowest energy lies outside of range of lowest value.
                         # we decrease the lattice parameter in the next
                         # iteration to find a minimum. This applies only when
@@ -680,42 +680,41 @@
             )
 
         with open(os.path.join(directory, "EOS.txt"), "w") as file:
             file.write(f"# {lattice_direction} energy\n")
             for key in sorted(energies):
                 file.write(f"{key} {energies[key]}\n")
 
-    def terminate(self, directory="./"):
+    def terminate(self, directory="./") -> None:
         """
         Kill all VASP processes associated with the current job.
         This is done by looping over all processes and selecting the ones
         that contain "vasp" as well as access files (vasprun.xml in particular)
         in the custodian working directory.
         There is also a safety that kills all VASP processes if none of the
         processes can be killed (This is bad if more than one VASP runs are
         simultaneously executed on the same node). However, this should never
         happen.
         """
-        workdir = directory
-        logger.info(f"Killing VASP processes in workdir {workdir}.")
+        work_dir = directory
+        logger.info(f"Killing VASP processes in {work_dir=}.")
         for proc in psutil.process_iter():
             try:
                 if "vasp" in proc.name().lower():
                     open_paths = [file.path for file in proc.open_files()]
-                    vasprun_path = os.path.join(workdir, "vasprun.xml")
+                    vasprun_path = os.path.join(work_dir, "vasprun.xml")
                     if (vasprun_path in open_paths) and psutil.pid_exists(proc.pid):
                         proc.kill()
                         return
             except (psutil.NoSuchProcess, psutil.AccessDenied) as exc:
                 logger.warning(f"Exception {exc} encountered while killing VASP.")
                 continue
 
         logger.warning(
-            f"Killing VASP processes in workdir {workdir} failed with subprocess.Popen.terminate(). "
-            "Resorting to 'killall'."
+            f"Killing VASP processes in {work_dir=} failed with subprocess.Popen.terminate(). Resorting to 'killall'."
         )
         cmds = self.vasp_cmd
         if self.gamma_vasp_cmd:
             cmds += self.gamma_vasp_cmd
         for cmd in cmds:
             if "vasp" in cmd:
                 subprocess.run(["killall", f"{cmd}"], check=False)
@@ -738,15 +737,15 @@
         backup=True,
         auto_npar=True,
         half_kpts=False,
         auto_gamma=True,
         auto_continue=False,
         gamma_vasp_cmd=None,
         settings_override=None,
-    ):
+    ) -> None:
         """
         This constructor is a simplified version of VaspJob, which satisfies
         the need for flexibility. For standard kinds of runs, it's often
         better to use one of the static constructors. The defaults are
         usually fine too.
 
         Args:
@@ -803,15 +802,15 @@
         self.auto_npar = auto_npar
         self.half_kpts = half_kpts
         self.auto_gamma = auto_gamma
         self.gamma_vasp_cmd = tuple(gamma_vasp_cmd) if gamma_vasp_cmd else None
         self.auto_continue = auto_continue
         self.settings_override = settings_override
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         """
         Performs initial setup for VaspNEBJob, including overriding any settings
         and backing up.
         """
         neb_dirs, neb_sub = self._get_neb_dirs(directory)
 
         if self.backup:
@@ -898,19 +897,19 @@
                 cmd,
                 cwd=directory,
                 stdout=f_std,
                 stderr=f_err,
                 start_new_session=True,
             )  # pylint: disable=R1732
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """Postprocessing includes renaming and gzipping where necessary."""
         # Add suffix to all sub_dir/{items}
 
-        neb_dirs, neb_sub = self._get_neb_dirs(directory)
+        neb_dirs, _neb_sub = self._get_neb_dirs(directory)
 
         for path in neb_dirs:
             for file in VASP_NEB_OUTPUT_SUB_FILES:
                 file = os.path.join(path, file)
                 if os.path.isfile(file):
                     if self.final and self.suffix != "":
                         shutil.move(file, f"{file}{self.suffix}")
@@ -936,38 +935,38 @@
 
 class GenerateVaspInputJob(Job):
     """
     Generates a VASP input based on an existing directory. This is typically
     used to modify the VASP input files before the next VaspJob.
     """
 
-    def __init__(self, input_set, contcar_only=True, **kwargs):
+    def __init__(self, input_set, contcar_only=True, **kwargs) -> None:
         """
         Args:
             input_set (str): Full path to the input set. E.g.,
                 "pymatgen.io.vasp.sets.MPNonSCFSet".
             contcar_only (bool): If True (default), only CONTCAR structures
                 are used as input to the input set.
             **kwargs: Additional kwargs to pass to the input set.
         """
         self.input_set = input_set
         self.contcar_only = contcar_only
         self.kwargs = kwargs
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         """Dummy setup."""
 
-    def run(self, directory="./"):
+    def run(self, directory="./") -> None:
         """Run the calculation."""
         if os.path.isfile(os.path.join(directory, "CONTCAR")):
             structure = Structure.from_file(os.path.join(directory, "CONTCAR"))
         elif (not self.contcar_only) and os.path.isfile(os.path.join(directory, "POSCAR")):
             structure = Structure.from_file(os.path.join(directory, "POSCAR"))
         else:
             raise RuntimeError("No CONTCAR/POSCAR detected to generate input!")
         modname, classname = self.input_set.rsplit(".", 1)
         mod = __import__(modname, globals(), locals(), [classname], 0)
         vis = getattr(mod, classname)(structure, **self.kwargs)
         vis.write_input(directory)
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         """Dummy postprocess."""
```

### Comparing `custodian-2024.3.12/custodian/vasp/validators.py` & `custodian-2024.4.18/custodian/vasp/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Implements various validators, e.g., check if vasprun.xml is valid, for VASP."""
 
+from __future__ import annotations
+
 import logging
 import os
 from collections import deque
 
 from pymatgen.io.vasp import Chgcar, Incar
 
 from custodian.custodian import Validator
@@ -21,20 +23,20 @@
             stderr_file (str): Name of file VASP standard error is direct to.
                 Defaults to "std_err.txt".
         """
         self.output_file = output_file
         self.stderr_file = stderr_file
         self.logger = logging.getLogger(type(self).__name__)
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         """Check for errors."""
         try:
             load_vasprun(os.path.join(directory, "vasprun.xml"))
         except Exception:
-            exception_context = {}
+            exception_context: dict[str, str | float] = {}
 
             if os.path.isfile(os.path.join(directory, self.output_file)):
                 with open(os.path.join(directory, self.output_file)) as output_file:
                     output_file_tail = deque(output_file, maxlen=10)
                 exception_context["output_file_tail"] = "".join(output_file_tail)
 
             if os.path.isfile(os.path.join(directory, self.stderr_file)):
@@ -61,61 +63,59 @@
 
 class VaspFilesValidator(Validator):
     """
     Check for existence of some of the files that VASP
         normally create upon running.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Dummy init."""
 
     def check(self, directory="./"):
         """Check for error."""
         return any(not os.path.isfile(os.path.join(directory, vfile)) for vfile in ("CONTCAR", "OSZICAR", "OUTCAR"))
 
 
 class VaspNpTMDValidator(Validator):
     """
     Check NpT-AIMD settings is loaded by VASP compiled with -Dtbdyn.
     Currently, VASP only have Langevin thermostat (MDALGO = 3) for NpT ensemble.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Dummy init."""
 
     def check(self, directory="./"):
         """Check for error."""
         incar = Incar.from_file(os.path.join(directory, "INCAR"))
         is_npt = incar.get("MDALGO") == 3
         if not is_npt:
             return False
 
         outcar = load_outcar(os.path.join(directory, "OUTCAR"))
         patterns = {"MDALGO": r"MDALGO\s+=\s+([\d]+)"}
         outcar.read_pattern(patterns=patterns)
-        if outcar.data["MDALGO"] == [["3"]]:
-            return False
-        return True
+        return outcar.data["MDALGO"] != [["3"]]
 
 
 class VaspAECCARValidator(Validator):
     """Check if the data in the AECCAR is corrupted."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Dummy init."""
 
     def check(self, directory="./"):
         """Check for error."""
         aeccar0 = Chgcar.from_file(os.path.join(directory, "AECCAR0"))
         aeccar2 = Chgcar.from_file(os.path.join(directory, "AECCAR2"))
         aeccar = aeccar0 + aeccar2
         return check_broken_chgcar(aeccar)
 
 
-def check_broken_chgcar(chgcar, diff_thresh=None):
+def check_broken_chgcar(chgcar, diff_thresh=None) -> bool:
     """
     Check if the charge density file is corrupt
     Args:
         chgcar (Chgcar): Chgcar-like object.
         diff_thresh (Float): Threshold for diagonal difference.
             None means we won't check for this.
     """
```

### Comparing `custodian-2024.3.12/custodian.egg-info/PKG-INFO` & `custodian-2024.4.18/custodian.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custodian
-Version: 2024.3.12
+Version: 2024.4.18
 Summary: A simple JIT job management framework in Python.
 Author: Matthew Horton, Samuel M. Blau, Stephen Dacek, William Davidson Richards, Xiaohui Qu
 Author-email: Janosh Riebesell <janosh.riebesell@gmail.com>, Shyue Ping Ong <ongsp@ucsd.edu>
 Maintainer: Janosh Riebesell, Shyue Ping Ong
 License: The MIT License (MIT)
         Copyright (c) 2011-2012 MIT & LBNL
```

### Comparing `custodian-2024.3.12/custodian.egg-info/SOURCES.txt` & `custodian-2024.4.18/custodian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custodian-2024.3.12/pyproject.toml` & `custodian-2024.4.18/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "custodian"
-version = "2024.3.12"
+version = "2024.4.18"
 description = "A simple JIT job management framework in Python."
 authors = [
   { name = "Janosh Riebesell", email = "janosh.riebesell@gmail.com" },
   { name = "Matthew Horton" },
   { name = "Samuel M. Blau" },
   { name = "Shyue Ping Ong", email = "ongsp@ucsd.edu" },
   { name = "Stephen Dacek" },
@@ -98,33 +98,35 @@
   "YTT",  # flake8-2020
 ]
 ignore = [
   "B023",    # Function definition does not bind loop variable
   "B028",    # No explicit stacklevel keyword argument found
   "B904",    # Within an except clause, raise exceptions with ...
   "C408",    # unnecessary-collection-call
+  "COM812",
   "D105",    # Missing docstring in magic method
   "D205",    # 1 blank line required between summary line and description
   "D212",    # Multi-line docstring summary should start at the first line
   "ISC001",
   "PD011",   # pandas-use-of-dot-values
   "PD901",   # pandas-df-variable-name
   "PERF203", # try-except-in-loop
   "PLR",     # pylint refactor
   "PLW2901", # Outer for loop variable overwritten by inner assignment target
   "PT013",   # pytest-incorrect-pytest-import
-  "RUF012",  # Disable checks for mutable class args. This is a non-problem.
+  "PTH",
+  "RUF012",  # Disable checks for mutable class args
   "SIM105",  # Use contextlib.suppress(OSError) instead of try-except-pass
 ]
 pydocstyle.convention = "google"
 isort.split-on-trailing-comma = false
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
-"tests/*" = ["D"]
+"tests/*" = ["D", "S101"]
 "tasks.py" = ["D", "E"]
 
 [tool.pytest.ini_options]
 addopts = "--color=yes -p no:warnings --import-mode=importlib"
 
 [tool.mypy]
 ignore_missing_imports = true
```

### Comparing `custodian-2024.3.12/tests/test_custodian.py` & `custodian-2024.4.18/tests/test_custodian.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,52 +18,52 @@
     ReturnCodeError,
     ValidationError,
     Validator,
 )
 
 
 class ExitCodeJob(Job):
-    def __init__(self, exitcode=0):
+    def __init__(self, exitcode=0) -> None:
         self.exitcode = exitcode
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         pass
 
     def run(self, directory="./"):
         return subprocess.Popen(f"exit {self.exitcode}", cwd=directory, shell=True)
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         pass
 
 
 class ExampleJob(Job):
-    def __init__(self, jobid, params=None):
+    def __init__(self, jobid, params=None) -> None:
         if params is None:
             params = {"initial": 0, "total": 0}
         self.jobid = jobid
         self.params = params
 
-    def setup(self, directory="./"):
+    def setup(self, directory="./") -> None:
         self.params["initial"] = 0
         self.params["total"] = 0
 
-    def run(self, directory="./"):
+    def run(self, directory="./") -> None:
         sequence = [random.uniform(0, 1) for i in range(100)]
         self.params["total"] = self.params["initial"] + sum(sequence)
 
-    def postprocess(self, directory="./"):
+    def postprocess(self, directory="./") -> None:
         pass
 
     @property
-    def name(self):
+    def name(self) -> str:
         return f"ExampleJob{self.jobid}"
 
 
 class ExampleHandler(ErrorHandler):
-    def __init__(self, params):
+    def __init__(self, params) -> None:
         self.params = params
 
     def check(self, directory="./"):
         return self.params["total"] < 50
 
     def correct(self, directory="./"):
         self.params["initial"] += 1
@@ -71,37 +71,37 @@
 
 
 class ExampleHandler1b(ExampleHandler):
     """
     This handler always can apply a correction, but will only apply it twice before raising.
     """
 
-    max_num_corrections = 2  # type: ignore
+    max_num_corrections = 2
     raise_on_max = True
 
 
 class ExampleHandler1c(ExampleHandler):
     """
     This handler always can apply a correction, but will only apply it twice and then not anymore.
     """
 
-    max_num_corrections = 2  # type: ignore
+    max_num_corrections = 2
     raise_on_max = False
 
 
 class ExampleHandler2(ErrorHandler):
     """
     This handler always result in an error.
     """
 
-    def __init__(self, params):
+    def __init__(self, params) -> None:
         self.params = params
         self.has_error = False
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         return True
 
     def correct(self, directory="./"):
         self.has_error = True
         return {"errors": "Unrecoverable error", "actions": None}
 
 
@@ -114,59 +114,59 @@
 
     def correct(self, directory="./"):
         self.has_error = True
         return {"errors": "Unrecoverable error", "actions": []}
 
 
 class ExampleValidator1(Validator):
-    def __init__(self):
+    def __init__(self) -> None:
         pass
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         return False
 
 
 class ExampleValidator2(Validator):
-    def __init__(self):
+    def __init__(self) -> None:
         pass
 
-    def check(self, directory="./"):
+    def check(self, directory="./") -> bool:
         return True
 
 
 class CustodianTest(unittest.TestCase):
-    def setUp(self):
+    def setUp(self) -> None:
         self.cwd = os.getcwd()
         os.chdir(os.path.abspath(os.path.dirname(__file__)))
 
-    def test_exitcode_error(self):
+    def test_exitcode_error(self) -> None:
         c = Custodian([], [ExitCodeJob(0)])
         c.run()
         c = Custodian([], [ExitCodeJob(1)])
         with pytest.raises(
             ReturnCodeError,
         ):
             c.run()
         assert c.run_log[-1]["nonzero_return_code"]
         c = Custodian([], [ExitCodeJob(1)], terminate_on_nonzero_returncode=False)
         c.run()
 
-    def test_run(self):
+    def test_run(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         c = Custodian(
             [ExampleHandler(params)],
             [ExampleJob(i, params) for i in range(n_jobs)],
             max_errors=n_jobs,
         )
         output = c.run()
         assert len(output) == n_jobs
         ExampleHandler(params).as_dict()
 
-    def test_run_interrupted(self):
+    def test_run_interrupted(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         c = Custodian(
             [ExampleHandler(params)],
             [ExampleJob(i, params) for i in range(n_jobs)],
             max_errors=n_jobs,
         )
@@ -177,57 +177,57 @@
         total_done = 1
         while total_done < n_jobs:
             c.jobs[n_jobs - 1].run()
             if params["total"] > 50:
                 assert c.run_interrupted() == n_jobs - total_done
                 total_done += 1
 
-    def test_unrecoverable(self):
+    def test_unrecoverable(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         handler = ExampleHandler2(params)
         c = Custodian([handler], [ExampleJob(i, params) for i in range(n_jobs)], max_errors=n_jobs)
         with pytest.raises(NonRecoverableError):
             c.run()
         assert handler.has_error
         handler = ExampleHandler2b(params)
         c = Custodian([handler], [ExampleJob(i, params) for i in range(n_jobs)], max_errors=n_jobs)
         c.run()
         assert handler.has_error
         assert c.run_log[-1]["handler"] == handler
 
-    def test_max_errors(self):
+    def test_max_errors(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         handler = ExampleHandler(params)
         c = Custodian(
             [handler],
             [ExampleJob(i, params) for i in range(n_jobs)],
             max_errors=1,
             max_errors_per_job=10,
         )
         with pytest.raises(MaxCorrectionsError):
             c.run()
         assert c.run_log[-1]["max_errors"]
 
-    def test_max_errors_per_job(self):
+    def test_max_errors_per_job(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         handler = ExampleHandler(params)
         c = Custodian(
             [handler],
             [ExampleJob(i, params) for i in range(n_jobs)],
             max_errors=n_jobs,
             max_errors_per_job=1,
         )
         with pytest.raises(MaxCorrectionsPerJobError):
             c.run()
         assert c.run_log[-1]["max_errors_per_job"]
 
-    def test_max_errors_per_handler_raise(self):
+    def test_max_errors_per_handler_raise(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         handler = ExampleHandler1b(params)
         c = Custodian(
             [handler],
             [ExampleJob(i, params) for i in range(n_jobs)],
             max_errors=n_jobs * 10,
@@ -236,27 +236,27 @@
         with pytest.raises(MaxCorrectionsPerHandlerError):
             c.run()
         assert handler.n_applied_corrections == 2
         assert len(c.run_log[-1]["corrections"]) == 2
         assert c.run_log[-1]["max_errors_per_handler"]
         assert c.run_log[-1]["handler"] == handler
 
-    def test_max_errors_per_handler_warning(self):
+    def test_max_errors_per_handler_warning(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         c = Custodian(
             [ExampleHandler1c(params)],
             [ExampleJob(i, params) for i in range(n_jobs)],
             max_errors=n_jobs * 10,
             max_errors_per_job=1000,
         )
         c.run()
         assert all(len(r["corrections"]) <= 2 for r in c.run_log)
 
-    def test_validators(self):
+    def test_validators(self) -> None:
         n_jobs = 100
         params = {"initial": 0, "total": 0}
         c = Custodian(
             [ExampleHandler(params)],
             [ExampleJob(i, params) for i in range(n_jobs)],
             [ExampleValidator1()],
             max_errors=n_jobs,
@@ -273,15 +273,15 @@
             [v],
             max_errors=n_jobs,
         )
         with pytest.raises(ValidationError):
             c.run()
         assert c.run_log[-1]["validator"] == v
 
-    def test_from_spec(self):
+    def test_from_spec(self) -> None:
         spec = """jobs:
 - jb: custodian.vasp.jobs.VaspJob
   params:
     final: False
     suffix: .relax1
 - jb: custodian.vasp.jobs.VaspJob
   params:
@@ -305,15 +305,15 @@
         c = Custodian.from_spec(dct)
         assert c.jobs[0].vasp_cmd[2] == "whatever"
         assert c.scratch_dir == "/tmp/random"
         assert len(c.jobs) == 2
         assert len(c.handlers) == 3
         assert len(c.validators) == 1
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         for file in glob("custodian.*.tar.gz"):
             os.remove(file)
         try:
             os.remove("custodian.json")
         except OSError:
             pass  # Ignore if file cannot be found.
         os.chdir(self.cwd)
```

### Comparing `custodian-2024.3.12/tests/test_utils.py` & `custodian-2024.4.18/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from custodian.utils import tracked_lru_cache
 
 
-def test_cache_and_clear():
+def test_cache_and_clear() -> None:
     n_calls = 0
 
     @tracked_lru_cache
     def some_func(x):
         nonlocal n_calls
         n_calls += 1
         return x
```

