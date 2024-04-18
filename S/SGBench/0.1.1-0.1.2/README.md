# Comparing `tmp/sgbench-0.1.1.tar.gz` & `tmp/sgbench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgbench-0.1.1.tar", max compression
+gzip compressed data, was "sgbench-0.1.2.tar", max compression
```

## Comparing `sgbench-0.1.1.tar` & `sgbench-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0       10 2024-04-15 14:31:09.731281 sgbench-0.1.1/README.md
--rw-r--r--   0        0        0      423 2024-04-15 14:47:15.117658 sgbench-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-15 14:47:21.176617 sgbench-0.1.1/sgbench/__init__.py
--rw-r--r--   0        0        0     2352 2024-04-15 14:35:13.985912 sgbench-0.1.1/sgbench/pred.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 sgbench-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-18 09:28:26.558772 sgbench-0.1.2/LICENSE
+-rw-r--r--   0        0        0      986 2024-04-18 09:27:38.525890 sgbench-0.1.2/README.md
+-rw-r--r--   0        0        0      423 2024-04-16 11:04:52.950991 sgbench-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-16 11:04:48.243744 sgbench-0.1.2/sgbench/__init__.py
+-rw-r--r--   0        0        0     1822 2024-04-16 11:06:41.531241 sgbench-0.1.2/sgbench/__main__.py
+-rw-r--r--   0        0        0     3288 2024-04-18 09:05:16.240281 sgbench-0.1.2/sgbench/match.py
+-rw-r--r--   0        0        0     2098 2024-04-18 09:07:00.851807 sgbench-0.1.2/sgbench/pred.py
+-rw-r--r--   0        0        0     9830 2024-04-16 11:10:01.242474 sgbench-0.1.2/sgbench/sg_eval.py
+-rw-r--r--   0        0        0      221 2024-04-16 11:06:22.780476 sgbench-0.1.2/sgbench/utils.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 sgbench-0.1.2/PKG-INFO
```

### Comparing `sgbench-0.1.1/sgbench/pred.py` & `sgbench-0.1.2/sgbench/pred.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,27 +32,25 @@
     for img in pred_data["images"]:
         img_id = img["id"]
 
         if len(img["triplets"]) == 0:
             triplets = np.empty((0, 3), dtype=int)
         else:
             triplets = deduplicate(np.array(img["triplets"]))
-        # TODO: remove these hard-coded assertions
-        assert (triplets[:, 2] >= 0).all() and (triplets[:, 2] < 56).all()
+        assert (triplets[:, 2] >= 0).all()
 
         if (
             "ng_triplets" not in img
             or img["ng_triplets"] is None
             or len(img["ng_triplets"]) == 0
         ):
             ng_triplets = np.empty((0, 3), dtype=int)
         else:
             ng_triplets = deduplicate(np.array(img["ng_triplets"]))
-        # TODO: remove these hard-coded assertions
-        assert (ng_triplets[:, 2] >= 0).all() and (ng_triplets[:, 2] < 56).all()
+        assert (ng_triplets[:, 2] >= 0).all()
 
         seg_ids = []
         cats = []
         bboxes = []
 
         for s in img["annotation"]:
             if "seg_id" in s:
@@ -61,17 +59,15 @@
             bboxes.append(s["bbox"])
 
         if seg_ids:
             seg_ids = np.array(seg_ids)
         else:
             seg_ids = None
         cats = np.array(cats)
-        # TODO: remove these hard-coded assertions
         assert (cats >= 0).all()
-        assert (cats < 133).all()
         bboxes = np.array(bboxes)
 
         imgs[img_id] = PredImg(
             id=img_id,
             triplets=triplets,
             ng_triplets=ng_triplets,
             seg_ids=seg_ids,
```

