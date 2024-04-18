# Comparing `tmp/einhoorntje_llm_lib-0.1.tar.gz` & `tmp/einhoorntje_llm_lib-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einhoorntje_llm_lib-0.1.tar", last modified: Thu Apr 18 09:52:39 2024, max compression
+gzip compressed data, was "einhoorntje_llm_lib-0.2.tar", last modified: Thu Apr 18 10:07:01 2024, max compression
```

## Comparing `einhoorntje_llm_lib-0.1.tar` & `einhoorntje_llm_lib-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 09:52:39.667050 einhoorntje_llm_lib-0.1/
--rw-rw-rw-   0        0        0      196 2024-04-18 09:52:39.666052 einhoorntje_llm_lib-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 09:52:39.666052 einhoorntje_llm_lib-0.1/einhoorntje_llm_lib.egg-info/
--rw-rw-rw-   0        0        0      196 2024-04-18 09:52:39.000000 einhoorntje_llm_lib-0.1/einhoorntje_llm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-04-18 09:52:39.000000 einhoorntje_llm_lib-0.1/einhoorntje_llm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 09:52:39.000000 einhoorntje_llm_lib-0.1/einhoorntje_llm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 09:52:39.000000 einhoorntje_llm_lib-0.1/einhoorntje_llm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 09:52:39.000000 einhoorntje_llm_lib-0.1/einhoorntje_llm_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 09:52:39.667050 einhoorntje_llm_lib-0.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2024-04-18 09:52:28.000000 einhoorntje_llm_lib-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:07:01.850770 einhoorntje_llm_lib-0.2/
+-rw-rw-rw-   0        0        0      196 2024-04-18 10:07:01.849774 einhoorntje_llm_lib-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 10:07:01.848776 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/
+-rw-rw-rw-   0        0        0      196 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 10:07:01.850770 einhoorntje_llm_lib-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      300 2024-04-18 10:06:48.000000 einhoorntje_llm_lib-0.2/setup.py
```

