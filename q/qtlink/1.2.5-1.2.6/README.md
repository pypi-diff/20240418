# Comparing `tmp/qtlink-1.2.5.tar.gz` & `tmp/qtlink-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.2.5.tar", last modified: Wed Apr 17 13:33:14 2024, max compression
+gzip compressed data, was "qtlink-1.2.6.tar", last modified: Thu Apr 18 14:04:35 2024, max compression
```

## Comparing `qtlink-1.2.5.tar` & `qtlink-1.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.919538 qtlink-1.2.5/
--rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      466 2024-04-17 13:33:14.917072 qtlink-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.858930 qtlink-1.2.5/qtlink/
--rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.5/qtlink/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.894569 qtlink-1.2.5/qtlink/dialog/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.5/qtlink/dialog/__init__.py
--rw-rw-rw-   0        0        0     1996 2024-04-17 13:33:05.000000 qtlink-1.2.5/qtlink/dialog/dialog_choice.py
--rw-rw-rw-   0        0        0     1719 2024-04-17 13:30:53.000000 qtlink-1.2.5/qtlink/dialog/dialog_info.py
--rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.5/qtlink/dialog/dialog_table_check.py
--rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.5/qtlink/dialog/dialog_table_display.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.897085 qtlink-1.2.5/qtlink/mpl_canvas/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.5/qtlink/mpl_canvas/__init__.py
--rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.5/qtlink/mpl_canvas/mpl_canvas.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.913294 qtlink-1.2.5/qtlink/table/
--rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.5/qtlink/table/__init__.py
--rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.5/qtlink/table/table_controller.py
--rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.5/qtlink/table/table_controller_multiple_check.py
--rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.5/qtlink/table/table_controller_single_check.py
--rw-rw-rw-   0        0        0     4812 2024-04-14 15:23:54.000000 qtlink-1.2.5/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.915727 qtlink-1.2.5/qtlink/widgets/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.5/qtlink/widgets/__init__.py
--rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.5/qtlink/widgets/drop_widget.py
--rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.5/qtlink/widgets/list_widget.py
-drwxrwxrwx   0        0        0        0 2024-04-17 13:33:14.917072 qtlink-1.2.5/qtlink.egg-info/
--rw-rw-rw-   0        0        0      466 2024-04-17 13:33:14.000000 qtlink-1.2.5/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      670 2024-04-17 13:33:14.000000 qtlink-1.2.5/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 13:33:14.000000 qtlink-1.2.5/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-17 13:33:14.000000 qtlink-1.2.5/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-17 13:33:14.000000 qtlink-1.2.5/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 13:33:14.919538 qtlink-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      637 2024-04-17 13:33:05.000000 qtlink-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.513302 qtlink-1.2.6/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      466 2024-04-18 14:04:35.512575 qtlink-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-04-15 02:16:32.000000 qtlink-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.424073 qtlink-1.2.6/qtlink/
+-rw-rw-rw-   0        0        0      117 2024-04-10 12:00:18.000000 qtlink-1.2.6/qtlink/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.466017 qtlink-1.2.6/qtlink/dialog/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:50:18.000000 qtlink-1.2.6/qtlink/dialog/__init__.py
+-rw-rw-rw-   0        0        0     1996 2024-04-17 13:33:05.000000 qtlink-1.2.6/qtlink/dialog/dialog_choice.py
+-rw-rw-rw-   0        0        0     1719 2024-04-17 13:30:53.000000 qtlink-1.2.6/qtlink/dialog/dialog_info.py
+-rw-rw-rw-   0        0        0     2060 2024-04-17 13:09:04.000000 qtlink-1.2.6/qtlink/dialog/dialog_table_check.py
+-rw-rw-rw-   0        0        0     2096 2024-04-17 13:09:04.000000 qtlink-1.2.6/qtlink/dialog/dialog_table_display.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.466017 qtlink-1.2.6/qtlink/mpl_canvas/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.6/qtlink/mpl_canvas/__init__.py
+-rw-rw-rw-   0        0        0     2601 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/mpl_canvas/mpl_canvas.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.486765 qtlink-1.2.6/qtlink/table/
+-rw-rw-rw-   0        0        0       25 2024-03-17 08:35:49.000000 qtlink-1.2.6/qtlink/table/__init__.py
+-rw-rw-rw-   0        0        0     7729 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/table/table_controller.py
+-rw-rw-rw-   0        0        0     6847 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/table/table_controller_multiple_check.py
+-rw-rw-rw-   0        0        0     2822 2024-04-14 15:07:00.000000 qtlink-1.2.6/qtlink/table/table_controller_single_check.py
+-rw-rw-rw-   0        0        0     5182 2024-04-18 14:03:24.000000 qtlink-1.2.6/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.500551 qtlink-1.2.6/qtlink/widgets/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:49:33.000000 qtlink-1.2.6/qtlink/widgets/__init__.py
+-rw-rw-rw-   0        0        0     2094 2024-04-17 09:07:46.000000 qtlink-1.2.6/qtlink/widgets/drop_widget.py
+-rw-rw-rw-   0        0        0     2073 2024-04-14 14:01:58.000000 qtlink-1.2.6/qtlink/widgets/list_widget.py
+drwxrwxrwx   0        0        0        0 2024-04-18 14:04:35.511439 qtlink-1.2.6/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      466 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-18 14:04:35.000000 qtlink-1.2.6/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 14:04:35.513302 qtlink-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      637 2024-04-18 14:04:15.000000 qtlink-1.2.6/setup.py
```

### Comparing `qtlink-1.2.5/LICENSE` & `qtlink-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/dialog/dialog_choice.py` & `qtlink-1.2.6/qtlink/dialog/dialog_choice.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/dialog/dialog_info.py` & `qtlink-1.2.6/qtlink/dialog/dialog_info.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/dialog/dialog_table_check.py` & `qtlink-1.2.6/qtlink/dialog/dialog_table_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/dialog/dialog_table_display.py` & `qtlink-1.2.6/qtlink/dialog/dialog_table_display.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/mpl_canvas/mpl_canvas.py` & `qtlink-1.2.6/qtlink/mpl_canvas/mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/table/table_controller.py` & `qtlink-1.2.6/qtlink/table/table_controller.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/table/table_controller_multiple_check.py` & `qtlink-1.2.6/qtlink/table/table_controller_multiple_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/table/table_controller_single_check.py` & `qtlink-1.2.6/qtlink/table/table_controller_single_check.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/util.py` & `qtlink-1.2.6/qtlink/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,16 @@
             self.when_success(data)
         elif flag == Progress.flag_failed:
             self.when_failed(data)
         elif flag == Progress.flag_end:
             self.when_end(data)
         elif flag == Progress.flag_info:
             self.when_info(data)
+        elif flag == Progress.flag_error:
+            self.when_error(data)
         elif flag == Progress.flag_other1:
             self.when_other1(data)
         elif flag == Progress.flag_other2:
             self.when_other2(data)
         elif flag == Progress.flag_other3:
             self.when_other3(data)
         else:
@@ -79,14 +81,20 @@
 
     def when_info(self, data: list = None):
         """事件信息
         :param data: 当需要传输数据时，使用此参数
         """
         pass
 
+    def when_error(self, data: list = None):
+        """事件错误
+        :param data: 当需要传输数据时，使用此参数
+        """
+        pass
+
     def when_other1(self, data: list = None):
         """预留的任意状态
         :param data: 当需要传输数据时，使用此参数
         """
         pass
 
     def when_other2(self, data: list = None):
@@ -112,18 +120,19 @@
     """
     flag_start = 0
     flag_doing = 1
     flag_end = 2
     flag_success = 3
     flag_failed = 4
     flag_info = 5
+    flag_error = 6
     # 预留的其他状态量
-    flag_other1 = 6
-    flag_other2 = 7
-    flag_other3 = 8
+    flag_other1 = 7
+    flag_other2 = 8
+    flag_other3 = 9
 
     @staticmethod
     def start(data: list = None) -> tuple:
         return Progress.flag_start, data
 
     @staticmethod
     def doing(data: list = None) -> tuple:
@@ -142,14 +151,18 @@
         return Progress.flag_failed, data
 
     @staticmethod
     def info(data: list = None) -> tuple:
         return Progress.flag_info, data
 
     @staticmethod
+    def error(data: list = None) -> tuple:
+        return Progress.flag_error, data
+
+    @staticmethod
     def other1(data: list = None) -> tuple:
         return Progress.flag_other1, data
 
     @staticmethod
     def other2(data: list = None) -> tuple:
         return Progress.flag_other2, data
```

### Comparing `qtlink-1.2.5/qtlink/widgets/drop_widget.py` & `qtlink-1.2.6/qtlink/widgets/drop_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink/widgets/list_widget.py` & `qtlink-1.2.6/qtlink/widgets/list_widget.py`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/qtlink.egg-info/SOURCES.txt` & `qtlink-1.2.6/qtlink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtlink-1.2.5/setup.py` & `qtlink-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.2.5",
+    version="1.2.6",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6'],
```

