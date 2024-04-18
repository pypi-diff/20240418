# Comparing `tmp/tooly-0.1.6.tar.gz` & `tmp/tooly-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooly-0.1.6.tar", max compression
+gzip compressed data, was "tooly-0.1.7.tar", max compression
```

## Comparing `tooly-0.1.6.tar` & `tooly-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      310 2024-04-18 01:20:30.982818 tooly-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       15 2024-04-18 00:19:44.325003 tooly-0.1.6/tooly/.gitignore
--rw-r--r--   0        0        0       61 2024-04-18 01:20:30.988784 tooly-0.1.6/tooly/__init__.py
--rw-r--r--   0        0        0    10973 2024-04-18 01:13:57.359124 tooly-0.1.6/tooly/args.py
--rw-r--r--   0        0        0      235 2024-04-18 00:19:44.326000 tooly-0.1.6/tooly/files.py
--rw-r--r--   0        0        0     2010 2024-04-18 00:19:44.326000 tooly-0.1.6/tooly/logs.py
--rw-r--r--   0        0        0     9674 2024-04-18 01:14:20.807339 tooly-0.1.6/tooly/sh.py
--rw-r--r--   0        0        0     4720 2024-04-18 01:13:57.363098 tooly-0.1.6/tooly/sqliteDb.py
--rw-r--r--   0        0        0     1534 2024-04-18 00:19:44.327403 tooly-0.1.6/tooly/thread.py
--rw-r--r--   0        0        0      404 2024-04-18 01:19:16.837710 tooly-0.1.6/tooly/types.py
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 tooly-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      310 2024-04-18 02:22:33.365352 tooly-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       15 2024-04-18 00:19:44.325003 tooly-0.1.7/tooly/.gitignore
+-rw-r--r--   0        0        0       61 2024-04-18 02:22:33.370352 tooly-0.1.7/tooly/__init__.py
+-rw-r--r--   0        0        0    10973 2024-04-18 01:13:57.359124 tooly-0.1.7/tooly/args.py
+-rw-r--r--   0        0        0      235 2024-04-18 00:19:44.326000 tooly-0.1.7/tooly/files.py
+-rw-r--r--   0        0        0     2010 2024-04-18 00:19:44.326000 tooly-0.1.7/tooly/logs.py
+-rw-r--r--   0        0        0    10034 2024-04-18 02:21:41.316686 tooly-0.1.7/tooly/sh.py
+-rw-r--r--   0        0        0     4720 2024-04-18 01:13:57.363098 tooly-0.1.7/tooly/sqliteDb.py
+-rw-r--r--   0        0        0     1534 2024-04-18 00:19:44.327403 tooly-0.1.7/tooly/thread.py
+-rw-r--r--   0        0        0      404 2024-04-18 01:19:16.837710 tooly-0.1.7/tooly/types.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 tooly-0.1.7/PKG-INFO
```

### Comparing `tooly-0.1.6/tooly/args.py` & `tooly-0.1.7/tooly/args.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.6/tooly/logs.py` & `tooly-0.1.7/tooly/logs.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.6/tooly/sh.py` & `tooly-0.1.7/tooly/sh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import os
 import subprocess
 import sys
 import zipfile
 from typing import Union, Dict, Callable
 
-
 from tooly.types import Encoding, Literal
 
 defaultShellEncoding: Encoding = 'utf8'
 if sys.platform.find('win'):
     defaultShellEncoding = 'gbk'
 
 isDir = os.path.isdir
@@ -41,20 +40,30 @@
         sys.exit()
     if withRetCode:
         return p.returncode, "".join(contents).strip()
     else:
         return "".join(contents).strip()
 
 
+def runS(cmd, encoding=defaultShellEncoding, failExit=True, withRetCode=False, log=print, showCmd=False,
+         showOutput=False):
+    """
+    以silent的模式运行命令，仅返回结果
+    """
+    return run(cmd, encoding=encoding, failExit=failExit, withRetCode=withRetCode, log=log, showCmd=showCmd,
+               showOutput=showOutput)
+
+
 class CustomHelpFormatter(argparse.HelpFormatter):
     """
     argparse的自定义help信息生成器，能在parser.add_argument函数没有help信息时打印default信息
     使用时，只需要在创建parser时传入即可，示例如下：
     >>> parser = argparse.ArgumentParser(formatter_class=CustomHelpFormatter)
     """
+
     def _format_args(self, action: argparse.Action, default_metavar: str) -> str:
         if action.default != argparse.SUPPRESS and action.default:
             default_val = "{" + f"{default_metavar}:{action.default}" + "}"
             return super()._format_args(action, default_val)
         else:
             return super()._format_args(action, default_metavar)
```

### Comparing `tooly-0.1.6/tooly/sqliteDb.py` & `tooly-0.1.7/tooly/sqliteDb.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.6/tooly/thread.py` & `tooly-0.1.7/tooly/thread.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.6/PKG-INFO` & `tooly-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tooly
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: 方块八
 Author-email: liyuan5202004@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

