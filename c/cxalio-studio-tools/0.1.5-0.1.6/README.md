# Comparing `tmp/cxalio_studio_tools-0.1.5.tar.gz` & `tmp/cxalio_studio_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.1.5.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.1.6.tar", max compression
```

## Comparing `cxalio_studio_tools-0.1.5.tar` & `cxalio_studio_tools-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.1.5/LICENSE
--rw-r--r--   0        0        0      939 2024-03-06 11:11:33.875444 cxalio_studio_tools-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      749 2024-02-22 17:29:55.909691 cxalio_studio_tools-0.1.5/README.md
--rw-r--r--   0        0        0      160 2024-01-27 13:17:34.142188 cxalio_studio_tools-0.1.5/src/cx_core/__init__.py
--rw-r--r--   0        0        0      145 2024-01-27 13:17:34.142188 cxalio_studio_tools-0.1.5/src/cx_core/abstract_app.py
--rw-r--r--   0        0        0      838 2024-01-27 12:52:22.610811 cxalio_studio_tools-0.1.5/src/cx_core/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-01-27 17:09:17.423551 cxalio_studio_tools-0.1.5/src/cx_core/app_logger.py
--rw-r--r--   0        0        0     2024 2024-01-27 13:17:34.143187 cxalio_studio_tools-0.1.5/src/cx_core/datapackage.py
--rw-r--r--   0        0        0     1826 2024-01-27 12:52:22.611806 cxalio_studio_tools-0.1.5/src/cx_core/ffmpeg_progress_parser.py
--rw-r--r--   0        0        0     1462 2024-01-27 12:52:22.612805 cxalio_studio_tools-0.1.5/src/cx_core/folder_expander.py
--rw-r--r--   0        0        0     2991 2024-02-05 14:10:41.883203 cxalio_studio_tools-0.1.5/src/cx_core/timecode.py
--rw-r--r--   0        0        0     1640 2024-02-05 14:10:41.883203 cxalio_studio_tools-0.1.5/src/cx_core/timepoint.py
--rw-r--r--   0        0        0      466 2024-03-06 11:11:33.875444 cxalio_studio_tools-0.1.5/src/cx_core/tui_elements.py
--rw-r--r--   0        0        0      956 2024-01-27 13:17:34.143187 cxalio_studio_tools-0.1.5/src/cx_core/utils.py
--rw-r--r--   0        0        0       83 2024-02-05 14:10:41.884204 cxalio_studio_tools-0.1.5/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4611 2024-02-05 14:10:41.884204 cxalio_studio_tools-0.1.5/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     4579 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.5/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      482 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.5/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     3271 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.5/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.1.5/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1377 2024-03-06 11:11:33.876366 cxalio_studio_tools-0.1.5/src/media_killer/env.py
--rw-r--r--   0        0        0     1840 2024-01-27 13:17:34.144189 cxalio_studio_tools-0.1.5/src/media_killer/example_project.toml
--rw-r--r--   0        0        0     3989 2024-01-27 17:09:17.423551 cxalio_studio_tools-0.1.5/src/media_killer/help.md
--rw-r--r--   0        0        0     7178 2024-03-06 11:11:33.877362 cxalio_studio_tools-0.1.5/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     3719 2024-01-27 17:09:17.424592 cxalio_studio_tools-0.1.5/src/media_killer/planner.py
--rw-r--r--   0        0        0     4696 2024-02-05 14:10:41.886706 cxalio_studio_tools-0.1.5/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     2382 2024-01-27 13:17:34.146188 cxalio_studio_tools-0.1.5/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     2791 2024-01-27 13:17:34.146188 cxalio_studio_tools-0.1.5/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     3773 2024-03-06 11:11:33.877362 cxalio_studio_tools-0.1.5/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.5/src/sub_conv/__init__.py
--rw-r--r--   0        0        0      278 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.5/src/sub_conv/env.py
--rw-r--r--   0        0        0       44 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.5/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     2937 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.5/src/sub_conv/help.md
--rw-r--r--   0        0        0     7432 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.5/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.1.6/LICENSE
+-rw-r--r--   0        0        0      939 2024-04-18 14:58:37.198179 cxalio_studio_tools-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      749 2024-02-22 17:29:55.909691 cxalio_studio_tools-0.1.6/README.md
+-rw-r--r--   0        0        0      160 2024-01-27 13:17:34.142188 cxalio_studio_tools-0.1.6/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      145 2024-01-27 13:17:34.142188 cxalio_studio_tools-0.1.6/src/cx_core/abstract_app.py
+-rw-r--r--   0        0        0      838 2024-01-27 12:52:22.610811 cxalio_studio_tools-0.1.6/src/cx_core/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-01-27 17:09:17.423551 cxalio_studio_tools-0.1.6/src/cx_core/app_logger.py
+-rw-r--r--   0        0        0     2024 2024-01-27 13:17:34.143187 cxalio_studio_tools-0.1.6/src/cx_core/datapackage.py
+-rw-r--r--   0        0        0     1826 2024-01-27 12:52:22.611806 cxalio_studio_tools-0.1.6/src/cx_core/ffmpeg_progress_parser.py
+-rw-r--r--   0        0        0     1462 2024-01-27 12:52:22.612805 cxalio_studio_tools-0.1.6/src/cx_core/folder_expander.py
+-rw-r--r--   0        0        0     2991 2024-02-05 14:10:41.883203 cxalio_studio_tools-0.1.6/src/cx_core/timecode.py
+-rw-r--r--   0        0        0     1640 2024-02-05 14:10:41.883203 cxalio_studio_tools-0.1.6/src/cx_core/timepoint.py
+-rw-r--r--   0        0        0      466 2024-03-06 11:11:33.875444 cxalio_studio_tools-0.1.6/src/cx_core/tui_elements.py
+-rw-r--r--   0        0        0      956 2024-01-27 13:17:34.143187 cxalio_studio_tools-0.1.6/src/cx_core/utils.py
+-rw-r--r--   0        0        0       83 2024-02-05 14:10:41.884204 cxalio_studio_tools-0.1.6/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4611 2024-02-05 14:10:41.884204 cxalio_studio_tools-0.1.6/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     4579 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.6/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      482 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.6/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     3271 2024-02-05 14:10:41.885202 cxalio_studio_tools-0.1.6/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.1.6/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1377 2024-03-06 11:11:33.876366 cxalio_studio_tools-0.1.6/src/media_killer/env.py
+-rw-r--r--   0        0        0     1840 2024-01-27 13:17:34.144189 cxalio_studio_tools-0.1.6/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0     3989 2024-01-27 17:09:17.423551 cxalio_studio_tools-0.1.6/src/media_killer/help.md
+-rw-r--r--   0        0        0     7178 2024-03-06 11:11:33.877362 cxalio_studio_tools-0.1.6/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     3719 2024-01-27 17:09:17.424592 cxalio_studio_tools-0.1.6/src/media_killer/planner.py
+-rw-r--r--   0        0        0     4696 2024-02-05 14:10:41.886706 cxalio_studio_tools-0.1.6/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     2382 2024-01-27 13:17:34.146188 cxalio_studio_tools-0.1.6/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     2791 2024-01-27 13:17:34.146188 cxalio_studio_tools-0.1.6/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     3773 2024-03-06 11:11:33.877362 cxalio_studio_tools-0.1.6/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.6/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0      278 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.6/src/sub_conv/env.py
+-rw-r--r--   0        0        0       44 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.6/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     2937 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.6/src/sub_conv/help.md
+-rw-r--r--   0        0        0     7432 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.1.6/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1624 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.1.6/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.1.5/LICENSE` & `cxalio_studio_tools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/pyproject.toml` & `cxalio_studio_tools-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.1.5"
+version = "0.1.6"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
```

### Comparing `cxalio_studio_tools-0.1.5/README.md` & `cxalio_studio_tools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/abstract_env.py` & `cxalio_studio_tools-0.1.6/src/cx_core/abstract_env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/app_logger.py` & `cxalio_studio_tools-0.1.6/src/cx_core/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/datapackage.py` & `cxalio_studio_tools-0.1.6/src/cx_core/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/ffmpeg_progress_parser.py` & `cxalio_studio_tools-0.1.6/src/cx_core/ffmpeg_progress_parser.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/folder_expander.py` & `cxalio_studio_tools-0.1.6/src/cx_core/folder_expander.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/timecode.py` & `cxalio_studio_tools-0.1.6/src/cx_core/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/timepoint.py` & `cxalio_studio_tools-0.1.6/src/cx_core/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_core/utils.py` & `cxalio_studio_tools-0.1.6/src/cx_core/utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.1.6/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.1.6/src/cx_subtitle/saver.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.1.6/src/cx_subtitle/subtitle_formatter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/env.py` & `cxalio_studio_tools-0.1.6/src/media_killer/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.1.6/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/help.md` & `cxalio_studio_tools-0.1.6/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.1.6/src/media_killer/media_killer_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/planner.py` & `cxalio_studio_tools-0.1.6/src/media_killer/planner.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.1.6/src/media_killer/profile_loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.1.6/src/media_killer/script_writer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.1.6/src/media_killer/source_adapter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.1.6/src/media_killer/transcoder.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/sub_conv/help.md` & `cxalio_studio_tools-0.1.6/src/sub_conv/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/src/sub_conv/subconv_app.py` & `cxalio_studio_tools-0.1.6/src/sub_conv/subconv_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.1.5/PKG-INFO` & `cxalio_studio_tools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
```

