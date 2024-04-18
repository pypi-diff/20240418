# Comparing `tmp/cubinlinker_cu11-0.3.0.post1.tar.gz` & `tmp/cubinlinker_cu11-0.3.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubinlinker_cu11-0.3.0.post1.tar", last modified: Wed Jan 25 17:33:35 2023, max compression
+gzip compressed data, was "cubinlinker_cu11-0.3.0.post2.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `cubinlinker_cu11-0.3.0.post1.tar` & `cubinlinker_cu11-0.3.0.post2.tar`

### file list

```diff
@@ -1,11 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-01-25 17:33:35.146364 cubinlinker_cu11-0.3.0.post1/
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-01-25 17:32:12.000000 cubinlinker_cu11-0.3.0.post1/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1617 2023-01-25 17:33:35.146364 cubinlinker_cu11-0.3.0.post1/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      253 2023-01-25 17:33:35.000000 cubinlinker_cu11-0.3.0.post1/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-01-25 17:33:35.145364 cubinlinker_cu11-0.3.0.post1/cubinlinker_cu11.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1617 2023-01-25 17:33:35.000000 cubinlinker_cu11-0.3.0.post1/cubinlinker_cu11.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      190 2023-01-25 17:33:35.000000 cubinlinker_cu11-0.3.0.post1/cubinlinker_cu11.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-01-25 17:33:35.000000 cubinlinker_cu11-0.3.0.post1/cubinlinker_cu11.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-01-25 17:33:35.000000 cubinlinker_cu11-0.3.0.post1/cubinlinker_cu11.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-01-25 17:33:35.146364 cubinlinker_cu11-0.3.0.post1/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-01-25 17:32:12.000000 cubinlinker_cu11-0.3.0.post1/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0      259 1993-04-05 07:00:00.000000 PKG-INFO
```

