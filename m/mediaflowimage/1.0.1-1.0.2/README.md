# Comparing `tmp/mediaflowimage-1.0.1.tar.gz` & `tmp/mediaflowimage-1.0.2.tar.gz`

## Comparing `mediaflowimage-1.0.1.tar` & `mediaflowimage-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/__init__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/admin.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/apps.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/blocks.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/forms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/models.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/tests.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/views.py
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/wagtail_hooks.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/migrations/__init__.py
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/LICENSE
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/README.md
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 mediaflowimage-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/__init__.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/admin.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/apps.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/blocks.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/forms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/models.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/tests.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/views.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/wagtail_hooks.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/migrations/__init__.py
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/src/mediaflowimage/templates/widgets/mediaflow-custom-imageinput.html
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/README.md
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 mediaflowimage-1.0.2/PKG-INFO
```

### Comparing `mediaflowimage-1.0.1/src/mediaflowimage/wagtail_hooks.py` & `mediaflowimage-1.0.2/src/mediaflowimage/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.1/src/mediaflowimage/widgets.py` & `mediaflowimage-1.0.2/src/mediaflowimage/widgets.py`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.1/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js` & `mediaflowimage-1.0.2/src/mediaflowimage/static/js/mediaflow-imagechooser-extensions.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -101,15 +101,21 @@
 
         const mapping_jsonstr = $('#mf-meta-mapping').val().replaceAll("'", '"')
         const meta_mapping = JSON.parse(mapping_jsonstr)
         for (key of Object.keys(meta_mapping)) {
             if (key == "id") {
                 idImage = metaData[key]
             }
-            formData.append('image-chooser-upload-' + meta_mapping[key], metaData[key] || '')
+
+            let fields = meta_mapping[key].split(',');
+            for (let field of fields) {
+                formData.append('image-chooser-upload-' + field, metaData[key] || '')
+            }
+
+
         }
         $.ajax({
             beforeSend: function(request) {
                 request.setRequestHeader('X-CSRFToken', csrfToken)
             },
             contentType: false,
             data: formData,
```

### Comparing `mediaflowimage-1.0.1/LICENSE` & `mediaflowimage-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.1/README.md` & `mediaflowimage-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mediaflowimage-1.0.1/pyproject.toml` & `mediaflowimage-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "mediaflowimage"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Mediaflow Europe AB", email="support@mediaflow.com" },
 ]
 description = "Wagtail image plugin for Mediaflow"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mediaflowimage-1.0.1/PKG-INFO` & `mediaflowimage-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mediaflowimage
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wagtail image plugin for Mediaflow
 Project-URL: Homepage, https://support.mediaflow.com
 Project-URL: Issues, https://support.mediaflow.com
 Author-email: Mediaflow Europe AB <support@mediaflow.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

