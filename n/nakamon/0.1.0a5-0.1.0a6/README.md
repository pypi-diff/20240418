# Comparing `tmp/nakamon-0.1.0a5.tar.gz` & `tmp/nakamon-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nakamon-0.1.0a5.tar", max compression
+gzip compressed data, was "nakamon-0.1.0a6.tar", max compression
```

## Comparing `nakamon-0.1.0a5.tar` & `nakamon-0.1.0a6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a5/README.md
--rw-r--r--   0        0        0   445554 2024-04-08 04:27:44.869120 nakamon-0.1.0a5/data/nakamon_status.csv
--rw-r--r--   0        0        0    13822 2024-04-09 04:15:52.083469 nakamon-0.1.0a5/data/orange_skill.csv
--rw-r--r--   0        0        0     8449 2024-04-05 00:15:11.226076 nakamon-0.1.0a5/data/red_skill.csv
--rw-r--r--   0        0        0     4474 2024-04-09 04:11:06.526795 nakamon-0.1.0a5/data/resistance_skill.csv
--rw-r--r--   0        0        0     5578 2024-04-08 04:44:28.569145 nakamon-0.1.0a5/data/resistance_status.csv
--rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a5/nakamon/__init__.py
--rw-r--r--   0        0        0     7648 2024-04-10 05:58:17.894293 nakamon-0.1.0a5/nakamon/damage.py
--rw-r--r--   0        0        0     5371 2024-04-11 03:24:50.237880 nakamon-0.1.0a5/nakamon/nakamon.py
--rw-r--r--   0        0        0      404 2024-04-12 06:04:48.131713 nakamon-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-09 03:43:26.006745 nakamon-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     7963 2024-04-10 04:51:49.510966 nakamon-0.1.0a6/README.md
+-rw-r--r--   0        0        0   445554 2024-04-08 04:27:44.869120 nakamon-0.1.0a6/data/nakamon_status.csv
+-rw-r--r--   0        0        0    13822 2024-04-09 04:15:52.083469 nakamon-0.1.0a6/data/orange_skill.csv
+-rw-r--r--   0        0        0     8607 2024-04-16 00:18:34.361048 nakamon-0.1.0a6/data/red_skill.csv
+-rw-r--r--   0        0        0     4474 2024-04-09 04:11:06.526795 nakamon-0.1.0a6/data/resistance_skill.csv
+-rw-r--r--   0        0        0     5578 2024-04-08 04:44:28.569145 nakamon-0.1.0a6/data/resistance_status.csv
+-rw-r--r--   0        0        0       58 2024-04-03 04:34:50.390579 nakamon-0.1.0a6/nakamon/__init__.py
+-rw-r--r--   0        0        0     7648 2024-04-10 05:58:17.894293 nakamon-0.1.0a6/nakamon/damage.py
+-rw-r--r--   0        0        0     5403 2024-04-16 00:25:05.884388 nakamon-0.1.0a6/nakamon/nakamon.py
+-rw-r--r--   0        0        0      404 2024-04-18 01:25:42.419022 nakamon-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0     8302 1970-01-01 00:00:00.000000 nakamon-0.1.0a6/PKG-INFO
```

### Comparing `nakamon-0.1.0a5/LICENSE` & `nakamon-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/README.md` & `nakamon-0.1.0a6/README.md`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/data/nakamon_status.csv` & `nakamon-0.1.0a6/data/nakamon_status.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/data/orange_skill.csv` & `nakamon-0.1.0a6/data/orange_skill.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/data/red_skill.csv` & `nakamon-0.1.0a6/data/red_skill.csv`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,19 @@
 撃・怪人系:C,0.06
 撃・怪人系:D,0.03
 撃・植物系:S,0.2
 撃・植物系:A,0.14
 撃・植物系:B,0.1
 撃・植物系:C,0.06
 撃・植物系:D,0.03
+撃・エレメント系:S,0.2
+撃・エレメント系:A,0.14
+撃・エレメント系:B,0.1
+撃・エレメント系:C,0.06
+撃・エレメント系:D,0.03
 転び成功率:S,0.3
 転び成功率:A,0.21
 転び成功率:B,0.14
 転び成功率:C,0.08
 転び成功率:D,0.04
 バギ・ブレス:S,0.15
 バギ・ブレス:A,0.1
```

### Comparing `nakamon-0.1.0a5/data/resistance_skill.csv` & `nakamon-0.1.0a6/data/resistance_skill.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/data/resistance_status.csv` & `nakamon-0.1.0a6/data/resistance_status.csv`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/nakamon/damage.py` & `nakamon-0.1.0a6/nakamon/damage.py`

 * *Files identical despite different names*

### Comparing `nakamon-0.1.0a5/nakamon/nakamon.py` & `nakamon-0.1.0a6/nakamon/nakamon.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     "撃・スライム系",
     "撃・ゾンビ系",
     "撃・悪魔系",
     "撃・ドラゴン系",
     "撃・怪人系",
     "撃・植物系",
     "撃・虫系",
+    "撃・エレメント系",
     "撃・⁇⁇系",
 ]
 probability_rates = [
     "会心率",
     "暴走率",
     "ガード率",
     "みかわし率",
```

### Comparing `nakamon-0.1.0a5/PKG-INFO` & `nakamon-0.1.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nakamon
-Version: 0.1.0a5
+Version: 0.1.0a6
 Summary: 
 Author: driller
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
```

