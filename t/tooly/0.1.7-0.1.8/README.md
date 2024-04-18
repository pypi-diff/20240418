# Comparing `tmp/tooly-0.1.7.tar.gz` & `tmp/tooly-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooly-0.1.7.tar", max compression
+gzip compressed data, was "tooly-0.1.8.tar", max compression
```

## Comparing `tooly-0.1.7.tar` & `tooly-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      310 2024-04-18 02:22:33.365352 tooly-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       15 2024-04-18 00:19:44.325003 tooly-0.1.7/tooly/.gitignore
--rw-r--r--   0        0        0       61 2024-04-18 02:22:33.370352 tooly-0.1.7/tooly/__init__.py
--rw-r--r--   0        0        0    10973 2024-04-18 01:13:57.359124 tooly-0.1.7/tooly/args.py
--rw-r--r--   0        0        0      235 2024-04-18 00:19:44.326000 tooly-0.1.7/tooly/files.py
--rw-r--r--   0        0        0     2010 2024-04-18 00:19:44.326000 tooly-0.1.7/tooly/logs.py
--rw-r--r--   0        0        0    10034 2024-04-18 02:21:41.316686 tooly-0.1.7/tooly/sh.py
--rw-r--r--   0        0        0     4720 2024-04-18 01:13:57.363098 tooly-0.1.7/tooly/sqliteDb.py
--rw-r--r--   0        0        0     1534 2024-04-18 00:19:44.327403 tooly-0.1.7/tooly/thread.py
--rw-r--r--   0        0        0      404 2024-04-18 01:19:16.837710 tooly-0.1.7/tooly/types.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 tooly-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      310 2024-04-18 02:27:47.224501 tooly-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       15 2024-04-18 00:19:44.325003 tooly-0.1.8/tooly/.gitignore
+-rw-r--r--   0        0        0       61 2024-04-18 02:27:47.218500 tooly-0.1.8/tooly/__init__.py
+-rw-r--r--   0        0        0    10973 2024-04-18 01:13:57.359124 tooly-0.1.8/tooly/args.py
+-rw-r--r--   0        0        0      235 2024-04-18 00:19:44.326000 tooly-0.1.8/tooly/files.py
+-rw-r--r--   0        0        0     2010 2024-04-18 00:19:44.326000 tooly-0.1.8/tooly/logs.py
+-rw-r--r--   0        0        0    10052 2024-04-18 02:27:32.633901 tooly-0.1.8/tooly/sh.py
+-rw-r--r--   0        0        0     4720 2024-04-18 01:13:57.363098 tooly-0.1.8/tooly/sqliteDb.py
+-rw-r--r--   0        0        0     1534 2024-04-18 00:19:44.327403 tooly-0.1.8/tooly/thread.py
+-rw-r--r--   0        0        0      404 2024-04-18 01:19:16.837710 tooly-0.1.8/tooly/types.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 tooly-0.1.8/PKG-INFO
```

### Comparing `tooly-0.1.7/tooly/args.py` & `tooly-0.1.8/tooly/args.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.7/tooly/logs.py` & `tooly-0.1.8/tooly/logs.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.7/tooly/sh.py` & `tooly-0.1.8/tooly/sh.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 
 def run(cmd, encoding=defaultShellEncoding, failExit=True, withRetCode=False, log=print, showCmd=True, showOutput=True):
     if not log:
         log = lambda *args: None
     if isinstance(cmd, list):
         if showCmd:
-            log(' \\\n\t'.join(cmd))
+            log("==>> ", ' \\\n\t'.join(cmd))
         cmd = ' '.join(cmd)
     else:
         if showCmd:
-            log(cmd)
+            log("==>> ", cmd)
     p = subprocess.Popen(cmd, shell=True, encoding=encoding, stdout=subprocess.PIPE)
     cmd = " ".join((i.strip("\\") for i in cmd.splitlines()))
     contents = []
     try:
         while p.poll() is None:
             line = p.stdout.readline()
             if showOutput:
```

### Comparing `tooly-0.1.7/tooly/sqliteDb.py` & `tooly-0.1.8/tooly/sqliteDb.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.7/tooly/thread.py` & `tooly-0.1.8/tooly/thread.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.7/PKG-INFO` & `tooly-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooly
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: 方块八
 Author-email: liyuan5202004@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```
