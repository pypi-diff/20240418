# Comparing `tmp/openav-1.0.0a0.tar.gz` & `tmp/openav-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openav-1.0.0a0.tar", last modified: Mon Dec 12 16:30:12 2022, max compression
+gzip compressed data, was "openav-1.0.0a2.tar", last modified: Thu Apr 18 13:37:01 2024, max compression
```

## Comparing `openav-1.0.0a0.tar` & `openav-1.0.0a2.tar`

### file list

```diff
@@ -1,20 +1,76 @@
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2022-12-12 16:30:12.047023 openav-1.0.0a0/
--rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a0/LICENSE
--rw-r--r--   0 dl         (501) staff       (20)      101 2022-12-12 12:29:20.000000 openav-1.0.0a0/MANIFEST.in
--rw-r--r--   0 dl         (501) staff       (20)     4022 2022-12-12 16:30:12.047230 openav-1.0.0a0/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)     1102 2022-12-12 12:32:53.000000 openav-1.0.0a0/README.md
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2022-12-12 16:30:12.042982 openav-1.0.0a0/openav/
--rw-r--r--   0 dl         (501) staff       (20)     1038 2022-12-12 15:20:25.000000 openav-1.0.0a0/openav/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2022-12-12 16:30:12.045812 openav-1.0.0a0/openav/modules/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a0/openav/modules/__init__.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2022-12-12 16:30:12.046313 openav-1.0.0a0/openav/modules/lab/
--rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a0/openav/modules/lab/__init__.py
--rw-r--r--   0 dl         (501) staff       (20)     2063 2022-12-12 15:34:26.000000 openav-1.0.0a0/openav/modules/lab/build.py
-drwxr-xr-x   0 dl         (501) staff       (20)        0 2022-12-12 16:30:12.045501 openav-1.0.0a0/openav.egg-info/
--rw-r--r--   0 dl         (501) staff       (20)     4022 2022-12-12 16:30:11.000000 openav-1.0.0a0/openav.egg-info/PKG-INFO
--rw-r--r--   0 dl         (501) staff       (20)      302 2022-12-12 16:30:11.000000 openav-1.0.0a0/openav.egg-info/SOURCES.txt
--rw-r--r--   0 dl         (501) staff       (20)        1 2022-12-12 16:30:11.000000 openav-1.0.0a0/openav.egg-info/dependency_links.txt
--rw-r--r--   0 dl         (501) staff       (20)       15 2022-12-12 16:30:11.000000 openav-1.0.0a0/openav.egg-info/requires.txt
--rw-r--r--   0 dl         (501) staff       (20)        7 2022-12-12 16:30:11.000000 openav-1.0.0a0/openav.egg-info/top_level.txt
--rw-r--r--   0 dl         (501) staff       (20)       79 2022-12-12 16:30:12.047759 openav-1.0.0a0/setup.cfg
--rw-r--r--   0 dl         (501) staff       (20)     3290 2022-12-12 16:29:50.000000 openav-1.0.0a0/setup.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.236189 openav-1.0.0a2/
+-rw-r--r--   0 dl         (501) staff       (20)     1151 2022-12-12 14:51:15.000000 openav-1.0.0a2/LICENSE
+-rw-r--r--   0 dl         (501) staff       (20)      101 2023-02-26 14:02:17.000000 openav-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-18 13:37:01.236538 openav-1.0.0a2/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1123 2023-02-26 13:59:14.000000 openav-1.0.0a2/README.md
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.135189 openav-1.0.0a2/openav/
+-rw-r--r--   0 dl         (501) staff       (20)     2903 2023-02-26 17:36:46.000000 openav-1.0.0a2/openav/__garbage__.py
+-rw-r--r--   0 dl         (501) staff       (20)     1074 2024-04-18 13:36:25.000000 openav-1.0.0a2/openav/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.155291 openav-1.0.0a2/openav/api/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a2/openav/api/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    23628 2024-04-17 13:01:05.000000 openav-1.0.0a2/openav/api/augmentation.py
+-rw-r--r--   0 dl         (501) staff       (20)    15668 2024-04-17 13:01:21.000000 openav-1.0.0a2/openav/api/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    20825 2024-04-18 12:59:22.000000 openav-1.0.0a2/openav/api/preprocess_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    17452 2023-11-01 09:37:48.000000 openav-1.0.0a2/openav/api/test_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    17453 2023-11-01 09:37:48.000000 openav-1.0.0a2/openav/api/test_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    12587 2023-10-16 09:10:27.000000 openav-1.0.0a2/openav/api/testing.py
+-rw-r--r--   0 dl         (501) staff       (20)    17771 2023-11-01 09:37:48.000000 openav-1.0.0a2/openav/api/train_audio.py
+-rw-r--r--   0 dl         (501) staff       (20)    17761 2023-11-01 09:37:48.000000 openav-1.0.0a2/openav/api/train_video.py
+-rw-r--r--   0 dl         (501) staff       (20)    23149 2024-04-17 21:11:51.000000 openav-1.0.0a2/openav/api/vad.py
+-rw-r--r--   0 dl         (501) staff       (20)     7301 2024-04-17 13:01:45.000000 openav-1.0.0a2/openav/api/vad_gui.py
+-rw-r--r--   0 dl         (501) staff       (20)    22993 2024-04-11 17:21:44.000000 openav-1.0.0a2/openav/api/vosk_sr.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.156420 openav-1.0.0a2/openav/modules/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a2/openav/modules/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.210508 openav-1.0.0a2/openav/modules/core/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a2/openav/modules/core/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    30506 2024-04-18 10:31:06.000000 openav-1.0.0a2/openav/modules/core/core.py
+-rw-r--r--   0 dl         (501) staff       (20)     3353 2023-10-16 08:55:02.000000 openav-1.0.0a2/openav/modules/core/exceptions.py
+-rw-r--r--   0 dl         (501) staff       (20)     9266 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/core/language.py
+-rw-r--r--   0 dl         (501) staff       (20)     9887 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/core/logging.py
+-rw-r--r--   0 dl         (501) staff       (20)     2906 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/core/messages.py
+-rw-r--r--   0 dl         (501) staff       (20)    14490 2023-10-16 08:55:02.000000 openav-1.0.0a2/openav/modules/core/settings.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.214460 openav-1.0.0a2/openav/modules/dataset_recording/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2024-04-11 17:37:56.000000 openav-1.0.0a2/openav/modules/dataset_recording/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     3539 2024-04-11 17:37:56.000000 openav-1.0.0a2/openav/modules/dataset_recording/app.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.222378 openav-1.0.0a2/openav/modules/file_manager/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-06-10 13:20:15.000000 openav-1.0.0a2/openav/modules/file_manager/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)    13911 2023-04-07 08:51:58.000000 openav-1.0.0a2/openav/modules/file_manager/download.py
+-rw-r--r--   0 dl         (501) staff       (20)    15231 2023-04-05 13:58:17.000000 openav-1.0.0a2/openav/modules/file_manager/file_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)     7272 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/file_manager/json_manager.py
+-rw-r--r--   0 dl         (501) staff       (20)    13451 2023-04-07 13:22:08.000000 openav-1.0.0a2/openav/modules/file_manager/unzip.py
+-rw-r--r--   0 dl         (501) staff       (20)     6804 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/file_manager/yaml_manager.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.229245 openav-1.0.0a2/openav/modules/lab/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-11-30 18:50:19.000000 openav-1.0.0a2/openav/modules/lab/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)   120726 2024-04-18 13:11:19.000000 openav-1.0.0a2/openav/modules/lab/audio.py
+-rw-r--r--   0 dl         (501) staff       (20)     4351 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/lab/audiovisual.py
+-rw-r--r--   0 dl         (501) staff       (20)     1726 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/lab/build.py
+-rw-r--r--   0 dl         (501) staff       (20)     4009 2023-11-01 09:37:48.000000 openav-1.0.0a2/openav/modules/lab/video.py
+-rw-r--r--   0 dl         (501) staff       (20)      215 2024-04-11 17:37:56.000000 openav-1.0.0a2/openav/modules/lab/video_converter.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.128032 openav-1.0.0a2/openav/modules/locales/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.127891 openav-1.0.0a2/openav/modules/locales/en/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.231164 openav-1.0.0a2/openav/modules/locales/en/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 14:16:44.000000 openav-1.0.0a2/openav/modules/locales/en/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      558 2022-12-21 13:56:06.000000 openav-1.0.0a2/openav/modules/locales/en/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.128140 openav-1.0.0a2/openav/modules/locales/ru/
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.233190 openav-1.0.0a2/openav/modules/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 dl         (501) staff       (20)     3736 2022-12-21 14:16:59.000000 openav-1.0.0a2/openav/modules/locales/ru/LC_MESSAGES/argparse.mo
+-rw-r--r--   0 dl         (501) staff       (20)      374 2022-12-21 13:56:18.000000 openav-1.0.0a2/openav/modules/locales/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.234230 openav-1.0.0a2/openav/modules/nn/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a2/openav/modules/nn/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.234896 openav-1.0.0a2/openav/modules/trml/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2020-05-28 10:15:52.000000 openav-1.0.0a2/openav/modules/trml/__init__.py
+-rw-r--r--   0 dl         (501) staff       (20)     2450 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/modules/trml/shell.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.235569 openav-1.0.0a2/openav/rsrs/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2022-12-17 13:05:02.000000 openav-1.0.0a2/openav/rsrs/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.235880 openav-1.0.0a2/openav/rsrs/favicon/
+-rw-r--r--   0 dl         (501) staff       (20)        0 2023-03-23 13:47:11.000000 openav-1.0.0a2/openav/rsrs/favicon/__init__.py
+drwxr-xr-x   0 dl         (501) staff       (20)        0 2024-04-18 13:37:01.138369 openav-1.0.0a2/openav.egg-info/
+-rw-r--r--   0 dl         (501) staff       (20)     4144 2024-04-18 13:37:00.000000 openav-1.0.0a2/openav.egg-info/PKG-INFO
+-rw-r--r--   0 dl         (501) staff       (20)     1684 2024-04-18 13:37:01.000000 openav-1.0.0a2/openav.egg-info/SOURCES.txt
+-rw-r--r--   0 dl         (501) staff       (20)        1 2024-04-18 13:37:00.000000 openav-1.0.0a2/openav.egg-info/dependency_links.txt
+-rw-r--r--   0 dl         (501) staff       (20)      151 2024-04-18 13:37:00.000000 openav-1.0.0a2/openav.egg-info/entry_points.txt
+-rw-r--r--   0 dl         (501) staff       (20)      341 2024-04-18 13:37:00.000000 openav-1.0.0a2/openav.egg-info/requires.txt
+-rw-r--r--   0 dl         (501) staff       (20)        7 2024-04-18 13:37:00.000000 openav-1.0.0a2/openav.egg-info/top_level.txt
+-rw-r--r--   0 dl         (501) staff       (20)       57 2023-02-26 13:53:20.000000 openav-1.0.0a2/pyproject.toml
+-rw-r--r--   0 dl         (501) staff       (20)       79 2024-04-18 13:37:01.237238 openav-1.0.0a2/setup.cfg
+-rw-r--r--   0 dl         (501) staff       (20)     4159 2024-04-18 13:35:58.000000 openav-1.0.0a2/setup.py
```

### Comparing `openav-1.0.0a0/LICENSE` & `openav-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `openav-1.0.0a0/PKG-INFO` & `openav-1.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a0
-Summary: openav
+Version: 1.0.0a2
+Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
 Project-URL: Bug Reports, https://github.com/DmitryRyumin/openav/issues
@@ -22,14 +22,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
@@ -58,23 +60,23 @@
 # [OpenAV](https://github.com/DmitryRyumin/openav)
 
 ![PyPI](https://img.shields.io/pypi/v/openav)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openav)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/openav)
 ![GitHub repo size](https://img.shields.io/github/repo-size/dmitryryumin/openav)
 ![PyPI - Status](https://img.shields.io/pypi/status/openav)
-![PyPI - License](https://img.shields.io/pypi/l/openav)
+![PyPI - License](https://img.shields.io/github/license/dmitryryumin/openav)
 ![GitHub top language](https://img.shields.io/github/languages/top/dmitryryumin/openav)
 ![Documentation Status](https://readthedocs.org/projects/openav/badge/?version=latest)
 
 <h4 align="center"><span style="color:#EC256F;">Description</span></h4>
 
 ---
 
->  **[OpenAV](https://github.com/DmitryRyumin/openav)** is an open-source library for recognition of speech commands in the user dictionary using audiovisual data of the speaker.
+> **[OpenAV](https://github.com/DmitryRyumin/openav)** is an open-source library for recognition of speech commands in the user dictionary using audiovisual data of the speaker.
 
 ---
 
 | [Documentation in Russian](https://github.com/DmitryRyumin/openav/blob/main/README_RU.md) |
 |-------------------------------------------------------------------------------------------|
 
 > The library under development
```

### Comparing `openav-1.0.0a0/README.md` & `openav-1.0.0a2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # [OpenAV](https://github.com/DmitryRyumin/openav)
 
 ![PyPI](https://img.shields.io/pypi/v/openav)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openav)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/openav)
 ![GitHub repo size](https://img.shields.io/github/repo-size/dmitryryumin/openav)
 ![PyPI - Status](https://img.shields.io/pypi/status/openav)
-![PyPI - License](https://img.shields.io/pypi/l/openav)
+![PyPI - License](https://img.shields.io/github/license/dmitryryumin/openav)
 ![GitHub top language](https://img.shields.io/github/languages/top/dmitryryumin/openav)
 ![Documentation Status](https://readthedocs.org/projects/openav/badge/?version=latest)
 
 <h4 align="center"><span style="color:#EC256F;">Description</span></h4>
 
 ---
 
->  **[OpenAV](https://github.com/DmitryRyumin/openav)** is an open-source library for recognition of speech commands in the user dictionary using audiovisual data of the speaker.
+> **[OpenAV](https://github.com/DmitryRyumin/openav)** is an open-source library for recognition of speech commands in the user dictionary using audiovisual data of the speaker.
 
 ---
 
 | [Documentation in Russian](https://github.com/DmitryRyumin/openav/blob/main/README_RU.md) |
 |-------------------------------------------------------------------------------------------|
 
-> The library under development
+> The library under development
```

### Comparing `openav-1.0.0a0/openav/modules/lab/build.py` & `openav-1.0.0a2/openav/modules/core/messages.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,65 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 """
-Сборка
+Сообщения
 """
 
 # ######################################################################################################################
 # Импорт необходимых инструментов
 # ######################################################################################################################
-# Подавление Warning
-import warnings
-for warn in [UserWarning, FutureWarning]: warnings.filterwarnings('ignore', category = warn)
+import warnings  # Подавление Warning
 
-from dataclasses import dataclass # Класс данных
+for warn in [UserWarning, FutureWarning]:
+    warnings.filterwarnings("ignore", category=warn)
 
-# ######################################################################################################################
-# Сообщения
-# ######################################################################################################################
-@dataclass
-class  RunMessages:
-    """Класс для сообщений"""
+from dataclasses import dataclass  # Класс данных
 
-    # ------------------------------------------------------------------------------------------------------------------
-    # Конструктор
-    # ------------------------------------------------------------------------------------------------------------------
+# Типы данных
+from typing import List
+
+# Персональные
+from openav.modules.core.language import Language  # Определение языка
 
-    def __post_init__(self):
-        self._in_development = 'The library under development'
 
 # ######################################################################################################################
-# Сборка
+# Сообщения
 # ######################################################################################################################
 @dataclass
-class Run(RunMessages):
-    """Класс для сборки"""
+class Messages(Language):
+    """Класс для сообщений
+
+    Args:
+        path_to_logs (str): Смотреть :attr:`~openav.modules.core.logging.Logging.path_to_logs`
+        lang (str): Смотреть :attr:`~openav.modules.core.language.Language.lang`
+    """
 
     # ------------------------------------------------------------------------------------------------------------------
     # Конструктор
     # ------------------------------------------------------------------------------------------------------------------
 
     def __post_init__(self):
-        super().__post_init__() # Выполнение конструктора из суперкласса
+        super().__post_init__()  # Выполнение конструктора из суперкласса
+
+        self._metadata: List[str] = [
+            self._(
+                "OpenAV - библиотека распознавания речевых команд на пользовательском словаре с использованием "
+                "аудиовизуальных данных диктора"
+            ),
+            self._("Авторы"),
+            self._("Сопровождающие"),
+            self._("Версия"),
+            self._("Лицензия"),
+        ]
+
+        self._format_time: str = "%Y-%m-%d %H:%M:%S"  # Формат времени
+
+        self._em: str = " ..."  # Конец сообщений (End Messages)
+
+        self._invalid_arguments: str = self._("Неверные типы или значения аргументов в") + ' "{}"' + self._em
+        self._unknown_err: str = (
+            self._("Не обработанную ошибку необходимо проанализировать и выявить причину") + self._em
+        )
 
-        print(self._in_development)
+        self._from_precent: str = self._("из")
+        self._curr_progress: str = "{} " + self._from_precent + " {} ({}%)" + self._em + " {}" + self._em
```

### Comparing `openav-1.0.0a0/openav.egg-info/PKG-INFO` & `openav-1.0.0a2/openav.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openav
-Version: 1.0.0a0
-Summary: openav
+Version: 1.0.0a2
+Summary: OpenAV
 Home-page: https://github.com/DmitryRyumin/openav
 Author: Dmitry Ryumin, Denis Ivanko, Nikolay Shilov, Maxim Markitantov, Alexey Karpov
 Author-email: dl_03.03.1991@mail.ru, denis.ivanko11@gmail.com, nick@iias.spb.su, m.markitantov@yandex.ru, karpov@iias.spb.su
 Maintainer: Dmitry Ryumin
 Maintainer-email: dl_03.03.1991@mail.ru
 License: MIT
 Project-URL: Bug Reports, https://github.com/DmitryRyumin/openav/issues
@@ -22,14 +22,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
@@ -58,23 +60,23 @@
 # [OpenAV](https://github.com/DmitryRyumin/openav)
 
 ![PyPI](https://img.shields.io/pypi/v/openav)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openav)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/openav)
 ![GitHub repo size](https://img.shields.io/github/repo-size/dmitryryumin/openav)
 ![PyPI - Status](https://img.shields.io/pypi/status/openav)
-![PyPI - License](https://img.shields.io/pypi/l/openav)
+![PyPI - License](https://img.shields.io/github/license/dmitryryumin/openav)
 ![GitHub top language](https://img.shields.io/github/languages/top/dmitryryumin/openav)
 ![Documentation Status](https://readthedocs.org/projects/openav/badge/?version=latest)
 
 <h4 align="center"><span style="color:#EC256F;">Description</span></h4>
 
 ---
 
->  **[OpenAV](https://github.com/DmitryRyumin/openav)** is an open-source library for recognition of speech commands in the user dictionary using audiovisual data of the speaker.
+> **[OpenAV](https://github.com/DmitryRyumin/openav)** is an open-source library for recognition of speech commands in the user dictionary using audiovisual data of the speaker.
 
 ---
 
 | [Documentation in Russian](https://github.com/DmitryRyumin/openav/blob/main/README_RU.md) |
 |-------------------------------------------------------------------------------------------|
 
 > The library under development
```

### Comparing `openav-1.0.0a0/setup.py` & `openav-1.0.0a2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,41 @@
 import sys
 
 from setuptools import setup, find_packages
 
 MIN_PYTHON_VERSION = (3, 9)
 
 if sys.version_info[:2] < MIN_PYTHON_VERSION:
-    raise RuntimeError('Python version required = {}.{}'.format(MIN_PYTHON_VERSION[0], MIN_PYTHON_VERSION[1]))
+    raise RuntimeError("Python version required = {}.{}".format(MIN_PYTHON_VERSION[0], MIN_PYTHON_VERSION[1]))
 
 import openav
 
 REQUIRED_PACKAGES = [
-    'ipython >= 8.7.0',
+    "ipython >= 8.10.0",
+    "colorama >= 0.4.6",
+    "numpy >= 1.24.2",
+    "pandas >= 1.5.3",
+    "prettytable >= 3.6.0",
+    "torch >= 1.13.1",
+    "torchaudio >= 0.13.1",
+    "torchvision >= 0.14.1",
+    "av >= 10.0.0",
+    "filetype >= 1.2.0",
+    "vosk >= 0.3.44",
+    "requests >= 2.28.2",
+    "pyyaml >= 6.0",
+    "streamlit >= 1.20.0",
+    "watchdog >= 2.3.1",
+    "pymediainfo >= 6.0.1",
+    "pillow >= 9.5.0",
+    "imgaug >= 0.4.0",
+    "flask >= 2.3.3",
+    "ffmpeg >= 1.4",
+    "librosa >= 0.10.1",
+    "matplotlib >= 3.6.3",
 ]
 
 CLASSIFIERS = """\
 Development Status :: 3 - Alpha
 Natural Language :: Russian
 Natural Language :: English
 Intended Audience :: Developers
@@ -23,14 +44,16 @@
 Intended Audience :: Science/Research
 Intended Audience :: Information Technology
 Intended Audience :: Science/Research
 License :: OSI Approved :: MIT License
 Programming Language :: Python
 Programming Language :: Python :: 3
 Programming Language :: Python :: 3.9
+Programming Language :: Python :: 3.10
+Programming Language :: Python :: 3.11
 Programming Language :: Python :: 3 :: Only
 Programming Language :: Python :: Implementation :: CPython
 Topic :: Scientific/Engineering
 Topic :: Scientific/Engineering :: Mathematics
 Topic :: Scientific/Engineering :: Artificial Intelligence
 Topic :: Scientific/Engineering :: Image Processing
 Topic :: Scientific/Engineering :: Image Recognition
@@ -50,42 +73,55 @@
 Operating System :: Microsoft :: Windows
 Operating System :: POSIX :: Linux
 Framework :: Jupyter
 Framework :: Jupyter :: JupyterLab :: 4
 Framework :: Sphinx
 """
 
-with open('README.md', 'r') as fh:
+with open("README.md", "r") as fh:
     long_description = fh.read()
 
     setup(
-        name = openav.__name__,
-        packages = find_packages(),
-        license = openav.__license__,
-        version = openav.__release__,
-        author = openav.__author__en__,
-        author_email = openav.__email__,
-        maintainer = openav.__maintainer__en__,
-        maintainer_email = openav.__maintainer_email__,
-        url = openav.__uri__,
-        description = openav.__summary__,
-        long_description = long_description,
-        long_description_content_type = 'text/markdown',
+        name=openav.__name__,
+        packages=find_packages(),
+        license=openav.__license__,
+        version=openav.__release__,
+        author=openav.__author__en__,
+        author_email=openav.__email__,
+        maintainer=openav.__maintainer__en__,
+        maintainer_email=openav.__maintainer_email__,
+        url=openav.__uri__,
+        description=openav.__summary__,
+        long_description=long_description,
+        long_description_content_type="text/markdown",
         install_requires=REQUIRED_PACKAGES,
-        keywords = [
-            'OpenAV', 'LipReading', 'SpeechRecognition', 'SignalProcessing', 'DataAugmentation',
-            'ArtificialNeuralNetworks', 'DeepMachineLearning', 'TransferLearning', 'Statistics', 'ComputerVision',
-            'ArtificialIntelligence', 'Preprocessing'
+        keywords=[
+            "OpenAV",
+            "LipReading",
+            "SpeechRecognition",
+            "SignalProcessing",
+            "DataAugmentation",
+            "ArtificialNeuralNetworks",
+            "DeepMachineLearning",
+            "TransferLearning",
+            "Statistics",
+            "ComputerVision",
+            "ArtificialIntelligence",
+            "Preprocessing",
         ],
-        include_package_data = True,
-        classifiers = [_f for _f in CLASSIFIERS.split('\n') if _f],
-        python_requires = '>=3.9, <4',
-        entry_points = {
-            'console_scripts': [],
+        include_package_data=True,
+        classifiers=[_f for _f in CLASSIFIERS.split("\n") if _f],
+        python_requires=">=3.9, <4",
+        entry_points={
+            "console_scripts": [
+                "openav_vad = openav.api.vad:main",
+                "openav_vosk_sr = openav.api.vosk_sr:main",
+                "openav_preprocess_audio = openav.api.preprocess_audio:main",
+            ],
         },
-        project_urls = {
-            'Bug Reports': 'https://github.com/DmitryRyumin/openav/issues',
-            'Documentation': 'https://openav.readthedocs.io',
-            'Source Code': 'https://github.com/DmitryRyumin/openav/tree/main/openav',
-            'Download': 'https://github.com/DmitryRyumin/openav/tags',
+        project_urls={
+            "Bug Reports": "https://github.com/DmitryRyumin/openav/issues",
+            "Documentation": "https://openav.readthedocs.io",
+            "Source Code": "https://github.com/DmitryRyumin/openav/tree/main/openav",
+            "Download": "https://github.com/DmitryRyumin/openav/tags",
         },
     )
```

