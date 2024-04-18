# Comparing `tmp/silicon_analyser-1.0.7.tar.gz` & `tmp/silicon_analyser-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silicon_analyser-1.0.7.tar", last modified: Wed Apr 17 18:29:27 2024, max compression
+gzip compressed data, was "silicon_analyser-1.0.8.tar", last modified: Thu Apr 18 18:34:42 2024, max compression
```

## Comparing `silicon_analyser-1.0.7.tar` & `silicon_analyser-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/
--rw-rw-rw-   0        0        0     1087 2024-04-07 16:13:23.000000 silicon_analyser-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     3334 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2530 2024-04-16 18:45:45.000000 silicon_analyser-1.0.7/README.md
--rw-rw-rw-   0        0        0     1154 2024-04-16 16:45:56.000000 silicon_analyser-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/
-drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/
--rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.py
--rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.ui
--rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.py
--rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.ui
--rw-rw-rw-   0        0        0     3883 2024-04-16 18:29:36.000000 silicon_analyser-1.0.7/silicon_analyser/grid.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/helper/
-drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/
--rw-rw-rw-   0        0        0     2406 2024-04-16 16:39:34.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractimage.py
--rw-rw-rw-   0        0        0     2812 2024-04-16 16:00:12.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractmywindow.py
--rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstracttreehelper.py
--rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.7/silicon_analyser/helper/addgridbtn.py
--rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.7/silicon_analyser/helper/addlabelbtn.py
--rw-rw-rw-   0        0        0     1403 2024-04-16 18:13:14.000000 silicon_analyser-1.0.7/silicon_analyser/helper/ai.py
--rw-rw-rw-   0        0        0    14568 2024-04-16 17:42:57.000000 silicon_analyser-1.0.7/silicon_analyser/helper/computebtn.py
--rw-rw-rw-   0        0        0    21170 2024-04-17 15:20:05.000000 silicon_analyser-1.0.7/silicon_analyser/helper/fullimage.py
--rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.7/silicon_analyser/helper/minimap.py
--rw-rw-rw-   0        0        0     3989 2024-04-16 18:29:06.000000 silicon_analyser-1.0.7/silicon_analyser/helper/properties.py
--rw-rw-rw-   0        0        0    20657 2024-04-16 18:12:59.000000 silicon_analyser-1.0.7/silicon_analyser/helper/tree.py
--rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.7/silicon_analyser/main.py
--rw-rw-rw-   0        0        0     6845 2024-04-16 15:59:53.000000 silicon_analyser-1.0.7/silicon_analyser/main_window.ui
--rw-rw-rw-   0        0        0     9878 2024-04-16 16:00:07.000000 silicon_analyser-1.0.7/silicon_analyser/mywindow.py
--rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.7/silicon_analyser/rect.py
--rw-rw-rw-   0        0        0     2305 2024-04-16 18:10:57.000000 silicon_analyser-1.0.7/silicon_analyser/savefiles.py
--rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.7/silicon_analyser/treeitem.py
-drwxrwxrwx   0        0        0        0 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/
--rw-rw-rw-   0        0        0     3334 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1078 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       64 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 18:29:27.000000 silicon_analyser-1.0.7/silicon_analyser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/
+-rw-rw-rw-   0        0        0     1087 2024-04-18 18:34:42.000000 silicon_analyser-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3334 2024-04-18 18:34:42.000000 silicon_analyser-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2530 2024-04-16 18:45:45.000000 silicon_analyser-1.0.8/README.md
+-rw-rw-rw-   0        0        0     1154 2024-04-18 18:33:46.000000 silicon_analyser-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-18 18:34:42.000000 silicon_analyser-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/
+-rw-rw-rw-   0        0        0     3487 2024-04-13 14:15:10.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.py
+-rw-rw-rw-   0        0        0     1508 2024-04-06 18:45:56.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.ui
+-rw-rw-rw-   0        0        0     3340 2024-04-14 09:21:04.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.py
+-rw-rw-rw-   0        0        0     3752 2024-04-14 09:20:00.000000 silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.ui
+-rw-rw-rw-   0        0        0     3883 2024-04-16 18:29:36.000000 silicon_analyser-1.0.8/silicon_analyser/grid.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/helper/
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/
+-rw-rw-rw-   0        0        0     2406 2024-04-16 16:39:34.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractimage.py
+-rw-rw-rw-   0        0        0     2881 2024-04-18 17:24:06.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractmywindow.py
+-rw-rw-rw-   0        0        0     1024 2024-04-13 06:54:26.000000 silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstracttreehelper.py
+-rw-rw-rw-   0        0        0      719 2024-04-13 07:29:28.000000 silicon_analyser-1.0.8/silicon_analyser/helper/addgridbtn.py
+-rw-rw-rw-   0        0        0      696 2024-04-08 17:17:53.000000 silicon_analyser-1.0.8/silicon_analyser/helper/addlabelbtn.py
+-rw-rw-rw-   0        0        0     1768 2024-04-18 18:06:25.000000 silicon_analyser-1.0.8/silicon_analyser/helper/ai.py
+-rw-rw-rw-   0        0        0    16999 2024-04-18 18:21:52.000000 silicon_analyser-1.0.8/silicon_analyser/helper/computebtn.py
+-rw-rw-rw-   0        0        0    21170 2024-04-17 15:20:05.000000 silicon_analyser-1.0.8/silicon_analyser/helper/fullimage.py
+-rw-rw-rw-   0        0        0     1532 2024-04-13 13:40:26.000000 silicon_analyser-1.0.8/silicon_analyser/helper/minimap.py
+-rw-rw-rw-   0        0        0     3989 2024-04-16 18:29:06.000000 silicon_analyser-1.0.8/silicon_analyser/helper/properties.py
+-rw-rw-rw-   0        0        0    20657 2024-04-16 18:12:59.000000 silicon_analyser-1.0.8/silicon_analyser/helper/tree.py
+-rw-rw-rw-   0        0        0      263 2024-04-08 17:15:10.000000 silicon_analyser-1.0.8/silicon_analyser/main.py
+-rw-rw-rw-   0        0        0     7687 2024-04-18 18:24:48.000000 silicon_analyser-1.0.8/silicon_analyser/main_window.ui
+-rw-rw-rw-   0        0        0    10412 2024-04-18 17:28:35.000000 silicon_analyser-1.0.8/silicon_analyser/mywindow.py
+-rw-rw-rw-   0        0        0      134 2024-04-07 08:11:27.000000 silicon_analyser-1.0.8/silicon_analyser/rect.py
+-rw-rw-rw-   0        0        0     2305 2024-04-16 18:10:57.000000 silicon_analyser-1.0.8/silicon_analyser/savefiles.py
+-rw-rw-rw-   0        0        0     1365 2024-04-13 14:16:41.000000 silicon_analyser-1.0.8/silicon_analyser/treeitem.py
+drwxrwxrwx   0        0        0        0 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/
+-rw-rw-rw-   0        0        0     3334 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1078 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       64 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-18 18:34:41.000000 silicon_analyser-1.0.8/silicon_analyser.egg-info/top_level.txt
```

### Comparing `silicon_analyser-1.0.7/LICENSE` & `silicon_analyser-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/PKG-INFO` & `silicon_analyser-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.7
+Version: 1.0.8
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `silicon_analyser-1.0.7/README.md` & `silicon_analyser-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/pyproject.toml` & `silicon_analyser-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "silicon-analyser"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="CrazyT", email="crazyt2019+sa@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.py` & `silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/dialogs/compute_stats.ui` & `silicon_analyser-1.0.8/silicon_analyser/dialogs/compute_stats.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.py` & `silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/dialogs/pixel_image.ui` & `silicon_analyser-1.0.8/silicon_analyser/dialogs/pixel_image.ui`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/grid.py` & `silicon_analyser-1.0.8/silicon_analyser/grid.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractimage.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractimage.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstractmywindow.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstractmywindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     _actionSaveModel: QAction
     _actionLoadModel: QAction
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     _actionExportCellsToImages: QAction
+    _actionDecisionTree: QAction
+    _actionNeuralNetwork: QAction
     autosave: bool
     def __init__(self):
         QMainWindow.__init__(self)
         
     def getManualItem(self) -> QStandardItem:
         raise NotImplementedError()
```

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/abstract/abstracttreehelper.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/abstract/abstracttreehelper.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/addgridbtn.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/addgridbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/addlabelbtn.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/addlabelbtn.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/computebtn.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/computebtn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from sklearn.model_selection import train_test_split
+from sklearn.tree import DecisionTreeClassifier
+from sklearn.metrics import accuracy_score
 import os
 from PyQt5.QtWidgets import QPushButton
 from PyQt5.QtCore import QObject, QThread, pyqtSignal
 from PyQt5.QtGui import QMouseEvent
 import random
 import numpy as np
 import sys
@@ -40,39 +42,51 @@
     
     def __init__(self,myWindow: AbstractMyWindow, computeStatsDlg: ComputeStatsDlg):
         QObject.__init__(self)
         self._myWindow = myWindow
         self._computeStatsDlg = computeStatsDlg
 
     def run(self):
-        self._computeStatsDlg.setStatus("Initialize keras ...")
-        os.environ["KERAS_BACKEND"] = "torch"
-        import keras
-        self._computeStatsDlg.setStatus("... finished Initializing keras")
+        useDecisionTree = self._myWindow._actionDecisionTree.isChecked()
+        useNeuralNetwork = self._myWindow._actionNeuralNetwork.isChecked()
         
-        def appendFoundRects(self, rectKeys, maxW, maxH, model_conv, MP):
+        if useNeuralNetwork:
+            self._computeStatsDlg.setStatus("Initialize keras ...")
+            os.environ["KERAS_BACKEND"] = "torch"
+            import keras
+            self._computeStatsDlg.setStatus("... finished Initializing keras")
+        
+        if useDecisionTree:
+            decisionTree = DecisionTreeClassifier(criterion = 'entropy')
+            self._computeStatsDlg.setStatus("Using decision tree")
+        
+        def appendFoundRects(self, rectKeys, maxW, maxH, model_conv, MP, decisionTree: DecisionTreeClassifier|None = None):
             import keras_cv
             bx = 10000
             by = 10000
             data = self._myWindow.getImage().fetchFullData()[:,:,0:3]
             dx = data.shape[0]
             dy = data.shape[1]
             dx -= dx % bx
             dy -= dy % by
             maxCnt = 20
             data = data[0:dx,0:dy]
             print("data.shape", data.shape)
-            model_conv.build(input_shape=[1,*data.shape[0:2],3])
+            if decisionTree is None:
+                model_conv.build(input_shape=[1,*data.shape[0:2],3])
             subdataIdx = 0
             cnt = 0
             for subdata in blockshaped(data, bx, by):
                 if cnt < maxCnt:
                     print("subdata.shape",subdata.shape)
-                    r = model_conv(np.array([subdata]))[0]
-                    r = r.cpu().detach().numpy()
+                    if decisionTree is None:
+                        r = model_conv(np.array([subdata]))[0]
+                        r = r.cpu().detach().numpy()
+                    else:
+                        r = decisionTree.predict(np.array([subdata]))
                     print("r.shape",r.shape)
                     for rx in range(0,r.shape[0]):
                         for ry in range(0,r.shape[1]):
                             if cnt >= maxCnt:
                                 continue
                             x = rx + int(subdataIdx * subdata.shape[0]) % data.shape[0]
                             y = ry + (int(subdataIdx * subdata.shape[0]) // data.shape[0])*subdata.shape[1]
@@ -83,43 +97,77 @@
                                 key = rectKeys[idx-1]
                                 ex = x+maxW
                                 ey = y+maxH
                                 self._myWindow.getImage().appendAIRect(key,x,y,ex,ey)
                                 cnt += 1
                 subdataIdx += 1
 
-        class MyPlottingCallback(keras.callbacks.Callback):
-            def __init__(self, plotDlg: ComputeStatsDlg):
-                self._plotDlg = plotDlg
-            
-            def on_epoch_end(self, epoch, logs=None): 
-                if logs is None:
-                    return
-                self._plotDlg.request_graph_update.emit(logs, epoch)
-                if self._plotDlg.isStop():
-                    self.model.stop_training = True # type: ignore
-            
-        class MyThresholdCallback(keras.callbacks.Callback):
-            def __init__(self, threshold, patience):
-                super(MyThresholdCallback, self).__init__()
-                self.threshold = threshold
-                self.patience = patience
-                self.count = 0
-
-            def on_epoch_end(self, epoch, logs=None): 
-                if logs is None:
-                    return
-                val_acc = logs["val_accuracy"]
-                if val_acc >= self.threshold:
-                    if self.count > self.patience:
+        if useNeuralNetwork:
+            class MyPlottingCallback(keras.callbacks.Callback):
+                def __init__(self, plotDlg: ComputeStatsDlg):
+                    self._plotDlg = plotDlg
+                
+                def on_epoch_end(self, epoch, logs=None): 
+                    if logs is None:
+                        return
+                    self._plotDlg.request_graph_update.emit(logs, epoch)
+                    if self._plotDlg.isStop():
                         self.model.stop_training = True # type: ignore
-                    else:
-                        self.count += 1
-                else:
+                
+            class MyThresholdCallback(keras.callbacks.Callback):
+                def __init__(self, threshold, patience):
+                    super(MyThresholdCallback, self).__init__()
+                    self.threshold = threshold
+                    self.patience = patience
                     self.count = 0
+
+                def on_epoch_end(self, epoch, logs=None): 
+                    if logs is None:
+                        return
+                    val_acc = logs["val_accuracy"]
+                    if val_acc >= self.threshold:
+                        if self.count > self.patience:
+                            self.model.stop_training = True # type: ignore
+                        else:
+                            self.count += 1
+                    else:
+                        self.count = 0
+                        
+            def createModels(countGroups, maxW, maxH, MP):
+                conv2 = keras.layers.Conv2D(
+                        countGroups*5,
+                        name="conv2d_2",
+                        kernel_size=(int(maxH//MP-5),int(maxW//MP-5)),
+                        activation="softmax"
+                )
+
+                conv3 = keras.layers.Conv2D(
+                        countGroups,
+                        name="conv2d_3",
+                        kernel_size=(1+5,1+5),
+                        activation="softmax"
+                )
+
+                model_conv = keras.Sequential([
+                    keras.layers.BatchNormalization(),
+                    keras.layers.MaxPooling2D(MP),
+                    conv2,
+                    conv3
+                ])
+
+                model_train = keras.Sequential([
+                    keras.layers.Input((maxH,maxW,3)),
+                    keras.layers.BatchNormalization(),
+                    keras.layers.MaxPooling2D(MP),
+                    conv2,
+                    conv3,
+                    keras.layers.Reshape((countGroups,))
+                ])
+                model_train.summary()
+                return model_conv,model_train
         
         print("_worker runs")
         try:
             self._computeStatsDlg.reset()
             selectedType = self._myWindow.getTree().selectedType()
             gridMode = (selectedType == TreeItem.TYPE_GRID) or (selectedType == TreeItem.TYPE_GRID_ITEM) or (selectedType == TreeItem.TYPE_AI_GRID) or (selectedType == TreeItem.TYPE_AI_GRID_ITEM)
             rects = self._myWindow.getImage().getRects()
@@ -128,51 +176,70 @@
 
             if gridMode:
                 grid: Grid = self._myWindow.getTree().getSelectedGrid()
                 maxW, maxH, labels, countGroups, MP, train, vals = self.initTrainAndValsForGrid(grid)
             else:
                 maxW, maxH, countGroups, MP, train, vals = self.initTrainAndValsForRects(rects, ignoreRects)
 
-            model_conv, model_train = self.createModels(keras, countGroups, maxW, maxH, MP)
+            if useNeuralNetwork:
+                model_conv, model_train = createModels(countGroups, maxW, maxH, MP)
             
             if gridMode:
                 aiGrid = self.prepareGridData(grid, labels, countGroups, maxW, maxH, train, vals)
             else:
                 self.prepareRectData(rects, countGroups, ignoreRects, maxW, maxH, train, vals)
             
-            callbacks = [MyPlottingCallback(self._computeStatsDlg),MyThresholdCallback(0.99,200)]
-            model_train.compile(optimizer=keras.optimizers.Adam(learning_rate=0.002),loss="binary_crossentropy",metrics=["accuracy"])
+            if useNeuralNetwork:
+                callbacks = [MyPlottingCallback(self._computeStatsDlg),MyThresholdCallback(0.99,200)]
+                model_train.compile(optimizer=keras.optimizers.Adam(learning_rate=0.002),loss="binary_crossentropy",metrics=["accuracy"])
+            
             print("before fit")
             print("vals",vals)
             print("train.shape",train.shape)
             print("vals.shape",vals.shape)
             
             xtraining, ytraining, xvalidation, yvalidation = train_test_split(train,vals,shuffle = True,test_size=0.1) 
 
-            history = model_train.fit(
-                x = xtraining,
-                y = xvalidation,
-                epochs = 100000,
-                verbose = 0,
-                validation_data=(ytraining,yvalidation),
-                shuffle = True,
-                batch_size = 512,
-                callbacks = callbacks
-            )
-            
-            print("after fit")
-            self._myWindow.setStatusText("Accuracy: %s" % history.history["accuracy"][-1])
-            
-            if gridMode:
-                appendFoundCellRects(self._myWindow.getImage(), grid, aiGrid, maxW, maxH, model_train)
-            else:
-                appendFoundRects(self, list(rects.keys()), maxW, maxH, model_conv, MP)
+            if useNeuralNetwork:
+                history = model_train.fit(
+                    x = xtraining,
+                    y = xvalidation,
+                    epochs = 100000,
+                    verbose = 0,
+                    validation_data=(ytraining,yvalidation),
+                    shuffle = True,
+                    batch_size = 512,
+                    callbacks = callbacks
+                )
+                print("after fit")
+                self._myWindow.setStatusText("Accuracy: %s" % history.history["accuracy"][-1])
+                if gridMode:
+                    appendFoundCellRects(self._myWindow.getImage(), grid, aiGrid, maxW, maxH, model_train)
+                else:
+                    appendFoundRects(self, list(rects.keys()), maxW, maxH, model_conv, MP)
+                            
+            if useDecisionTree:
+                xtraining2 = xtraining.reshape(xtraining.shape[0],xtraining.shape[1]*xtraining.shape[2]*xtraining.shape[3])
+                ytraining2 = ytraining.reshape(ytraining.shape[0],ytraining.shape[1]*ytraining.shape[2]*ytraining.shape[3])
+                decisionTree.fit(xtraining2, xvalidation)
+                y2 = decisionTree.predict(ytraining2)
+                print("after fit")
+                accuracy = accuracy_score(y2, yvalidation)
+                self._computeStatsDlg.request_graph_update.emit({"loss":1,"val_loss":1,"accuracy":accuracy,"val_accuracy":accuracy}, 0)
+                self._computeStatsDlg.request_graph_update.emit({"loss":1,"val_loss":1,"accuracy":accuracy,"val_accuracy":accuracy}, 1)
+                self._myWindow.setStatusText("Accuracy: %s" % accuracy)
+                if gridMode:
+                    appendFoundCellRects(self._myWindow.getImage(), grid, aiGrid, maxW, maxH, None, decisionTree)
+                else:
+                    appendFoundRects(self, list(rects.keys()), maxW, maxH, None, MP, decisionTree)
+                self._computeStatsDlg.setStatus("Decision tree finished with accuracy: %s" % accuracy)
             
             self._myWindow.getImage().drawImage()
-            self._myWindow.setLastModel(aiGrid.name, model_train)
+            if useNeuralNetwork:
+                self._myWindow.setLastModel(aiGrid.name, model_train)
         except Exception as e:
             self._computeStatsDlg.setError(e)
         finally:
             self.finished.emit()
     
     # TODO: maybe deprecated, not shure yet
     def initTrainAndValsForRects(self, rects, ignoreRects):
@@ -262,88 +329,52 @@
         ii = 0
         aiGrid, aiTreeItem = self._myWindow.getTree().addTreeItem(grid.name,TreeItem.TYPE_AI_GRID)
         for l in labels:
             self._myWindow.getTree().addTreeItem(l,TreeItem.TYPE_AI_GRID_ITEM,aiGrid,aiTreeItem)
             for cx in range(0,grid.cols):
                 for cy in range(0,grid.rows):
                     if grid.isRectSet(cx,cy,l):
-                        x = int(grid.x + cx*maxW)
-                        y = int(grid.y + cy*maxH)
+                        x = grid.absX(cx,cy)
+                        y = grid.absY(cy,cx)
                         ex = x + maxW - 1
                         ey = y + maxH - 1
                         data = self._myWindow.getImage().fetchData(x,y,ex,ey)
                         train[i,0:maxH,0:maxW] = data
                         #np.save(f"samples/{l}_{cx:03d}_{cy:03d}_{x:04d}_{y:04d}.bin",data)
                         vals[i] = np.eye(countGroups,dtype=np.float32)[ii]
                         i += 1
             ii += 1
         return aiGrid
-
-    def createModels(self, keras, countGroups, maxW, maxH, MP):
-        conv2 = keras.layers.Conv2D(
-                countGroups*5,
-                name="conv2d_2",
-                kernel_size=(int(maxH//MP-5),int(maxW//MP-5)),
-                activation="softmax"
-        )
-
-        conv3 = keras.layers.Conv2D(
-                countGroups,
-                name="conv2d_3",
-                kernel_size=(1+5,1+5),
-                activation="softmax"
-        )
-
-        model_conv = keras.Sequential([
-            keras.layers.BatchNormalization(),
-            keras.layers.MaxPooling2D(MP),
-            conv2,
-            conv3
-        ])
-
-        model_train = keras.Sequential([
-            keras.layers.Input((maxH,maxW,3)),
-            keras.layers.BatchNormalization(),
-            keras.layers.MaxPooling2D(MP),
-            conv2,
-            conv3,
-            keras.layers.Reshape((countGroups,))
-        ])
-        model_train.summary()
-        return model_conv,model_train
         
 class ComputeBtn(QPushButton):
     _computeStatsDlg: ComputeStatsDlg
 
     def __init__(self, text: str):
         QPushButton.__init__(self, text)
         self._computeStatsDlg = ComputeStatsDlg()
         self.clicked.connect(self.buttonClicked)
       
     def initialize(self, myWindow: AbstractMyWindow):
         self._myWindow = myWindow
     
+    def finished(self):
+        self.setText("Compute")
+        self.setEnabled(True)
+        print("finished")
+        
     def buttonClicked(self, event: QMouseEvent):
         print("ComputeBtn: buttonClicked")
         self._computeStatsDlg.show()
         self._worker = Worker(self._myWindow,self._computeStatsDlg)
         self._worker.finished.connect(self._worker.deleteLater)
         self._thread = QThread()
         self._worker.finished.connect(self._thread.quit)
         self._worker.moveToThread(self._thread)
         self._thread.started.connect(self._worker.run)
         self._thread.finished.connect(self._thread.deleteLater)
-        self._thread.finished.connect(
-            lambda: print("finished")
-        )
-        self._thread.finished.connect(
-            lambda: self.setText("Compute")
-        )
-        self._thread.finished.connect(
-            lambda: self.setEnabled(True)
-        )
+        self._thread.finished.connect(self.finished)
         self.setText("...")
         self.setEnabled(False)
         if isSingleThread():
             self._worker.run()
         else:
             self._thread.start()
```

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/fullimage.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/fullimage.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/minimap.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/minimap.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/properties.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/properties.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/helper/tree.py` & `silicon_analyser-1.0.8/silicon_analyser/helper/tree.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.8/silicon_analyser/main_window.ui`

 * *Files 4% similar despite different names*

#### Comparing `silicon_analyser-1.0.7/silicon_analyser/main_window.ui` & `silicon_analyser-1.0.8/silicon_analyser/main_window.ui`

```diff
@@ -146,15 +146,23 @@
         <property name="title">
           <string>Info</string>
         </property>
         <addaction name="_actionMade_by_TheCrazyT"/>
         <addaction name="_actionUrl"/>
         <addaction name="separator"/>
       </widget>
+      <widget class="QMenu" name="menuComputation_method">
+        <property name="title">
+          <string>Computation method</string>
+        </property>
+        <addaction name="_actionDecisionTree"/>
+        <addaction name="_actionNeuralNetwork"/>
+      </widget>
       <addaction name="menuInfo"/>
+      <addaction name="menuComputation_method"/>
     </widget>
     <action name="_actionGridAddRowTop">
       <property name="text">
         <string>Add row to top</string>
       </property>
       <property name="toolTip">
         <string>Add row to top</string>
@@ -213,14 +221,36 @@
       </property>
     </action>
     <action name="_actionExportCellsToImages">
       <property name="text">
         <string>Export cells to images</string>
       </property>
     </action>
+    <action name="_actionDecisionTree">
+      <property name="checkable">
+        <bool>true</bool>
+      </property>
+      <property name="checked">
+        <bool>false</bool>
+      </property>
+      <property name="text">
+        <string>Decision Tree</string>
+      </property>
+    </action>
+    <action name="_actionNeuralNetwork">
+      <property name="checkable">
+        <bool>true</bool>
+      </property>
+      <property name="checked">
+        <bool>true</bool>
+      </property>
+      <property name="text">
+        <string>Neural network</string>
+      </property>
+    </action>
   </widget>
   <customwidgets>
     <customwidget>
       <class>ComputeBtn</class>
       <extends>QPushButton</extends>
       <header>silicon_analyser.helper.computebtn</header>
     </customwidget>
```

### Comparing `silicon_analyser-1.0.7/silicon_analyser/mywindow.py` & `silicon_analyser-1.0.8/silicon_analyser/mywindow.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,17 @@
     _actionRemoveGrid: QAction
     _actionRemoveLabel: QAction
     _actionMade_by_TheCrazyT: QAction
     _actionUrl: QAction
     _actionSaveAsCsv: QAction
     _actionViewAsPixelimage: QAction
     _actionExportCellsToImages: QAction
+    _actionDecisionTree: QAction
+    _actionNeuralNetwork: QAction
+
     autosave: bool
     menuBar: QMenu
     
     def __init__(self):
         AbstractMyWindow.__init__(self)
         path: str = p.abspath(p.join(p.dirname(__file__), '.')) + '/main_window.ui'
         uic.loadUi(path, self)
@@ -92,14 +95,17 @@
         addLabelBtn.initialize(self)
         minimap.initialize(self, self._pixmap)
         image.initialize(self, self._pixmap)
         
         computeBtn.setDisabled(True)
         addLabelBtn.setDisabled(True)
         tree.evtTreeSelectionChanged.connect(self.treeSelectionChanged)
+
+        self._actionDecisionTree.triggered.connect(self.decisionTreeChecked)
+        self._actionNeuralNetwork.triggered.connect(self.neuralNetworkChecked)
         
         self._posX = 0
         self._posY = 0
         
         self._scale = 1.0
         self.drawImgAndMinimap()
         
@@ -131,14 +137,23 @@
         
         menuBar: QMenu = self.menuBar    
 
         version = importlib.metadata.version("silicon-analyser")
         action = menuBar.addAction(f"Version: {version}")
         action.triggered.connect(self.openMainUrl)
         
+
+    def decisionTreeChecked(self):
+        if(self._actionDecisionTree.isChecked()):
+            self._actionNeuralNetwork.setChecked(False)
+
+    def neuralNetworkChecked(self):
+        if(self._actionNeuralNetwork.isChecked()):
+            self._actionDecisionTree.setChecked(False)
+        
     def treeSelectionChanged(self, selection: QItemSelection):
         tree: Tree = self._tree
         selectedType: str|None = tree.selectedType()
         computeBtn: ComputeBtn = self._computeBtn
         addLabelBtn: AddLabelBtn = self._addLabelBtn
         if((selectedType == TreeItem.TYPE_GRID_ITEM)
            or (selectedType == TreeItem.TYPE_GRID)
```

### Comparing `silicon_analyser-1.0.7/silicon_analyser/savefiles.py` & `silicon_analyser-1.0.8/silicon_analyser/savefiles.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser/treeitem.py` & `silicon_analyser-1.0.8/silicon_analyser/treeitem.py`

 * *Files identical despite different names*

### Comparing `silicon_analyser-1.0.7/silicon_analyser.egg-info/PKG-INFO` & `silicon_analyser-1.0.8/silicon_analyser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silicon-analyser
-Version: 1.0.7
+Version: 1.0.8
 Summary: helps to analyse integrated circuit die images (for example from siliconpr0n.org) with the help of ai.
 Author-email: CrazyT <crazyt2019+sa@gmail.com>
 Project-URL: Homepage, https://github.com/TheCrazyT/SiliconAnalyser
 Project-URL: Bug Tracker, https://github.com/TheCrazyT/SiliconAnalyser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `silicon_analyser-1.0.7/silicon_analyser.egg-info/SOURCES.txt` & `silicon_analyser-1.0.8/silicon_analyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

