# Comparing `tmp/ssl_framework-0.2.1.tar.gz` & `tmp/ssl_framework-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssl_framework-0.2.1.tar", last modified: Mon Apr 15 19:47:31 2024, max compression
+gzip compressed data, was "ssl_framework-0.2.2.tar", last modified: Wed Apr 17 20:03:39 2024, max compression
```

## Comparing `ssl_framework-0.2.1.tar` & `ssl_framework-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-15 19:47:31.808786 ssl_framework-0.2.1/
--rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-04-01 02:04:29.000000 ssl_framework-0.2.1/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      741 2024-04-15 19:47:31.808786 ssl_framework-0.2.1/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 02:05:00.000000 ssl_framework-0.2.1/README.md
--rw-r--r--   0 carl      (1000) carl      (1000)     1008 2024-04-15 19:47:11.000000 ssl_framework-0.2.1/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-15 19:47:31.808786 ssl_framework-0.2.1/setup.cfg
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-15 19:47:31.805453 ssl_framework-0.2.1/ssl_framework/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 12:00:19.000000 ssl_framework-0.2.1/ssl_framework/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     8347 2024-04-04 15:45:05.000000 ssl_framework-0.2.1/ssl_framework/byol.py
--rw-r--r--   0 carl      (1000) carl      (1000)     8347 2024-04-04 15:20:29.000000 ssl_framework-0.2.1/ssl_framework/simclr.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-15 19:47:31.808786 ssl_framework-0.2.1/ssl_framework.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      741 2024-04-15 19:47:31.000000 ssl_framework-0.2.1/ssl_framework.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      288 2024-04-15 19:47:31.000000 ssl_framework-0.2.1/ssl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-15 19:47:31.000000 ssl_framework-0.2.1/ssl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-15 19:47:31.000000 ssl_framework-0.2.1/ssl_framework.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       27 2024-04-15 19:47:31.000000 ssl_framework-0.2.1/ssl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:03:39.426990 ssl_framework-0.2.2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1072 2024-04-01 02:04:29.000000 ssl_framework-0.2.2/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      741 2024-04-17 20:03:39.426990 ssl_framework-0.2.2/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 02:05:00.000000 ssl_framework-0.2.2/README.md
+-rw-r--r--   0 carl      (1000) carl      (1000)     1008 2024-04-17 20:02:16.000000 ssl_framework-0.2.2/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-17 20:03:39.426990 ssl_framework-0.2.2/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:03:39.423656 ssl_framework-0.2.2/ssl_framework/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-01 12:00:19.000000 ssl_framework-0.2.2/ssl_framework/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     8347 2024-04-04 15:45:05.000000 ssl_framework-0.2.2/ssl_framework/byol.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     8791 2024-04-17 20:02:04.000000 ssl_framework-0.2.2/ssl_framework/simclr.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-17 20:03:39.426990 ssl_framework-0.2.2/ssl_framework.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      741 2024-04-17 20:03:39.000000 ssl_framework-0.2.2/ssl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      288 2024-04-17 20:03:39.000000 ssl_framework-0.2.2/ssl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-17 20:03:39.000000 ssl_framework-0.2.2/ssl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       33 2024-04-17 20:03:39.000000 ssl_framework-0.2.2/ssl_framework.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       27 2024-04-17 20:03:39.000000 ssl_framework-0.2.2/ssl_framework.egg-info/top_level.txt
```

### Comparing `ssl_framework-0.2.1/LICENSE` & `ssl_framework-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ssl_framework-0.2.1/PKG-INFO` & `ssl_framework-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl_framework
-Version: 0.2.1
+Version: 0.2.2
 Summary: A framework for training self supervized learning models in PyTorch. It makes it easy to train an SSL model from scratch, on top of a pre-trained model, or add it to an existing code base.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ssl_framework
 Project-URL: Issues, https://github.com/carlschader/ssl_framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ssl_framework-0.2.1/pyproject.toml` & `ssl_framework-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssl_framework"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "A framework for training self supervized learning models in PyTorch. It makes it easy to train an SSL model from scratch, on top of a pre-trained model, or add it to an existing code base."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ssl_framework-0.2.1/ssl_framework/byol.py` & `ssl_framework-0.2.2/ssl_framework/byol.py`

 * *Files identical despite different names*

### Comparing `ssl_framework-0.2.1/ssl_framework/simclr.py` & `ssl_framework-0.2.2/ssl_framework/simclr.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,30 @@
     color_jitter = transforms.ColorJitter(0.8*s, 0.8*s, 0.8*s, 0.2*s)
     rnd_color_jitter = transforms.RandomApply([color_jitter], p=0.8)
     rnd_gray = transforms.RandomGrayscale(p=0.2)
     color_distort = transforms.Compose([rnd_color_jitter, rnd_gray])
     return color_distort
 
 def NT_Xent(batch1, batch2, temp=0.1):
-    batch_size = batch1.size(0)
-    x = torch.cat([batch1, batch2], dim=0)
-    x = x / x.norm(dim=1)[:, None]
-    x = torch.mm(x, x.t())
-    x = torch.exp(x / temp)
-    sums = x.sum(dim=0)
-    x = torch.cat((torch.diagonal(x, offset=batch_size, dim1=1, dim2=0), torch.diagonal(x, offset=batch_size, dim1=0, dim2=1)))
-    return -torch.log((x / (sums-x))).mean()
+    # batch_size = batch1.size(0)
+    # x = torch.cat([batch1, batch2], dim=0)
+    # x = x / x.norm(dim=1)[:, None]
+    # x = torch.mm(x, x.t())
+    # x = torch.exp(x / temp)
+    # sums = x.sum(dim=0)
+    # x = torch.cat((torch.diagonal(x, offset=batch_size, dim1=1, dim2=0), torch.diagonal(x, offset=batch_size, dim1=0, dim2=1)))
+    # return -torch.log((x / (sums-x))).mean()
+    
+    batch1 = batch1 / torch.norm(batch1, dim=1, keepdim=True)
+    batch2 = batch2 / torch.norm(batch2, dim=1, keepdim=True)
+    sim_matrix = torch.mm(batch1, batch2.t()) / temp
+    sim_matrix = sim_matrix - torch.max(sim_matrix, dim=1, keepdim=True)[0]
+    sim_matrix = torch.exp(sim_matrix)
+    sim_matrix = sim_matrix / torch.sum(sim_matrix, dim=1, keepdim=True)
+    return -torch.mean(torch.log(torch.diag(sim_matrix)))
 
 def simCLR_train_iteration(model, train_loader, projector, augment, optimizer, scheduler, criterion=NT_Xent, logger=None, device=DETECTED_DEVICE, gradient_clip=None):
     model.train()
     total_loss = 0
     batches = len(train_loader)
     for batch_idx, (batch, _) in enumerate(train_loader):
         optimizer.zero_grad()
```

### Comparing `ssl_framework-0.2.1/ssl_framework.egg-info/PKG-INFO` & `ssl_framework-0.2.2/ssl_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssl_framework
-Version: 0.2.1
+Version: 0.2.2
 Summary: A framework for training self supervized learning models in PyTorch. It makes it easy to train an SSL model from scratch, on top of a pre-trained model, or add it to an existing code base.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/ssl_framework
 Project-URL: Issues, https://github.com/carlschader/ssl_framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

