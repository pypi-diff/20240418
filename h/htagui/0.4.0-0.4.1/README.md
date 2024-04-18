# Comparing `tmp/htagui-0.4.0.tar.gz` & `tmp/htagui-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.4.0.tar", max compression
+gzip compressed data, was "htagui-0.4.1.tar", max compression
```

## Comparing `htagui-0.4.0.tar` & `htagui-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2024-04-17 15:42:08.855575 htagui-0.4.0/LICENSE
--rw-r--r--   0        0        0     7363 2024-04-17 15:42:08.855575 htagui-0.4.0/README.md
--rw-r--r--   0        0        0      330 2024-04-17 15:42:09.127575 htagui-0.4.0/htagui/__init__.py
--rw-r--r--   0        0        0     1313 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/basics/__init__.py
--rw-r--r--   0        0        0     7815 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/basics/bases.py
--rw-r--r--   0        0        0     1314 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   654506 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/bulma/bases.py
--rw-r--r--   0        0        0     3214 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/common.py
--rw-r--r--   0        0        0     3037 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/flex.py
--rw-r--r--   0        0        0      771 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/form.py
--rw-r--r--   0        0        0     3380 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/ifields.py
--rw-r--r--   0        0        0     1317 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     7402 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/shoelace/bases.py
--rw-r--r--   0        0        0     8884 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/splitters.py
--rw-r--r--   0        0        0     1441 2024-04-17 15:42:08.855575 htagui-0.4.0/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-17 15:42:09.127575 htagui-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 htagui-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-18 07:21:50.369397 htagui-0.4.1/LICENSE
+-rw-r--r--   0        0        0     7363 2024-04-18 07:21:50.369397 htagui-0.4.1/README.md
+-rw-r--r--   0        0        0      330 2024-04-18 07:21:50.617398 htagui-0.4.1/htagui/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-18 07:21:50.369397 htagui-0.4.1/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     7815 2024-04-18 07:21:50.369397 htagui-0.4.1/htagui/basics/bases.py
+-rw-r--r--   0        0        0     1315 2024-04-18 07:21:50.369397 htagui-0.4.1/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   654506 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/bulma/bases.py
+-rw-r--r--   0        0        0     3214 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/common.py
+-rw-r--r--   0        0        0     3037 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/flex.py
+-rw-r--r--   0        0        0      771 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/form.py
+-rw-r--r--   0        0        0     3380 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/ifields.py
+-rw-r--r--   0        0        0     1317 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     7402 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/shoelace/bases.py
+-rw-r--r--   0        0        0     8884 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/splitters.py
+-rw-r--r--   0        0        0     1441 2024-04-18 07:21:50.373397 htagui-0.4.1/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-18 07:21:50.617398 htagui-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 htagui-0.4.1/PKG-INFO
```

### Comparing `htagui-0.4.0/LICENSE` & `htagui-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/README.md` & `htagui-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/basics/__init__.py` & `htagui-0.4.1/htagui/basics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     @property
     def ui(self):
         if self._ui is None:
             self._ui = Dialog(self)
         return self._ui
 
 ALL=[App,Button,Input,Textarea,Select,Menu,Spinner,Form,Tabs,Dialog,HSplit,IText,ITextarea,IRange,IBool,ISelect]
-__all__=["App","Button","Input","Textarea","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",  "IText","ITextarea","IRange","IBool","ISelect"     "hflex","vflex", "ALL"]
+__all__=["App","Button","Input","Textarea","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",  "IText","ITextarea","IRange","IBool","ISelect",     "hflex","vflex", "ALL"]
```

### Comparing `htagui-0.4.0/htagui/basics/bases.py` & `htagui-0.4.1/htagui/basics/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/bulma/__init__.py` & `htagui-0.4.1/htagui/bulma/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     @property
     def ui(self):
         if self._ui is None:
             self._ui = Dialog(self)
         return self._ui
 
 ALL=[App,Button,Input,Textarea,Select,Menu,Spinner,Form,Tabs,Dialog,HSplit,IText,ITextarea,IRange,IBool,ISelect]
-__all__=["App","Button","Input","Textarea","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",  "IText","ITextarea","IRange","IBool","ISelect"     "hflex","vflex", "ALL"]
+__all__=["App","Button","Input","Textarea","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",  "IText","ITextarea","IRange","IBool","ISelect",     "hflex","vflex", "ALL"]
```

### Comparing `htagui-0.4.0/htagui/bulma/bases.py` & `htagui-0.4.1/htagui/bulma/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/common.py` & `htagui-0.4.1/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/dialog.py` & `htagui-0.4.1/htagui/dialog.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/flex.py` & `htagui-0.4.1/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/form.py` & `htagui-0.4.1/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/ifields.py` & `htagui-0.4.1/htagui/ifields.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/shoelace/__init__.py` & `htagui-0.4.1/htagui/shoelace/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     @property
     def ui(self):
         if self._ui is None:
             self._ui = Dialog(self)
         return self._ui
 
 ALL=[App,Button,Input,Textarea,Select,Menu,Spinner,Form,Tabs,Dialog,HSplit,IText,ITextarea,IRange,IBool,ISelect]
-__all__=["App","Button","Input","Textarea","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",  "IText","ITextarea","IRange","IBool","ISelect"     "hflex","vflex", "ALL"]
+__all__=["App","Button","Input","Textarea","Select","Menu","Spinner","Form","Tabs","Dialog","HSplit",  "IText","ITextarea","IRange","IBool","ISelect",    "hflex","vflex", "ALL"]
```

### Comparing `htagui-0.4.0/htagui/shoelace/bases.py` & `htagui-0.4.1/htagui/shoelace/bases.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/splitters.py` & `htagui-0.4.1/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/htagui/tabs.py` & `htagui-0.4.1/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.4.0/pyproject.toml` & `htagui-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.4.0" # auto-updated
+version = "0.4.1" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.4.0/PKG-INFO` & `htagui-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.4.0
+Version: 0.4.1
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
```

