# Comparing `tmp/Termical-0.2.tar.gz` & `tmp/Termical-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Termical-0.2.tar", last modified: Tue Apr 16 21:03:57 2024, max compression
+gzip compressed data, was "Termical-0.3.tar", last modified: Thu Apr 18 14:29:43 2024, max compression
```

## Comparing `Termical-0.2.tar` & `Termical-0.3.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-16 21:03:57.549563 Termical-0.2/
--rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-16 21:03:57.549563 Termical-0.2/PKG-INFO
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-16 21:03:57.549563 Termical-0.2/Termical.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      167 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       71 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-16 21:03:57.000000 Termical-0.2/Termical.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-04-16 21:03:57.549563 Termical-0.2/setup.cfg
--rw-rw-r--   0 marek     (1000) marek     (1000)      386 2024-04-16 21:03:53.000000 Termical-0.2/setup.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-18 14:29:43.402401 Termical-0.3/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-18 14:29:43.402401 Termical-0.3/PKG-INFO
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-18 14:29:43.402401 Termical-0.3/Termical.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      210 2024-04-18 14:29:43.000000 Termical-0.3/Termical.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      282 2024-04-18 14:29:43.000000 Termical-0.3/Termical.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-04-18 14:29:43.000000 Termical-0.3/Termical.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       72 2024-04-18 14:29:43.000000 Termical-0.3/Termical.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       13 2024-04-18 14:29:43.000000 Termical-0.3/Termical.egg-info/top_level.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-04-18 14:29:43.402401 Termical-0.3/setup.cfg
+-rw-rw-r--   0 marek     (1000) marek     (1000)      390 2024-04-18 14:28:33.000000 Termical-0.3/setup.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-04-18 14:29:43.402401 Termical-0.3/termical_lib/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      305 2024-04-15 18:03:31.000000 Termical-0.3/termical_lib/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1173 2024-04-15 18:03:31.000000 Termical-0.3/termical_lib/authentication.py
+-rwxrwxr-x   0 marek     (1000) marek     (1000)     1409 2024-04-16 21:00:20.000000 Termical-0.3/termical_lib/termical.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     6111 2024-04-15 18:03:31.000000 Termical-0.3/termical_lib/termicalFunctions.py
```

