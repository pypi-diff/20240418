# Comparing `tmp/pynvjitlink-cu12-0.1.6.tar.gz` & `tmp/pynvjitlink_cu12-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynvjitlink-cu12-0.1.6.tar", last modified: Tue Jan  9 16:31:17 2024, max compression
+gzip compressed data, was "pynvjitlink_cu12-0.2.1.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `pynvjitlink-cu12-0.1.6.tar` & `pynvjitlink_cu12-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,2 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-09 16:31:17.840858 pynvjitlink-cu12-0.1.6/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      463 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2024-01-09 16:28:41.000000 pynvjitlink-cu12-0.1.6/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       16 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1649 2024-01-09 16:31:17.838858 pynvjitlink-cu12-0.1.6/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      268 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2024-01-09 16:31:17.837858 pynvjitlink-cu12-0.1.6/pynvjitlink_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1649 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/pynvjitlink_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      213 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/pynvjitlink_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/pynvjitlink_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2024-01-09 16:31:17.000000 pynvjitlink-cu12-0.1.6/pynvjitlink_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2024-01-09 16:31:17.840858 pynvjitlink-cu12-0.1.6/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4864 2024-01-09 16:28:41.000000 pynvjitlink-cu12-0.1.6/setup.py
+-rw-r--r--   0        0        0      217 1993-04-05 07:00:00.000000 pyproject.toml
+-rw-r--r--   0        0        0     1323 1993-04-05 07:00:00.000000 PKG-INFO
```

