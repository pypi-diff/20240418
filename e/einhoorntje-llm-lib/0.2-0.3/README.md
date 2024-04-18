# Comparing `tmp/einhoorntje_llm_lib-0.2.tar.gz` & `tmp/einhoorntje_llm_lib-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "einhoorntje_llm_lib-0.2.tar", last modified: Thu Apr 18 10:07:01 2024, max compression
+gzip compressed data, was "einhoorntje_llm_lib-0.3.tar", last modified: Thu Apr 18 10:24:54 2024, max compression
```

## Comparing `einhoorntje_llm_lib-0.2.tar` & `einhoorntje_llm_lib-0.3.tar`

### file list

```diff
@@ -1,10 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 10:07:01.850770 einhoorntje_llm_lib-0.2/
--rw-rw-rw-   0        0        0      196 2024-04-18 10:07:01.849774 einhoorntje_llm_lib-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 10:07:01.848776 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/
--rw-rw-rw-   0        0        0      196 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-04-18 10:07:01.000000 einhoorntje_llm_lib-0.2/einhoorntje_llm_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 10:07:01.850770 einhoorntje_llm_lib-0.2/setup.cfg
--rw-rw-rw-   0        0        0      300 2024-04-18 10:06:48.000000 einhoorntje_llm_lib-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:24:54.747595 einhoorntje_llm_lib-0.3/
+-rw-rw-rw-   0        0        0      196 2024-04-18 10:24:54.746599 einhoorntje_llm_lib-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 10:24:54.727677 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-18 09:27:19.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib/__init__.py
+-rw-rw-rw-   0        0        0     1414 2024-04-18 10:05:28.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib/llm.py
+-rw-rw-rw-   0        0        0     1988 2024-04-18 09:36:38.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib/llm_cache.py
+drwxrwxrwx   0        0        0        0 2024-04-18 10:24:54.745637 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib.egg-info/
+-rw-rw-rw-   0        0        0      196 2024-04-18 10:24:54.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-04-18 10:24:54.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 10:24:54.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 10:24:54.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-18 10:24:54.000000 einhoorntje_llm_lib-0.3/einhoorntje_llm_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 10:24:54.747595 einhoorntje_llm_lib-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      305 2024-04-18 10:14:56.000000 einhoorntje_llm_lib-0.3/setup.py
```

