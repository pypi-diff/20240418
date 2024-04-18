# Comparing `tmp/ziptimezone-0.1.0.tar.gz` & `tmp/ziptimezone-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-0.1.0.tar", max compression
+gzip compressed data, was "ziptimezone-0.1.1.tar", max compression
```

## Comparing `ziptimezone-0.1.0.tar` & `ziptimezone-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.1.0/LICENSE
--rw-r--r--   0        0        0      467 2024-04-18 18:53:54.259716 ziptimezone-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.1.0/ziptimezone/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-18 17:39:45.000000 ziptimezone-0.1.0/ziptimezone/core.py
--rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.1.0/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.1.0/ziptimezone/mappings.py
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 ziptimezone-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        1 2024-04-18 17:39:45.000000 ziptimezone-0.1.1/LICENSE
+-rw-r--r--   0        0        0      298 2024-04-18 20:05:12.524095 ziptimezone-0.1.1/README.md
+-rw-r--r--   0        0        0      488 2024-04-18 20:05:26.620003 ziptimezone-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      969 2024-04-18 17:39:45.000000 ziptimezone-0.1.1/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-18 17:39:45.000000 ziptimezone-0.1.1/ziptimezone/core.py
+-rw-r--r--   0        0        0     1050 2024-04-18 19:09:15.017940 ziptimezone-0.1.1/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1825 2024-04-18 17:39:45.000000 ziptimezone-0.1.1/ziptimezone/mappings.py
+-rw-r--r--   0        0        0      973 1970-01-01 00:00:00.000000 ziptimezone-0.1.1/PKG-INFO
```

### Comparing `ziptimezone-0.1.0/ziptimezone/__init__.py` & `ziptimezone-0.1.1/ziptimezone/__init__.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.0/ziptimezone/core.py` & `ziptimezone-0.1.1/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.0/ziptimezone/geocode.py` & `ziptimezone-0.1.1/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-0.1.0/ziptimezone/mappings.py` & `ziptimezone-0.1.1/ziptimezone/mappings.py`

 * *Files identical despite different names*

