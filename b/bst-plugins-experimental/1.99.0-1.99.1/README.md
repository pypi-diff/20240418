# Comparing `tmp/bst_plugins_experimental-1.99.0.tar.gz` & `tmp/bst_plugins_experimental-1.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bst_plugins_experimental-1.99.0.tar", last modified: Wed Apr 17 09:25:56 2024, max compression
+gzip compressed data, was "bst_plugins_experimental-1.99.1.tar", last modified: Thu Apr 18 16:23:50 2024, max compression
```

## Comparing `bst_plugins_experimental-1.99.0.tar` & `bst_plugins_experimental-1.99.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.436927 bst_plugins_experimental-1.99.0/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/LICENSE
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/MANIFEST.in
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-17 09:25:56.436927 bst_plugins_experimental-1.99.0/PKG-INFO
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/README.rst
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      773 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/project.conf
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2731 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/pyproject.toml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.420927 bst_plugins_experimental-1.99.0/requirements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      213 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/requirements/plugin-requirements.txt
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/requirements/test-requirements.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       38 2024-04-17 09:25:56.436927 bst_plugins_experimental-1.99.0/setup.cfg
--rwxrwxrwx   0 testuser  (1000) testuser  (1000)       61 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/setup.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.417927 bst_plugins_experimental-1.99.0/src/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.421927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.430927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11344 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazelize.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazelize.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2149 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/check_forbidden.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_integration.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10889 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_manifest.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7669 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1084 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/oci.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/pyproject.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/pyproject.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2895 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/snap_image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/snap_image.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/tar_element.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/tar_element.yaml
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.yaml
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.433927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    15419 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_git_utils.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6386 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_utils.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13073 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/bazel_source.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4025 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/cpan.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/deb.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_module.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3672 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_repo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35633 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_tag.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5113 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/go_module.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/ostree.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2663 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/patch_queue.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5888 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/pypi.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/quilt.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/zip.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.433927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/__init__.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.434927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/__init__.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/gitrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/tarrepo.py
--rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2024-04-17 09:25:43.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ziprepo.py
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.435927 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1000) testuser  (1000)     3476 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)     1806 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/requires.txt
--rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2024-04-17 09:25:56.000000 bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/top_level.txt
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/lib/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/lib/python3.11/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.418927 bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/
-drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-17 09:25:56.435927 bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/markdown_it/
--rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2024-04-17 09:25:53.000000 bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/markdown_it/port.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.897105 bst_plugins_experimental-1.99.1/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    26471 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/LICENSE
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       66 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/MANIFEST.in
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-18 16:23:50.897105 bst_plugins_experimental-1.99.1/PKG-INFO
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2705 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/README.rst
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      773 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/project.conf
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2731 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/pyproject.toml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.883105 bst_plugins_experimental-1.99.1/requirements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      213 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/requirements/plugin-requirements.txt
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      166 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/requirements/test-requirements.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       38 2024-04-18 16:23:50.897105 bst_plugins_experimental-1.99.1/setup.cfg
+-rwxrwxrwx   0 testuser  (1000) testuser  (1000)       61 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/setup.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.880105 bst_plugins_experimental-1.99.1/src/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.883105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.891105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2574 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1082 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    11344 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazelize.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazelize.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2149 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/check_forbidden.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3925 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_integration.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10872 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_manifest.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8503 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1536 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    10286 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      912 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2752 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1354 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3023 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1045 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     7669 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       36 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4757 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1432 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1634 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1079 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1650 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1084 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35832 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/oci.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      985 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/pyproject.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      339 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/pyproject.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1570 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      894 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2895 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/snap_image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)       60 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/snap_image.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3979 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/tar_element.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      286 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/tar_element.yaml
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3021 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4551 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.yaml
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.894105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    15455 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_git_utils.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6386 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_utils.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    13073 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/bazel_source.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     4025 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/cpan.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     8759 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/deb.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1685 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3672 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_repo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)    35633 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_tag.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5113 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/go_module.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     9055 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/ostree.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2662 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/patch_queue.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     5888 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/pypi.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     2672 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/quilt.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     6947 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/zip.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.894105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      375 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/__init__.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.895105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      106 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/__init__.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     3831 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/gitrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)     1883 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ostreerepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      743 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/tarrepo.py
+-rw-rw-rw-   0 testuser  (1000) testuser  (1000)      946 2024-04-18 16:23:37.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ziprepo.py
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.896105 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3301 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     3476 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)        1 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     1806 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       40 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/requires.txt
+-rw-r--r--   0 testuser  (1000) testuser  (1000)       25 2024-04-18 16:23:50.000000 bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/top_level.txt
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/lib/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/lib/python3.11/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.881105 bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/
+drwxr-xr-x   0 testuser  (1000) testuser  (1000)        0 2024-04-18 16:23:50.896105 bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/markdown_it/
+-rw-r--r--   0 testuser  (1000) testuser  (1000)     2446 2024-04-18 16:23:47.000000 bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/markdown_it/port.yaml
```

### Comparing `bst_plugins_experimental-1.99.0/LICENSE` & `bst_plugins_experimental-1.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/PKG-INFO` & `bst_plugins_experimental-1.99.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.99.0
+Version: 1.99.1
 Summary: A collection of experimental BuildStream plugins.
 License: LGPL-2.1-or-later
 Project-URL: documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Project-URL: repository, https://gitlab.com/BuildStream/bst-plugins-experimental
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `bst_plugins_experimental-1.99.0/README.rst` & `bst_plugins_experimental-1.99.1/README.rst`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/project.conf` & `bst_plugins_experimental-1.99.1/project.conf`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/pyproject.toml` & `bst_plugins_experimental-1.99.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazel_build.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazel_build.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/bazelize.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/bazelize.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/check_forbidden.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/check_forbidden.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_integration.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_integration.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/collect_manifest.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/collect_manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,19 +82,20 @@
        "type": "patch",
        "path": "path/to/patches"
     }
 
 Version will be calculated from commit for git and from basename of URL for
 archive.
 
-The default version regular expression is ``\\d+\\.\\d+(?:\\.\\d+)?`` (2 or 3
-numerical components separated by dots). It is possible to
-change the version regular expression with field ``version-match``.
+The default version regular expression is
+``(\\d+)(?:\\.|_|-)(\\d+)(?:\\.|_|-)?(\\d+)?`` (1, 2 or 3 numerical components
+separated by dots, underscores or dashes). It is possible to change the version
+regular expression with the field ``version-match``.
 
-The version regular exression must follow Python regular expression
+The version regular expression must follow Python regular expression
 syntax.  A version regular expression with no group will match exactly
 the version. A version regular expression with groups will match
 components of the version with each groups. The components will then
 be concatenated using ``.`` (dot) as a separator.
 
 ``version-match`` in the ``cpe`` public data will never be exported in
 the ``x-cpe`` field of the manifest.
@@ -115,15 +116,15 @@
 import posixpath
 
 from buildstream import Element, Node, ElementError
 
 
 class CollectManifestElement(Element):
     BST_MIN_VERSION = "2.0"
-    BST_ARTIFACT_VERSION = 1
+    BST_ARTIFACT_VERSION = 2
 
     def configure(self, node):
         if "path" in node:
             self.path = self.node_subst_vars(node.get_scalar("path"))
         else:
             self.path = None
 
@@ -139,39 +140,33 @@
 
     def stage(self, sandbox):
         pass
 
     def extract_cpe(self, dep):
         cpe = dep.get_public_data("cpe")
 
-        sources = list(dep.sources())
-
         if cpe is None:
             cpe = {}
         else:
             cpe = cpe.strip_node_info()
 
         if "product" not in cpe:
             cpe["product"] = os.path.basename(os.path.splitext(dep.name)[0])
 
         version_match = cpe.pop("version-match", None)
 
-        if "version" not in cpe:
+        sources = list(dep.sources())
+
+        if "version" not in cpe and sources:
             matcher = VersionMatcher(version_match)
             version = matcher.get_version(sources)
-            self.info(
-                "{} version {}".format(
-                    dep.name,
-                    version,
-                )
-            )
 
             if version is None:
                 if version_match is None:
-                    self.status("Missing version to {}.".format(dep.name))
+                    self.warn("Missing version to {}.".format(dep.name))
                 else:
                     fmt = '{}: {}: version match string "{}" did not match anything.'
                     msg = fmt.format(self.name, dep, version_match)
                     raise ElementError(msg)
 
             if version:
                 cpe["version"] = version
@@ -248,30 +243,31 @@
         manifest_node = Node.from_dict(dict(manifest))
         self.set_public_data("cpe-manifest", manifest_node)
         return os.path.sep
 
 
 class VersionMatcher:
 
-    DEFAULT_VERSION_RE = re.compile(r"\d+\.\d+(?:\.\d+)?")
+    DEFAULT_VERSION_RE = re.compile(r"(\d+)(?:\.|_|-)(\d+)(?:\.|_|-)?(\d+)?")
 
     def __init__(self, match):
         if match is None:
             self.__match = self.DEFAULT_VERSION_RE
         else:
             self.__match = re.compile(match)
 
     def _parse_version(self, text):
         m = self.__match.search(text)
         if not m:
             return None
         if self.__match.groups == 0:
             return m.group(0)
         else:
-            return ".".join(m.groups())
+            groups = [x for x in m.groups() if x is not None]
+            return ".".join(groups)
 
     def get_version(self, sources):
         """
         This method attempts to extract the source version
         from a dependency. This data can generally be found
         in the url for tar balls, or the ref for git repos.
```

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_build.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_build.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/dpkg_deploy.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/dpkg_deploy.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_bootimg.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/fastboot_ext4.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/fastboot_ext4.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_image.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_image.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/flatpak_repo.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/flatpak_repo.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/makemaker.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/makemaker.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/modulebuild.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/modulebuild.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/oci.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/oci.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/pyproject.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/pyproject.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/qmake.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/qmake.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/snap_image.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/snap_image.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/tar_element.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/tar_element.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/elements/x86image.yaml` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/elements/x86image.yaml`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_git_utils.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_git_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,17 +410,17 @@
             for ref in matching_refs
             if not any(regex.match(ref) for regex in exclude_regexs)
         ]
 
     return matching_refs
 
 
-def resolve_ref(source, url, tracking, ref_format, exclude):
-    mirror_dir = resolve_mirror_dir(source, url)
-    url = source.translate_url(url)
+def resolve_ref(source, original_url, tracking, ref_format, exclude):
+    mirror_dir = resolve_mirror_dir(source, original_url)
+    url = source.translate_url(original_url)
     source.status(f"Tracking {tracking} from {url}")
 
     client, path = get_authenticated_transport_and_path(url)
 
     try:
         refs = client.get_refs(path)
     except (GitProtocolError, HTTPUnauthorized) as exc:
@@ -453,15 +453,15 @@
         return resolved
 
     if "tags" in ref:
         tag = ref.split("/", 2)[-1]
         return f"{tag}-0-g{resolved}"
 
     # Need to fetch to generate the ref in git-describe format
-    fetcher = GitMirror(source, url, resolved)
+    fetcher = GitMirror(source, original_url, resolved)
     fetcher.fetch()
 
     with Repo(mirror_dir) as repo:
         return git_describe(repo, resolved, refs)
 
 
 def get_authenticated_transport_and_path(url):
```

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/_utils.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/_utils.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/bazel_source.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/bazel_source.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/cpan.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/cpan.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/deb.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/deb.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_module.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_module.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_repo.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_repo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/git_tag.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/git_tag.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/go_module.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/go_module.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/ostree.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/ostree.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/patch_queue.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/patch_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                         directory,
                         "apply",
                         patch,
                     ],
                     fail="Failed to apply patches from {}".format(self.path),
                 )
 
-    def extract_manifest(self):
+    def export_manifest(self):
         return {
             "type": "patch",
             "path": self.path,
         }
 
 
 def setup():
```

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/pypi.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/pypi.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/quilt.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/quilt.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/sources/zip.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/sources/zip.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/gitrepo.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/gitrepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ostreerepo.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ostreerepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/tarrepo.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/tarrepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental/testutils/repo/ziprepo.py` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental/testutils/repo/ziprepo.py`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/PKG-INFO` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bst-plugins-experimental
-Version: 1.99.0
+Version: 1.99.1
 Summary: A collection of experimental BuildStream plugins.
 License: LGPL-2.1-or-later
 Project-URL: documentation, https://buildstream.gitlab.io/bst-plugins-experimental/
 Project-URL: repository, https://gitlab.com/BuildStream/bst-plugins-experimental
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/SOURCES.txt` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/src/bst_plugins_experimental.egg-info/entry_points.txt` & `bst_plugins_experimental-1.99.1/src/bst_plugins_experimental.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bst_plugins_experimental-1.99.0/venv/lib/python3.11/site-packages/markdown_it/port.yaml` & `bst_plugins_experimental-1.99.1/venv/lib/python3.11/site-packages/markdown_it/port.yaml`

 * *Files identical despite different names*

