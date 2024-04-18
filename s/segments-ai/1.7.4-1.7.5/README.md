# Comparing `tmp/segments-ai-1.7.4.tar.gz` & `tmp/segments-ai-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segments-ai-1.7.4.tar", last modified: Wed Apr 10 09:53:33 2024, max compression
+gzip compressed data, was "segments-ai-1.7.5.tar", last modified: Thu Apr 18 15:18:55 2024, max compression
```

## Comparing `segments-ai-1.7.4.tar` & `segments-ai-1.7.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/
--rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.7.4/LICENSE.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.7.4/MANIFEST.in
--rw-rw-r--   0 bert      (1000) bert      (1000)     1134 2024-04-10 09:53:33.137741 segments-ai-1.7.4/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.7.4/README.md
--rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.7.4/pyproject.toml
--rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.7.4/requirements.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.7.4/requirements_dev.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.7.4/requirements_docs.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-04-10 09:53:33.137741 segments-ai-1.7.4/setup.cfg
--rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-04-10 09:51:52.000000 segments-ai-1.7.4/setup.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/segments/
--rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.7.4/src/segments/__init__.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    87565 2024-03-15 11:08:21.000000 segments-ai-1.7.4/src/segments/client.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/segments/data/
--rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.7.4/src/segments/data/dataset_card_template.md
--rw-rw-r--   0 bert      (1000) bert      (1000)    14548 2024-03-05 14:46:29.000000 segments-ai-1.7.4/src/segments/dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.7.4/src/segments/exceptions.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    30413 2023-11-23 10:20:03.000000 segments-ai-1.7.4/src/segments/export.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.7.4/src/segments/huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.4/src/segments/py.typed
--rw-rw-r--   0 bert      (1000) bert      (1000)    22856 2024-04-10 09:51:23.000000 segments-ai-1.7.4/src/segments/typing.py
--rw-rw-r--   0 bert      (1000) bert      (1000)    35687 2024-04-07 13:40:19.000000 segments-ai-1.7.4/src/segments/utils.py
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/src/segments_ai.egg-info/
--rw-r--r--   0 bert      (1000) bert      (1000)     1134 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/PKG-INFO
--rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-04-10 09:53:33.000000 segments-ai-1.7.4/src/segments_ai.egg-info/SOURCES.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/dependency_links.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/requires.txt
--rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-04-10 09:53:32.000000 segments-ai-1.7.4/src/segments_ai.egg-info/top_level.txt
-drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-10 09:53:33.137741 segments-ai-1.7.4/tests/
--rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.7.4/tests/test_client.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.7.4/tests/test_dataset.py
--rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.4/tests/test_huggingface.py
--rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.7.4/tests/test_random.py
--rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.7.4/tests/test_utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-18 15:18:55.818469 segments-ai-1.7.5/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1062 2020-01-04 18:38:00.000000 segments-ai-1.7.5/LICENSE.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)       83 2023-09-06 09:45:12.000000 segments-ai-1.7.5/MANIFEST.in
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1134 2024-04-18 15:18:55.818469 segments-ai-1.7.5/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2955 2023-11-23 15:51:52.000000 segments-ai-1.7.5/README.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)      714 2023-11-23 10:20:03.000000 segments-ai-1.7.5/pyproject.toml
+-rw-rw-r--   0 bert      (1000) bert      (1000)      194 2024-02-01 10:25:04.000000 segments-ai-1.7.5/requirements.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      197 2023-11-23 10:20:03.000000 segments-ai-1.7.5/requirements_dev.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      171 2023-09-21 17:58:29.000000 segments-ai-1.7.5/requirements_docs.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      233 2024-04-18 15:18:55.818469 segments-ai-1.7.5/setup.cfg
+-rw-rw-r--   0 bert      (1000) bert      (1000)     3287 2024-04-18 15:17:50.000000 segments-ai-1.7.5/setup.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-18 15:18:55.814469 segments-ai-1.7.5/src/
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-18 15:18:55.818469 segments-ai-1.7.5/src/segments/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      138 2023-11-23 10:20:03.000000 segments-ai-1.7.5/src/segments/__init__.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    87565 2024-03-15 11:08:21.000000 segments-ai-1.7.5/src/segments/client.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-18 15:18:55.818469 segments-ai-1.7.5/src/segments/data/
+-rw-rw-r--   0 bert      (1000) bert      (1000)      501 2022-08-02 10:22:42.000000 segments-ai-1.7.5/src/segments/data/dataset_card_template.md
+-rw-rw-r--   0 bert      (1000) bert      (1000)    14548 2024-03-05 14:46:29.000000 segments-ai-1.7.5/src/segments/dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     2191 2023-10-10 09:44:13.000000 segments-ai-1.7.5/src/segments/exceptions.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    30413 2023-11-23 10:20:03.000000 segments-ai-1.7.5/src/segments/export.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    11870 2023-11-23 10:20:03.000000 segments-ai-1.7.5/src/segments/huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.5/src/segments/py.typed
+-rw-rw-r--   0 bert      (1000) bert      (1000)    23003 2024-04-18 15:17:40.000000 segments-ai-1.7.5/src/segments/typing.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)    35687 2024-04-07 13:40:19.000000 segments-ai-1.7.5/src/segments/utils.py
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-18 15:18:55.818469 segments-ai-1.7.5/src/segments_ai.egg-info/
+-rw-r--r--   0 bert      (1000) bert      (1000)     1134 2024-04-18 15:18:55.000000 segments-ai-1.7.5/src/segments_ai.egg-info/PKG-INFO
+-rw-rw-r--   0 bert      (1000) bert      (1000)      691 2024-04-18 15:18:55.000000 segments-ai-1.7.5/src/segments_ai.egg-info/SOURCES.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        1 2024-04-18 15:18:55.000000 segments-ai-1.7.5/src/segments_ai.egg-info/dependency_links.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)      446 2024-04-18 15:18:55.000000 segments-ai-1.7.5/src/segments_ai.egg-info/requires.txt
+-rw-rw-r--   0 bert      (1000) bert      (1000)        9 2024-04-18 15:18:55.000000 segments-ai-1.7.5/src/segments_ai.egg-info/top_level.txt
+drwxrwxr-x   0 bert      (1000) bert      (1000)        0 2024-04-18 15:18:55.818469 segments-ai-1.7.5/tests/
+-rw-rw-r--   0 bert      (1000) bert      (1000)    38723 2023-11-23 15:51:56.000000 segments-ai-1.7.5/tests/test_client.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1270 2023-11-23 10:20:03.000000 segments-ai-1.7.5/tests/test_dataset.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)        0 2022-08-02 10:22:42.000000 segments-ai-1.7.5/tests/test_huggingface.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)      226 2022-08-02 10:22:42.000000 segments-ai-1.7.5/tests/test_random.py
+-rw-rw-r--   0 bert      (1000) bert      (1000)     1052 2023-07-21 08:16:50.000000 segments-ai-1.7.5/tests/test_utils.py
```

### Comparing `segments-ai-1.7.4/LICENSE.txt` & `segments-ai-1.7.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/PKG-INFO` & `segments-ai-1.7.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.7.4
+Version: 1.7.5
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.4.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.5.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `segments-ai-1.7.4/README.md` & `segments-ai-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/pyproject.toml` & `segments-ai-1.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/setup.py` & `segments-ai-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from typing import List
 
 
 #############
 # Constants #
 #############
-MAJOR, MINOR, PATCH = 1, 7, 4
+MAJOR, MINOR, PATCH = 1, 7, 5
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 
 ####################
 # Helper functions #
 ####################
 # https://github.com/allenai/python-package-template
```

### Comparing `segments-ai-1.7.4/src/segments/client.py` & `segments-ai-1.7.5/src/segments/client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/src/segments/dataset.py` & `segments-ai-1.7.5/src/segments/dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/src/segments/exceptions.py` & `segments-ai-1.7.5/src/segments/exceptions.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/src/segments/export.py` & `segments-ai-1.7.5/src/segments/export.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/src/segments/huggingface.py` & `segments-ai-1.7.5/src/segments/huggingface.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/src/segments/typing.py` & `segments-ai-1.7.5/src/segments/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 class InputType(str, Enum):
     SELECT = "select"
     TEXT = "text"
     NUMBER = "number"
     CHECKBOX = "checkbox"
     VECTOR3 = "vector3"
     QUATERNION = "quaternion"
+    POINTS = "points"
 
 
 class CameraDistortionModel(str, Enum):
     FISH_EYE = "fisheye"
     BROWN_CONRADY = "brown-conrady"
 
 
@@ -303,20 +304,18 @@
 
 # Image sequence segmentation
 class ImageSequenceSegmentationAnnotation(Annotation):
     track_id: int
     is_keyframe: bool = False
 
 
-class ImageSequenceSegmentationFrame(BaseModel):
+class ImageSequenceSegmentationFrame(ImageSegmentationLabelAttributes):
     annotations: List[ImageSequenceSegmentationAnnotation]
-    segmentation_bitmap: Optional[URL] = None
-    format_version: Optional[FormatVersion] = None
-    image_attributes: Optional[ImageAttributes] = None
     timestamp: Optional[Timestamp] = None
+    format_version: Optional[FormatVersion] = None
 
 
 class ImageSequenceSegmentationLabelAttributes(BaseModel):
     frames: List[ImageSequenceSegmentationFrame]
     format_version: Optional[FormatVersion] = None
 
 
@@ -743,21 +742,29 @@
 class QuaternionTaskAttribute(BaseModel):
     name: str
     input_type: Literal[InputType.QUATERNION]
     is_mandatory: Optional[bool] = None
     is_track_level: Optional[bool] = None
 
 
+class PointsTaskAttribute(BaseModel):
+    name: str
+    input_type: Literal[InputType.POINTS]
+    is_mandatory: Optional[bool] = None
+    is_track_level: Optional[bool] = None
+
+
 TaskAttribute = Union[
     SelectTaskAttribute,
     TextTaskAttribute,
     NumberTaskAttribute,
     CheckboxTaskAttribute,
     Vector3TaskAttribute,
     QuaternionTaskAttribute,
+    PointsTaskAttribute,
 ]
 
 
 class TaskAttributeCategory(BaseModel):
     name: str
     id: int
     color: Optional[Union[RGB, RGBA]] = None
```

### Comparing `segments-ai-1.7.4/src/segments/utils.py` & `segments-ai-1.7.5/src/segments/utils.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/src/segments_ai.egg-info/PKG-INFO` & `segments-ai-1.7.5/src/segments_ai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: segments-ai
-Version: 1.7.4
+Version: 1.7.5
 Home-page: https://github.com/segments-ai/segments-ai
-Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.4.tar.gz
+Download-URL: https://github.com/segments-ai/segments-ai/archive/v1.7.5.tar.gz
 Author: Segments.ai
 Author-email: bert@segments.ai
 License: MIT
 Keywords: image,segmentation,labeling,vision
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `segments-ai-1.7.4/src/segments_ai.egg-info/SOURCES.txt` & `segments-ai-1.7.5/src/segments_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/tests/test_client.py` & `segments-ai-1.7.5/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/tests/test_dataset.py` & `segments-ai-1.7.5/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `segments-ai-1.7.4/tests/test_utils.py` & `segments-ai-1.7.5/tests/test_utils.py`

 * *Files identical despite different names*

