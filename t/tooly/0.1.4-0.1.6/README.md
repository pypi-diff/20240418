# Comparing `tmp/tooly-0.1.4.tar.gz` & `tmp/tooly-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooly-0.1.4.tar", max compression
+gzip compressed data, was "tooly-0.1.6.tar", max compression
```

## Comparing `tooly-0.1.4.tar` & `tooly-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      310 2022-03-26 11:38:59.855207 tooly-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       15 2022-03-26 05:42:31.369159 tooly-0.1.4/tooly/.gitignore
--rw-r--r--   0        0        0       61 2022-03-26 11:38:59.849195 tooly-0.1.4/tooly/__init__.py
--rw-r--r--   0        0        0    10947 2022-03-25 15:21:55.099913 tooly-0.1.4/tooly/args.py
--rw-r--r--   0        0        0     2010 2022-03-26 11:37:32.280602 tooly-0.1.4/tooly/logs.py
--rw-r--r--   0        0        0     3220 2022-03-26 09:28:37.847122 tooly-0.1.4/tooly/sh.py
--rw-r--r--   0        0        0     4694 2022-03-25 15:38:48.081499 tooly-0.1.4/tooly/sqliteDb.py
--rw-r--r--   0        0        0       65 2022-03-26 03:57:31.108365 tooly-0.1.4/tooly/types.py
--rw-r--r--   0        0        0      488 2022-03-26 11:39:43.848999 tooly-0.1.4/setup.py
--rw-r--r--   0        0        0      339 2022-03-26 11:39:43.850000 tooly-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      310 2024-04-18 01:20:30.982818 tooly-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       15 2024-04-18 00:19:44.325003 tooly-0.1.6/tooly/.gitignore
+-rw-r--r--   0        0        0       61 2024-04-18 01:20:30.988784 tooly-0.1.6/tooly/__init__.py
+-rw-r--r--   0        0        0    10973 2024-04-18 01:13:57.359124 tooly-0.1.6/tooly/args.py
+-rw-r--r--   0        0        0      235 2024-04-18 00:19:44.326000 tooly-0.1.6/tooly/files.py
+-rw-r--r--   0        0        0     2010 2024-04-18 00:19:44.326000 tooly-0.1.6/tooly/logs.py
+-rw-r--r--   0        0        0     9674 2024-04-18 01:14:20.807339 tooly-0.1.6/tooly/sh.py
+-rw-r--r--   0        0        0     4720 2024-04-18 01:13:57.363098 tooly-0.1.6/tooly/sqliteDb.py
+-rw-r--r--   0        0        0     1534 2024-04-18 00:19:44.327403 tooly-0.1.6/tooly/thread.py
+-rw-r--r--   0        0        0      404 2024-04-18 01:19:16.837710 tooly-0.1.6/tooly/types.py
+-rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 tooly-0.1.6/PKG-INFO
```

### Comparing `tooly-0.1.4/tooly/args.py` & `tooly-0.1.6/tooly/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import json
 import os
 import tkinter
 import tkinter.font
 import tkinter.ttk
 import tkinter.messagebox
 import tkinter.filedialog
-from typing import List, Any, Literal, Union
+from typing import List, Any, Union
+
+from tooly.types import Literal
 
 """
 此文件能实现通过简单的函数调用，实现基本的参数设置。
 参数的类型支持：SingleChoiceParam（单选）、MultiChoiceParam（多选）、FileParam（文件）、TextParam（文本类型）以及ask_option(弹窗）
 具体使用方法见代码中__main__
 """
```

### Comparing `tooly-0.1.4/tooly/logs.py` & `tooly-0.1.6/tooly/logs.py`

 * *Files identical despite different names*

### Comparing `tooly-0.1.4/tooly/sqliteDb.py` & `tooly-0.1.6/tooly/sqliteDb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # python操作sqlite的简单封装，具体使用见__main__代码块
 import os
 import random
 import sqlite3
 import sys
-from typing import Literal, List
+from typing import List
+
+from tooly.types import Literal
 
 
 class Column:
     def __init__(self, colName: str,
                  colType: Literal["text", "integer"],
                  unique=False,
                  length=256,
```

