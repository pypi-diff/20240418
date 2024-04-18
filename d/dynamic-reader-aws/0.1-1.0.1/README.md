# Comparing `tmp/dynamic_reader_aws-0.1.tar.gz` & `tmp/dynamic_reader_aws-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic_reader_aws-0.1.tar", last modified: Thu Apr 18 17:31:09 2024, max compression
+gzip compressed data, was "dynamic_reader_aws-1.0.1.tar", last modified: Wed Apr 17 13:53:46 2024, max compression
```

## Comparing `dynamic_reader_aws-0.1.tar` & `dynamic_reader_aws-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxr-xr-x   0 hunaidv    (501) staff       (20)        0 2024-04-18 17:31:09.677155 dynamic_reader_aws-0.1/
--rw-r--r--   0 hunaidv    (501) staff       (20)     1821 2024-04-18 17:31:09.676919 dynamic_reader_aws-0.1/PKG-INFO
--rw-r--r--   0 hunaidv    (501) staff       (20)     1565 2024-04-18 17:29:22.000000 dynamic_reader_aws-0.1/README.md
-drwxr-xr-x   0 hunaidv    (501) staff       (20)        0 2024-04-18 17:31:09.675683 dynamic_reader_aws-0.1/dynamic_reader_aws/
--rw-r--r--   0 hunaidv    (501) staff       (20)       41 2024-04-18 17:20:58.000000 dynamic_reader_aws-0.1/dynamic_reader_aws/__init__.py
--rw-r--r--   0 hunaidv    (501) staff       (20)     1746 2024-04-18 17:19:57.000000 dynamic_reader_aws-0.1/dynamic_reader_aws/main.py
-drwxr-xr-x   0 hunaidv    (501) staff       (20)        0 2024-04-18 17:31:09.676672 dynamic_reader_aws-0.1/dynamic_reader_aws.egg-info/
--rw-r--r--   0 hunaidv    (501) staff       (20)     1821 2024-04-18 17:31:09.000000 dynamic_reader_aws-0.1/dynamic_reader_aws.egg-info/PKG-INFO
--rw-r--r--   0 hunaidv    (501) staff       (20)      285 2024-04-18 17:31:09.000000 dynamic_reader_aws-0.1/dynamic_reader_aws.egg-info/SOURCES.txt
--rw-r--r--   0 hunaidv    (501) staff       (20)        1 2024-04-18 17:31:09.000000 dynamic_reader_aws-0.1/dynamic_reader_aws.egg-info/dependency_links.txt
--rw-r--r--   0 hunaidv    (501) staff       (20)       14 2024-04-18 17:31:09.000000 dynamic_reader_aws-0.1/dynamic_reader_aws.egg-info/requires.txt
--rw-r--r--   0 hunaidv    (501) staff       (20)       19 2024-04-18 17:31:09.000000 dynamic_reader_aws-0.1/dynamic_reader_aws.egg-info/top_level.txt
--rw-r--r--   0 hunaidv    (501) staff       (20)       38 2024-04-18 17:31:09.677204 dynamic_reader_aws-0.1/setup.cfg
--rw-r--r--   0 hunaidv    (501) staff       (20)      434 2024-04-18 17:30:59.000000 dynamic_reader_aws-0.1/setup.py
+drwxr-xr-x   0 hunaidv    (501) staff       (20)        0 2024-04-17 13:53:46.589806 dynamic_reader_aws-1.0.1/
+-rw-r--r--   0 hunaidv    (501) staff       (20)      795 2024-04-17 13:53:46.589582 dynamic_reader_aws-1.0.1/PKG-INFO
+-rw-r--r--   0 hunaidv    (501) staff       (20)       18 2024-04-17 13:37:59.000000 dynamic_reader_aws-1.0.1/README.md
+drwxr-xr-x   0 hunaidv    (501) staff       (20)        0 2024-04-17 13:53:46.589282 dynamic_reader_aws-1.0.1/dynamic_reader_aws.egg-info/
+-rw-r--r--   0 hunaidv    (501) staff       (20)      795 2024-04-17 13:53:46.000000 dynamic_reader_aws-1.0.1/dynamic_reader_aws.egg-info/PKG-INFO
+-rw-r--r--   0 hunaidv    (501) staff       (20)      227 2024-04-17 13:53:46.000000 dynamic_reader_aws-1.0.1/dynamic_reader_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 hunaidv    (501) staff       (20)        1 2024-04-17 13:53:46.000000 dynamic_reader_aws-1.0.1/dynamic_reader_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 hunaidv    (501) staff       (20)        6 2024-04-17 13:53:46.000000 dynamic_reader_aws-1.0.1/dynamic_reader_aws.egg-info/requires.txt
+-rw-r--r--   0 hunaidv    (501) staff       (20)        1 2024-04-17 13:53:46.000000 dynamic_reader_aws-1.0.1/dynamic_reader_aws.egg-info/top_level.txt
+-rw-r--r--   0 hunaidv    (501) staff       (20)       38 2024-04-17 13:53:46.589853 dynamic_reader_aws-1.0.1/setup.cfg
+-rw-r--r--   0 hunaidv    (501) staff       (20)     1018 2024-04-17 13:48:27.000000 dynamic_reader_aws-1.0.1/setup.py
```

