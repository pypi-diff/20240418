# Comparing `tmp/scdecipher-0.1.0.tar.gz` & `tmp/scdecipher-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdecipher-0.1.0.tar", max compression
+gzip compressed data, was "scdecipher-0.1.2.tar", max compression
```

## Comparing `scdecipher-0.1.0.tar` & `scdecipher-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,59 @@
--rw-r--r--   0        0        0      567 2023-11-13 16:21:53.826785 scdecipher-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2023-11-13 20:49:25.719024 scdecipher-0.1.0/decipher/.DS_Store
--rw-r--r--   0        0        0       51 2023-11-13 16:21:53.827012 scdecipher-0.1.0/decipher/__init__.py
--rw-r--r--   0        0        0      290 2023-11-13 16:21:53.827235 scdecipher-0.1.0/decipher/plot/__init__.py
--rw-r--r--   0        0        0      647 2023-11-13 18:32:22.241657 scdecipher-0.1.0/decipher/plot/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6468 2023-11-13 18:32:25.886805 scdecipher-0.1.0/decipher/plot/__pycache__/basis_decomposition.cpython-311.pyc
--rw-r--r--   0        0        0     6574 2023-11-13 18:32:25.885273 scdecipher-0.1.0/decipher/plot/__pycache__/decipher.cpython-311.pyc
--rw-r--r--   0        0        0    12389 2023-11-13 18:32:22.244591 scdecipher-0.1.0/decipher/plot/__pycache__/trajectory_inference.cpython-311.pyc
--rw-r--r--   0        0        0      964 2023-11-13 18:32:22.242461 scdecipher-0.1.0/decipher/plot/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     3773 2023-11-13 16:21:53.827397 scdecipher-0.1.0/decipher/plot/basis_decomposition.py
--rw-r--r--   0        0        0     4704 2023-11-13 16:21:53.827557 scdecipher-0.1.0/decipher/plot/decipher.py
--rw-r--r--   0        0        0     9092 2023-11-13 16:21:53.827760 scdecipher-0.1.0/decipher/plot/trajectory_inference.py
--rw-r--r--   0        0        0      541 2023-11-13 16:21:53.827906 scdecipher-0.1.0/decipher/plot/utils.py
--rw-r--r--   0        0        0     6148 2023-11-13 20:49:25.718381 scdecipher-0.1.0/decipher/tools/.DS_Store
--rw-r--r--   0        0        0      506 2023-11-13 21:43:40.420443 scdecipher-0.1.0/decipher/tools/__init__.py
--rw-r--r--   0        0        0      906 2023-11-13 21:44:41.149684 scdecipher-0.1.0/decipher/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12504 2023-11-13 21:07:46.327125 scdecipher-0.1.0/decipher/tools/__pycache__/basis_decomposition.cpython-311.pyc
--rw-r--r--   0        0        0    18809 2023-11-13 21:42:19.535509 scdecipher-0.1.0/decipher/tools/__pycache__/decipher.cpython-311.pyc
--rw-r--r--   0        0        0    23289 2023-11-13 17:29:14.536894 scdecipher-0.1.0/decipher/tools/__pycache__/trajectory_inference.cpython-311.pyc
--rw-r--r--   0        0        0     1988 2023-11-13 18:32:22.238248 scdecipher-0.1.0/decipher/tools/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-11-13 16:21:53.828253 scdecipher-0.1.0/decipher/tools/_basis_decomposition/__init__.py
--rw-r--r--   0        0        0      194 2023-11-13 18:32:22.231340 scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2522 2023-11-13 18:32:22.232475 scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/inference.cpython-311.pyc
--rw-r--r--   0        0        0     9659 2023-11-13 18:32:22.236468 scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     5991 2023-11-13 18:32:22.234522 scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/run.cpython-311.pyc
--rw-r--r--   0        0        0     1456 2023-11-13 16:21:53.828420 scdecipher-0.1.0/decipher/tools/_basis_decomposition/inference.py
--rw-r--r--   0        0        0     4219 2023-11-13 16:21:53.828589 scdecipher-0.1.0/decipher/tools/_basis_decomposition/model.py
--rw-r--r--   0        0        0     3880 2023-11-13 16:21:53.828730 scdecipher-0.1.0/decipher/tools/_basis_decomposition/run.py
--rw-r--r--   0        0        0      106 2023-11-13 16:21:53.828920 scdecipher-0.1.0/decipher/tools/_decipher/__init__.py
--rw-r--r--   0        0        0      369 2023-11-13 18:26:47.133233 scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5681 2023-11-13 18:31:06.079682 scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/data.cpython-311.pyc
--rw-r--r--   0        0        0    12243 2023-11-13 18:26:47.135181 scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/decipher.cpython-311.pyc
--rw-r--r--   0        0        0     6265 2023-11-13 18:31:06.077606 scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     3280 2023-11-13 16:21:53.829074 scdecipher-0.1.0/decipher/tools/_decipher/data.py
--rw-r--r--   0        0        0     6399 2023-11-13 16:21:53.829229 scdecipher-0.1.0/decipher/tools/_decipher/decipher.py
--rw-r--r--   0        0        0     3793 2023-11-13 16:21:53.829388 scdecipher-0.1.0/decipher/tools/_decipher/module.py
--rw-r--r--   0        0        0     9203 2023-11-13 21:07:41.406385 scdecipher-0.1.0/decipher/tools/basis_decomposition.py
--rw-r--r--   0        0        0    12845 2023-11-13 21:41:54.988060 scdecipher-0.1.0/decipher/tools/decipher.py
--rw-r--r--   0        0        0    19292 2023-11-13 16:21:53.829947 scdecipher-0.1.0/decipher/tools/trajectory_inference.py
--rw-r--r--   0        0        0     1282 2023-11-13 16:21:53.830104 scdecipher-0.1.0/decipher/tools/utils.py
--rw-r--r--   0        0        0     2462 2023-11-13 16:21:53.830245 scdecipher-0.1.0/decipher/utils.py
--rw-r--r--   0        0        0      660 2023-11-15 21:55:24.176432 scdecipher-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1554 1970-01-01 00:00:00.000000 scdecipher-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1747 2024-04-18 13:35:02.281842 scdecipher-0.1.2/README.md
+-rw-r--r--   0        0        0       75 2024-04-18 13:43:19.081971 scdecipher-0.1.2/decipher/__init__.py
+-rw-r--r--   0        0        0      545 2024-04-18 13:43:40.915794 scdecipher-0.1.2/decipher/plot/__init__.py
+-rw-r--r--   0        0        0      527 2024-03-27 00:09:30.862379 scdecipher-0.1.2/decipher/plot/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      736 2024-04-18 14:03:55.409541 scdecipher-0.1.2/decipher/plot/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3821 2024-03-27 00:09:32.992969 scdecipher-0.1.2/decipher/plot/__pycache__/basis_decomposition.cpython-310.pyc
+-rw-r--r--   0        0        0     6465 2024-04-18 14:03:55.473146 scdecipher-0.1.2/decipher/plot/__pycache__/basis_decomposition.cpython-311.pyc
+-rw-r--r--   0        0        0     4769 2024-03-27 00:09:32.992099 scdecipher-0.1.2/decipher/plot/__pycache__/decipher.cpython-310.pyc
+-rw-r--r--   0        0        0     6572 2024-04-18 14:03:55.471289 scdecipher-0.1.2/decipher/plot/__pycache__/decipher.cpython-311.pyc
+-rw-r--r--   0        0        0     7783 2024-03-27 00:09:30.863792 scdecipher-0.1.2/decipher/plot/__pycache__/trajectory_inference.cpython-310.pyc
+-rw-r--r--   0        0        0    12377 2024-04-18 14:03:55.410423 scdecipher-0.1.2/decipher/plot/__pycache__/trajectory_inference.cpython-311.pyc
+-rw-r--r--   0        0        0      761 2024-03-27 00:09:30.862759 scdecipher-0.1.2/decipher/plot/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0      964 2024-02-21 16:03:15.375082 scdecipher-0.1.2/decipher/plot/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0     3769 2024-04-18 13:41:09.437316 scdecipher-0.1.2/decipher/plot/basis_decomposition.py
+-rw-r--r--   0        0        0     4708 2024-04-18 13:41:09.439349 scdecipher-0.1.2/decipher/plot/decipher.py
+-rw-r--r--   0        0        0     9129 2024-04-18 13:41:34.500208 scdecipher-0.1.2/decipher/plot/trajectory_inference.py
+-rw-r--r--   0        0        0      541 2024-02-21 15:40:45.566186 scdecipher-0.1.2/decipher/plot/utils.py
+-rw-r--r--   0        0        0      839 2024-04-18 13:43:40.910334 scdecipher-0.1.2/decipher/tools/__init__.py
+-rw-r--r--   0        0        0      697 2024-03-27 00:09:30.705214 scdecipher-0.1.2/decipher/tools/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1010 2024-04-18 14:03:55.282605 scdecipher-0.1.2/decipher/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7994 2024-03-27 00:09:30.856892 scdecipher-0.1.2/decipher/tools/__pycache__/basis_decomposition.cpython-310.pyc
+-rw-r--r--   0        0        0    12496 2024-04-18 14:03:55.404874 scdecipher-0.1.2/decipher/tools/__pycache__/basis_decomposition.cpython-311.pyc
+-rw-r--r--   0        0        0    12475 2024-03-27 00:09:30.861685 scdecipher-0.1.2/decipher/tools/__pycache__/decipher.cpython-310.pyc
+-rw-r--r--   0        0        0    20927 2024-04-18 14:03:55.409224 scdecipher-0.1.2/decipher/tools/__pycache__/decipher.cpython-311.pyc
+-rw-r--r--   0        0        0    15374 2024-03-27 00:09:30.707864 scdecipher-0.1.2/decipher/tools/__pycache__/trajectory_inference.cpython-310.pyc
+-rw-r--r--   0        0        0    23291 2024-04-18 14:03:55.284381 scdecipher-0.1.2/decipher/tools/__pycache__/trajectory_inference.cpython-311.pyc
+-rw-r--r--   0        0        0     1606 2024-03-27 00:09:30.860247 scdecipher-0.1.2/decipher/tools/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     1988 2024-02-21 16:03:15.373215 scdecipher-0.1.2/decipher/tools/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2024-02-21 15:40:45.566413 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__init__.py
+-rw-r--r--   0        0        0      178 2024-03-27 00:09:30.857155 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      194 2024-02-21 16:03:15.371661 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1098 2024-03-27 00:09:30.857716 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/inference.cpython-310.pyc
+-rw-r--r--   0        0        0     2522 2024-04-18 14:03:55.405673 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/inference.cpython-311.pyc
+-rw-r--r--   0        0        0     4645 2024-03-27 00:09:30.859824 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/model.cpython-310.pyc
+-rw-r--r--   0        0        0     9613 2024-04-18 14:03:55.407188 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/model.cpython-311.pyc
+-rw-r--r--   0        0        0     3196 2024-03-27 00:09:30.858582 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0        0        0     5991 2024-04-18 14:03:55.406436 scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/run.cpython-311.pyc
+-rw-r--r--   0        0        0     1456 2024-04-18 13:37:49.084603 scdecipher-0.1.2/decipher/tools/_basis_decomposition/inference.py
+-rw-r--r--   0        0        0     4184 2024-04-18 13:39:46.976917 scdecipher-0.1.2/decipher/tools/_basis_decomposition/model.py
+-rw-r--r--   0        0        0     3878 2024-04-18 13:35:02.625658 scdecipher-0.1.2/decipher/tools/_basis_decomposition/run.py
+-rw-r--r--   0        0        0      194 2024-04-18 13:43:41.906141 scdecipher-0.1.2/decipher/tools/_decipher/__init__.py
+-rw-r--r--   0        0        0      311 2024-03-27 00:09:30.810833 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      417 2024-04-18 14:03:55.323721 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3389 2024-03-27 00:09:30.851728 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     6104 2024-04-18 14:03:55.401497 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/data.cpython-311.pyc
+-rw-r--r--   0        0        0     6368 2024-03-27 00:09:30.812200 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/decipher.cpython-310.pyc
+-rw-r--r--   0        0        0    12660 2024-04-18 14:03:55.325408 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/decipher.cpython-311.pyc
+-rw-r--r--   0        0        0     3395 2024-03-27 00:09:30.850267 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/module.cpython-310.pyc
+-rw-r--r--   0        0        0     6265 2024-04-18 14:03:55.399419 scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/module.cpython-311.pyc
+-rw-r--r--   0        0        0     3549 2024-04-18 13:37:49.109069 scdecipher-0.1.2/decipher/tools/_decipher/data.py
+-rw-r--r--   0        0        0     6596 2024-04-18 14:28:16.746230 scdecipher-0.1.2/decipher/tools/_decipher/decipher.py
+-rw-r--r--   0        0        0     3793 2024-04-18 13:37:49.106220 scdecipher-0.1.2/decipher/tools/_decipher/module.py
+-rw-r--r--   0        0        0     9211 2024-04-18 13:41:56.177829 scdecipher-0.1.2/decipher/tools/basis_decomposition.py
+-rw-r--r--   0        0        0    14325 2024-04-18 14:07:21.699947 scdecipher-0.1.2/decipher/tools/decipher.py
+-rw-r--r--   0        0        0    19329 2024-04-18 13:37:49.196375 scdecipher-0.1.2/decipher/tools/trajectory_inference.py
+-rw-r--r--   0        0        0     1282 2024-02-21 15:40:45.567731 scdecipher-0.1.2/decipher/tools/utils.py
+-rw-r--r--   0        0        0     2462 2024-02-21 15:40:45.567827 scdecipher-0.1.2/decipher/utils.py
+-rw-r--r--   0        0        0      664 2024-04-18 14:58:47.813499 scdecipher-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2694 1970-01-01 00:00:00.000000 scdecipher-0.1.2/PKG-INFO
```

### Comparing `scdecipher-0.1.0/decipher/plot/__pycache__/basis_decomposition.cpython-311.pyc` & `scdecipher-0.1.2/decipher/plot/__pycache__/basis_decomposition.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,18 +1,18 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 3773
+moddate:  0xf5222166 (Thu Apr 18 13:41:09 2024 UTC)
+files sz: 3769
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a01640064016c025a03640064026c046d055a0601
-      00640d640584015a07640664076c086d095a0a0100090009000900640e64
+      00640364046c076d085a090100640d640784015a0a090009000900640e64
       0984015a0b090009000900640f640c84015a0c64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (numpy)
                  8 STORE_NAME               1 (np)
@@ -25,53 +25,55 @@
      3          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               2 (('pyplot',))
                 22 IMPORT_NAME              4 (matplotlib)
                 24 IMPORT_FROM              5 (pyplot)
                 26 STORE_NAME               6 (plt)
                 28 POP_TOP
    
-     6          30 LOAD_CONST              13 ((None, (5, 2.5), 3, None))
-                32 LOAD_CONST               5 (<code object basis, file "/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py", line 6>)
-                34 MAKE_FUNCTION            1 (defaults)
-                36 STORE_NAME               7 (basis)
-   
-    46          38 LOAD_CONST               6 (1)
-                40 LOAD_CONST               7 (('gene_patterns',))
-                42 IMPORT_NAME              8 (trajectory_inference)
-                44 IMPORT_FROM              9 (gene_patterns)
-                46 STORE_NAME              10 (plot_gene_patterns)
-                48 POP_TOP
+     5          30 LOAD_CONST               3 (1)
+                32 LOAD_CONST               4 (('gene_patterns',))
+                34 IMPORT_NAME              7 (trajectory_inference)
+                36 IMPORT_FROM              8 (gene_patterns)
+                38 STORE_NAME               9 (plot_gene_patterns)
+                40 POP_TOP
+   
+     8          42 LOAD_CONST              13 ((None, (5, 2.5), 3, None))
+                44 LOAD_CONST               7 (<code object basis, file "/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py", line 8>)
+                46 MAKE_FUNCTION            1 (defaults)
+                48 STORE_NAME              10 (basis)
    
-    53          50 NOP
+    52          50 NOP
    
-    54          52 NOP
+    53          52 NOP
    
-    55          54 NOP
+    54          54 NOP
    
-    49          56 LOAD_CONST              14 ((None, None, (7, 2)))
-                58 LOAD_CONST               9 (<code object gene_patterns_decomposition, file "/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py", line 49>)
+    48          56 LOAD_CONST              14 ((None, None, (7, 2)))
+                58 LOAD_CONST               9 (<code object gene_patterns_decomposition, file "/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py", line 48>)
                 60 MAKE_FUNCTION            1 (defaults)
                 62 STORE_NAME              11 (gene_patterns_decomposition)
    
-    96          64 NOP
+    95          64 NOP
    
-    97          66 NOP
+    96          66 NOP
    
-    98          68 NOP
+    97          68 NOP
    
-    93          70 LOAD_CONST              15 ((None, 'shape', (3, 4)))
-                72 LOAD_CONST              12 (<code object disruption_scores, file "/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py", line 93>)
+    92          70 LOAD_CONST              15 ((None, 'shape', (3, 4)))
+                72 LOAD_CONST              12 (<code object disruption_scores, file "/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py", line 92>)
                 74 MAKE_FUNCTION            1 (defaults)
                 76 STORE_NAME              12 (disruption_scores)
                 78 LOAD_CONST               1 (None)
                 80 RETURN_VALUE
    consts
       0
       None
       ('pyplot',)
+      1
+      ('gene_patterns',)
       (5, 2.5)
       3
       code
          argcount  : 5
          nlocals   : 8
          stacksize : 8
          flags     : 3
@@ -88,124 +90,124 @@
             00640619000000000000000000a6010000ab01000000000000000044005d
             3b7d077c04a00900000000000000000000000000000000000000007c0564
             04640485027c076602190000000000000000007c0181087c017c07190000
             000000000000006e01640464077c0764067a0000007a0600007c037c0719
             000000000000000000ac08a6040000ab04000000000000000001008c3c7c
             04a00a00000000000000000000000000000000000000006409640a640bac
             0ca6030000ab03000000000000000001007c065300
-           6           0 RESUME                   0
+           8           0 RESUME                   0
          
-          27           2 LOAD_FAST                0 (adata)
+          29           2 LOAD_FAST                0 (adata)
                        4 LOAD_ATTR                0 (uns)
                       14 LOAD_CONST               1 ('decipher')
                       16 BINARY_SUBSCR
                       26 LOAD_CONST               2 ('basis_decomposition')
                       28 BINARY_SUBSCR
                       38 LOAD_CONST               3 ('basis')
                       40 BINARY_SUBSCR
                       50 STORE_FAST               5 (bases)
          
-          28          52 LOAD_FAST                4 (ax)
+          30          52 LOAD_FAST                4 (ax)
                       54 POP_JUMP_FORWARD_IF_NOT_NONE    42 (to 140)
          
-          29          56 LOAD_GLOBAL              3 (NULL + plt)
+          31          56 LOAD_GLOBAL              3 (NULL + plt)
                       68 LOAD_ATTR                2 (figure)
                       78 LOAD_FAST                2 (figsize)
                       80 KW_NAMES                 5
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               6 (fig)
          
-          30          98 LOAD_FAST                6 (fig)
+          32          98 LOAD_FAST                6 (fig)
                      100 LOAD_METHOD              3 (gca)
                      122 PRECALL                  0
                      126 CALL                     0
                      136 STORE_FAST               4 (ax)
                      138 JUMP_FORWARD             7 (to 154)
          
-          32     >>  140 LOAD_FAST                4 (ax)
+          34     >>  140 LOAD_FAST                4 (ax)
                      142 LOAD_ATTR                2 (figure)
                      152 STORE_FAST               6 (fig)
          
-          33     >>  154 LOAD_GLOBAL              9 (NULL + type)
+          35     >>  154 LOAD_GLOBAL              9 (NULL + type)
                      166 LOAD_FAST                3 (linewidth)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 LOAD_GLOBAL             10 (int)
                      194 LOAD_GLOBAL             12 (float)
                      206 BUILD_TUPLE              2
                      208 CONTAINS_OP              0
                      210 POP_JUMP_FORWARD_IF_FALSE    17 (to 246)
          
-          34         212 LOAD_FAST                3 (linewidth)
+          36         212 LOAD_FAST                3 (linewidth)
                      214 BUILD_LIST               1
                      216 LOAD_FAST                5 (bases)
                      218 LOAD_ATTR                7 (shape)
                      228 LOAD_CONST               6 (1)
                      230 BINARY_SUBSCR
                      240 BINARY_OP                5 (*)
                      244 STORE_FAST               3 (linewidth)
          
-          35     >>  246 LOAD_GLOBAL             17 (NULL + range)
+          37     >>  246 LOAD_GLOBAL             17 (NULL + range)
                      258 LOAD_FAST                5 (bases)
                      260 LOAD_ATTR                7 (shape)
                      270 LOAD_CONST               6 (1)
                      272 BINARY_SUBSCR
                      282 PRECALL                  1
                      286 CALL                     1
                      296 GET_ITER
                  >>  298 FOR_ITER                59 (to 418)
                      300 STORE_FAST               7 (i)
          
-          36         302 LOAD_FAST                4 (ax)
+          38         302 LOAD_FAST                4 (ax)
                      304 LOAD_METHOD              9 (plot)
          
-          37         326 LOAD_FAST                5 (bases)
+          39         326 LOAD_FAST                5 (bases)
                      328 LOAD_CONST               4 (None)
                      330 LOAD_CONST               4 (None)
                      332 BUILD_SLICE              2
                      334 LOAD_FAST                7 (i)
                      336 BUILD_TUPLE              2
                      338 BINARY_SUBSCR
          
-          38         348 LOAD_FAST                1 (colors)
+          40         348 LOAD_FAST                1 (colors)
                      350 POP_JUMP_FORWARD_IF_NONE     8 (to 368)
                      352 LOAD_FAST                1 (colors)
                      354 LOAD_FAST                7 (i)
                      356 BINARY_SUBSCR
                      366 JUMP_FORWARD             1 (to 370)
                  >>  368 LOAD_CONST               4 (None)
          
-          39     >>  370 LOAD_CONST               7 ('basis %d')
+          41     >>  370 LOAD_CONST               7 ('basis %d')
                      372 LOAD_FAST                7 (i)
                      374 LOAD_CONST               6 (1)
                      376 BINARY_OP                0 (+)
                      380 BINARY_OP                6 (%)
          
-          40         384 LOAD_FAST                3 (linewidth)
+          42         384 LOAD_FAST                3 (linewidth)
                      386 LOAD_FAST                7 (i)
                      388 BINARY_SUBSCR
          
-          36         398 KW_NAMES                 8
+          38         398 KW_NAMES                 8
                      400 PRECALL                  4
                      404 CALL                     4
                      414 POP_TOP
                      416 JUMP_BACKWARD           60 (to 298)
          
-          42     >>  418 LOAD_FAST                4 (ax)
+          44     >>  418 LOAD_FAST                4 (ax)
                      420 LOAD_METHOD             10 (legend)
                      442 LOAD_CONST               9 ('right')
                      444 LOAD_CONST              10 ((1.35, 0.5))
                      446 LOAD_CONST              11 (False)
                      448 KW_NAMES                12
                      450 PRECALL                  3
                      454 CALL                     3
                      464 POP_TOP
          
-          43         466 LOAD_FAST                6 (fig)
+          45         466 LOAD_FAST                6 (fig)
                      468 RETURN_VALUE
          consts
             'Plot the basis functions learned by the basis decomposition.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n    colors : list of str, optional\n        The colors to use for each basis.\n    figsize : tuple of float, default (5, 2.5)\n        The size of the figure.\n    linewidth : float or list of float, default 3\n        The width of the lines to plot.\n    ax : matplotlib.pyplot.Axes, optional\n        The axes on which to plot. If None, create a new figure and axes.\n\n    Returns\n    -------\n    fig : matplotlib.pyplot.Figure\n        The matplotlib figure.\n    '
             'decipher'
             'basis_decomposition'
             'basis'
             None
@@ -217,22 +219,20 @@
             (1.35, 0.5)
             False
             ('loc', 'bbox_to_anchor', 'fancybox')
          names      ('uns', 'plt', 'figure', 'gca', 'type', 'int', 'float', 'shape', 'range', 'plot', 'legend')
          varnames   ('adata', 'colors', 'figsize', 'linewidth', 'ax', 'bases', 'fig', 'i')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py'
          name       'basis'
-         firstlineno 6
+         firstlineno 8
          lnotab
             0x0215320104012a012a020e013a01220138011801160116010e010efc14
             063001
-      1
-      ('gene_patterns',)
       (7, 2)
       code
          argcount  : 6
          nlocals   : 14
          stacksize : 9
          flags     : 3
          code
@@ -268,52 +268,52 @@
             0000000000000001007c0da0100000000000000000000000000000000000
             000000640b6405a6020000ab02000000000000000001007c0da011000000
             000000000000000000000000000000000064158400741f00000000000000
             0000007c0ca6010000ab0100000000000000004400a6000000ab00000000
             00000000006416ac17a6020000ab02000000000000000001007c0a44005d
             177d0d7c0da01200000000000000000000000000000000000000006700a6
             010000ab01000000000000000001008c187c095300
-          49           0 RESUME                   0
+          48           0 RESUME                   0
          
-          57           2 LOAD_FAST                0 (adata)
+          56           2 LOAD_FAST                0 (adata)
                        4 LOAD_ATTR                0 (var_names)
                       14 LOAD_METHOD              1 (tolist)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_METHOD              2 (index)
                       72 LOAD_FAST                1 (gene_name)
                       74 PRECALL                  1
                       78 CALL                     1
                       88 STORE_FAST               6 (gene_id)
          
-          58          90 LOAD_FAST                0 (adata)
+          57          90 LOAD_FAST                0 (adata)
                       92 LOAD_ATTR                3 (uns)
                      102 LOAD_CONST               1 ('decipher')
                      104 BINARY_SUBSCR
                      114 LOAD_CONST               2 ('basis_decomposition')
                      116 BINARY_SUBSCR
                      126 LOAD_CONST               3 ('pattern_names')
                      128 BINARY_SUBSCR
                      138 LOAD_METHOD              2 (index)
                      160 LOAD_FAST                2 (pattern_name)
                      162 PRECALL                  1
                      166 CALL                     1
                      176 STORE_FAST               7 (pattern_id)
          
-          59         178 LOAD_FAST                0 (adata)
+          58         178 LOAD_FAST                0 (adata)
                      180 LOAD_ATTR                3 (uns)
                      190 LOAD_CONST               1 ('decipher')
                      192 BINARY_SUBSCR
                      202 LOAD_CONST               2 ('basis_decomposition')
                      204 BINARY_SUBSCR
                      214 LOAD_CONST               4 ('length')
                      216 BINARY_SUBSCR
                      226 STORE_FAST               8 (max_length)
          
-          60         228 LOAD_GLOBAL              9 (NULL + plt)
+          59         228 LOAD_GLOBAL              9 (NULL + plt)
                      240 LOAD_ATTR                5 (subplots)
                      250 LOAD_CONST               5 (1)
                      252 LOAD_CONST               6 (3)
                      254 LOAD_CONST               7 ('width_ratios')
                      256 BUILD_LIST               0
                      258 LOAD_CONST               8 ((3, 3, 1))
                      260 LIST_EXTEND              1
@@ -322,109 +322,109 @@
                      266 KW_NAMES                 9
                      268 PRECALL                  4
                      272 CALL                     4
                      282 UNPACK_SEQUENCE          2
                      286 STORE_FAST               9 (fig)
                      288 STORE_FAST              10 (axes)
          
-          62         290 LOAD_GLOBAL             13 (NULL + plot_gene_patterns)
+          61         290 LOAD_GLOBAL             13 (NULL + plot_gene_patterns)
          
-          63         302 LOAD_FAST                0 (adata)
+          62         302 LOAD_FAST                0 (adata)
          
-          64         304 LOAD_FAST                1 (gene_name)
+          63         304 LOAD_FAST                1 (gene_name)
          
-          65         306 LOAD_CONST              10 (False)
+          64         306 LOAD_CONST              10 (False)
          
-          66         308 LOAD_FAST               10 (axes)
+          65         308 LOAD_FAST               10 (axes)
                      310 LOAD_CONST              11 (0)
                      312 BINARY_SUBSCR
          
-          67         322 LOAD_FAST                3 (palette)
+          66         322 LOAD_FAST                3 (palette)
          
-          68         324 LOAD_FAST                2 (pattern_name)
+          67         324 LOAD_FAST                2 (pattern_name)
          
-          69         326 LOAD_FAST                8 (max_length)
+          68         326 LOAD_FAST                8 (max_length)
          
-          62         328 KW_NAMES                12
+          61         328 KW_NAMES                12
                      330 PRECALL                  7
                      334 CALL                     7
                      344 POP_TOP
          
-          72         346 LOAD_FAST                0 (adata)
+          71         346 LOAD_FAST                0 (adata)
                      348 LOAD_ATTR                3 (uns)
                      358 LOAD_CONST               1 ('decipher')
                      360 BINARY_SUBSCR
                      370 LOAD_CONST               2 ('basis_decomposition')
                      372 BINARY_SUBSCR
                      382 LOAD_CONST              13 ('betas')
                      384 BINARY_SUBSCR
                      394 LOAD_FAST                7 (pattern_id)
                      396 LOAD_FAST                6 (gene_id)
                      398 BUILD_TUPLE              2
                      400 BINARY_SUBSCR
                      410 STORE_FAST              11 (beta)
          
-          73         412 LOAD_FAST               11 (beta)
+          72         412 LOAD_FAST               11 (beta)
                      414 LOAD_ATTR                7 (shape)
                      424 LOAD_CONST              11 (0)
                      426 BINARY_SUBSCR
                      436 STORE_FAST              12 (n_basis)
          
-          74         438 LOAD_FAST                4 (basis_colors)
+          73         438 LOAD_FAST                4 (basis_colors)
                      440 POP_JUMP_FORWARD_IF_NOT_NONE    22 (to 486)
          
-          75         442 LOAD_GLOBAL             17 (NULL + sns)
+          74         442 LOAD_GLOBAL             17 (NULL + sns)
                      454 LOAD_ATTR                9 (color_palette)
                      464 LOAD_CONST              14 ('Accent')
                      466 LOAD_FAST               12 (n_basis)
                      468 KW_NAMES                15
                      470 PRECALL                  2
                      474 CALL                     2
                      484 STORE_FAST               4 (basis_colors)
          
-          76     >>  486 LOAD_GLOBAL             21 (NULL + basis)
+          75     >>  486 LOAD_GLOBAL             21 (NULL + basis)
                      498 LOAD_FAST                0 (adata)
                      500 LOAD_FAST                4 (basis_colors)
                      502 LOAD_FAST               11 (beta)
                      504 LOAD_CONST              16 (10)
                      506 BINARY_OP                5 (*)
                      510 LOAD_FAST               10 (axes)
                      512 LOAD_CONST               5 (1)
                      514 BINARY_SUBSCR
                      524 KW_NAMES                17
                      526 PRECALL                  4
                      530 CALL                     4
                      540 POP_TOP
          
-          77         542 LOAD_FAST               10 (axes)
+          76         542 LOAD_FAST               10 (axes)
                      544 LOAD_CONST               5 (1)
                      546 BINARY_SUBSCR
                      556 LOAD_METHOD             11 (set_yticks)
                      578 BUILD_LIST               0
                      580 PRECALL                  1
                      584 CALL                     1
                      594 POP_TOP
          
-          78         596 LOAD_FAST               10 (axes)
+          77         596 LOAD_FAST               10 (axes)
                      598 LOAD_CONST               5 (1)
                      600 BINARY_SUBSCR
                      610 LOAD_METHOD             12 (get_legend)
                      632 PRECALL                  0
                      636 CALL                     0
                      646 LOAD_METHOD             13 (remove)
                      668 PRECALL                  0
                      672 CALL                     0
                      682 POP_TOP
          
-          80         684 LOAD_FAST               10 (axes)
+          79         684 LOAD_FAST               10 (axes)
                      686 LOAD_CONST              18 (2)
                      688 BINARY_SUBSCR
                      698 STORE_FAST              13 (ax)
          
-          81         700 LOAD_FAST               13 (ax)
+          80         700 LOAD_FAST               13 (ax)
                      702 LOAD_METHOD             14 (barh)
                      724 LOAD_GLOBAL             31 (NULL + range)
                      736 LOAD_FAST               12 (n_basis)
                      738 PRECALL                  1
                      742 CALL                     1
                      752 LOAD_CONST               0 (None)
                      754 LOAD_CONST               0 (None)
@@ -434,68 +434,68 @@
                      770 LOAD_FAST               11 (beta)
                      772 LOAD_FAST                4 (basis_colors)
                      774 KW_NAMES                20
                      776 PRECALL                  3
                      780 CALL                     3
                      790 POP_TOP
          
-          83         792 LOAD_FAST               13 (ax)
+          82         792 LOAD_FAST               13 (ax)
                      794 LOAD_METHOD             11 (set_yticks)
                      816 LOAD_GLOBAL             31 (NULL + range)
                      828 LOAD_FAST               12 (n_basis)
                      830 PRECALL                  1
                      834 CALL                     1
                      844 LOAD_CONST               0 (None)
                      846 LOAD_CONST               0 (None)
                      848 LOAD_CONST              19 (-1)
                      850 BUILD_SLICE              3
                      852 BINARY_SUBSCR
                      862 PRECALL                  1
                      866 CALL                     1
                      876 POP_TOP
          
-          84         878 LOAD_FAST               13 (ax)
+          83         878 LOAD_FAST               13 (ax)
                      880 LOAD_METHOD             16 (set_xlim)
                      902 LOAD_CONST              11 (0)
                      904 LOAD_CONST               5 (1)
                      906 PRECALL                  2
                      910 CALL                     2
                      920 POP_TOP
          
-          85         922 LOAD_FAST               13 (ax)
+          84         922 LOAD_FAST               13 (ax)
                      924 LOAD_METHOD             17 (set_yticklabels)
-                     946 LOAD_CONST              21 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py", line 85>)
+                     946 LOAD_CONST              21 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py", line 84>)
                      948 MAKE_FUNCTION            0
                      950 LOAD_GLOBAL             31 (NULL + range)
                      962 LOAD_FAST               12 (n_basis)
                      964 PRECALL                  1
                      968 CALL                     1
                      978 GET_ITER
                      980 PRECALL                  0
                      984 CALL                     0
                      994 LOAD_CONST              22 (12)
                      996 KW_NAMES                23
                      998 PRECALL                  2
                     1002 CALL                     2
                     1012 POP_TOP
          
-          87        1014 LOAD_FAST               10 (axes)
+          86        1014 LOAD_FAST               10 (axes)
                     1016 GET_ITER
                  >> 1018 FOR_ITER                23 (to 1066)
                     1020 STORE_FAST              13 (ax)
          
-          88        1022 LOAD_FAST               13 (ax)
+          87        1022 LOAD_FAST               13 (ax)
                     1024 LOAD_METHOD             18 (set_xticks)
                     1046 BUILD_LIST               0
                     1048 PRECALL                  1
                     1052 CALL                     1
                     1062 POP_TOP
                     1064 JUMP_BACKWARD           24 (to 1018)
          
-          90     >> 1066 LOAD_FAST                9 (fig)
+          89     >> 1066 LOAD_FAST                9 (fig)
                     1068 RETURN_VALUE
          consts
             None
             'decipher'
             'basis_decomposition'
             'pattern_names'
             'length'
@@ -517,15 +517,15 @@
             ('y', 'width', 'color')
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code 0x970067007c005d077d0164007c017a06000091028c085300
-                85           0 RESUME                   0
+                84           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                 7 (to 22)
                              8 STORE_FAST               1 (i)
                             10 LOAD_CONST               0 ('$\\beta_%d$')
                             12 LOAD_FAST                1 (i)
                             14 BINARY_OP                6 (%)
@@ -534,27 +534,27 @@
                        >>   22 RETURN_VALUE
                consts
                   '$\\beta_%d$'
                names      ()
                varnames   ('.0', 'i')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py'
                name       '<listcomp>'
-               firstlineno 85
+               firstlineno 84
                lnotab 0x
             12
             ('fontsize',)
          names      ('var_names', 'tolist', 'index', 'uns', 'plt', 'subplots', 'plot_gene_patterns', 'shape', 'sns', 'color_palette', 'basis', 'set_yticks', 'get_legend', 'remove', 'barh', 'range', 'set_xlim', 'set_yticklabels', 'set_xticks')
          varnames   ('adata', 'gene_name', 'pattern_name', 'palette', 'basis_colors', 'figsize', 'gene_id', 'pattern_id', 'max_length', 'fig', 'axes', 'beta', 'n_basis', 'ax')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py'
          name       'gene_patterns_decomposition'
-         firstlineno 49
+         firstlineno 48
          lnotab
             0x02085801580132013e020c010201020102010e010201020102f9120a42
             011a0104012c0138013601580210015c0256012c015c0208012c02
       'shape'
       (3, 4)
       code
          argcount  : 5
@@ -580,144 +580,144 @@
             0000000000000000000000000000007c016415641664176418ac19a60500
             00ab05000000000000000001007c06640519000000000000000000a00800
             000000000000000000000000000000000000006400a6010000ab01000000
             0000000000010064005300
                        0 MAKE_CELL                0 (adata)
                        2 MAKE_CELL                3 (sort_by)
          
-          93           4 RESUME                   0
+          92           4 RESUME                   0
          
-         100           6 LOAD_DEREF               3 (sort_by)
+          99           6 LOAD_DEREF               3 (sort_by)
                        8 LOAD_CONST               1 (('shape', 'combined', 'scale'))
                       10 CONTAINS_OP              0
                       12 POP_JUMP_FORWARD_IF_FALSE    21 (to 56)
          
-         101          14 LOAD_GLOBAL              1 (NULL + sorted)
+         100          14 LOAD_GLOBAL              1 (NULL + sorted)
          
-         102          26 LOAD_FAST                1 (gene_names)
+         101          26 LOAD_FAST                1 (gene_names)
          
-         103          28 LOAD_CLOSURE             0 (adata)
+         102          28 LOAD_CLOSURE             0 (adata)
                       30 LOAD_CLOSURE             3 (sort_by)
                       32 BUILD_TUPLE              2
-                      34 LOAD_CONST               2 (<code object <lambda>, file "/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py", line 103>)
+                      34 LOAD_CONST               2 (<code object <lambda>, file "/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py", line 102>)
                       36 MAKE_FUNCTION            8 (closure)
          
-         101          38 KW_NAMES                 3
+         100          38 KW_NAMES                 3
                       40 PRECALL                  2
                       44 CALL                     2
                       54 STORE_FAST               1 (gene_names)
          
-         105     >>   56 LOAD_GLOBAL              3 (NULL + plt)
+         104     >>   56 LOAD_GLOBAL              3 (NULL + plt)
                       68 LOAD_ATTR                2 (subplots)
                       78 LOAD_CONST               4 (2)
                       80 LOAD_CONST               5 (1)
                       82 LOAD_FAST                4 (figsize)
                       84 LOAD_CONST               6 ('col')
                       86 KW_NAMES                 7
                       88 PRECALL                  4
                       92 CALL                     4
                      102 UNPACK_SEQUENCE          2
                      106 STORE_FAST               5 (fig)
                      108 STORE_FAST               6 (axs)
          
-         106         110 LOAD_GLOBAL              7 (NULL + zip)
+         105         110 LOAD_GLOBAL              7 (NULL + zip)
                      122 LOAD_FAST                6 (axs)
                      124 LOAD_CONST               8 ('shape')
                      126 LOAD_CONST               9 ('combined')
                      128 BUILD_LIST               2
                      130 PRECALL                  2
                      134 CALL                     2
                      144 GET_ITER
                  >>  146 FOR_ITER                55 (to 258)
                      148 UNPACK_SEQUENCE          2
                      152 STORE_FAST               7 (ax)
                      154 STORE_FAST               8 (col)
          
-         107         156 LOAD_GLOBAL              9 (NULL + sns)
+         106         156 LOAD_GLOBAL              9 (NULL + sns)
                      168 LOAD_ATTR                5 (boxplot)
          
-         108         178 LOAD_DEREF               0 (adata)
+         107         178 LOAD_DEREF               0 (adata)
                      180 LOAD_ATTR                6 (uns)
                      190 LOAD_CONST              10 ('decipher')
                      192 BINARY_SUBSCR
                      202 LOAD_CONST              11 ('disruption_scores_samples')
                      204 BINARY_SUBSCR
          
-         109         214 LOAD_CONST              12 ('gene')
+         108         214 LOAD_CONST              12 ('gene')
          
-         110         216 LOAD_FAST                8 (col)
+         109         216 LOAD_FAST                8 (col)
          
-         111         218 LOAD_FAST                1 (gene_names)
+         110         218 LOAD_FAST                1 (gene_names)
          
-         112         220 LOAD_FAST                2 (color_palette)
+         111         220 LOAD_FAST                2 (color_palette)
          
-         113         222 LOAD_CONST              13 ((0, 100))
+         112         222 LOAD_CONST              13 ((0, 100))
          
-         114         224 LOAD_CONST              14 ('lw')
+         113         224 LOAD_CONST              14 ('lw')
                      226 LOAD_CONST              15 (0)
                      228 BUILD_MAP                1
          
-         115         230 LOAD_CONST              14 ('lw')
+         114         230 LOAD_CONST              14 ('lw')
                      232 LOAD_CONST              15 (0)
                      234 BUILD_MAP                1
          
-         116         236 LOAD_FAST                7 (ax)
+         115         236 LOAD_FAST                7 (ax)
          
-         107         238 KW_NAMES                16
+         106         238 KW_NAMES                16
                      240 PRECALL                  9
                      244 CALL                     9
                      254 POP_TOP
                      256 JUMP_BACKWARD           56 (to 146)
          
-         118     >>  258 LOAD_FAST                6 (axs)
+         117     >>  258 LOAD_FAST                6 (axs)
                      260 LOAD_CONST              15 (0)
                      262 BINARY_SUBSCR
                      272 LOAD_METHOD              7 (set_ylabel)
                      294 LOAD_CONST              17 ('Shape disruption')
                      296 LOAD_CONST              18 (13)
                      298 KW_NAMES                19
                      300 PRECALL                  2
                      304 CALL                     2
                      314 POP_TOP
          
-         119         316 LOAD_FAST                6 (axs)
+         118         316 LOAD_FAST                6 (axs)
                      318 LOAD_CONST              15 (0)
                      320 BINARY_SUBSCR
                      330 LOAD_METHOD              8 (set_xlabel)
                      352 LOAD_CONST               0 (None)
                      354 PRECALL                  1
                      358 CALL                     1
                      368 POP_TOP
          
-         120         370 LOAD_FAST                6 (axs)
+         119         370 LOAD_FAST                6 (axs)
                      372 LOAD_CONST               5 (1)
                      374 BINARY_SUBSCR
                      384 LOAD_METHOD              7 (set_ylabel)
                      406 LOAD_CONST              20 ('Combined disruption')
                      408 LOAD_CONST              18 (13)
                      410 KW_NAMES                19
                      412 PRECALL                  2
                      416 CALL                     2
                      426 POP_TOP
          
-         121         428 LOAD_FAST                6 (axs)
+         120         428 LOAD_FAST                6 (axs)
                      430 LOAD_CONST               5 (1)
                      432 BINARY_SUBSCR
                      442 LOAD_METHOD              9 (set_xticklabels)
                      464 LOAD_FAST                1 (gene_names)
                      466 LOAD_CONST              21 (45)
                      468 LOAD_CONST              22 ('right')
                      470 LOAD_CONST              23 ('anchor')
                      472 LOAD_CONST              24 (10)
                      474 KW_NAMES                25
                      476 PRECALL                  5
                      480 CALL                     5
                      490 POP_TOP
          
-         122         492 LOAD_FAST                6 (axs)
+         121         492 LOAD_FAST                6 (axs)
                      494 LOAD_CONST               5 (1)
                      496 BINARY_SUBSCR
                      506 LOAD_METHOD              8 (set_xlabel)
                      528 LOAD_CONST               0 (None)
                      530 PRECALL                  1
                      534 CALL                     1
                      544 POP_TOP
@@ -734,15 +734,15 @@
                code
                   0x950297007401000000000000000000006a01000000000000000089016a
                   020000000000000000640119000000000000000000640219000000000000
                   0000006a0300000000000000007c008902660219000000000000000000a6
                   010000ab0100000000000000005300
                              0 COPY_FREE_VARS           2
                
-               103           2 RESUME                   0
+               102           2 RESUME                   0
                              4 LOAD_GLOBAL              1 (NULL + np)
                             16 LOAD_ATTR                1 (mean)
                             26 LOAD_DEREF               1 (adata)
                             28 LOAD_ATTR                2 (uns)
                             38 LOAD_CONST               1 ('decipher')
                             40 BINARY_SUBSCR
                             50 LOAD_CONST               2 ('disruption_scores')
@@ -759,17 +759,17 @@
                   None
                   'decipher'
                   'disruption_scores'
                names      ('np', 'mean', 'uns', 'loc')
                varnames   ('gn',)
                freevars   ('adata', 'sort_by')
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py'
                name       '<lambda>'
-               firstlineno 103
+               firstlineno 102
                lnotab 0x
             ('key',)
             2
             1
             'col'
             ('figsize', 'sharex')
             'shape'
@@ -790,24 +790,24 @@
             'anchor'
             10
             ('rotation', 'ha', 'rotation_mode', 'fontsize')
          names      ('sorted', 'plt', 'subplots', 'zip', 'sns', 'boxplot', 'uns', 'set_ylabel', 'set_xlabel', 'set_xticklabels')
          varnames   ('adata', 'gene_names', 'color_palette', 'sort_by', 'figsize', 'fig', 'axs', 'ax', 'col')
          freevars   ()
          cellvars   ('adata', 'sort_by')
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py'
          name       'disruption_scores'
-         firstlineno 93
+         firstlineno 92
          lnotab
             0x060708010c0102010afe120436012e0116012401020102010201020102
             010601060102f7140b3a0136013a014001
       (None, (5, 2.5), 3, None)
       (None, None, (7, 2))
       (None, 'shape', (3, 4))
-   names      ('numpy', 'np', 'seaborn', 'sns', 'matplotlib', 'pyplot', 'plt', 'basis', 'trajectory_inference', 'gene_patterns', 'plot_gene_patterns', 'gene_patterns_decomposition', 'disruption_scores')
+   names      ('numpy', 'np', 'seaborn', 'sns', 'matplotlib', 'pyplot', 'plt', 'trajectory_inference', 'gene_patterns', 'plot_gene_patterns', 'basis', 'gene_patterns_decomposition', 'disruption_scores')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/plot/basis_decomposition.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/plot/basis_decomposition.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080108010c0308280c070201020102fa082f0201020102fb
+   lnotab 0x00ff0201080108010c020c03082c0201020102fa082f0201020102fb
```

### Comparing `scdecipher-0.1.0/decipher/plot/__pycache__/decipher.cpython-311.pyc` & `scdecipher-0.1.2/decipher/plot/__pycache__/decipher.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 4704
+moddate:  0xf5222166 (Thu Apr 18 13:41:09 2024 UTC)
+files sz: 4708
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
       0x9700640064016c005a01640064016c025a03640064026c046d055a0601
@@ -32,15 +32,15 @@
      8          30 NOP
    
      9          32 NOP
    
     10          34 NOP
    
      6          36 LOAD_CONST              15 (('decipher_v', 'decipher_z', None))
-                38 LOAD_CONST               5 (<code object decipher_z, file "/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py", line 6>)
+                38 LOAD_CONST               5 (<code object decipher_z, file "/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py", line 6>)
                 40 MAKE_FUNCTION            1 (defaults)
                 42 STORE_NAME               7 (decipher_z)
    
     57          44 LOAD_CONST               1 (None)
    
     58          46 LOAD_CONST               1 (None)
    
@@ -56,19 +56,19 @@
    
     64          58 LOAD_CONST              10 ('Decipher 2')
    
     65          60 LOAD_CONST              11 ('arrow')
    
     66          62 LOAD_CONST              12 ((3.5, 3.5))
    
-    67          64 LOAD_CONST              13 (<code object <lambda>, file "/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py", line 67>)
+    67          64 LOAD_CONST              13 (<code object <lambda>, file "/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py", line 67>)
                 66 MAKE_FUNCTION            0
    
     55          68 BUILD_TUPLE             11
-                70 LOAD_CONST              14 (<code object decipher, file "/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py", line 55>)
+                70 LOAD_CONST              14 (<code object decipher, file "/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py", line 55>)
                 72 MAKE_FUNCTION            1 (defaults)
                 74 STORE_NAME               8 (decipher)
                 76 LOAD_CONST               1 (None)
                 78 RETURN_VALUE
    consts
       0
       None
@@ -152,25 +152,25 @@
          
           41         260 LOAD_FAST                0 (adata)
          
           40         262 BUILD_TUPLE              1
          
           42         264 LOAD_FAST                1 (basis)
          
-          43         266 LOAD_CONST               4 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py", line 43>)
+          43         266 LOAD_CONST               4 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py", line 43>)
                      268 MAKE_FUNCTION            0
                      270 LOAD_FAST                3 (subset_of_zs)
                      272 GET_ITER
                      274 PRECALL                  0
                      278 CALL                     0
          
-          44         288 LOAD_CONST               5 (<code object <lambda>, file "/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py", line 44>)
+          44         288 LOAD_CONST               5 (<code object <lambda>, file "/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py", line 44>)
                      290 MAKE_FUNCTION            0
          
-          45         292 LOAD_CONST               6 (<code object <lambda>, file "/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py", line 45>)
+          45         292 LOAD_CONST               6 (<code object <lambda>, file "/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py", line 45>)
                      294 MAKE_FUNCTION            0
          
           46         296 LOAD_CONST               7 ('cool_r')
          
           47         298 LOAD_CONST               8 (False)
          
           48         300 LOAD_CONST               8 (False)
@@ -212,15 +212,15 @@
                        >>   22 RETURN_VALUE
                consts
                   'z'
                names      ()
                varnames   ('.0', 'i')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
                name       '<listcomp>'
                firstlineno 43
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -239,15 +239,15 @@
                consts
                   None
                   0.99
                names      ('np', 'quantile')
                varnames   ('xs',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
                name       '<lambda>'
                firstlineno 44
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -266,27 +266,27 @@
                consts
                   None
                   0.01
                names      ('np', 'quantile')
                varnames   ('xs',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
                name       '<lambda>'
                firstlineno 45
                lnotab 0x
             'cool_r'
             False
             True
             ('basis', 'color', 'vmax', 'vmin', 'color_map', 'frameon', 'show', 'sort_order', 'return_fig')
          names      ('obsm', 'shape', 'range', 'obs', 'list', 'sc', 'pl', 'embedding')
          varnames   ('adata', 'basis', 'decipher_z_key', 'subset_of_zs', 'kwargs', 'dim_z', 'i')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
          name       'decipher_z'
          firstlineno 6
          lnotab
             0x021b300122014c0204014002200102ff02020201160104010401020102
             010201020102f6040b02f5
       2
       1.0
@@ -323,15 +323,15 @@
          consts
             None
             0.99
          names      ('np', 'quantile', 'isnan')
          varnames   ('xs',)
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
          name       '<lambda>'
          firstlineno 67
          lnotab 0x
       code
          argcount  : 12
          nlocals   : 16
          stacksize : 12
@@ -341,40 +341,40 @@
             01a6010000ab010000000000000000350001007405000000000000000000
             006a0300000000000000006a040000000000000000740400000000000000
             0000006a050000000000000000a006000000000000000000000000000000
             00000000007c007c046402ac03a6030000ab03000000000000000066017c
             067c017c0264027c09640476007c037c0181027c0b6e01640564069c077c
             0ca4018e017d0d640564056405a6020000ab02000000000000000001006e
             0b230031007304770278035900770101005900010001007c0d6a07000000
-            00000000006407190000000000000000007d0e7c01811874110000000000
-            00000000007c01a6010000ab010000000000000000741200000000000000
-            0000006b020000000072037c0167017d017415000000000000000000007c
-            01a6010000ab01000000000000000064086b020000000072157c0ea00b00
-            000000000000000000000000000000000000007c05a6010000ab01000000
-            000000000001007419000000000000000000007c0d6a0700000000000000
-            00a6010000ab010000000000000000440090015d185c0200007d0f7d0e7c
-            0e6a0d000000000000000064096b020000000072018c127c09640a6b0200
-            000000727e7c0e6a0e0000000000000000640b19000000000000000000a0
-            0f0000000000000000000000000000000000000000640ca6010000ab0100
-            0000000000000001007c0e6a0e0000000000000000640d19000000000000
-            000000a00f0000000000000000000000000000000000000000640ca60100
-            00ab01000000000000000001007c0ea01000000000000000000000000000
-            0000000000000064086407640e7c0e6a110000000000000000640cac0fa6
-            050000ab05000000000000000001007c0ea0100000000000000000000000
-            0000000000000000006407640864107c0e6a110000000000000000640cac
-            0fa6050000ab05000000000000000001007c0964116b0300000000727c7c
-            0f7c037a06000064076b020000000072167c0ea012000000000000000000
-            00000000000000000000007c08a6010000ab01000000000000000001006e
-            157c0ea01200000000000000000000000000000000000000006405a60100
-            00ab01000000000000000001007c0f7c037a020000741500000000000000
-            0000007c01a6010000ab01000000000000000064087a0a00007c037a0200
-            006b020000000072177c0ea0130000000000000000000000000000000000
-            0000007c07a6010000ab010000000000000000010090018c037c0ea01300
+            00000000006407190000000000000000007d0e7c01811574110000000000
+            00000000007c01741200000000000000000000a6020000ab020000000000
+            00000072037c0167017d017415000000000000000000007c01a6010000ab
+            01000000000000000064086b020000000072157c0ea00b00000000000000
+            000000000000000000000000007c05a6010000ab01000000000000000001
+            007419000000000000000000007c0d6a070000000000000000a6010000ab
+            010000000000000000440090015d185c0200007d0f7d0e7c0e6a0d000000
+            000000000064096b020000000072018c127c09640a6b0200000000727e7c
+            0e6a0e0000000000000000640b19000000000000000000a00f0000000000
+            000000000000000000000000000000640ca6010000ab0100000000000000
+            0001007c0e6a0e0000000000000000640d19000000000000000000a00f00
+            00000000000000000000000000000000000000640ca6010000ab01000000
+            000000000001007c0ea01000000000000000000000000000000000000000
+            0064086407640e7c0e6a110000000000000000640cac0fa6050000ab0500
+            0000000000000001007c0ea0100000000000000000000000000000000000
+            0000006407640864107c0e6a110000000000000000640cac0fa6050000ab
+            05000000000000000001007c0964116b0300000000727c7c0f7c037a0600
+            0064076b020000000072167c0ea012000000000000000000000000000000
+            00000000007c08a6010000ab01000000000000000001006e157c0ea01200
             000000000000000000000000000000000000006405a6010000ab01000000
-            0000000000010090018c1a7c0d5300
+            000000000001007c0f7c037a0200007415000000000000000000007c01a6
+            010000ab01000000000000000064087a0a00007c037a0200006b02000000
+            0072177c0ea01300000000000000000000000000000000000000007c07a6
+            010000ab010000000000000000010090018c037c0ea01300000000000000
+            000000000000000000000000006405a6010000ab01000000000000000001
+            0090018c1a7c0d5300
           55           0 RESUME                   0
          
          116           2 LOAD_GLOBAL              1 (NULL + plt)
                       14 LOAD_ATTR                1 (rc_context)
                       24 LOAD_CONST               1 ('figure.figsize')
                       26 LOAD_FAST               10 (figsize)
                       28 BUILD_MAP                1
@@ -450,174 +450,173 @@
          128     >>  232 LOAD_FAST               13 (fig)
                      234 LOAD_ATTR                7 (axes)
                      244 LOAD_CONST               7 (0)
                      246 BINARY_SUBSCR
                      256 STORE_FAST              14 (ax)
          
          129         258 LOAD_FAST                1 (color)
-                     260 POP_JUMP_FORWARD_IF_NONE    24 (to 310)
-                     262 LOAD_GLOBAL             17 (NULL + type)
+                     260 POP_JUMP_FORWARD_IF_NONE    21 (to 304)
+                     262 LOAD_GLOBAL             17 (NULL + isinstance)
                      274 LOAD_FAST                1 (color)
-                     276 PRECALL                  1
-                     280 CALL                     1
-                     290 LOAD_GLOBAL             18 (str)
-                     302 COMPARE_OP               2 (==)
-                     308 POP_JUMP_FORWARD_IF_FALSE     3 (to 316)
-         
-         130     >>  310 LOAD_FAST                1 (color)
-                     312 BUILD_LIST               1
-                     314 STORE_FAST               1 (color)
-         
-         132     >>  316 LOAD_GLOBAL             21 (NULL + len)
-                     328 LOAD_FAST                1 (color)
-                     330 PRECALL                  1
-                     334 CALL                     1
-                     344 LOAD_CONST               8 (1)
-                     346 COMPARE_OP               2 (==)
-                     352 POP_JUMP_FORWARD_IF_FALSE    21 (to 396)
-         
-         133         354 LOAD_FAST               14 (ax)
-                     356 LOAD_METHOD             11 (set_title)
-                     378 LOAD_FAST                5 (title)
-                     380 PRECALL                  1
-                     384 CALL                     1
-                     394 POP_TOP
-         
-         135     >>  396 LOAD_GLOBAL             25 (NULL + enumerate)
-                     408 LOAD_FAST               13 (fig)
-                     410 LOAD_ATTR                7 (axes)
-                     420 PRECALL                  1
-                     424 CALL                     1
-                     434 GET_ITER
-                 >>  436 EXTENDED_ARG             1
-                     438 FOR_ITER               280 (to 1000)
-                     440 UNPACK_SEQUENCE          2
-                     444 STORE_FAST              15 (i)
-                     446 STORE_FAST              14 (ax)
-         
-         136         448 LOAD_FAST               14 (ax)
-                     450 LOAD_ATTR               13 (_label)
-                     460 LOAD_CONST               9 ('<colorbar>')
-                     462 COMPARE_OP               2 (==)
-                     468 POP_JUMP_FORWARD_IF_FALSE     1 (to 472)
-         
-         137         470 JUMP_BACKWARD           18 (to 436)
-         
-         138     >>  472 LOAD_FAST                9 (axis_type)
-                     474 LOAD_CONST              10 ('arrow')
-                     476 COMPARE_OP               2 (==)
-                     482 POP_JUMP_FORWARD_IF_FALSE   126 (to 736)
-         
-         139         484 LOAD_FAST               14 (ax)
-                     486 LOAD_ATTR               14 (spines)
-                     496 LOAD_CONST              11 ('top')
-                     498 BINARY_SUBSCR
-                     508 LOAD_METHOD             15 (set_visible)
-                     530 LOAD_CONST              12 (False)
-                     532 PRECALL                  1
-                     536 CALL                     1
-                     546 POP_TOP
-         
-         140         548 LOAD_FAST               14 (ax)
-                     550 LOAD_ATTR               14 (spines)
-                     560 LOAD_CONST              13 ('right')
-                     562 BINARY_SUBSCR
-                     572 LOAD_METHOD             15 (set_visible)
-                     594 LOAD_CONST              12 (False)
-                     596 PRECALL                  1
-                     600 CALL                     1
-                     610 POP_TOP
-         
-         141         612 LOAD_FAST               14 (ax)
-                     614 LOAD_METHOD             16 (plot)
-                     636 LOAD_CONST               8 (1)
-                     638 LOAD_CONST               7 (0)
-                     640 LOAD_CONST              14 ('>k')
-                     642 LOAD_FAST               14 (ax)
-                     644 LOAD_ATTR               17 (transAxes)
-                     654 LOAD_CONST              12 (False)
-                     656 KW_NAMES                15
-                     658 PRECALL                  5
-                     662 CALL                     5
-                     672 POP_TOP
-         
-         142         674 LOAD_FAST               14 (ax)
-                     676 LOAD_METHOD             16 (plot)
-                     698 LOAD_CONST               7 (0)
-                     700 LOAD_CONST               8 (1)
-                     702 LOAD_CONST              16 ('^k')
-                     704 LOAD_FAST               14 (ax)
-                     706 LOAD_ATTR               17 (transAxes)
-                     716 LOAD_CONST              12 (False)
-                     718 KW_NAMES                15
-                     720 PRECALL                  5
-                     724 CALL                     5
-                     734 POP_TOP
-         
-         144     >>  736 LOAD_FAST                9 (axis_type)
-                     738 LOAD_CONST              17 ('none')
-                     740 COMPARE_OP               3 (!=)
-                     746 POP_JUMP_FORWARD_IF_FALSE   124 (to 996)
-         
-         145         748 LOAD_FAST               15 (i)
-                     750 LOAD_FAST                3 (ncols)
-                     752 BINARY_OP                6 (%)
-                     756 LOAD_CONST               7 (0)
-                     758 COMPARE_OP               2 (==)
-                     764 POP_JUMP_FORWARD_IF_FALSE    22 (to 810)
-         
-         146         766 LOAD_FAST               14 (ax)
-                     768 LOAD_METHOD             18 (set_ylabel)
-                     790 LOAD_FAST                8 (y_label)
-                     792 PRECALL                  1
-                     796 CALL                     1
-                     806 POP_TOP
-                     808 JUMP_FORWARD            21 (to 852)
-         
-         148     >>  810 LOAD_FAST               14 (ax)
-                     812 LOAD_METHOD             18 (set_ylabel)
-                     834 LOAD_CONST               5 (None)
-                     836 PRECALL                  1
-                     840 CALL                     1
-                     850 POP_TOP
-         
-         149     >>  852 LOAD_FAST               15 (i)
-                     854 LOAD_FAST                3 (ncols)
-                     856 BINARY_OP                2 (//)
-                     860 LOAD_GLOBAL             21 (NULL + len)
-                     872 LOAD_FAST                1 (color)
-                     874 PRECALL                  1
-                     878 CALL                     1
-                     888 LOAD_CONST               8 (1)
-                     890 BINARY_OP               10 (-)
-                     894 LOAD_FAST                3 (ncols)
-                     896 BINARY_OP                2 (//)
-                     900 COMPARE_OP               2 (==)
-                     906 POP_JUMP_FORWARD_IF_FALSE    23 (to 954)
-         
-         150         908 LOAD_FAST               14 (ax)
-                     910 LOAD_METHOD             19 (set_xlabel)
-                     932 LOAD_FAST                7 (x_label)
-                     934 PRECALL                  1
-                     938 CALL                     1
-                     948 POP_TOP
-                     950 EXTENDED_ARG             1
-                     952 JUMP_BACKWARD          259 (to 436)
-         
-         152     >>  954 LOAD_FAST               14 (ax)
-                     956 LOAD_METHOD             19 (set_xlabel)
-                     978 LOAD_CONST               5 (None)
-                     980 PRECALL                  1
-                     984 CALL                     1
-                     994 POP_TOP
-                 >>  996 EXTENDED_ARG             1
-                     998 JUMP_BACKWARD          282 (to 436)
+                     276 LOAD_GLOBAL             18 (str)
+                     288 PRECALL                  2
+                     292 CALL                     2
+                     302 POP_JUMP_FORWARD_IF_FALSE     3 (to 310)
+         
+         130     >>  304 LOAD_FAST                1 (color)
+                     306 BUILD_LIST               1
+                     308 STORE_FAST               1 (color)
+         
+         132     >>  310 LOAD_GLOBAL             21 (NULL + len)
+                     322 LOAD_FAST                1 (color)
+                     324 PRECALL                  1
+                     328 CALL                     1
+                     338 LOAD_CONST               8 (1)
+                     340 COMPARE_OP               2 (==)
+                     346 POP_JUMP_FORWARD_IF_FALSE    21 (to 390)
+         
+         133         348 LOAD_FAST               14 (ax)
+                     350 LOAD_METHOD             11 (set_title)
+                     372 LOAD_FAST                5 (title)
+                     374 PRECALL                  1
+                     378 CALL                     1
+                     388 POP_TOP
+         
+         135     >>  390 LOAD_GLOBAL             25 (NULL + enumerate)
+                     402 LOAD_FAST               13 (fig)
+                     404 LOAD_ATTR                7 (axes)
+                     414 PRECALL                  1
+                     418 CALL                     1
+                     428 GET_ITER
+                 >>  430 EXTENDED_ARG             1
+                     432 FOR_ITER               280 (to 994)
+                     434 UNPACK_SEQUENCE          2
+                     438 STORE_FAST              15 (i)
+                     440 STORE_FAST              14 (ax)
+         
+         136         442 LOAD_FAST               14 (ax)
+                     444 LOAD_ATTR               13 (_label)
+                     454 LOAD_CONST               9 ('<colorbar>')
+                     456 COMPARE_OP               2 (==)
+                     462 POP_JUMP_FORWARD_IF_FALSE     1 (to 466)
+         
+         137         464 JUMP_BACKWARD           18 (to 430)
+         
+         138     >>  466 LOAD_FAST                9 (axis_type)
+                     468 LOAD_CONST              10 ('arrow')
+                     470 COMPARE_OP               2 (==)
+                     476 POP_JUMP_FORWARD_IF_FALSE   126 (to 730)
+         
+         139         478 LOAD_FAST               14 (ax)
+                     480 LOAD_ATTR               14 (spines)
+                     490 LOAD_CONST              11 ('top')
+                     492 BINARY_SUBSCR
+                     502 LOAD_METHOD             15 (set_visible)
+                     524 LOAD_CONST              12 (False)
+                     526 PRECALL                  1
+                     530 CALL                     1
+                     540 POP_TOP
+         
+         140         542 LOAD_FAST               14 (ax)
+                     544 LOAD_ATTR               14 (spines)
+                     554 LOAD_CONST              13 ('right')
+                     556 BINARY_SUBSCR
+                     566 LOAD_METHOD             15 (set_visible)
+                     588 LOAD_CONST              12 (False)
+                     590 PRECALL                  1
+                     594 CALL                     1
+                     604 POP_TOP
+         
+         141         606 LOAD_FAST               14 (ax)
+                     608 LOAD_METHOD             16 (plot)
+                     630 LOAD_CONST               8 (1)
+                     632 LOAD_CONST               7 (0)
+                     634 LOAD_CONST              14 ('>k')
+                     636 LOAD_FAST               14 (ax)
+                     638 LOAD_ATTR               17 (transAxes)
+                     648 LOAD_CONST              12 (False)
+                     650 KW_NAMES                15
+                     652 PRECALL                  5
+                     656 CALL                     5
+                     666 POP_TOP
+         
+         142         668 LOAD_FAST               14 (ax)
+                     670 LOAD_METHOD             16 (plot)
+                     692 LOAD_CONST               7 (0)
+                     694 LOAD_CONST               8 (1)
+                     696 LOAD_CONST              16 ('^k')
+                     698 LOAD_FAST               14 (ax)
+                     700 LOAD_ATTR               17 (transAxes)
+                     710 LOAD_CONST              12 (False)
+                     712 KW_NAMES                15
+                     714 PRECALL                  5
+                     718 CALL                     5
+                     728 POP_TOP
+         
+         144     >>  730 LOAD_FAST                9 (axis_type)
+                     732 LOAD_CONST              17 ('none')
+                     734 COMPARE_OP               3 (!=)
+                     740 POP_JUMP_FORWARD_IF_FALSE   124 (to 990)
+         
+         145         742 LOAD_FAST               15 (i)
+                     744 LOAD_FAST                3 (ncols)
+                     746 BINARY_OP                6 (%)
+                     750 LOAD_CONST               7 (0)
+                     752 COMPARE_OP               2 (==)
+                     758 POP_JUMP_FORWARD_IF_FALSE    22 (to 804)
+         
+         146         760 LOAD_FAST               14 (ax)
+                     762 LOAD_METHOD             18 (set_ylabel)
+                     784 LOAD_FAST                8 (y_label)
+                     786 PRECALL                  1
+                     790 CALL                     1
+                     800 POP_TOP
+                     802 JUMP_FORWARD            21 (to 846)
+         
+         148     >>  804 LOAD_FAST               14 (ax)
+                     806 LOAD_METHOD             18 (set_ylabel)
+                     828 LOAD_CONST               5 (None)
+                     830 PRECALL                  1
+                     834 CALL                     1
+                     844 POP_TOP
+         
+         149     >>  846 LOAD_FAST               15 (i)
+                     848 LOAD_FAST                3 (ncols)
+                     850 BINARY_OP                2 (//)
+                     854 LOAD_GLOBAL             21 (NULL + len)
+                     866 LOAD_FAST                1 (color)
+                     868 PRECALL                  1
+                     872 CALL                     1
+                     882 LOAD_CONST               8 (1)
+                     884 BINARY_OP               10 (-)
+                     888 LOAD_FAST                3 (ncols)
+                     890 BINARY_OP                2 (//)
+                     894 COMPARE_OP               2 (==)
+                     900 POP_JUMP_FORWARD_IF_FALSE    23 (to 948)
+         
+         150         902 LOAD_FAST               14 (ax)
+                     904 LOAD_METHOD             19 (set_xlabel)
+                     926 LOAD_FAST                7 (x_label)
+                     928 PRECALL                  1
+                     932 CALL                     1
+                     942 POP_TOP
+                     944 EXTENDED_ARG             1
+                     946 JUMP_BACKWARD          259 (to 430)
+         
+         152     >>  948 LOAD_FAST               14 (ax)
+                     950 LOAD_METHOD             19 (set_xlabel)
+                     972 LOAD_CONST               5 (None)
+                     974 PRECALL                  1
+                     978 CALL                     1
+                     988 POP_TOP
+                 >>  990 EXTENDED_ARG             1
+                     992 JUMP_BACKWARD          282 (to 430)
          
-         153     >> 1000 LOAD_FAST               13 (fig)
-                    1002 RETURN_VALUE
+         153     >>  994 LOAD_FAST               13 (fig)
+                     996 RETURN_VALUE
          ExceptionTable:
            46 to 184 -> 210 [1] lasti
            210 to 216 -> 218 [3] lasti
            224 to 224 -> 218 [3] lasti
          consts
             'Plot the Decipher v space.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n    color : str or list of str\n        Keys for annotations of cells, given to `sc.pl.embedding`.\n    palette : dict, optional\n        A dictionary mapping color keys to colors.\n    ncols : int, default 2\n        Number of columns in the plot.\n    subsample_frac : float, default 1.0\n        Fraction of cells to plot. Useful for large datasets.\n    title : str, default ""\n        Title of the plot. Only used if `color` is a single key, otherwise the title for each\n        subplot is set automatically to the name of the color key.\n    basis : str, default "decipher_v"\n        The basis to use for the plot.\n    x_label : str, default "Decipher 1"\n        The label for the x-axis.\n    y_label : str, default "Decipher 2"\n        The label for the y-axis.\n    axis_type : str, default "arrow"\n        The type of axis to use. Can be "arrow", "line", or "none".\n        If "arrow", the axes are drawn as arrows, with no top or right spines.\n        If "line", the axes are drawn as lines, with all spines.\n        If "none", no axes are drawn.\n    figsize : tuple, default (3.5, 3.5)\n        The size of the figure.\n    vmax : function, optional\n        A function that takes a numpy array and returns a float. Used to set the maximum value of\n        the colorbar. By default, the 99th percentile of the data is used.\n    **kwargs : dict, optional\n        Additional arguments passed to `sc.pl.embedding`.\n\n    Returns\n    -------\n    fig : matplotlib.pyplot.Figure\n        The matplotlib figure.\n\n    See Also\n    --------\n    sc.pl.embedding\n\n    '
             'figure.figsize'
@@ -633,29 +632,29 @@
             'top'
             False
             'right'
             '>k'
             ('transform', 'clip_on')
             '^k'
             'none'
-         names      ('plt', 'rc_context', 'sc', 'pl', 'embedding', 'pp', 'subsample', 'axes', 'type', 'str', 'len', 'set_title', 'enumerate', '_label', 'spines', 'set_visible', 'plot', 'transAxes', 'set_ylabel', 'set_xlabel')
+         names      ('plt', 'rc_context', 'sc', 'pl', 'embedding', 'pp', 'subsample', 'axes', 'isinstance', 'str', 'len', 'set_title', 'enumerate', '_label', 'spines', 'set_visible', 'plot', 'transAxes', 'set_ylabel', 'set_xlabel')
          varnames   ('adata', 'color', 'palette', 'ncols', 'subsample_frac', 'title', 'basis', 'x_label', 'y_label', 'axis_type', 'figsize', 'vmax', 'kwargs', 'fig', 'ax', 'i')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
          name       'decipher'
          firstlineno 55
          lnotab
             0x023d2e01200142ff02020201020102010201060102010af8040902f706
-            ff2e0c1a013401060226012a023401160102010c01400140013e013e020c
+            ff2e0c1a012e01060226012a023401160102010c01400140013e013e020c
             0112012c022a0138012e022e01
       ('decipher_v', 'decipher_z', None)
    names      ('numpy', 'np', 'scanpy', 'sc', 'matplotlib', 'pyplot', 'plt', 'decipher_z', 'decipher')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/plot/decipher.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/plot/decipher.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108010c050201020102fc08330201020102010201020102
       01020102010201020104f4
```

### Comparing `scdecipher-0.1.0/decipher/plot/__pycache__/trajectory_inference.cpython-311.pyc` & `scdecipher-0.1.2/decipher/plot/__pycache__/trajectory_inference.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 9092
+moddate:  0x0e232166 (Thu Apr 18 13:41:34 2024 UTC)
+files sz: 9129
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c016d025a030100640064016c045a
@@ -79,62 +79,62 @@
    
     12         134 KW_NAMES                 6
                136 PRECALL                  2
                140 CALL                     2
                150 POP_TOP
    
     18         152 LOAD_CONST              20 (('on data', 10))
-               154 LOAD_CONST               9 (<code object cell_clusters, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 18>)
+               154 LOAD_CONST               9 (<code object cell_clusters, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 18>)
                156 MAKE_FUNCTION            1 (defaults)
                158 STORE_NAME              21 (cell_clusters)
    
-    26         160 NOP
+    29         160 NOP
    
-    27         162 NOP
+    30         162 NOP
    
-    28         164 NOP
+    31         164 NOP
    
-    24         166 LOAD_CONST              21 ((None, None, None))
-               168 LOAD_CONST              10 (<code object trajectories, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 24>)
+    27         166 LOAD_CONST              21 ((None, None, None))
+               168 LOAD_CONST              10 (<code object trajectories, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 27>)
                170 MAKE_FUNCTION            1 (defaults)
                172 STORE_NAME              22 (trajectories)
    
-    93         174 NOP
+    96         174 NOP
    
-    94         176 NOP
+    97         176 NOP
    
-    95         178 NOP
+    98         178 NOP
    
-    96         180 NOP
+    99         180 NOP
    
-    97         182 NOP
+   100         182 NOP
    
-    98         184 NOP
+   101         184 NOP
    
-    99         186 NOP
+   102         186 NOP
    
-   100         188 NOP
+   103         188 NOP
    
-   101         190 NOP
+   104         190 NOP
    
-   102         192 NOP
+   105         192 NOP
    
-    90         194 LOAD_CONST              22 ((False, 5, None, None, None, (3, 2.3), None, True, None, None))
-               196 LOAD_CONST              15 (<code object gene_patterns, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 90>)
+    93         194 LOAD_CONST              22 ((False, 5, None, None, None, (3, 2.3), None, True, None, None))
+               196 LOAD_CONST              15 (<code object gene_patterns, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 93>)
                198 MAKE_FUNCTION            1 (defaults)
                200 STORE_NAME              23 (gene_patterns)
    
-   207         202 LOAD_CONST              16 (<code object decipher_time, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 207>)
+   210         202 LOAD_CONST              16 (<code object decipher_time, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 210>)
                204 MAKE_FUNCTION            0
                206 STORE_NAME              24 (decipher_time)
    
-   226         208 NOP
+   229         208 NOP
    
-   225         210 LOAD_CONST              23 ((50, 1))
-               212 LOAD_CONST              19 (<code object _add_cell_type_band, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 225>)
+   228         210 LOAD_CONST              23 ((50, 1))
+               212 LOAD_CONST              19 (<code object _add_cell_type_band, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 228>)
                214 MAKE_FUNCTION            1 (defaults)
                216 STORE_NAME              25 (_add_cell_type_band)
                218 LOAD_CONST               1 (None)
                220 RETURN_VALUE
    consts
       0
       None
@@ -154,237 +154,239 @@
             0x97007401000000000000000000007c0064017c017c02ac02a6040000ab
             0400000000000000005300
           18           0 RESUME                   0
          
           19           2 LOAD_GLOBAL              1 (NULL + plot_decipher_v)
          
           20          14 LOAD_FAST                0 (adata)
-                      16 LOAD_CONST               1 ('decipher_clusters')
-                      18 LOAD_FAST                1 (legend_loc)
-                      20 LOAD_FAST                2 (legend_fontsize)
+         
+          21          16 LOAD_CONST               1 ('decipher_clusters')
+         
+          22          18 LOAD_FAST                1 (legend_loc)
+         
+          23          20 LOAD_FAST                2 (legend_fontsize)
          
           19          22 KW_NAMES                 2
                       24 PRECALL                  4
                       28 CALL                     4
                       38 RETURN_VALUE
          consts
             None
             'decipher_clusters'
             ('color', 'legend_loc', 'legend_fontsize')
          names      ('plot_decipher_v',)
          varnames   ('adata', 'legend_loc', 'legend_fontsize')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
          name       'cell_clusters'
          firstlineno 18
-         lnotab 0x02010c0108ff
+         lnotab 0x02010c0102010201020102fc
       code
          argcount  : 4
          nlocals   : 10
          stacksize : 13
          flags     : 3
          code
             0x97007401000000000000000000007c007c017c03ac01a6030000ab0300
             000000000000007d047c046a010000000000000000640219000000000000
             0000007d057c0280257c006a020000000000000000640419000000000000
             000000640519000000000000000000a00300000000000000000000000000
             00000000000000a6000000ab0000000000000000007d0274090000000000
-            00000000007c02a6010000ab010000000000000000740a00000000000000
-            0000006b020000000072037c0267017d02740d000000000000000000006a
-            0700000000000000007411000000000000000000007c02a6010000ab0100
-            00000000000000ac06a6010000ab0100000000000000007d067413000000
-            000000000000007c02a6010000ab01000000000000000044005dc15c0200
-            007d077d087c006a02000000000000000064041900000000000000000064
-            05190000000000000000007c081900000000000000000064071900000000
-            00000000007d097c03810d7c087c03760072097c037c0819000000000000
-            0000007d016e087c067c07190000000000000000007d017c05a00a000000
-            00000000000000000000000000000000007c096403640385026402660219
-            0000000000000000007c0964036403850264086602190000000000000000
-            0064097c017c01640a7417000000000000000000006a0c00000000000000
-            00640b640cac0da6020000ab020000000000000000741700000000000000
-            0000006a0d0000000000000000a6000000ab0000000000000000006702ac
-            0ea6070000ab07000000000000000001007c05a00a000000000000000000
-            00000000000000000000007c096403640885026402660219000000000000
-            0000007c096403640885026408660219000000000000000000640f641064
-            0c7c01ac11a6060000ab06000000000000000001008cc27c045300
-          24           0 RESUME                   0
+            00000000007c02740a00000000000000000000a6020000ab020000000000
+            00000072037c0267017d02740d000000000000000000006a070000000000
+            0000007411000000000000000000007c02a6010000ab0100000000000000
+            00ac06a6010000ab0100000000000000007d067413000000000000000000
+            007c02a6010000ab01000000000000000044005dc15c0200007d077d087c
+            006a02000000000000000064041900000000000000000064051900000000
+            00000000007c08190000000000000000006407190000000000000000007d
+            097c03810d7c087c03760072097c037c08190000000000000000007d016e
+            087c067c07190000000000000000007d017c05a00a000000000000000000
+            00000000000000000000007c096403640385026402660219000000000000
+            0000007c09640364038502640866021900000000000000000064097c017c
+            01640a7417000000000000000000006a0c0000000000000000640b640cac
+            0da6020000ab0200000000000000007417000000000000000000006a0d00
+            00000000000000a6000000ab0000000000000000006702ac0ea6070000ab
+            07000000000000000001007c05a00a000000000000000000000000000000
+            00000000007c0964036408850264026602190000000000000000007c0964
+            03640885026408660219000000000000000000640f6410640c7c01ac11a6
+            060000ab06000000000000000001008cc27c045300
+          27           0 RESUME                   0
          
-          55           2 LOAD_GLOBAL              1 (NULL + plot_decipher_v)
+          58           2 LOAD_GLOBAL              1 (NULL + plot_decipher_v)
                       14 LOAD_FAST                0 (adata)
                       16 LOAD_FAST                1 (color)
                       18 LOAD_FAST                3 (palette)
                       20 KW_NAMES                 1
                       22 PRECALL                  3
                       26 CALL                     3
                       36 STORE_FAST               4 (fig)
          
-          56          38 LOAD_FAST                4 (fig)
+          59          38 LOAD_FAST                4 (fig)
                       40 LOAD_ATTR                1 (axes)
                       50 LOAD_CONST               2 (0)
                       52 BINARY_SUBSCR
                       62 STORE_FAST               5 (ax)
          
-          57          64 LOAD_FAST                2 (trajectory_names)
+          60          64 LOAD_FAST                2 (trajectory_names)
                       66 POP_JUMP_FORWARD_IF_NOT_NONE    37 (to 142)
          
-          58          68 LOAD_FAST                0 (adata)
+          61          68 LOAD_FAST                0 (adata)
                       70 LOAD_ATTR                2 (uns)
                       80 LOAD_CONST               4 ('decipher')
                       82 BINARY_SUBSCR
                       92 LOAD_CONST               5 ('trajectories')
                       94 BINARY_SUBSCR
                      104 LOAD_METHOD              3 (keys)
                      126 PRECALL                  0
                      130 CALL                     0
                      140 STORE_FAST               2 (trajectory_names)
          
-          59     >>  142 LOAD_GLOBAL              9 (NULL + type)
+          62     >>  142 LOAD_GLOBAL              9 (NULL + isinstance)
                      154 LOAD_FAST                2 (trajectory_names)
-                     156 PRECALL                  1
-                     160 CALL                     1
-                     170 LOAD_GLOBAL             10 (str)
-                     182 COMPARE_OP               2 (==)
-                     188 POP_JUMP_FORWARD_IF_FALSE     3 (to 196)
-         
-          60         190 LOAD_FAST                2 (trajectory_names)
-                     192 BUILD_LIST               1
-                     194 STORE_FAST               2 (trajectory_names)
-         
-          62     >>  196 LOAD_GLOBAL             13 (NULL + sns)
-                     208 LOAD_ATTR                7 (color_palette)
-                     218 LOAD_GLOBAL             17 (NULL + len)
-                     230 LOAD_FAST                2 (trajectory_names)
-                     232 PRECALL                  1
-                     236 CALL                     1
-                     246 KW_NAMES                 6
-                     248 PRECALL                  1
-                     252 CALL                     1
-                     262 STORE_FAST               6 (default_color_palette)
-         
-          63         264 LOAD_GLOBAL             19 (NULL + enumerate)
-                     276 LOAD_FAST                2 (trajectory_names)
-                     278 PRECALL                  1
-                     282 CALL                     1
-                     292 GET_ITER
-                 >>  294 FOR_ITER               193 (to 682)
-                     296 UNPACK_SEQUENCE          2
-                     300 STORE_FAST               7 (i)
-                     302 STORE_FAST               8 (t_name)
-         
-          64         304 LOAD_FAST                0 (adata)
-                     306 LOAD_ATTR                2 (uns)
-                     316 LOAD_CONST               4 ('decipher')
-                     318 BINARY_SUBSCR
-                     328 LOAD_CONST               5 ('trajectories')
-                     330 BINARY_SUBSCR
-                     340 LOAD_FAST                8 (t_name)
-                     342 BINARY_SUBSCR
-                     352 LOAD_CONST               7 ('cluster_locations')
-                     354 BINARY_SUBSCR
-                     364 STORE_FAST               9 (cluster_locations)
-         
-          65         366 LOAD_FAST                3 (palette)
-                     368 POP_JUMP_FORWARD_IF_NONE    13 (to 396)
-                     370 LOAD_FAST                8 (t_name)
-                     372 LOAD_FAST                3 (palette)
-                     374 CONTAINS_OP              0
-                     376 POP_JUMP_FORWARD_IF_FALSE     9 (to 396)
-         
-          66         378 LOAD_FAST                3 (palette)
-                     380 LOAD_FAST                8 (t_name)
-                     382 BINARY_SUBSCR
-                     392 STORE_FAST               1 (color)
-                     394 JUMP_FORWARD             8 (to 412)
-         
-          68     >>  396 LOAD_FAST                6 (default_color_palette)
-                     398 LOAD_FAST                7 (i)
-                     400 BINARY_SUBSCR
-                     410 STORE_FAST               1 (color)
-         
-          69     >>  412 LOAD_FAST                5 (ax)
-                     414 LOAD_METHOD             10 (plot)
-         
-          70         436 LOAD_FAST                9 (cluster_locations)
-                     438 LOAD_CONST               3 (None)
-                     440 LOAD_CONST               3 (None)
-                     442 BUILD_SLICE              2
-                     444 LOAD_CONST               2 (0)
-                     446 BUILD_TUPLE              2
-                     448 BINARY_SUBSCR
-         
-          71         458 LOAD_FAST                9 (cluster_locations)
-                     460 LOAD_CONST               3 (None)
-                     462 LOAD_CONST               3 (None)
-                     464 BUILD_SLICE              2
-                     466 LOAD_CONST               8 (1)
-                     468 BUILD_TUPLE              2
-                     470 BINARY_SUBSCR
-         
-          72         480 LOAD_CONST               9 ('o')
-         
-          73         482 LOAD_FAST                1 (color)
-         
-          74         484 LOAD_FAST                1 (color)
-         
-          75         486 LOAD_CONST              10 (7)
-         
-          76         488 LOAD_GLOBAL             23 (NULL + pe)
-                     500 LOAD_ATTR               12 (Stroke)
-                     510 LOAD_CONST              11 (3)
-                     512 LOAD_CONST              12 ('black')
-                     514 KW_NAMES                13
-                     516 PRECALL                  2
-                     520 CALL                     2
-                     530 LOAD_GLOBAL             23 (NULL + pe)
-                     542 LOAD_ATTR               13 (Normal)
-                     552 PRECALL                  0
-                     556 CALL                     0
-                     566 BUILD_LIST               2
-         
-          69         568 KW_NAMES                14
-                     570 PRECALL                  7
-                     574 CALL                     7
-                     584 POP_TOP
-         
-          78         586 LOAD_FAST                5 (ax)
-                     588 LOAD_METHOD             10 (plot)
+                     156 LOAD_GLOBAL             10 (str)
+                     168 PRECALL                  2
+                     172 CALL                     2
+                     182 POP_JUMP_FORWARD_IF_FALSE     3 (to 190)
+         
+          63         184 LOAD_FAST                2 (trajectory_names)
+                     186 BUILD_LIST               1
+                     188 STORE_FAST               2 (trajectory_names)
+         
+          65     >>  190 LOAD_GLOBAL             13 (NULL + sns)
+                     202 LOAD_ATTR                7 (color_palette)
+                     212 LOAD_GLOBAL             17 (NULL + len)
+                     224 LOAD_FAST                2 (trajectory_names)
+                     226 PRECALL                  1
+                     230 CALL                     1
+                     240 KW_NAMES                 6
+                     242 PRECALL                  1
+                     246 CALL                     1
+                     256 STORE_FAST               6 (default_color_palette)
+         
+          66         258 LOAD_GLOBAL             19 (NULL + enumerate)
+                     270 LOAD_FAST                2 (trajectory_names)
+                     272 PRECALL                  1
+                     276 CALL                     1
+                     286 GET_ITER
+                 >>  288 FOR_ITER               193 (to 676)
+                     290 UNPACK_SEQUENCE          2
+                     294 STORE_FAST               7 (i)
+                     296 STORE_FAST               8 (t_name)
+         
+          67         298 LOAD_FAST                0 (adata)
+                     300 LOAD_ATTR                2 (uns)
+                     310 LOAD_CONST               4 ('decipher')
+                     312 BINARY_SUBSCR
+                     322 LOAD_CONST               5 ('trajectories')
+                     324 BINARY_SUBSCR
+                     334 LOAD_FAST                8 (t_name)
+                     336 BINARY_SUBSCR
+                     346 LOAD_CONST               7 ('cluster_locations')
+                     348 BINARY_SUBSCR
+                     358 STORE_FAST               9 (cluster_locations)
+         
+          68         360 LOAD_FAST                3 (palette)
+                     362 POP_JUMP_FORWARD_IF_NONE    13 (to 390)
+                     364 LOAD_FAST                8 (t_name)
+                     366 LOAD_FAST                3 (palette)
+                     368 CONTAINS_OP              0
+                     370 POP_JUMP_FORWARD_IF_FALSE     9 (to 390)
+         
+          69         372 LOAD_FAST                3 (palette)
+                     374 LOAD_FAST                8 (t_name)
+                     376 BINARY_SUBSCR
+                     386 STORE_FAST               1 (color)
+                     388 JUMP_FORWARD             8 (to 406)
+         
+          71     >>  390 LOAD_FAST                6 (default_color_palette)
+                     392 LOAD_FAST                7 (i)
+                     394 BINARY_SUBSCR
+                     404 STORE_FAST               1 (color)
+         
+          72     >>  406 LOAD_FAST                5 (ax)
+                     408 LOAD_METHOD             10 (plot)
+         
+          73         430 LOAD_FAST                9 (cluster_locations)
+                     432 LOAD_CONST               3 (None)
+                     434 LOAD_CONST               3 (None)
+                     436 BUILD_SLICE              2
+                     438 LOAD_CONST               2 (0)
+                     440 BUILD_TUPLE              2
+                     442 BINARY_SUBSCR
+         
+          74         452 LOAD_FAST                9 (cluster_locations)
+                     454 LOAD_CONST               3 (None)
+                     456 LOAD_CONST               3 (None)
+                     458 BUILD_SLICE              2
+                     460 LOAD_CONST               8 (1)
+                     462 BUILD_TUPLE              2
+                     464 BINARY_SUBSCR
+         
+          75         474 LOAD_CONST               9 ('o')
+         
+          76         476 LOAD_FAST                1 (color)
+         
+          77         478 LOAD_FAST                1 (color)
+         
+          78         480 LOAD_CONST              10 (7)
+         
+          79         482 LOAD_GLOBAL             23 (NULL + pe)
+                     494 LOAD_ATTR               12 (Stroke)
+                     504 LOAD_CONST              11 (3)
+                     506 LOAD_CONST              12 ('black')
+                     508 KW_NAMES                13
+                     510 PRECALL                  2
+                     514 CALL                     2
+                     524 LOAD_GLOBAL             23 (NULL + pe)
+                     536 LOAD_ATTR               13 (Normal)
+                     546 PRECALL                  0
+                     550 CALL                     0
+                     560 BUILD_LIST               2
+         
+          72         562 KW_NAMES                14
+                     564 PRECALL                  7
+                     568 CALL                     7
+                     578 POP_TOP
+         
+          81         580 LOAD_FAST                5 (ax)
+                     582 LOAD_METHOD             10 (plot)
+         
+          82         604 LOAD_FAST                9 (cluster_locations)
+                     606 LOAD_CONST               3 (None)
+                     608 LOAD_CONST               8 (1)
+                     610 BUILD_SLICE              2
+                     612 LOAD_CONST               2 (0)
+                     614 BUILD_TUPLE              2
+                     616 BINARY_SUBSCR
+         
+          83         626 LOAD_FAST                9 (cluster_locations)
+                     628 LOAD_CONST               3 (None)
+                     630 LOAD_CONST               8 (1)
+                     632 BUILD_SLICE              2
+                     634 LOAD_CONST               8 (1)
+                     636 BUILD_TUPLE              2
+                     638 BINARY_SUBSCR
+         
+          84         648 LOAD_CONST              15 ('*')
+         
+          85         650 LOAD_CONST              16 (20)
+         
+          86         652 LOAD_CONST              12 ('black')
+         
+          87         654 LOAD_FAST                1 (color)
+         
+          81         656 KW_NAMES                17
+                     658 PRECALL                  6
+                     662 CALL                     6
+                     672 POP_TOP
+                     674 JUMP_BACKWARD          194 (to 288)
          
-          79         610 LOAD_FAST                9 (cluster_locations)
-                     612 LOAD_CONST               3 (None)
-                     614 LOAD_CONST               8 (1)
-                     616 BUILD_SLICE              2
-                     618 LOAD_CONST               2 (0)
-                     620 BUILD_TUPLE              2
-                     622 BINARY_SUBSCR
-         
-          80         632 LOAD_FAST                9 (cluster_locations)
-                     634 LOAD_CONST               3 (None)
-                     636 LOAD_CONST               8 (1)
-                     638 BUILD_SLICE              2
-                     640 LOAD_CONST               8 (1)
-                     642 BUILD_TUPLE              2
-                     644 BINARY_SUBSCR
-         
-          81         654 LOAD_CONST              15 ('*')
-         
-          82         656 LOAD_CONST              16 (20)
-         
-          83         658 LOAD_CONST              12 ('black')
-         
-          84         660 LOAD_FAST                1 (color)
-         
-          78         662 KW_NAMES                17
-                     664 PRECALL                  6
-                     668 CALL                     6
-                     678 POP_TOP
-                     680 JUMP_BACKWARD          194 (to 294)
-         
-          87     >>  682 LOAD_FAST                4 (fig)
-                     684 RETURN_VALUE
+          90     >>  676 LOAD_FAST                4 (fig)
+                     678 RETURN_VALUE
          consts
             'Plot the trajectories over the Decipher v space.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n    color : str, optional\n        Key (or list of keys) for color annotations of cells, passed to `dc.pl.decipher` which\n        in turn passes it to `sc.pl.embedding`. The keys should be in `adata.obs` or should be\n        gene names.\n    trajectory_names : str or list of str, optional\n        The names of the trajectories to plot. If None, plot all trajectories.\n    palette : dict, optional\n        A dictionary mapping trajectory names to colors and/or mapping color keys to colors.\n\n    Returns\n    -------\n    fig : matplotlib.pyplot.Figure\n        The matplotlib figure.\n\n    See Also\n    --------\n    dc.pl.decipher\n    sc.pl.embedding\n    '
             ('color', 'palette')
             0
             None
             'decipher'
             'trajectories'
@@ -396,528 +398,525 @@
             3
             'black'
             ('linewidth', 'foreground')
             ('marker', 'c', 'markerfacecolor', 'markersize', 'path_effects')
             '*'
             20
             ('marker', 'markersize', 'c', 'markerfacecolor')
-         names      ('plot_decipher_v', 'axes', 'uns', 'keys', 'type', 'str', 'sns', 'color_palette', 'len', 'enumerate', 'plot', 'pe', 'Stroke', 'Normal')
+         names      ('plot_decipher_v', 'axes', 'uns', 'keys', 'isinstance', 'str', 'sns', 'color_palette', 'len', 'enumerate', 'plot', 'pe', 'Stroke', 'Normal')
          varnames   ('adata', 'color', 'trajectory_names', 'palette', 'fig', 'ax', 'default_color_palette', 'i', 't_name', 'cluster_locations')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
          name       'trajectories'
-         firstlineno 24
+         firstlineno 27
          lnotab
-            0x021f24011a0104014a0130010602440128013e010c0112021001180116
+            0x021f24011a0104014a012a010602440128013e010c0112021001180116
             011601020102010201020150f9120918011601160102010201020102fa14
             09
       False
       5
       (3, 2.3)
       True
       code
          argcount  : 12
          nlocals   : 26
          stacksize : 10
          flags     : 3
          code
-            0x870097007401000000000000000000007c01a6010000ab010000000000
-            0000007402000000000000000000006b0200000000720f88006601640184
-            087c014400a6000000ab0000000000000000007d0c6e2d89006a02000000
-            0000000000a0030000000000000000000000000000000000000000a60000
-            00ab000000000000000000a0040000000000000000000000000000000000
-            0000007c01a6010000ab01000000000000000067017d0c640284007d0d7c
-            06803374030000000000000000000089006a050000000000000000640419
-            000000000000000000640519000000000000000000a00600000000000000
-            00000000000000000000000000a6000000ab000000000000000000a60100
-            00ab0100000000000000007d066e1b7401000000000000000000007c06a6
-            010000ab010000000000000000740e000000000000000000006b02000000
-            0072037c0667017d067c08802a7411000000000000000000006a09000000
-            00000000007c07ac06a6010000ab0100000000000000007d0e7c0ea00a00
-            00000000000000000000000000000000000000a6000000ab000000000000
-            0000007d086e077c086a0900000000000000007d0e67007d0f67007d1074
-            17000000000000000000006a0c0000000000000000741b00000000000000
-            0000007c06a6010000ab010000000000000000ac07a6010000ab01000000
-            00000000007d11741d000000000000000000007c06a6010000ab01000000
-            0000000000440090015d685c0200007d127d1389006a0500000000000000
-            006404190000000000000000006405190000000000000000007c13190000
-            000000000000007d147c146408190000000000000000006403640385027c
-            0c660219000000000000000000a00f000000000000000000000000000000
-            00000000006409ac0aa6010000ab0100000000000000007d1502007c0d7c
-            157c03a6020000ab0200000000000000007d157c14640b19000000000000
-            0000006403640385027c0c660219000000000000000000a00f0000000000
-            0000000000000000000000000000006409ac0aa6010000ab010000000000
-            0000007d1602007c0d7c167c03a6020000ab0200000000000000007d167c
-            14640c190000000000000000006403640385027c0c660219000000000000
-            000000a00f00000000000000000000000000000000000000006409ac0aa6
-            010000ab0100000000000000007d1702007c0d7c177c03a6020000ab0200
-            000000000000007d177c14640d190000000000000000007d187c1864037c
-            0a8502190000000000000000007d187c1564037c0a850219000000000000
-            0000007d157c1664037c0a8502190000000000000000007d167c1764037c
-            0a8502190000000000000000007d177c05810d7c137c05760072097c057c
-            13190000000000000000007d196e087c117c12190000000000000000007d
-            197c0fa01000000000000000000000000000000000000000007c18640e19
-            000000000000000000a6010000ab01000000000000000001007c10a01000
-            000000000000000000000000000000000000007c18640f19000000000000
-            000000a6010000ab01000000000000000001007c09721a7c08a011000000
-            00000000000000000000000000000000007c187c167c177c196410ac11a6
-            050000ab05000000000000000001007c08a0120000000000000000000000
-            0000000000000000007c187c157c137c196412ac13a6050000ab05000000
-            0000000000010090018c6a7c0481317c0b80027c067d0b741d0000000000
-            00000000007c0ba6010000ab01000000000000000044005d1d5c0200007d
-            127d1374270000000000000000000089007c137c047c087c057c1264097a
-            000000ac14a6060000ab06000000000000000001008c1e7c0272317c08a0
-            140000000000000000000000000000000000000000742b00000000000000
-            0000007c0fa6010000ab010000000000000000742d000000000000000000
-            007c10a6010000ab010000000000000000a6020000ab0200000000000000
-            0001006e307c08a014000000000000000000000000000000000000000074
-            2d000000000000000000007c0fa6010000ab010000000000000000742b00
-            0000000000000000007c10a6010000ab010000000000000000a6020000ab
-            02000000000000000001007c08a017000000000000000000000000000000
-            00000000006700a6010000ab01000000000000000001007c08a018000000
-            000000000000000000000000000000000064156416ac17a6020000ab0200
-            0000000000000001007c08a0190000000000000000000000000000000000
-            00000064186416ac17a6020000ab02000000000000000001007c08a01a00
-            00000000000000000000000000000000000000640ea6010000ab01000000
-            000000000001007c08a01b00000000000000000000000000000000000000
-            006419ac1aa6010000ab01000000000000000001007c08a01c0000000000
-            0000000000000000000000000000007c01641bac17a6020000ab02000000
-            000000000001007c0e5300
+            0x870097007401000000000000000000007c017402000000000000000000
+            00a6020000ab020000000000000000720f88006601640184087c014400a6
+            000000ab0000000000000000007d0c6e2d89006a020000000000000000a0
+            030000000000000000000000000000000000000000a6000000ab00000000
+            0000000000a00400000000000000000000000000000000000000007c01a6
+            010000ab01000000000000000067017d0c640284007d0d7c068033740300
+            00000000000000000089006a050000000000000000640419000000000000
+            000000640519000000000000000000a00600000000000000000000000000
+            00000000000000a6000000ab000000000000000000a6010000ab01000000
+            00000000007d066e187401000000000000000000007c06740e0000000000
+            0000000000a6020000ab02000000000000000072037c0667017d067c0880
+            2a7411000000000000000000006a0900000000000000007c07ac06a60100
+            00ab0100000000000000007d0e7c0ea00a00000000000000000000000000
+            00000000000000a6000000ab0000000000000000007d086e077c086a0900
+            000000000000007d0e67007d0f67007d107417000000000000000000006a
+            0c0000000000000000741b000000000000000000007c06a6010000ab0100
+            00000000000000ac07a6010000ab0100000000000000007d11741d000000
+            000000000000007c06a6010000ab010000000000000000440090015d685c
+            0200007d127d1389006a0500000000000000006404190000000000000000
+            006405190000000000000000007c13190000000000000000007d147c1464
+            08190000000000000000006403640385027c0c6602190000000000000000
+            00a00f00000000000000000000000000000000000000006409ac0aa60100
+            00ab0100000000000000007d1502007c0d7c157c03a6020000ab02000000
+            00000000007d157c14640b190000000000000000006403640385027c0c66
+            0219000000000000000000a00f0000000000000000000000000000000000
+            0000006409ac0aa6010000ab0100000000000000007d1602007c0d7c167c
+            03a6020000ab0200000000000000007d167c14640c190000000000000000
+            006403640385027c0c660219000000000000000000a00f00000000000000
+            000000000000000000000000006409ac0aa6010000ab0100000000000000
+            007d1702007c0d7c177c03a6020000ab0200000000000000007d177c1464
+            0d190000000000000000007d187c1864037c0a8502190000000000000000
+            007d187c1564037c0a8502190000000000000000007d157c1664037c0a85
+            02190000000000000000007d167c1764037c0a8502190000000000000000
+            007d177c05810d7c137c05760072097c057c13190000000000000000007d
+            196e087c117c12190000000000000000007d197c0fa01000000000000000
+            000000000000000000000000007c18640e19000000000000000000a60100
+            00ab01000000000000000001007c10a01000000000000000000000000000
+            000000000000007c18640f19000000000000000000a6010000ab01000000
+            000000000001007c09721a7c08a011000000000000000000000000000000
+            00000000007c187c167c177c196410ac11a6050000ab0500000000000000
+            0001007c08a01200000000000000000000000000000000000000007c187c
+            157c137c196412ac13a6050000ab050000000000000000010090018c6a7c
+            0481317c0b80027c067d0b741d000000000000000000007c0ba6010000ab
+            01000000000000000044005d1d5c0200007d127d13742700000000000000
+            00000089007c137c047c087c057c1264097a000000ac14a6060000ab0600
+            0000000000000001008c1e7c0272317c08a0140000000000000000000000
+            000000000000000000742b000000000000000000007c0fa6010000ab0100
+            00000000000000742d000000000000000000007c10a6010000ab01000000
+            0000000000a6020000ab02000000000000000001006e307c08a014000000
+            0000000000000000000000000000000000742d000000000000000000007c
+            0fa6010000ab010000000000000000742b000000000000000000007c10a6
+            010000ab010000000000000000a6020000ab02000000000000000001007c
+            08a01700000000000000000000000000000000000000006700a6010000ab
+            01000000000000000001007c08a018000000000000000000000000000000
+            000000000064156416ac17a6020000ab02000000000000000001007c08a0
+            19000000000000000000000000000000000000000064186416ac17a60200
+            00ab02000000000000000001007c08a01a00000000000000000000000000
+            00000000000000640ea6010000ab01000000000000000001007c08a01b00
+            000000000000000000000000000000000000006419ac1aa6010000ab0100
+            0000000000000001007c08a01c0000000000000000000000000000000000
+            0000007c01641bac17a6020000ab02000000000000000001007c0e5300
                        0 MAKE_CELL                0 (adata)
          
-          90           2 RESUME                   0
+          93           2 RESUME                   0
          
-         137           4 LOAD_GLOBAL              1 (NULL + type)
+         140           4 LOAD_GLOBAL              1 (NULL + isinstance)
                       16 LOAD_FAST                1 (gene_name)
-                      18 PRECALL                  1
-                      22 CALL                     1
-                      32 LOAD_GLOBAL              2 (list)
-                      44 COMPARE_OP               2 (==)
-                      50 POP_JUMP_FORWARD_IF_FALSE    15 (to 82)
-         
-         138          52 LOAD_CLOSURE             0 (adata)
-                      54 BUILD_TUPLE              1
-                      56 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 138>)
-                      58 MAKE_FUNCTION            8 (closure)
-                      60 LOAD_FAST                1 (gene_name)
-                      62 GET_ITER
-                      64 PRECALL                  0
-                      68 CALL                     0
-                      78 STORE_FAST              12 (gene_id)
-                      80 JUMP_FORWARD            45 (to 172)
-         
-         140     >>   82 LOAD_DEREF               0 (adata)
-                      84 LOAD_ATTR                2 (var_names)
-                      94 LOAD_METHOD              3 (tolist)
-                     116 PRECALL                  0
-                     120 CALL                     0
-                     130 LOAD_METHOD              4 (index)
-                     152 LOAD_FAST                1 (gene_name)
-                     154 PRECALL                  1
-                     158 CALL                     1
-                     168 BUILD_LIST               1
-                     170 STORE_FAST              12 (gene_id)
-         
-         142     >>  172 LOAD_CONST               2 (<code object moving_average, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 142>)
-                     174 MAKE_FUNCTION            0
-                     176 STORE_FAST              13 (moving_average)
-         
-         145         178 LOAD_FAST                6 (pattern_names)
-                     180 POP_JUMP_FORWARD_IF_NOT_NONE    51 (to 284)
-         
-         146         182 LOAD_GLOBAL              3 (NULL + list)
-                     194 LOAD_DEREF               0 (adata)
-                     196 LOAD_ATTR                5 (uns)
-                     206 LOAD_CONST               4 ('decipher')
-                     208 BINARY_SUBSCR
-                     218 LOAD_CONST               5 ('gene_patterns')
-                     220 BINARY_SUBSCR
-                     230 LOAD_METHOD              6 (keys)
-                     252 PRECALL                  0
-                     256 CALL                     0
-                     266 PRECALL                  1
-                     270 CALL                     1
-                     280 STORE_FAST               6 (pattern_names)
-                     282 JUMP_FORWARD            27 (to 338)
-         
-         147     >>  284 LOAD_GLOBAL              1 (NULL + type)
-                     296 LOAD_FAST                6 (pattern_names)
-                     298 PRECALL                  1
-                     302 CALL                     1
-                     312 LOAD_GLOBAL             14 (str)
-                     324 COMPARE_OP               2 (==)
-                     330 POP_JUMP_FORWARD_IF_FALSE     3 (to 338)
-         
-         148         332 LOAD_FAST                6 (pattern_names)
-                     334 BUILD_LIST               1
-                     336 STORE_FAST               6 (pattern_names)
-         
-         150     >>  338 LOAD_FAST                8 (ax)
-                     340 POP_JUMP_FORWARD_IF_NOT_NONE    42 (to 426)
-         
-         151         342 LOAD_GLOBAL             17 (NULL + plt)
-                     354 LOAD_ATTR                9 (figure)
-                     364 LOAD_FAST                7 (figsize)
-                     366 KW_NAMES                 6
-                     368 PRECALL                  1
-                     372 CALL                     1
-                     382 STORE_FAST              14 (fig)
-         
-         152         384 LOAD_FAST               14 (fig)
-                     386 LOAD_METHOD             10 (gca)
-                     408 PRECALL                  0
-                     412 CALL                     0
-                     422 STORE_FAST               8 (ax)
-                     424 JUMP_FORWARD             7 (to 440)
-         
-         154     >>  426 LOAD_FAST                8 (ax)
-                     428 LOAD_ATTR                9 (figure)
-                     438 STORE_FAST              14 (fig)
-         
-         155     >>  440 BUILD_LIST               0
-                     442 STORE_FAST              15 (start_times)
-         
-         156         444 BUILD_LIST               0
-                     446 STORE_FAST              16 (end_times)
-         
-         158         448 LOAD_GLOBAL             23 (NULL + sns)
-                     460 LOAD_ATTR               12 (color_palette)
-                     470 LOAD_GLOBAL             27 (NULL + len)
-                     482 LOAD_FAST                6 (pattern_names)
-                     484 PRECALL                  1
-                     488 CALL                     1
-                     498 KW_NAMES                 7
-                     500 PRECALL                  1
-                     504 CALL                     1
-                     514 STORE_FAST              17 (default_color_palette)
-         
-         159         516 LOAD_GLOBAL             29 (NULL + enumerate)
-                     528 LOAD_FAST                6 (pattern_names)
-                     530 PRECALL                  1
-                     534 CALL                     1
-                     544 GET_ITER
-                 >>  546 EXTENDED_ARG             1
-                     548 FOR_ITER               360 (to 1270)
-                     550 UNPACK_SEQUENCE          2
-                     554 STORE_FAST              18 (i)
-                     556 STORE_FAST              19 (p_name)
-         
-         160         558 LOAD_DEREF               0 (adata)
-                     560 LOAD_ATTR                5 (uns)
-                     570 LOAD_CONST               4 ('decipher')
+                      18 LOAD_GLOBAL              2 (list)
+                      30 PRECALL                  2
+                      34 CALL                     2
+                      44 POP_JUMP_FORWARD_IF_FALSE    15 (to 76)
+         
+         141          46 LOAD_CLOSURE             0 (adata)
+                      48 BUILD_TUPLE              1
+                      50 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 141>)
+                      52 MAKE_FUNCTION            8 (closure)
+                      54 LOAD_FAST                1 (gene_name)
+                      56 GET_ITER
+                      58 PRECALL                  0
+                      62 CALL                     0
+                      72 STORE_FAST              12 (gene_id)
+                      74 JUMP_FORWARD            45 (to 166)
+         
+         143     >>   76 LOAD_DEREF               0 (adata)
+                      78 LOAD_ATTR                2 (var_names)
+                      88 LOAD_METHOD              3 (tolist)
+                     110 PRECALL                  0
+                     114 CALL                     0
+                     124 LOAD_METHOD              4 (index)
+                     146 LOAD_FAST                1 (gene_name)
+                     148 PRECALL                  1
+                     152 CALL                     1
+                     162 BUILD_LIST               1
+                     164 STORE_FAST              12 (gene_id)
+         
+         145     >>  166 LOAD_CONST               2 (<code object moving_average, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 145>)
+                     168 MAKE_FUNCTION            0
+                     170 STORE_FAST              13 (moving_average)
+         
+         148         172 LOAD_FAST                6 (pattern_names)
+                     174 POP_JUMP_FORWARD_IF_NOT_NONE    51 (to 278)
+         
+         149         176 LOAD_GLOBAL              3 (NULL + list)
+                     188 LOAD_DEREF               0 (adata)
+                     190 LOAD_ATTR                5 (uns)
+                     200 LOAD_CONST               4 ('decipher')
+                     202 BINARY_SUBSCR
+                     212 LOAD_CONST               5 ('gene_patterns')
+                     214 BINARY_SUBSCR
+                     224 LOAD_METHOD              6 (keys)
+                     246 PRECALL                  0
+                     250 CALL                     0
+                     260 PRECALL                  1
+                     264 CALL                     1
+                     274 STORE_FAST               6 (pattern_names)
+                     276 JUMP_FORWARD            24 (to 326)
+         
+         150     >>  278 LOAD_GLOBAL              1 (NULL + isinstance)
+                     290 LOAD_FAST                6 (pattern_names)
+                     292 LOAD_GLOBAL             14 (str)
+                     304 PRECALL                  2
+                     308 CALL                     2
+                     318 POP_JUMP_FORWARD_IF_FALSE     3 (to 326)
+         
+         151         320 LOAD_FAST                6 (pattern_names)
+                     322 BUILD_LIST               1
+                     324 STORE_FAST               6 (pattern_names)
+         
+         153     >>  326 LOAD_FAST                8 (ax)
+                     328 POP_JUMP_FORWARD_IF_NOT_NONE    42 (to 414)
+         
+         154         330 LOAD_GLOBAL             17 (NULL + plt)
+                     342 LOAD_ATTR                9 (figure)
+                     352 LOAD_FAST                7 (figsize)
+                     354 KW_NAMES                 6
+                     356 PRECALL                  1
+                     360 CALL                     1
+                     370 STORE_FAST              14 (fig)
+         
+         155         372 LOAD_FAST               14 (fig)
+                     374 LOAD_METHOD             10 (gca)
+                     396 PRECALL                  0
+                     400 CALL                     0
+                     410 STORE_FAST               8 (ax)
+                     412 JUMP_FORWARD             7 (to 428)
+         
+         157     >>  414 LOAD_FAST                8 (ax)
+                     416 LOAD_ATTR                9 (figure)
+                     426 STORE_FAST              14 (fig)
+         
+         158     >>  428 BUILD_LIST               0
+                     430 STORE_FAST              15 (start_times)
+         
+         159         432 BUILD_LIST               0
+                     434 STORE_FAST              16 (end_times)
+         
+         161         436 LOAD_GLOBAL             23 (NULL + sns)
+                     448 LOAD_ATTR               12 (color_palette)
+                     458 LOAD_GLOBAL             27 (NULL + len)
+                     470 LOAD_FAST                6 (pattern_names)
+                     472 PRECALL                  1
+                     476 CALL                     1
+                     486 KW_NAMES                 7
+                     488 PRECALL                  1
+                     492 CALL                     1
+                     502 STORE_FAST              17 (default_color_palette)
+         
+         162         504 LOAD_GLOBAL             29 (NULL + enumerate)
+                     516 LOAD_FAST                6 (pattern_names)
+                     518 PRECALL                  1
+                     522 CALL                     1
+                     532 GET_ITER
+                 >>  534 EXTENDED_ARG             1
+                     536 FOR_ITER               360 (to 1258)
+                     538 UNPACK_SEQUENCE          2
+                     542 STORE_FAST              18 (i)
+                     544 STORE_FAST              19 (p_name)
+         
+         163         546 LOAD_DEREF               0 (adata)
+                     548 LOAD_ATTR                5 (uns)
+                     558 LOAD_CONST               4 ('decipher')
+                     560 BINARY_SUBSCR
+                     570 LOAD_CONST               5 ('gene_patterns')
                      572 BINARY_SUBSCR
-                     582 LOAD_CONST               5 ('gene_patterns')
+                     582 LOAD_FAST               19 (p_name)
                      584 BINARY_SUBSCR
-                     594 LOAD_FAST               19 (p_name)
-                     596 BINARY_SUBSCR
-                     606 STORE_FAST              20 (gene_pattern)
-         
-         162         608 LOAD_FAST               20 (gene_pattern)
-                     610 LOAD_CONST               8 ('mean')
-                     612 BINARY_SUBSCR
-                     622 LOAD_CONST               3 (None)
-                     624 LOAD_CONST               3 (None)
-                     626 BUILD_SLICE              2
-                     628 LOAD_FAST               12 (gene_id)
-                     630 BUILD_TUPLE              2
-                     632 BINARY_SUBSCR
-                     642 LOAD_METHOD             15 (mean)
-                     664 LOAD_CONST               9 (1)
-                     666 KW_NAMES                10
-                     668 PRECALL                  1
-                     672 CALL                     1
-                     682 STORE_FAST              21 (gene_pattern_mean)
-         
-         163         684 PUSH_NULL
-                     686 LOAD_FAST               13 (moving_average)
-                     688 LOAD_FAST               21 (gene_pattern_mean)
-                     690 LOAD_FAST                3 (smoothing_window)
-                     692 PRECALL                  2
-                     696 CALL                     2
-                     706 STORE_FAST              21 (gene_pattern_mean)
-         
-         164         708 LOAD_FAST               20 (gene_pattern)
-                     710 LOAD_CONST              11 ('q25')
-                     712 BINARY_SUBSCR
-                     722 LOAD_CONST               3 (None)
-                     724 LOAD_CONST               3 (None)
-                     726 BUILD_SLICE              2
-                     728 LOAD_FAST               12 (gene_id)
-                     730 BUILD_TUPLE              2
-                     732 BINARY_SUBSCR
-                     742 LOAD_METHOD             15 (mean)
-                     764 LOAD_CONST               9 (1)
-                     766 KW_NAMES                10
-                     768 PRECALL                  1
-                     772 CALL                     1
-                     782 STORE_FAST              22 (gene_pattern_q25)
-         
-         165         784 PUSH_NULL
-                     786 LOAD_FAST               13 (moving_average)
-                     788 LOAD_FAST               22 (gene_pattern_q25)
-                     790 LOAD_FAST                3 (smoothing_window)
-                     792 PRECALL                  2
-                     796 CALL                     2
-                     806 STORE_FAST              22 (gene_pattern_q25)
-         
-         166         808 LOAD_FAST               20 (gene_pattern)
-                     810 LOAD_CONST              12 ('q75')
-                     812 BINARY_SUBSCR
-                     822 LOAD_CONST               3 (None)
-                     824 LOAD_CONST               3 (None)
-                     826 BUILD_SLICE              2
-                     828 LOAD_FAST               12 (gene_id)
-                     830 BUILD_TUPLE              2
-                     832 BINARY_SUBSCR
-                     842 LOAD_METHOD             15 (mean)
-                     864 LOAD_CONST               9 (1)
-                     866 KW_NAMES                10
-                     868 PRECALL                  1
-                     872 CALL                     1
-                     882 STORE_FAST              23 (gene_pattern_q75)
-         
-         167         884 PUSH_NULL
-                     886 LOAD_FAST               13 (moving_average)
-                     888 LOAD_FAST               23 (gene_pattern_q75)
-                     890 LOAD_FAST                3 (smoothing_window)
-                     892 PRECALL                  2
-                     896 CALL                     2
-                     906 STORE_FAST              23 (gene_pattern_q75)
-         
-         168         908 LOAD_FAST               20 (gene_pattern)
-                     910 LOAD_CONST              13 ('times')
-                     912 BINARY_SUBSCR
-                     922 STORE_FAST              24 (times)
-         
-         170         924 LOAD_FAST               24 (times)
-                     926 LOAD_CONST               3 (None)
-                     928 LOAD_FAST               10 (max_length)
-                     930 BUILD_SLICE              2
-                     932 BINARY_SUBSCR
-                     942 STORE_FAST              24 (times)
-         
-         171         944 LOAD_FAST               21 (gene_pattern_mean)
-                     946 LOAD_CONST               3 (None)
-                     948 LOAD_FAST               10 (max_length)
-                     950 BUILD_SLICE              2
-                     952 BINARY_SUBSCR
-                     962 STORE_FAST              21 (gene_pattern_mean)
-         
-         172         964 LOAD_FAST               22 (gene_pattern_q25)
-                     966 LOAD_CONST               3 (None)
-                     968 LOAD_FAST               10 (max_length)
-                     970 BUILD_SLICE              2
-                     972 BINARY_SUBSCR
-                     982 STORE_FAST              22 (gene_pattern_q25)
-         
-         173         984 LOAD_FAST               23 (gene_pattern_q75)
-                     986 LOAD_CONST               3 (None)
-                     988 LOAD_FAST               10 (max_length)
-                     990 BUILD_SLICE              2
-                     992 BINARY_SUBSCR
-                    1002 STORE_FAST              23 (gene_pattern_q75)
-         
-         175        1004 LOAD_FAST                5 (palette)
-                    1006 POP_JUMP_FORWARD_IF_NONE    13 (to 1034)
-                    1008 LOAD_FAST               19 (p_name)
-                    1010 LOAD_FAST                5 (palette)
-                    1012 CONTAINS_OP              0
-                    1014 POP_JUMP_FORWARD_IF_FALSE     9 (to 1034)
-         
-         176        1016 LOAD_FAST                5 (palette)
-                    1018 LOAD_FAST               19 (p_name)
-                    1020 BINARY_SUBSCR
-                    1030 STORE_FAST              25 (color)
-                    1032 JUMP_FORWARD             8 (to 1050)
-         
-         178     >> 1034 LOAD_FAST               17 (default_color_palette)
-                    1036 LOAD_FAST               18 (i)
-                    1038 BINARY_SUBSCR
-                    1048 STORE_FAST              25 (color)
-         
-         180     >> 1050 LOAD_FAST               15 (start_times)
-                    1052 LOAD_METHOD             16 (append)
-                    1074 LOAD_FAST               24 (times)
-                    1076 LOAD_CONST              14 (0)
-                    1078 BINARY_SUBSCR
-                    1088 PRECALL                  1
-                    1092 CALL                     1
-                    1102 POP_TOP
-         
-         181        1104 LOAD_FAST               16 (end_times)
-                    1106 LOAD_METHOD             16 (append)
-                    1128 LOAD_FAST               24 (times)
-                    1130 LOAD_CONST              15 (-1)
-                    1132 BINARY_SUBSCR
-                    1142 PRECALL                  1
-                    1146 CALL                     1
-                    1156 POP_TOP
-         
-         183        1158 LOAD_FAST                9 (include_uncertainty)
-                    1160 POP_JUMP_FORWARD_IF_FALSE    26 (to 1214)
-         
-         184        1162 LOAD_FAST                8 (ax)
-                    1164 LOAD_METHOD             17 (fill_between)
-                    1186 LOAD_FAST               24 (times)
-                    1188 LOAD_FAST               22 (gene_pattern_q25)
-                    1190 LOAD_FAST               23 (gene_pattern_q75)
-                    1192 LOAD_FAST               25 (color)
-                    1194 LOAD_CONST              16 (0.3)
-                    1196 KW_NAMES                17
-                    1198 PRECALL                  5
-                    1202 CALL                     5
-                    1212 POP_TOP
-         
-         185     >> 1214 LOAD_FAST                8 (ax)
-                    1216 LOAD_METHOD             18 (plot)
-                    1238 LOAD_FAST               24 (times)
-                    1240 LOAD_FAST               21 (gene_pattern_mean)
-                    1242 LOAD_FAST               19 (p_name)
-                    1244 LOAD_FAST               25 (color)
-                    1246 LOAD_CONST              18 (3)
-                    1248 KW_NAMES                19
-                    1250 PRECALL                  5
-                    1254 CALL                     5
-                    1264 POP_TOP
-                    1266 EXTENDED_ARG             1
-                    1268 JUMP_BACKWARD          362 (to 546)
-         
-         186     >> 1270 LOAD_FAST                4 (cell_type_key)
-                    1272 POP_JUMP_FORWARD_IF_NONE    49 (to 1372)
-         
-         187        1274 LOAD_FAST               11 (cell_type_band_pattern_names)
-                    1276 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 1282)
-         
-         188        1278 LOAD_FAST                6 (pattern_names)
-                    1280 STORE_FAST              11 (cell_type_band_pattern_names)
-         
-         189     >> 1282 LOAD_GLOBAL             29 (NULL + enumerate)
-                    1294 LOAD_FAST               11 (cell_type_band_pattern_names)
-                    1296 PRECALL                  1
-                    1300 CALL                     1
-                    1310 GET_ITER
-                 >> 1312 FOR_ITER                29 (to 1372)
-                    1314 UNPACK_SEQUENCE          2
-                    1318 STORE_FAST              18 (i)
-                    1320 STORE_FAST              19 (p_name)
-         
-         190        1322 LOAD_GLOBAL             39 (NULL + _add_cell_type_band)
-                    1334 LOAD_DEREF               0 (adata)
-                    1336 LOAD_FAST               19 (p_name)
-                    1338 LOAD_FAST                4 (cell_type_key)
-                    1340 LOAD_FAST                8 (ax)
-                    1342 LOAD_FAST                5 (palette)
-                    1344 LOAD_FAST               18 (i)
-                    1346 LOAD_CONST               9 (1)
-                    1348 BINARY_OP                0 (+)
-                    1352 KW_NAMES                20
-                    1354 PRECALL                  6
-                    1358 CALL                     6
-                    1368 POP_TOP
-                    1370 JUMP_BACKWARD           30 (to 1312)
-         
-         192     >> 1372 LOAD_FAST                2 (crop_to_min_length)
-                    1374 POP_JUMP_FORWARD_IF_FALSE    49 (to 1474)
-         
-         193        1376 LOAD_FAST                8 (ax)
-                    1378 LOAD_METHOD             20 (set_xlim)
-                    1400 LOAD_GLOBAL             43 (NULL + max)
-                    1412 LOAD_FAST               15 (start_times)
-                    1414 PRECALL                  1
-                    1418 CALL                     1
-                    1428 LOAD_GLOBAL             45 (NULL + min)
-                    1440 LOAD_FAST               16 (end_times)
-                    1442 PRECALL                  1
-                    1446 CALL                     1
-                    1456 PRECALL                  2
-                    1460 CALL                     2
-                    1470 POP_TOP
-                    1472 JUMP_FORWARD            48 (to 1570)
-         
-         195     >> 1474 LOAD_FAST                8 (ax)
-                    1476 LOAD_METHOD             20 (set_xlim)
-                    1498 LOAD_GLOBAL             45 (NULL + min)
-                    1510 LOAD_FAST               15 (start_times)
-                    1512 PRECALL                  1
-                    1516 CALL                     1
-                    1526 LOAD_GLOBAL             43 (NULL + max)
-                    1538 LOAD_FAST               16 (end_times)
-                    1540 PRECALL                  1
-                    1544 CALL                     1
-                    1554 PRECALL                  2
-                    1558 CALL                     2
-                    1568 POP_TOP
-         
-         197     >> 1570 LOAD_FAST                8 (ax)
-                    1572 LOAD_METHOD             23 (set_xticks)
-                    1594 BUILD_LIST               0
-                    1596 PRECALL                  1
-                    1600 CALL                     1
-                    1610 POP_TOP
-         
-         198        1612 LOAD_FAST                8 (ax)
-                    1614 LOAD_METHOD             24 (set_xlabel)
-                    1636 LOAD_CONST              21 ('Decipher time')
-                    1638 LOAD_CONST              22 (14)
-                    1640 KW_NAMES                23
-                    1642 PRECALL                  2
-                    1646 CALL                     2
-                    1656 POP_TOP
-         
-         199        1658 LOAD_FAST                8 (ax)
-                    1660 LOAD_METHOD             25 (set_ylabel)
-                    1682 LOAD_CONST              24 ('Gene expression')
-                    1684 LOAD_CONST              22 (14)
-                    1686 KW_NAMES                23
-                    1688 PRECALL                  2
-                    1692 CALL                     2
-                    1702 POP_TOP
-         
-         200        1704 LOAD_FAST                8 (ax)
-                    1706 LOAD_METHOD             26 (set_ylim)
-                    1728 LOAD_CONST              14 (0)
-                    1730 PRECALL                  1
-                    1734 CALL                     1
-                    1744 POP_TOP
-         
-         201        1746 LOAD_FAST                8 (ax)
-                    1748 LOAD_METHOD             27 (legend)
-                    1770 LOAD_CONST              25 (False)
-                    1772 KW_NAMES                26
-                    1774 PRECALL                  1
-                    1778 CALL                     1
-                    1788 POP_TOP
-         
-         202        1790 LOAD_FAST                8 (ax)
-                    1792 LOAD_METHOD             28 (set_title)
-                    1814 LOAD_FAST                1 (gene_name)
-                    1816 LOAD_CONST              27 (18)
-                    1818 KW_NAMES                23
-                    1820 PRECALL                  2
-                    1824 CALL                     2
-                    1834 POP_TOP
+                     594 STORE_FAST              20 (gene_pattern)
+         
+         165         596 LOAD_FAST               20 (gene_pattern)
+                     598 LOAD_CONST               8 ('mean')
+                     600 BINARY_SUBSCR
+                     610 LOAD_CONST               3 (None)
+                     612 LOAD_CONST               3 (None)
+                     614 BUILD_SLICE              2
+                     616 LOAD_FAST               12 (gene_id)
+                     618 BUILD_TUPLE              2
+                     620 BINARY_SUBSCR
+                     630 LOAD_METHOD             15 (mean)
+                     652 LOAD_CONST               9 (1)
+                     654 KW_NAMES                10
+                     656 PRECALL                  1
+                     660 CALL                     1
+                     670 STORE_FAST              21 (gene_pattern_mean)
+         
+         166         672 PUSH_NULL
+                     674 LOAD_FAST               13 (moving_average)
+                     676 LOAD_FAST               21 (gene_pattern_mean)
+                     678 LOAD_FAST                3 (smoothing_window)
+                     680 PRECALL                  2
+                     684 CALL                     2
+                     694 STORE_FAST              21 (gene_pattern_mean)
+         
+         167         696 LOAD_FAST               20 (gene_pattern)
+                     698 LOAD_CONST              11 ('q25')
+                     700 BINARY_SUBSCR
+                     710 LOAD_CONST               3 (None)
+                     712 LOAD_CONST               3 (None)
+                     714 BUILD_SLICE              2
+                     716 LOAD_FAST               12 (gene_id)
+                     718 BUILD_TUPLE              2
+                     720 BINARY_SUBSCR
+                     730 LOAD_METHOD             15 (mean)
+                     752 LOAD_CONST               9 (1)
+                     754 KW_NAMES                10
+                     756 PRECALL                  1
+                     760 CALL                     1
+                     770 STORE_FAST              22 (gene_pattern_q25)
+         
+         168         772 PUSH_NULL
+                     774 LOAD_FAST               13 (moving_average)
+                     776 LOAD_FAST               22 (gene_pattern_q25)
+                     778 LOAD_FAST                3 (smoothing_window)
+                     780 PRECALL                  2
+                     784 CALL                     2
+                     794 STORE_FAST              22 (gene_pattern_q25)
+         
+         169         796 LOAD_FAST               20 (gene_pattern)
+                     798 LOAD_CONST              12 ('q75')
+                     800 BINARY_SUBSCR
+                     810 LOAD_CONST               3 (None)
+                     812 LOAD_CONST               3 (None)
+                     814 BUILD_SLICE              2
+                     816 LOAD_FAST               12 (gene_id)
+                     818 BUILD_TUPLE              2
+                     820 BINARY_SUBSCR
+                     830 LOAD_METHOD             15 (mean)
+                     852 LOAD_CONST               9 (1)
+                     854 KW_NAMES                10
+                     856 PRECALL                  1
+                     860 CALL                     1
+                     870 STORE_FAST              23 (gene_pattern_q75)
+         
+         170         872 PUSH_NULL
+                     874 LOAD_FAST               13 (moving_average)
+                     876 LOAD_FAST               23 (gene_pattern_q75)
+                     878 LOAD_FAST                3 (smoothing_window)
+                     880 PRECALL                  2
+                     884 CALL                     2
+                     894 STORE_FAST              23 (gene_pattern_q75)
+         
+         171         896 LOAD_FAST               20 (gene_pattern)
+                     898 LOAD_CONST              13 ('times')
+                     900 BINARY_SUBSCR
+                     910 STORE_FAST              24 (times)
+         
+         173         912 LOAD_FAST               24 (times)
+                     914 LOAD_CONST               3 (None)
+                     916 LOAD_FAST               10 (max_length)
+                     918 BUILD_SLICE              2
+                     920 BINARY_SUBSCR
+                     930 STORE_FAST              24 (times)
+         
+         174         932 LOAD_FAST               21 (gene_pattern_mean)
+                     934 LOAD_CONST               3 (None)
+                     936 LOAD_FAST               10 (max_length)
+                     938 BUILD_SLICE              2
+                     940 BINARY_SUBSCR
+                     950 STORE_FAST              21 (gene_pattern_mean)
+         
+         175         952 LOAD_FAST               22 (gene_pattern_q25)
+                     954 LOAD_CONST               3 (None)
+                     956 LOAD_FAST               10 (max_length)
+                     958 BUILD_SLICE              2
+                     960 BINARY_SUBSCR
+                     970 STORE_FAST              22 (gene_pattern_q25)
+         
+         176         972 LOAD_FAST               23 (gene_pattern_q75)
+                     974 LOAD_CONST               3 (None)
+                     976 LOAD_FAST               10 (max_length)
+                     978 BUILD_SLICE              2
+                     980 BINARY_SUBSCR
+                     990 STORE_FAST              23 (gene_pattern_q75)
+         
+         178         992 LOAD_FAST                5 (palette)
+                     994 POP_JUMP_FORWARD_IF_NONE    13 (to 1022)
+                     996 LOAD_FAST               19 (p_name)
+                     998 LOAD_FAST                5 (palette)
+                    1000 CONTAINS_OP              0
+                    1002 POP_JUMP_FORWARD_IF_FALSE     9 (to 1022)
+         
+         179        1004 LOAD_FAST                5 (palette)
+                    1006 LOAD_FAST               19 (p_name)
+                    1008 BINARY_SUBSCR
+                    1018 STORE_FAST              25 (color)
+                    1020 JUMP_FORWARD             8 (to 1038)
+         
+         181     >> 1022 LOAD_FAST               17 (default_color_palette)
+                    1024 LOAD_FAST               18 (i)
+                    1026 BINARY_SUBSCR
+                    1036 STORE_FAST              25 (color)
+         
+         183     >> 1038 LOAD_FAST               15 (start_times)
+                    1040 LOAD_METHOD             16 (append)
+                    1062 LOAD_FAST               24 (times)
+                    1064 LOAD_CONST              14 (0)
+                    1066 BINARY_SUBSCR
+                    1076 PRECALL                  1
+                    1080 CALL                     1
+                    1090 POP_TOP
+         
+         184        1092 LOAD_FAST               16 (end_times)
+                    1094 LOAD_METHOD             16 (append)
+                    1116 LOAD_FAST               24 (times)
+                    1118 LOAD_CONST              15 (-1)
+                    1120 BINARY_SUBSCR
+                    1130 PRECALL                  1
+                    1134 CALL                     1
+                    1144 POP_TOP
+         
+         186        1146 LOAD_FAST                9 (include_uncertainty)
+                    1148 POP_JUMP_FORWARD_IF_FALSE    26 (to 1202)
+         
+         187        1150 LOAD_FAST                8 (ax)
+                    1152 LOAD_METHOD             17 (fill_between)
+                    1174 LOAD_FAST               24 (times)
+                    1176 LOAD_FAST               22 (gene_pattern_q25)
+                    1178 LOAD_FAST               23 (gene_pattern_q75)
+                    1180 LOAD_FAST               25 (color)
+                    1182 LOAD_CONST              16 (0.3)
+                    1184 KW_NAMES                17
+                    1186 PRECALL                  5
+                    1190 CALL                     5
+                    1200 POP_TOP
+         
+         188     >> 1202 LOAD_FAST                8 (ax)
+                    1204 LOAD_METHOD             18 (plot)
+                    1226 LOAD_FAST               24 (times)
+                    1228 LOAD_FAST               21 (gene_pattern_mean)
+                    1230 LOAD_FAST               19 (p_name)
+                    1232 LOAD_FAST               25 (color)
+                    1234 LOAD_CONST              18 (3)
+                    1236 KW_NAMES                19
+                    1238 PRECALL                  5
+                    1242 CALL                     5
+                    1252 POP_TOP
+                    1254 EXTENDED_ARG             1
+                    1256 JUMP_BACKWARD          362 (to 534)
+         
+         189     >> 1258 LOAD_FAST                4 (cell_type_key)
+                    1260 POP_JUMP_FORWARD_IF_NONE    49 (to 1360)
+         
+         190        1262 LOAD_FAST               11 (cell_type_band_pattern_names)
+                    1264 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 1270)
+         
+         191        1266 LOAD_FAST                6 (pattern_names)
+                    1268 STORE_FAST              11 (cell_type_band_pattern_names)
+         
+         192     >> 1270 LOAD_GLOBAL             29 (NULL + enumerate)
+                    1282 LOAD_FAST               11 (cell_type_band_pattern_names)
+                    1284 PRECALL                  1
+                    1288 CALL                     1
+                    1298 GET_ITER
+                 >> 1300 FOR_ITER                29 (to 1360)
+                    1302 UNPACK_SEQUENCE          2
+                    1306 STORE_FAST              18 (i)
+                    1308 STORE_FAST              19 (p_name)
+         
+         193        1310 LOAD_GLOBAL             39 (NULL + _add_cell_type_band)
+                    1322 LOAD_DEREF               0 (adata)
+                    1324 LOAD_FAST               19 (p_name)
+                    1326 LOAD_FAST                4 (cell_type_key)
+                    1328 LOAD_FAST                8 (ax)
+                    1330 LOAD_FAST                5 (palette)
+                    1332 LOAD_FAST               18 (i)
+                    1334 LOAD_CONST               9 (1)
+                    1336 BINARY_OP                0 (+)
+                    1340 KW_NAMES                20
+                    1342 PRECALL                  6
+                    1346 CALL                     6
+                    1356 POP_TOP
+                    1358 JUMP_BACKWARD           30 (to 1300)
+         
+         195     >> 1360 LOAD_FAST                2 (crop_to_min_length)
+                    1362 POP_JUMP_FORWARD_IF_FALSE    49 (to 1462)
+         
+         196        1364 LOAD_FAST                8 (ax)
+                    1366 LOAD_METHOD             20 (set_xlim)
+                    1388 LOAD_GLOBAL             43 (NULL + max)
+                    1400 LOAD_FAST               15 (start_times)
+                    1402 PRECALL                  1
+                    1406 CALL                     1
+                    1416 LOAD_GLOBAL             45 (NULL + min)
+                    1428 LOAD_FAST               16 (end_times)
+                    1430 PRECALL                  1
+                    1434 CALL                     1
+                    1444 PRECALL                  2
+                    1448 CALL                     2
+                    1458 POP_TOP
+                    1460 JUMP_FORWARD            48 (to 1558)
+         
+         198     >> 1462 LOAD_FAST                8 (ax)
+                    1464 LOAD_METHOD             20 (set_xlim)
+                    1486 LOAD_GLOBAL             45 (NULL + min)
+                    1498 LOAD_FAST               15 (start_times)
+                    1500 PRECALL                  1
+                    1504 CALL                     1
+                    1514 LOAD_GLOBAL             43 (NULL + max)
+                    1526 LOAD_FAST               16 (end_times)
+                    1528 PRECALL                  1
+                    1532 CALL                     1
+                    1542 PRECALL                  2
+                    1546 CALL                     2
+                    1556 POP_TOP
+         
+         200     >> 1558 LOAD_FAST                8 (ax)
+                    1560 LOAD_METHOD             23 (set_xticks)
+                    1582 BUILD_LIST               0
+                    1584 PRECALL                  1
+                    1588 CALL                     1
+                    1598 POP_TOP
+         
+         201        1600 LOAD_FAST                8 (ax)
+                    1602 LOAD_METHOD             24 (set_xlabel)
+                    1624 LOAD_CONST              21 ('Decipher time')
+                    1626 LOAD_CONST              22 (14)
+                    1628 KW_NAMES                23
+                    1630 PRECALL                  2
+                    1634 CALL                     2
+                    1644 POP_TOP
+         
+         202        1646 LOAD_FAST                8 (ax)
+                    1648 LOAD_METHOD             25 (set_ylabel)
+                    1670 LOAD_CONST              24 ('Gene expression')
+                    1672 LOAD_CONST              22 (14)
+                    1674 KW_NAMES                23
+                    1676 PRECALL                  2
+                    1680 CALL                     2
+                    1690 POP_TOP
+         
+         203        1692 LOAD_FAST                8 (ax)
+                    1694 LOAD_METHOD             26 (set_ylim)
+                    1716 LOAD_CONST              14 (0)
+                    1718 PRECALL                  1
+                    1722 CALL                     1
+                    1732 POP_TOP
+         
+         204        1734 LOAD_FAST                8 (ax)
+                    1736 LOAD_METHOD             27 (legend)
+                    1758 LOAD_CONST              25 (False)
+                    1760 KW_NAMES                26
+                    1762 PRECALL                  1
+                    1766 CALL                     1
+                    1776 POP_TOP
+         
+         205        1778 LOAD_FAST                8 (ax)
+                    1780 LOAD_METHOD             28 (set_title)
+                    1802 LOAD_FAST                1 (gene_name)
+                    1804 LOAD_CONST              27 (18)
+                    1806 KW_NAMES                23
+                    1808 PRECALL                  2
+                    1812 CALL                     2
+                    1822 POP_TOP
          
-         204        1836 LOAD_FAST               14 (fig)
-                    1838 RETURN_VALUE
+         207        1824 LOAD_FAST               14 (fig)
+                    1826 RETURN_VALUE
          consts
             'Plot the gene patterns over the Decipher time.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n    gene_name : str or list of str\n        The name(s) of the gene(s) to plot.\n    crop_to_min_length : bool, default False\n        Crop the plot to the minimum length of the gene patterns.\n    smoothing_window : int, default 5\n        The size of the window for the moving average smoothing.\n    cell_type_key : str, optional\n        The key of the cell type annotations in `adata.obs`. If provided, the cell types will be\n        plotted as colored bands on the x-axis. See `cell_type_band_pattern_names` for more details.\n    palette : dict, optional\n        A dictionary mapping pattern names and cell type names to colors.\n    pattern_names : str or list of str, optional\n        The names of the gene patterns to plot. If None, plot all gene patterns.\n    figsize : tuple of float, default (3, 2.3)\n        The size of the figure.\n    ax : matplotlib.pyplot.Axes, optional\n        The axes on which to plot. If None, create a new figure and axes.\n    include_uncertainty : bool, default True\n        Whether to include the uncertainty of the gene patterns in the plot, as a shaded area.\n    max_length : int, optional\n        The maximum length of the gene patterns to plot. If None, plot the full length, up to the\n        minimum length of the gene patterns if `crop_to_min_length` is True.\n    cell_type_band_pattern_names : str or list of str, optional\n        The names of the gene patterns to use for the cell type bands. If None, use the same gene\n        patterns as `pattern_names`. It is useful to use a subset of the gene patterns to avoid\n        multiple bands.\n    '
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 19
                code
                   0x9501970067007c005d2e7d0189026a000000000000000000a001000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00a00200000000000000000000000000000000000000007c01a6010000ab
                   01000000000000000091028c2f5300
                              0 COPY_FREE_VARS           1
                
-               138           2 RESUME                   0
+               141           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                46 (to 102)
                             10 STORE_FAST               1 (gn)
                             12 LOAD_DEREF               2 (adata)
                             14 LOAD_ATTR                0 (var_names)
                             24 LOAD_METHOD              1 (tolist)
@@ -931,34 +930,34 @@
                            100 JUMP_BACKWARD           47 (to 8)
                        >>  102 RETURN_VALUE
                consts
                names      ('var_names', 'tolist', 'index')
                varnames   ('.0', 'gn')
                freevars   ('adata',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
                name       '<listcomp>'
-               firstlineno 138
+               firstlineno 141
                lnotab 0x
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 7
                flags     : 19
                code
                   0x97007401000000000000000000006a0100000000000000007c00740100
                   0000000000000000006a0200000000000000007c01a6010000ab01000000
                   00000000006401a6030000ab030000000000000000740100000000000000
                   0000006a0100000000000000007401000000000000000000006a03000000
                   00000000007c00a6010000ab010000000000000000740100000000000000
                   0000006a0200000000000000007c01a6010000ab01000000000000000064
                   01a6030000ab0300000000000000007a0b00005300
-               142           0 RESUME                   0
+               145           0 RESUME                   0
                
-               143           2 LOAD_GLOBAL              1 (NULL + np)
+               146           2 LOAD_GLOBAL              1 (NULL + np)
                             14 LOAD_ATTR                1 (convolve)
                             24 LOAD_FAST                0 (x)
                             26 LOAD_GLOBAL              1 (NULL + np)
                             38 LOAD_ATTR                2 (ones)
                             48 LOAD_FAST                1 (w)
                             50 PRECALL                  1
                             54 CALL                     1
@@ -985,17 +984,17 @@
                consts
                   None
                   'same'
                names      ('np', 'convolve', 'ones', 'ones_like')
                varnames   ('x', 'w')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
                name       'moving_average'
-               firstlineno 142
+               firstlineno 145
                lnotab 0x0201
             None
             'decipher'
             'gene_patterns'
             ('figsize',)
             ('n_colors',)
             'mean'
@@ -1014,37 +1013,37 @@
             'Decipher time'
             14
             ('fontsize',)
             'Gene expression'
             False
             ('frameon',)
             18
-         names      ('type', 'list', 'var_names', 'tolist', 'index', 'uns', 'keys', 'str', 'plt', 'figure', 'gca', 'sns', 'color_palette', 'len', 'enumerate', 'mean', 'append', 'fill_between', 'plot', '_add_cell_type_band', 'set_xlim', 'max', 'min', 'set_xticks', 'set_xlabel', 'set_ylabel', 'set_ylim', 'legend', 'set_title')
+         names      ('isinstance', 'list', 'var_names', 'tolist', 'index', 'uns', 'keys', 'str', 'plt', 'figure', 'gca', 'sns', 'color_palette', 'len', 'enumerate', 'mean', 'append', 'fill_between', 'plot', '_add_cell_type_band', 'set_xlim', 'max', 'min', 'set_xticks', 'set_xlabel', 'set_ylabel', 'set_ylim', 'legend', 'set_title')
          varnames   ('adata', 'gene_name', 'crop_to_min_length', 'smoothing_window', 'cell_type_key', 'palette', 'pattern_names', 'figsize', 'ax', 'include_uncertainty', 'max_length', 'cell_type_band_pattern_names', 'gene_id', 'moving_average', 'fig', 'start_times', 'end_times', 'default_color_palette', 'i', 'p_name', 'gene_pattern', 'gene_pattern_mean', 'gene_pattern_q25', 'gene_pattern_q75', 'times', 'color')
          freevars   ()
          cellvars   ('adata',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
          name       'gene_patterns'
-         firstlineno 90
+         firstlineno 93
          lnotab
-            0x042f30011e025a020603040166013001060204012a012a020e01040104
+            0x042f2a011e025a020603040166012a01060204012a012a020e01040104
             0244012a0132024c0118014c0118014c011801100214011401140114020c
             011202100236013602040134013801040104010401280132020401620260
             022a012e012e012a012c012e02
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 11
          code
             0x97007401000000000000000000007c006401660269007c01a4018e0153
             00
-         207           0 RESUME                   0
+         210           0 RESUME                   0
          
-         222           2 LOAD_GLOBAL              1 (NULL + plot_decipher_v)
+         225           2 LOAD_GLOBAL              1 (NULL + plot_decipher_v)
                       14 LOAD_FAST                0 (adata)
                       16 LOAD_CONST               1 ('decipher_time')
                       18 BUILD_TUPLE              2
                       20 BUILD_MAP                0
                       22 LOAD_FAST                1 (kwargs)
                       24 DICT_MERGE               1
                       26 CALL_FUNCTION_EX         1
@@ -1052,17 +1051,17 @@
          consts
             'Plot the Decipher time over the Decipher v space.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n    **kwargs : dict\n        Keyword arguments passed to `dc.pl.decipher` and ultimately to `sc.pl.embedding`.\n\n    Returns\n    -------\n    fig : matplotlib.pyplot.Figure\n        The matplotlib figure.\n    '
             'decipher_time'
          names      ('plot_decipher_v',)
          varnames   ('adata', 'kwargs')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
          name       'decipher_time'
-         firstlineno 207
+         firstlineno 210
          lnotab 0x020f
       50
       1
       code
          argcount  : 7
          nlocals   : 12
          stacksize : 10
@@ -1095,57 +1094,57 @@
             0064116412741f000000000000000000006a120000000000000000a60000
             00ab000000000000000000a0130000000000000000000000000000000000
             000000a6000000ab00000000000000000064136400ac14a6080000ab0800
             000000000000000100641564157c067a0500007a0000007c036a14000000
             00000000005f15000000000000000064005300
                        0 MAKE_CELL                4 (palette)
          
-         225           2 RESUME                   0
+         228           2 RESUME                   0
          
-         228           4 LOAD_FAST                0 (adata)
+         231           4 LOAD_FAST                0 (adata)
                        6 LOAD_ATTR                0 (uns)
                       16 LOAD_CONST               1 ('decipher')
                       18 BINARY_SUBSCR
                       28 LOAD_CONST               2 ('trajectories')
                       30 BINARY_SUBSCR
                       40 LOAD_FAST                1 (trajectory_name)
                       42 BINARY_SUBSCR
                       52 STORE_FAST               7 (trajectory)
          
-         230          54 LOAD_CONST               3 ('cell_types')
+         233          54 LOAD_CONST               3 ('cell_types')
                       56 LOAD_FAST                7 (trajectory)
                       58 CONTAINS_OP              1
                       60 POP_JUMP_FORWARD_IF_TRUE    36 (to 134)
          
-         231          62 LOAD_FAST                7 (trajectory)
+         234          62 LOAD_FAST                7 (trajectory)
                       64 LOAD_CONST               3 ('cell_types')
                       66 BINARY_SUBSCR
                       76 LOAD_CONST               4 ('key')
                       78 BINARY_SUBSCR
                       88 LOAD_FAST                2 (cell_type_key)
                       90 COMPARE_OP               3 (!=)
                       96 POP_JUMP_FORWARD_IF_TRUE    18 (to 134)
          
-         232          98 LOAD_FAST                7 (trajectory)
+         235          98 LOAD_FAST                7 (trajectory)
                      100 LOAD_CONST               3 ('cell_types')
                      102 BINARY_SUBSCR
                      112 LOAD_CONST               5 ('n_neighbors')
                      114 BINARY_SUBSCR
                      124 LOAD_FAST                5 (n_neighbors)
                      126 COMPARE_OP               3 (!=)
                      132 POP_JUMP_FORWARD_IF_FALSE   102 (to 338)
          
-         234     >>  134 LOAD_GLOBAL              3 (NULL + KNeighborsClassifier)
+         237     >>  134 LOAD_GLOBAL              3 (NULL + KNeighborsClassifier)
                      146 LOAD_FAST                5 (n_neighbors)
                      148 KW_NAMES                 6
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_FAST               8 (knc)
          
-         235         166 LOAD_FAST                8 (knc)
+         238         166 LOAD_FAST                8 (knc)
                      168 LOAD_METHOD              2 (fit)
                      190 LOAD_FAST                0 (adata)
                      192 LOAD_ATTR                3 (obsm)
                      202 LOAD_FAST                7 (trajectory)
                      204 LOAD_CONST               7 ('rep_key')
                      206 BINARY_SUBSCR
                      216 BINARY_SUBSCR
@@ -1153,65 +1152,65 @@
                      228 LOAD_ATTR                4 (obs)
                      238 LOAD_FAST                2 (cell_type_key)
                      240 BINARY_SUBSCR
                      250 PRECALL                  2
                      254 CALL                     2
                      264 POP_TOP
          
-         236         266 LOAD_FAST                8 (knc)
+         239         266 LOAD_FAST                8 (knc)
                      268 LOAD_METHOD              5 (predict)
                      290 LOAD_FAST                7 (trajectory)
                      292 LOAD_CONST               8 ('points')
                      294 BINARY_SUBSCR
                      304 PRECALL                  1
                      308 CALL                     1
                      318 STORE_FAST               9 (cell_types)
          
-         238         320 LOAD_FAST                2 (cell_type_key)
+         241         320 LOAD_FAST                2 (cell_type_key)
          
-         239         322 LOAD_FAST                5 (n_neighbors)
+         242         322 LOAD_FAST                5 (n_neighbors)
          
-         240         324 LOAD_FAST                9 (cell_types)
+         243         324 LOAD_FAST                9 (cell_types)
          
-         237         326 LOAD_CONST               9 (('key', 'n_neighbors', 'values'))
+         240         326 LOAD_CONST               9 (('key', 'n_neighbors', 'values'))
                      328 BUILD_CONST_KEY_MAP      3
                      330 LOAD_FAST                7 (trajectory)
                      332 LOAD_CONST               3 ('cell_types')
                      334 STORE_SUBSCR
          
-         243     >>  338 LOAD_FAST                7 (trajectory)
+         246     >>  338 LOAD_FAST                7 (trajectory)
                      340 LOAD_CONST              10 ('times')
                      342 BINARY_SUBSCR
                      352 STORE_FAST              10 (times)
          
-         244         354 LOAD_FAST                7 (trajectory)
+         247         354 LOAD_FAST                7 (trajectory)
                      356 LOAD_CONST               3 ('cell_types')
                      358 BINARY_SUBSCR
                      368 LOAD_CONST              11 ('values')
                      370 BINARY_SUBSCR
                      380 STORE_FAST               9 (cell_types)
          
-         246         382 LOAD_DEREF               4 (palette)
+         249         382 LOAD_DEREF               4 (palette)
                      384 POP_JUMP_FORWARD_IF_NOT_NONE   101 (to 588)
          
-         247         386 LOAD_GLOBAL             13 (NULL + logging)
+         250         386 LOAD_GLOBAL             13 (NULL + logging)
                      398 LOAD_ATTR                7 (info)
                      408 LOAD_CONST              12 ('No palette provided for the cell types, using default.')
                      410 PRECALL                  1
                      414 CALL                     1
                      424 POP_TOP
          
-         248         426 LOAD_GLOBAL             17 (NULL + np)
+         251         426 LOAD_GLOBAL             17 (NULL + np)
                      438 LOAD_ATTR                9 (unique)
                      448 LOAD_FAST                9 (cell_types)
                      450 PRECALL                  1
                      454 CALL                     1
                      464 STORE_FAST              11 (ct)
          
-         249         466 LOAD_GLOBAL             21 (NULL + dict)
+         252         466 LOAD_GLOBAL             21 (NULL + dict)
                      478 LOAD_GLOBAL             23 (NULL + zip)
                      490 LOAD_FAST               11 (ct)
                      492 LOAD_GLOBAL             25 (NULL + sns)
                      504 LOAD_ATTR               13 (color_palette)
                      514 LOAD_GLOBAL             29 (NULL + len)
                      526 LOAD_FAST               11 (ct)
                      528 PRECALL                  1
@@ -1221,65 +1220,65 @@
                      548 CALL                     1
                      558 PRECALL                  2
                      562 CALL                     2
                      572 PRECALL                  1
                      576 CALL                     1
                      586 STORE_DEREF              4 (palette)
          
-         251     >>  588 LOAD_GLOBAL             31 (NULL + plt)
+         254     >>  588 LOAD_GLOBAL             31 (NULL + plt)
                      600 LOAD_ATTR               16 (scatter)
          
-         252         610 LOAD_FAST               10 (times)
+         255         610 LOAD_FAST               10 (times)
          
-         253         612 LOAD_GLOBAL             17 (NULL + np)
+         256         612 LOAD_GLOBAL             17 (NULL + np)
                      624 LOAD_ATTR               17 (zeros)
                      634 LOAD_GLOBAL             29 (NULL + len)
                      646 LOAD_FAST               10 (times)
                      648 PRECALL                  1
                      652 CALL                     1
                      662 PRECALL                  1
                      666 CALL                     1
                      676 LOAD_CONST              14 (0.05)
                      678 LOAD_FAST                6 (offset)
                      680 BINARY_OP                5 (*)
                      684 BINARY_OP               10 (-)
                      688 LOAD_CONST              15 (0.025)
                      690 BINARY_OP                0 (+)
          
-         254         694 LOAD_CLOSURE             4 (palette)
+         257         694 LOAD_CLOSURE             4 (palette)
                      696 BUILD_TUPLE              1
-                     698 LOAD_CONST              16 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py", line 254>)
+                     698 LOAD_CONST              16 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py", line 257>)
                      700 MAKE_FUNCTION            8 (closure)
                      702 LOAD_FAST                9 (cell_types)
                      704 GET_ITER
                      706 PRECALL                  0
                      710 CALL                     0
          
-         255         720 LOAD_CONST              17 ('s')
+         258         720 LOAD_CONST              17 ('s')
          
-         256         722 LOAD_CONST              18 (20)
+         259         722 LOAD_CONST              18 (20)
          
-         257         724 LOAD_GLOBAL             31 (NULL + plt)
+         260         724 LOAD_GLOBAL             31 (NULL + plt)
                      736 LOAD_ATTR               18 (gca)
                      746 PRECALL                  0
                      750 CALL                     0
                      760 LOAD_METHOD             19 (get_xaxis_transform)
                      782 PRECALL                  0
                      786 CALL                     0
          
-         258         796 LOAD_CONST              19 (False)
+         261         796 LOAD_CONST              19 (False)
          
-         259         798 LOAD_CONST               0 (None)
+         262         798 LOAD_CONST               0 (None)
          
-         251         800 KW_NAMES                20
+         254         800 KW_NAMES                20
                      802 PRECALL                  8
                      806 CALL                     8
                      816 POP_TOP
          
-         261         818 LOAD_CONST              21 (5)
+         264         818 LOAD_CONST              21 (5)
                      820 LOAD_CONST              21 (5)
                      822 LOAD_FAST                6 (offset)
                      824 BINARY_OP                5 (*)
                      828 BINARY_OP                0 (+)
                      832 LOAD_FAST                3 (ax)
                      834 LOAD_ATTR               20 (xaxis)
                      844 STORE_ATTR              21 (labelpad)
@@ -1308,15 +1307,15 @@
                stacksize : 4
                flags     : 19
                code
                   0x9501970067007c005d0a7d0189027c011900000000000000000091028c
                   0b5300
                              0 COPY_FREE_VARS           1
                
-               254           2 RESUME                   0
+               257           2 RESUME                   0
                              4 BUILD_LIST               0
                              6 LOAD_FAST                0 (.0)
                        >>    8 FOR_ITER                10 (to 30)
                             10 STORE_FAST               1 (c)
                             12 LOAD_DEREF               2 (palette)
                             14 LOAD_FAST                1 (c)
                             16 BINARY_SUBSCR
@@ -1324,41 +1323,41 @@
                             28 JUMP_BACKWARD           11 (to 8)
                        >>   30 RETURN_VALUE
                consts
                names      ()
                varnames   ('.0', 'c')
                freevars   ('palette',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
                name       '<listcomp>'
-               firstlineno 254
+               firstlineno 257
                lnotab 0x
             's'
             20
             False
             ('c', 'marker', 's', 'transform', 'clip_on', 'edgecolors')
             5
          names      ('uns', 'KNeighborsClassifier', 'fit', 'obsm', 'obs', 'predict', 'logging', 'info', 'np', 'unique', 'dict', 'zip', 'sns', 'color_palette', 'len', 'plt', 'scatter', 'zeros', 'gca', 'get_xaxis_transform', 'xaxis', 'labelpad')
          varnames   ('adata', 'trajectory_name', 'cell_type_key', 'ax', 'palette', 'n_neighbors', 'offset', 'trajectory', 'knc', 'cell_types', 'times', 'ct')
          freevars   ()
          cellvars   ('palette',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
          name       '_add_cell_type_band'
-         firstlineno 225
+         firstlineno 228
          lnotab
             0x040332020801240124022001640136020201020102fd0c0610011c0204
             01280128017a021601020152011a01020102014801020102f8120a
       ('on data', 10)
       (None, None, None)
       (False, 5, None, None, None, (3, 2.3), None, True, None, None)
       (50, 1)
    names      ('logging', 'matplotlib.patheffects', 'patheffects', 'pe', 'numpy', 'np', 'seaborn', 'sns', 'matplotlib', 'pyplot', 'plt', 'sklearn.neighbors', 'KNeighborsClassifier', 'decipher.plot.decipher', 'decipher', 'plot_decipher_v', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'cell_clusters', 'trajectories', 'gene_patterns', 'decipher_time', '_add_cell_type_band')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/plot/trajectory_inference.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/plot/trajectory_inference.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108020c01080108010c010c020c0220010e0102010cfe120608
-      080201020102fc084502010201020102010201020102010201020102f408
+      0b0201020102fc084502010201020102010201020102010201020102f408
       75061302ff
```

### Comparing `scdecipher-0.1.0/decipher/plot/__pycache__/utils.cpython-311.pyc` & `scdecipher-0.1.2/decipher/plot/__pycache__/utils.cpython-311.pyc`

 * *Files 12% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,19 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
+moddate:  0x7d19d665 (Wed Feb 21 15:40:45 2024 UTC)
 files sz: 541
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 1
    flags     : 0
    code 0x9700640084005a0064015300
      0           0 RESUME                   0
    
-     1           2 LOAD_CONST               0 (<code object activate_journal_quality, file "/Users/achille/Documents/decipher-pip/decipher/plot/utils.py", line 1>)
+     1           2 LOAD_CONST               0 (<code object activate_journal_quality, file "/Users/achille/Documents/decipher_dev/decipher/plot/utils.py", line 1>)
                  4 MAKE_FUNCTION            0
                  6 STORE_NAME               0 (activate_journal_quality)
                  8 LOAD_CONST               1 (None)
                 10 RETURN_VALUE
    consts
       code
          argcount  : 0
@@ -89,20 +89,20 @@
             'ps.fonttype'
             False
             'axes.grid'
          names      ('matplotlib.pyplot', 'pyplot', 'scanpy', 'matplotlib', 'settings', 'set_figure_params', 'rcParams')
          varnames   ('plt', 'sc', 'mpl')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/plot/utils.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/plot/utils.py'
          name       'activate_journal_quality'
          firstlineno 1
          lnotab 0x02060c01080108023a0114011402
       None
    names      ('activate_journal_quality',)
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/plot/utils.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/plot/utils.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff0201
```

### Comparing `scdecipher-0.1.0/decipher/plot/basis_decomposition.py` & `scdecipher-0.1.2/decipher/plot/basis_decomposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import numpy as np
 import seaborn as sns
 from matplotlib import pyplot as plt
 
+from .trajectory_inference import gene_patterns as plot_gene_patterns
+
 
 def basis(adata, colors=None, figsize=(5, 2.5), linewidth=3, ax=None):
     """Plot the basis functions learned by the basis decomposition.
 
     Parameters
     ----------
     adata : sc.AnnData
@@ -39,17 +41,14 @@
             label="basis %d" % (i + 1),
             linewidth=linewidth[i],
         )
     ax.legend(loc="right", bbox_to_anchor=(1.35, 0.5), fancybox=False)
     return fig
 
 
-from .trajectory_inference import gene_patterns as plot_gene_patterns
-
-
 def gene_patterns_decomposition(
     adata,
     gene_name,
     pattern_name,
     palette=None,
     basis_colors=None,
     figsize=(7, 2),
@@ -78,15 +77,15 @@
     axes[1].get_legend().remove()
 
     ax = axes[2]
     ax.barh(y=range(n_basis)[::-1], width=beta, color=basis_colors)
 
     ax.set_yticks(range(n_basis)[::-1])
     ax.set_xlim(0, 1)
-    ax.set_yticklabels([f"$\\beta_%d$" % i for i in range(n_basis)], fontsize=12)
+    ax.set_yticklabels(["$\\beta_%d$" % i for i in range(n_basis)], fontsize=12)
 
     for ax in axes:
         ax.set_xticks([])
 
     return fig
 
 
@@ -99,15 +98,15 @@
 ):
     if sort_by in ["shape", "combined", "scale"]:
         gene_names = sorted(
             gene_names,
             key=lambda gn: np.mean(adata.uns["decipher"]["disruption_scores"].loc[gn, sort_by]),
         )
     fig, axs = plt.subplots(2, 1, figsize=figsize, sharex="col")
-    for (ax, col) in zip(axs, ["shape", "combined"]):
+    for ax, col in zip(axs, ["shape", "combined"]):
         sns.boxplot(
             data=adata.uns["decipher"]["disruption_scores_samples"],
             x="gene",
             y=col,
             order=gene_names,
             palette=color_palette,
             whis=(0, 100),
```

### Comparing `scdecipher-0.1.0/decipher/plot/decipher.py` & `scdecipher-0.1.2/decipher/plot/decipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
             return_fig=True,
             frameon=(axis_type in ["line", "arrow"]),
             ncols=ncols,
             vmax=vmax if color is not None else None,
             **kwargs,
         )
     ax = fig.axes[0]
-    if color is None or type(color) == str:
+    if color is None or isinstance(color, str):
         color = [color]
 
     if len(color) == 1:
         ax.set_title(title)
 
     for i, ax in enumerate(fig.axes):
         if ax._label == "<colorbar>":
```

### Comparing `scdecipher-0.1.0/decipher/plot/trajectory_inference.py` & `scdecipher-0.1.2/decipher/plot/trajectory_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,18 @@
     format="%(asctime)s | %(levelname)s : %(message)s",
     level=logging.INFO,
 )
 
 
 def cell_clusters(adata, legend_loc="on data", legend_fontsize=10):
     return plot_decipher_v(
-        adata, color="decipher_clusters", legend_loc=legend_loc, legend_fontsize=legend_fontsize
+        adata,
+        color="decipher_clusters",
+        legend_loc=legend_loc,
+        legend_fontsize=legend_fontsize,
     )
 
 
 def trajectories(
     adata,
     color=None,
     trajectory_names=None,
@@ -52,15 +55,15 @@
     dc.pl.decipher
     sc.pl.embedding
     """
     fig = plot_decipher_v(adata, color=color, palette=palette)
     ax = fig.axes[0]
     if trajectory_names is None:
         trajectory_names = adata.uns["decipher"]["trajectories"].keys()
-    if type(trajectory_names) == str:
+    if isinstance(trajectory_names, str):
         trajectory_names = [trajectory_names]
 
     default_color_palette = sns.color_palette(n_colors=len(trajectory_names))
     for i, t_name in enumerate(trajectory_names):
         cluster_locations = adata.uns["decipher"]["trajectories"][t_name]["cluster_locations"]
         if palette is not None and t_name in palette:
             color = palette[t_name]
@@ -130,25 +133,25 @@
         The maximum length of the gene patterns to plot. If None, plot the full length, up to the
         minimum length of the gene patterns if `crop_to_min_length` is True.
     cell_type_band_pattern_names : str or list of str, optional
         The names of the gene patterns to use for the cell type bands. If None, use the same gene
         patterns as `pattern_names`. It is useful to use a subset of the gene patterns to avoid
         multiple bands.
     """
-    if type(gene_name) == list:
+    if isinstance(gene_name, list):
         gene_id = [adata.var_names.tolist().index(gn) for gn in gene_name]
     else:
         gene_id = [adata.var_names.tolist().index(gene_name)]
 
     def moving_average(x, w):
         return np.convolve(x, np.ones(w), "same") / np.convolve(np.ones_like(x), np.ones(w), "same")
 
     if pattern_names is None:
         pattern_names = list(adata.uns["decipher"]["gene_patterns"].keys())
-    elif type(pattern_names) == str:
+    elif isinstance(pattern_names, str):
         pattern_names = [pattern_names]
 
     if ax is None:
         fig = plt.figure(figsize=figsize)
         ax = fig.gca()
     else:
         fig = ax.figure
```

### Comparing `scdecipher-0.1.0/decipher/plot/utils.py` & `scdecipher-0.1.2/decipher/plot/utils.py`

 * *Files identical despite different names*

### Comparing `scdecipher-0.1.0/decipher/tools/__pycache__/__init__.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/__pycache__/__init__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x8c985265 (Mon Nov 13 21:43:40 2023 UTC)
-files sz: 506
+moddate:  0x8c232166 (Thu Apr 18 13:43:40 2024 UTC)
+files sz: 839
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a056d
       065a060100640064026c076d075a076d085a080100640364046c096d0a5a
       0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064056c0e6d0f5a0f0100640064
-      066c106d115a11010064075300
+      066c106d115a11010067006407a2015a1264085300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (1)
                  4 LOAD_CONST               1 (('cell_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns', 'TConfig'))
                  6 IMPORT_NAME              0 (trajectory_inference)
                  8 IMPORT_FROM              1 (cell_clusters)
                 10 STORE_NAME               1 (cell_clusters)
@@ -61,26 +61,32 @@
    
     17          86 LOAD_CONST               0 (1)
                 88 LOAD_CONST               6 (('DecipherConfig',))
                 90 IMPORT_NAME             16 (_decipher.decipher)
                 92 IMPORT_FROM             17 (DecipherConfig)
                 94 STORE_NAME              17 (DecipherConfig)
                 96 POP_TOP
-                98 LOAD_CONST               7 (None)
-               100 RETURN_VALUE
+   
+    19          98 BUILD_LIST               0
+               100 LOAD_CONST               7 (('cell_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns', 'basis_decomposition', 'disruption_scores', 'decipher_train', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance', 'decipher_load_model', 'DecipherConfig', 'TConfig'))
+               102 LIST_EXTEND              1
+               104 STORE_NAME              18 (__all__)
+               106 LOAD_CONST               8 (None)
+               108 RETURN_VALUE
    consts
       1
       ('cell_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns', 'TConfig')
       ('basis_decomposition', 'disruption_scores')
       0
       ('decipher_train', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance')
       ('decipher_load_model',)
       ('DecipherConfig',)
+      ('cell_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns', 'basis_decomposition', 'disruption_scores', 'decipher_train', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance', 'decipher_load_model', 'DecipherConfig', 'TConfig')
       None
-   names      ('trajectory_inference', 'cell_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns', 'TConfig', 'basis_decomposition', 'disruption_scores', 'decipher.tools.decipher', 'decipher_train', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance', '_decipher.data', 'decipher_load_model', '_decipher.decipher', 'DecipherConfig')
+   names      ('trajectory_inference', 'cell_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns', 'TConfig', 'basis_decomposition', 'disruption_scores', 'decipher.tools.decipher', 'decipher_train', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance', '_decipher.data', 'decipher_load_model', '_decipher.decipher', 'DecipherConfig', '__all__')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/__init__.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02012008100118060c01
+   lnotab 0x00ff02012008100118060c010c02
```

### Comparing `scdecipher-0.1.0/decipher/tools/__pycache__/basis_decomposition.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/__pycache__/basis_decomposition.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x1d905265 (Mon Nov 13 21:07:41 2023 UTC)
-files sz: 9203
+moddate:  0x24232166 (Thu Apr 18 13:41:56 2024 UTC)
+files sz: 9211
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064016c035a04640064
@@ -86,20 +86,20 @@
     26         152 NOP
    
     27         154 NOP
    
     28         156 NOP
    
     20         158 LOAD_CONST              14 ((None, 5, 10000, 0.005, 1, 0, -1))
-               160 LOAD_CONST              12 (<code object basis_decomposition, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 20>)
+               160 LOAD_CONST              12 (<code object basis_decomposition, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 20>)
                162 MAKE_FUNCTION            1 (defaults)
                164 STORE_NAME              18 (basis_decomposition)
    
    124         166 LOAD_CONST              15 ((0, 1))
-               168 LOAD_CONST              13 (<code object disruption_scores, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 124>)
+               168 LOAD_CONST              13 (<code object disruption_scores, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 124>)
                170 MAKE_FUNCTION            1 (defaults)
                172 STORE_NAME              19 (disruption_scores)
                174 LOAD_CONST               1 (None)
                176 RETURN_VALUE
    consts
       0
       None
@@ -207,38 +207,38 @@
                      188 CALL                     0
                      198 PRECALL                  1
                      202 CALL                     1
                      212 STORE_FAST               1 (pattern_names)
          
           78     >>  214 LOAD_CLOSURE             0 (adata)
                      216 BUILD_TUPLE              1
-                     218 LOAD_CONST               7 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 78>)
+                     218 LOAD_CONST               7 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 78>)
                      220 MAKE_FUNCTION            8 (closure)
          
           79         222 LOAD_FAST                1 (pattern_names)
          
           78         224 GET_ITER
                      226 PRECALL                  0
                      230 CALL                     0
                      240 STORE_FAST               8 (gene_patterns)
          
           81         242 LOAD_GLOBAL             13 (NULL + min)
-                     254 LOAD_CONST               8 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 81>)
+                     254 LOAD_CONST               8 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 81>)
                      256 MAKE_FUNCTION            0
                      258 LOAD_FAST                8 (gene_patterns)
                      260 GET_ITER
                      262 PRECALL                  0
                      266 CALL                     0
                      276 PRECALL                  1
                      280 CALL                     1
                      290 STORE_DEREF             20 (min_len)
          
           82         292 LOAD_CLOSURE            20 (min_len)
                      294 BUILD_TUPLE              1
-                     296 LOAD_CONST               9 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 82>)
+                     296 LOAD_CONST               9 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 82>)
                      298 MAKE_FUNCTION            8 (closure)
                      300 LOAD_FAST                8 (gene_patterns)
                      302 GET_ITER
                      304 PRECALL                  0
                      308 CALL                     0
                      318 STORE_FAST               8 (gene_patterns)
          
@@ -384,15 +384,15 @@
                     1038 PRECALL                  0
                     1042 CALL                     0
          
          111        1052 LOAD_DEREF              20 (min_len)
          
          112        1054 LOAD_CLOSURE            21 (samples)
                     1056 BUILD_TUPLE              1
-                    1058 LOAD_CONST              18 (<code object <dictcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 112>)
+                    1058 LOAD_CONST              18 (<code object <dictcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 112>)
                     1060 MAKE_FUNCTION            8 (closure)
          
          114        1062 LOAD_GLOBAL             35 (NULL + enumerate)
                     1074 LOAD_FAST                1 (pattern_names)
                     1076 PRECALL                  1
                     1080 CALL                     1
          
@@ -485,15 +485,15 @@
                   'decipher'
                   'gene_patterns'
                   'mean'
                names      ('uns',)
                varnames   ('.0', 'gp_name')
                freevars   ('adata',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
                name       '<listcomp>'
                firstlineno 78
                lnotab 0x0a013eff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
@@ -515,15 +515,15 @@
                        >>   38 RETURN_VALUE
                consts
                   0
                names      ('shape',)
                varnames   ('.0', 'gp')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
                name       '<listcomp>'
                firstlineno 81
                lnotab 0x
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
@@ -549,15 +549,15 @@
                        >>   44 RETURN_VALUE
                consts
                   None
                names      ('T',)
                varnames   ('.0', 'gp')
                freevars   ('min_len',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
                name       '<listcomp>'
                firstlineno 82
                lnotab 0x
             0
             ('axis',)
             'times'
             ('n_basis', 'lr', 'n_iter', 'beta_prior', 'seed', 'times', 'plot_every_k_epochs')
@@ -612,470 +612,468 @@
                consts
                   '_RETURN'
                   'mean'
                names      ('squeeze', 'detach', 'numpy')
                varnames   ('.0', 'i', 'gp_name')
                freevars   ('samples',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
                name       '<dictcomp>'
                firstlineno 112
                lnotab 0x0a0208ff94ff
             ('scales', 'betas', 'betas_samples', 'basis', 'times', 'length', 'gene_patterns_reconstruction', 'pattern_names')
             'basis_decomposition'
             'decipher_betas_'
          names      ('is_notebook', 'logger', 'info', 'list', 'uns', 'keys', 'min', 'np', 'stack', 'run_compute_basis_decomposition', 'InferenceMode', 'GAUSSIAN_BETA_ONLY', 'detach', 'numpy', 'get_basis', 'shape', 'reshape', 'enumerate', 'varm')
          varnames   ('adata', 'pattern_names', 'n_basis', 'n_iter', 'lr', 'beta_prior', 'seed', 'plot_every_k_epochs', 'gene_patterns', 'p_name', 'gene_patterns_times', 'trajectory_model', 'guide', 'times', 'gene_scales', 'losses', 'basis', 'betas_shape', 'betas_mean', 'i')
          freevars   ()
          cellvars   ('adata', 'min_len', 'samples')
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
          name       'basis_decomposition'
          firstlineno 20
          lnotab
             0x0832280104012201020102ff04ff100404016401080102ff120332011c
             012c0310014e020c010201160102010201020102010201020102f7200b4c
             01240126018a0302010201900102014a01020108021cfe100402f5220d28
             013602
       code
          argcount  : 3
          nlocals   : 17
          stacksize : 9
          flags     : 3
          code
-            0x97007401000000000000000000007c01a6010000ab0100000000000000
-            007402000000000000000000006b0200000000722c7c006a020000000000
-            000000640119000000000000000000640219000000000000000000640319
-            000000000000000000a00300000000000000000000000000000000000000
-            007c01a6010000ab0100000000000000007d017401000000000000000000
-            007c02a6010000ab0100000000000000007402000000000000000000006b
-            0200000000722c7c006a0200000000000000006401190000000000000000
-            00640219000000000000000000640319000000000000000000a003000000
-            00000000000000000000000000000000007c02a6010000ab010000000000
-            0000007d027c017d037c027d04640484007d057c006a0200000000000000
-            006401190000000000000000006402190000000000000000006405190000
-            000000000000006406640685027c03640664068502640664068502660419
-            0000000000000000007d067c006a02000000000000000064011900000000
-            000000000064021900000000000000000064051900000000000000000064
-            06640685027c046406640685026406640685026604190000000000000000
-            007d077c006a020000000000000000640119000000000000000000640219
-            0000000000000000006407190000000000000000007c0364066406850266
-            02190000000000000000007d087c006a0200000000000000006401190000
-            000000000000006402190000000000000000006407190000000000000000
-            007c046406640685026602190000000000000000007d0974090000000000
-            00000000007c006a050000000000000000a6010000ab0100000000000000
-            007d0a02007c057c067c07a6020000ab0200000000000000007d0b7c0ba0
-            06000000000000000000000000000000000000000064087c0aa6020000ab
-            0200000000000000007d0b740f000000000000000000006a080000000000
-            000000740f000000000000000000006a0900000000000000007c08a60100
-            00ab010000000000000000740f000000000000000000006a090000000000
-            0000007c09a6010000ab0100000000000000007a0a0000a6010000ab0100
-            000000000000007d0c02007c05740f000000000000000000006a09000000
-            00000000007c08640664066406850264066603190000000000000000007c
-            067a050000a6010000ab010000000000000000740f000000000000000000
-            006a0900000000000000007c096406640664068502640666031900000000
-            00000000007c077a050000a6010000ab010000000000000000a6020000ab
-            0200000000000000007d0d7c0da006000000000000000000000000000000
-            000000000064087c0aa6020000ab0200000000000000007d0d7415000000
-            000000000000006a0b00000000000000007c006a0500000000000000007c
-            0ba00c00000000000000000000000000000000000000006409ac0aa60100
-            00ab0100000000000000007c0c7c0da00c00000000000000000000000000
-            000000000000006409ac0aa6010000ab010000000000000000640b9c04a6
-            010000ab010000000000000000a00d000000000000000000000000000000
-            0000000000640ca6010000ab0100000000000000007d0e7c0e640d190000
-            000000000000007c006a0e0000000000000000640e3c0000007c0e640f19
-            0000000000000000007c006a0e000000000000000064103c0000007c0e64
-            11190000000000000000007c006a0e000000000000000064123c00000074
-            1e00000000000000000000a0100000000000000000000000000000000000
-            0000006413a6010000ab0100000000000000000100741e00000000000000
-            000000a01000000000000000000000000000000000000000006414a60100
-            00ab0100000000000000000100741e00000000000000000000a010000000
-            00000000000000000000000000000000006415a6010000ab010000000000
-            00000001007c0b6a1100000000000000006409190000000000000000007d
-            0f7415000000000000000000006a0b0000000000000000740f0000000000
-            00000000006a1200000000000000007c006a0500000000000000007c0fa6
-            020000ab0200000000000000007c0ba00600000000000000000000000000
-            000000000000006408a6010000ab0100000000000000007c0da006000000
-            00000000000000000000000000000000006408a6010000ab010000000000
-            00000064169c03a6010000ab0100000000000000007d107c107c006a0200
-            0000000000000064011900000000000000000064173c0000007c0e7c006a
-            02000000000000000064011900000000000000000064183c000000741e00
-            000000000000000000a01000000000000000000000000000000000000000
-            006419a6010000ab0100000000000000000100741e000000000000000000
-            00a0100000000000000000000000000000000000000000641aa6010000ab
-            010000000000000000010064065300
+            0x97007401000000000000000000007c01740200000000000000000000a6
+            020000ab020000000000000000722c7c006a020000000000000000640119
+            000000000000000000640219000000000000000000640319000000000000
+            000000a00300000000000000000000000000000000000000007c01a60100
+            00ab0100000000000000007d017401000000000000000000007c02740200
+            000000000000000000a6020000ab020000000000000000722c7c006a0200
+            000000000000006401190000000000000000006402190000000000000000
+            00640319000000000000000000a003000000000000000000000000000000
+            00000000007c02a6010000ab0100000000000000007d027c017d037c027d
+            04640484007d057c006a0200000000000000006401190000000000000000
+            006402190000000000000000006405190000000000000000006406640685
+            027c036406640685026406640685026604190000000000000000007d067c
+            006a02000000000000000064011900000000000000000064021900000000
+            00000000006405190000000000000000006406640685027c046406640685
+            026406640685026604190000000000000000007d077c006a020000000000
+            000000640119000000000000000000640219000000000000000000640719
+            0000000000000000007c036406640685026602190000000000000000007d
+            087c006a0200000000000000006401190000000000000000006402190000
+            000000000000006407190000000000000000007c04640664068502660219
+            0000000000000000007d097409000000000000000000007c006a05000000
+            0000000000a6010000ab0100000000000000007d0a02007c057c067c07a6
+            020000ab0200000000000000007d0b7c0ba0060000000000000000000000
+            00000000000000000064087c0aa6020000ab0200000000000000007d0b74
+            0f000000000000000000006a080000000000000000740f00000000000000
+            0000006a0900000000000000007c08a6010000ab01000000000000000074
+            0f000000000000000000006a0900000000000000007c09a6010000ab0100
+            000000000000007a0a0000a6010000ab0100000000000000007d0c02007c
+            05740f000000000000000000006a0900000000000000007c086406640664
+            06850264066603190000000000000000007c067a050000a6010000ab0100
+            00000000000000740f000000000000000000006a0900000000000000007c
+            09640664066406850264066603190000000000000000007c077a050000a6
+            010000ab010000000000000000a6020000ab0200000000000000007d0d7c
+            0da006000000000000000000000000000000000000000064087c0aa60200
+            00ab0200000000000000007d0d7415000000000000000000006a0b000000
+            00000000007c006a0500000000000000007c0ba00c000000000000000000
+            00000000000000000000006409ac0aa6010000ab0100000000000000007c
+            0c7c0da00c00000000000000000000000000000000000000006409ac0aa6
+            010000ab010000000000000000640b9c04a6010000ab0100000000000000
+            00a00d0000000000000000000000000000000000000000640ca6010000ab
+            0100000000000000007d0e7c0e640d190000000000000000007c006a0e00
+            00000000000000640e3c0000007c0e640f190000000000000000007c006a
+            0e000000000000000064103c0000007c0e6411190000000000000000007c
+            006a0e000000000000000064123c000000741e00000000000000000000a0
+            1000000000000000000000000000000000000000006413a6010000ab0100
+            000000000000000100741e00000000000000000000a01000000000000000
+            000000000000000000000000006414a6010000ab01000000000000000001
+            00741e00000000000000000000a010000000000000000000000000000000
+            00000000006415a6010000ab01000000000000000001007c0b6a11000000
+            00000000006409190000000000000000007d0f7415000000000000000000
+            006a0b0000000000000000740f000000000000000000006a120000000000
+            0000007c006a0500000000000000007c0fa6020000ab0200000000000000
+            007c0ba00600000000000000000000000000000000000000006408a60100
+            00ab0100000000000000007c0da006000000000000000000000000000000
+            00000000006408a6010000ab01000000000000000064169c03a6010000ab
+            0100000000000000007d107c107c006a0200000000000000006401190000
+            0000000000000064173c0000007c0e7c006a020000000000000000640119
+            00000000000000000064183c000000741e00000000000000000000a01000
+            000000000000000000000000000000000000006419a6010000ab01000000
+            00000000000100741e00000000000000000000a010000000000000000000
+            0000000000000000000000641aa6010000ab010000000000000000010064
+            065300
          124           0 RESUME                   0
          
-         152           2 LOAD_GLOBAL              1 (NULL + type)
+         152           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                1 (pattern_name_a)
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 LOAD_GLOBAL              2 (str)
-                      42 COMPARE_OP               2 (==)
-                      48 POP_JUMP_FORWARD_IF_FALSE    44 (to 138)
-         
-         153          50 LOAD_FAST                0 (adata)
-                      52 LOAD_ATTR                2 (uns)
-                      62 LOAD_CONST               1 ('decipher')
-                      64 BINARY_SUBSCR
-                      74 LOAD_CONST               2 ('basis_decomposition')
-                      76 BINARY_SUBSCR
-                      86 LOAD_CONST               3 ('pattern_names')
-                      88 BINARY_SUBSCR
-                      98 LOAD_METHOD              3 (index)
-         
-         154         120 LOAD_FAST                1 (pattern_name_a)
-         
-         153         122 PRECALL                  1
-                     126 CALL                     1
-                     136 STORE_FAST               1 (pattern_name_a)
-         
-         156     >>  138 LOAD_GLOBAL              1 (NULL + type)
-                     150 LOAD_FAST                2 (pattern_name_b)
-                     152 PRECALL                  1
-                     156 CALL                     1
-                     166 LOAD_GLOBAL              2 (str)
-                     178 COMPARE_OP               2 (==)
-                     184 POP_JUMP_FORWARD_IF_FALSE    44 (to 274)
-         
-         157         186 LOAD_FAST                0 (adata)
-                     188 LOAD_ATTR                2 (uns)
-                     198 LOAD_CONST               1 ('decipher')
+                      16 LOAD_GLOBAL              2 (str)
+                      28 PRECALL                  2
+                      32 CALL                     2
+                      42 POP_JUMP_FORWARD_IF_FALSE    44 (to 132)
+         
+         153          44 LOAD_FAST                0 (adata)
+                      46 LOAD_ATTR                2 (uns)
+                      56 LOAD_CONST               1 ('decipher')
+                      58 BINARY_SUBSCR
+                      68 LOAD_CONST               2 ('basis_decomposition')
+                      70 BINARY_SUBSCR
+                      80 LOAD_CONST               3 ('pattern_names')
+                      82 BINARY_SUBSCR
+                      92 LOAD_METHOD              3 (index)
+         
+         154         114 LOAD_FAST                1 (pattern_name_a)
+         
+         153         116 PRECALL                  1
+                     120 CALL                     1
+                     130 STORE_FAST               1 (pattern_name_a)
+         
+         156     >>  132 LOAD_GLOBAL              1 (NULL + isinstance)
+                     144 LOAD_FAST                2 (pattern_name_b)
+                     146 LOAD_GLOBAL              2 (str)
+                     158 PRECALL                  2
+                     162 CALL                     2
+                     172 POP_JUMP_FORWARD_IF_FALSE    44 (to 262)
+         
+         157         174 LOAD_FAST                0 (adata)
+                     176 LOAD_ATTR                2 (uns)
+                     186 LOAD_CONST               1 ('decipher')
+                     188 BINARY_SUBSCR
+                     198 LOAD_CONST               2 ('basis_decomposition')
                      200 BINARY_SUBSCR
-                     210 LOAD_CONST               2 ('basis_decomposition')
+                     210 LOAD_CONST               3 ('pattern_names')
                      212 BINARY_SUBSCR
-                     222 LOAD_CONST               3 ('pattern_names')
-                     224 BINARY_SUBSCR
-                     234 LOAD_METHOD              3 (index)
+                     222 LOAD_METHOD              3 (index)
          
-         158         256 LOAD_FAST                2 (pattern_name_b)
+         158         244 LOAD_FAST                2 (pattern_name_b)
          
-         157         258 PRECALL                  1
-                     262 CALL                     1
-                     272 STORE_FAST               2 (pattern_name_b)
+         157         246 PRECALL                  1
+                     250 CALL                     1
+                     260 STORE_FAST               2 (pattern_name_b)
          
-         160     >>  274 LOAD_FAST                1 (pattern_name_a)
-                     276 STORE_FAST               3 (idx_a)
+         160     >>  262 LOAD_FAST                1 (pattern_name_a)
+                     264 STORE_FAST               3 (idx_a)
          
-         161         278 LOAD_FAST                2 (pattern_name_b)
-                     280 STORE_FAST               4 (idx_b)
+         161         266 LOAD_FAST                2 (pattern_name_b)
+                     268 STORE_FAST               4 (idx_b)
          
-         163         282 LOAD_CONST               4 (<code object pairwise_distances, file "/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py", line 163>)
-                     284 MAKE_FUNCTION            0
-                     286 STORE_FAST               5 (pairwise_distances)
+         163         270 LOAD_CONST               4 (<code object pairwise_distances, file "/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py", line 163>)
+                     272 MAKE_FUNCTION            0
+                     274 STORE_FAST               5 (pairwise_distances)
          
-         181         288 LOAD_FAST                0 (adata)
-                     290 LOAD_ATTR                2 (uns)
-                     300 LOAD_CONST               1 ('decipher')
+         181         276 LOAD_FAST                0 (adata)
+                     278 LOAD_ATTR                2 (uns)
+                     288 LOAD_CONST               1 ('decipher')
+                     290 BINARY_SUBSCR
+                     300 LOAD_CONST               2 ('basis_decomposition')
                      302 BINARY_SUBSCR
-                     312 LOAD_CONST               2 ('basis_decomposition')
+                     312 LOAD_CONST               5 ('betas_samples')
                      314 BINARY_SUBSCR
-                     324 LOAD_CONST               5 ('betas_samples')
-                     326 BINARY_SUBSCR
-                     336 LOAD_CONST               6 (None)
+                     324 LOAD_CONST               6 (None)
+                     326 LOAD_CONST               6 (None)
+                     328 BUILD_SLICE              2
+                     330 LOAD_FAST                3 (idx_a)
+                     332 LOAD_CONST               6 (None)
+                     334 LOAD_CONST               6 (None)
+                     336 BUILD_SLICE              2
                      338 LOAD_CONST               6 (None)
-                     340 BUILD_SLICE              2
-                     342 LOAD_FAST                3 (idx_a)
-                     344 LOAD_CONST               6 (None)
-                     346 LOAD_CONST               6 (None)
-                     348 BUILD_SLICE              2
-                     350 LOAD_CONST               6 (None)
-                     352 LOAD_CONST               6 (None)
-                     354 BUILD_SLICE              2
-                     356 BUILD_TUPLE              4
-                     358 BINARY_SUBSCR
-                     368 STORE_FAST               6 (beta_a)
-         
-         182         370 LOAD_FAST                0 (adata)
-                     372 LOAD_ATTR                2 (uns)
-                     382 LOAD_CONST               1 ('decipher')
+                     340 LOAD_CONST               6 (None)
+                     342 BUILD_SLICE              2
+                     344 BUILD_TUPLE              4
+                     346 BINARY_SUBSCR
+                     356 STORE_FAST               6 (beta_a)
+         
+         182         358 LOAD_FAST                0 (adata)
+                     360 LOAD_ATTR                2 (uns)
+                     370 LOAD_CONST               1 ('decipher')
+                     372 BINARY_SUBSCR
+                     382 LOAD_CONST               2 ('basis_decomposition')
                      384 BINARY_SUBSCR
-                     394 LOAD_CONST               2 ('basis_decomposition')
+                     394 LOAD_CONST               5 ('betas_samples')
                      396 BINARY_SUBSCR
-                     406 LOAD_CONST               5 ('betas_samples')
-                     408 BINARY_SUBSCR
-                     418 LOAD_CONST               6 (None)
+                     406 LOAD_CONST               6 (None)
+                     408 LOAD_CONST               6 (None)
+                     410 BUILD_SLICE              2
+                     412 LOAD_FAST                4 (idx_b)
+                     414 LOAD_CONST               6 (None)
+                     416 LOAD_CONST               6 (None)
+                     418 BUILD_SLICE              2
                      420 LOAD_CONST               6 (None)
-                     422 BUILD_SLICE              2
-                     424 LOAD_FAST                4 (idx_b)
-                     426 LOAD_CONST               6 (None)
-                     428 LOAD_CONST               6 (None)
-                     430 BUILD_SLICE              2
-                     432 LOAD_CONST               6 (None)
-                     434 LOAD_CONST               6 (None)
-                     436 BUILD_SLICE              2
-                     438 BUILD_TUPLE              4
-                     440 BINARY_SUBSCR
-                     450 STORE_FAST               7 (beta_b)
-         
-         184         452 LOAD_FAST                0 (adata)
-                     454 LOAD_ATTR                2 (uns)
-                     464 LOAD_CONST               1 ('decipher')
+                     422 LOAD_CONST               6 (None)
+                     424 BUILD_SLICE              2
+                     426 BUILD_TUPLE              4
+                     428 BINARY_SUBSCR
+                     438 STORE_FAST               7 (beta_b)
+         
+         184         440 LOAD_FAST                0 (adata)
+                     442 LOAD_ATTR                2 (uns)
+                     452 LOAD_CONST               1 ('decipher')
+                     454 BINARY_SUBSCR
+                     464 LOAD_CONST               2 ('basis_decomposition')
                      466 BINARY_SUBSCR
-                     476 LOAD_CONST               2 ('basis_decomposition')
+                     476 LOAD_CONST               7 ('scales')
                      478 BINARY_SUBSCR
-                     488 LOAD_CONST               7 ('scales')
-                     490 BINARY_SUBSCR
-                     500 LOAD_FAST                3 (idx_a)
-                     502 LOAD_CONST               6 (None)
-                     504 LOAD_CONST               6 (None)
-                     506 BUILD_SLICE              2
-                     508 BUILD_TUPLE              2
-                     510 BINARY_SUBSCR
-                     520 STORE_FAST               8 (gene_scales_a)
-         
-         185         522 LOAD_FAST                0 (adata)
-                     524 LOAD_ATTR                2 (uns)
-                     534 LOAD_CONST               1 ('decipher')
+                     488 LOAD_FAST                3 (idx_a)
+                     490 LOAD_CONST               6 (None)
+                     492 LOAD_CONST               6 (None)
+                     494 BUILD_SLICE              2
+                     496 BUILD_TUPLE              2
+                     498 BINARY_SUBSCR
+                     508 STORE_FAST               8 (gene_scales_a)
+         
+         185         510 LOAD_FAST                0 (adata)
+                     512 LOAD_ATTR                2 (uns)
+                     522 LOAD_CONST               1 ('decipher')
+                     524 BINARY_SUBSCR
+                     534 LOAD_CONST               2 ('basis_decomposition')
                      536 BINARY_SUBSCR
-                     546 LOAD_CONST               2 ('basis_decomposition')
+                     546 LOAD_CONST               7 ('scales')
                      548 BINARY_SUBSCR
-                     558 LOAD_CONST               7 ('scales')
-                     560 BINARY_SUBSCR
-                     570 LOAD_FAST                4 (idx_b)
-                     572 LOAD_CONST               6 (None)
-                     574 LOAD_CONST               6 (None)
-                     576 BUILD_SLICE              2
-                     578 BUILD_TUPLE              2
-                     580 BINARY_SUBSCR
-                     590 STORE_FAST               9 (gene_scales_b)
-         
-         187         592 LOAD_GLOBAL              9 (NULL + len)
-                     604 LOAD_FAST                0 (adata)
-                     606 LOAD_ATTR                5 (var_names)
-                     616 PRECALL                  1
-                     620 CALL                     1
-                     630 STORE_FAST              10 (n_genes)
-         
-         188         632 PUSH_NULL
-                     634 LOAD_FAST                5 (pairwise_distances)
-                     636 LOAD_FAST                6 (beta_a)
-                     638 LOAD_FAST                7 (beta_b)
-                     640 PRECALL                  2
-                     644 CALL                     2
-                     654 STORE_FAST              11 (shape_disruption)
-         
-         189         656 LOAD_FAST               11 (shape_disruption)
-                     658 LOAD_METHOD              6 (reshape)
-                     680 LOAD_CONST               8 (-1)
-                     682 LOAD_FAST               10 (n_genes)
-                     684 PRECALL                  2
-                     688 CALL                     2
-                     698 STORE_FAST              11 (shape_disruption)
-         
-         190         700 LOAD_GLOBAL             15 (NULL + np)
-                     712 LOAD_ATTR                8 (abs)
-                     722 LOAD_GLOBAL             15 (NULL + np)
-                     734 LOAD_ATTR                9 (log)
-                     744 LOAD_FAST                8 (gene_scales_a)
-                     746 PRECALL                  1
-                     750 CALL                     1
-                     760 LOAD_GLOBAL             15 (NULL + np)
-                     772 LOAD_ATTR                9 (log)
-                     782 LOAD_FAST                9 (gene_scales_b)
-                     784 PRECALL                  1
-                     788 CALL                     1
-                     798 BINARY_OP               10 (-)
-                     802 PRECALL                  1
-                     806 CALL                     1
-                     816 STORE_FAST              12 (scale_disruption)
-         
-         191         818 PUSH_NULL
-                     820 LOAD_FAST                5 (pairwise_distances)
-         
-         192         822 LOAD_GLOBAL             15 (NULL + np)
-                     834 LOAD_ATTR                9 (log)
-                     844 LOAD_FAST                8 (gene_scales_a)
-                     846 LOAD_CONST               6 (None)
-                     848 LOAD_CONST               6 (None)
-                     850 LOAD_CONST               6 (None)
-                     852 BUILD_SLICE              2
-                     854 LOAD_CONST               6 (None)
-                     856 BUILD_TUPLE              3
-                     858 BINARY_SUBSCR
-                     868 LOAD_FAST                6 (beta_a)
-                     870 BINARY_OP                5 (*)
-                     874 PRECALL                  1
-                     878 CALL                     1
-         
-         193         888 LOAD_GLOBAL             15 (NULL + np)
-                     900 LOAD_ATTR                9 (log)
-                     910 LOAD_FAST                9 (gene_scales_b)
-                     912 LOAD_CONST               6 (None)
-                     914 LOAD_CONST               6 (None)
-                     916 LOAD_CONST               6 (None)
-                     918 BUILD_SLICE              2
-                     920 LOAD_CONST               6 (None)
-                     922 BUILD_TUPLE              3
-                     924 BINARY_SUBSCR
-                     934 LOAD_FAST                7 (beta_b)
-                     936 BINARY_OP                5 (*)
-                     940 PRECALL                  1
-                     944 CALL                     1
-         
-         191         954 PRECALL                  2
-                     958 CALL                     2
-                     968 STORE_FAST              13 (combined_disruption)
-         
-         195         970 LOAD_FAST               13 (combined_disruption)
-                     972 LOAD_METHOD              6 (reshape)
-                     994 LOAD_CONST               8 (-1)
-                     996 LOAD_FAST               10 (n_genes)
-                     998 PRECALL                  2
-                    1002 CALL                     2
-                    1012 STORE_FAST              13 (combined_disruption)
-         
-         196        1014 LOAD_GLOBAL             21 (NULL + pd)
-                    1026 LOAD_ATTR               11 (DataFrame)
-         
-         198        1036 LOAD_FAST                0 (adata)
-                    1038 LOAD_ATTR                5 (var_names)
-         
-         199        1048 LOAD_FAST               11 (shape_disruption)
-                    1050 LOAD_METHOD             12 (mean)
-                    1072 LOAD_CONST               9 (0)
-                    1074 KW_NAMES                10
-                    1076 PRECALL                  1
-                    1080 CALL                     1
-         
-         200        1090 LOAD_FAST               12 (scale_disruption)
-         
-         201        1092 LOAD_FAST               13 (combined_disruption)
-                    1094 LOAD_METHOD             12 (mean)
-                    1116 LOAD_CONST               9 (0)
-                    1118 KW_NAMES                10
-                    1120 PRECALL                  1
-                    1124 CALL                     1
-         
-         197        1134 LOAD_CONST              11 (('gene', 'shape', 'scale', 'combined'))
-                    1136 BUILD_CONST_KEY_MAP      4
-         
-         196        1138 PRECALL                  1
-                    1142 CALL                     1
-         
-         203        1152 LOAD_METHOD             13 (set_index)
-                    1174 LOAD_CONST              12 ('gene')
-                    1176 PRECALL                  1
-                    1180 CALL                     1
-         
-         196        1190 STORE_FAST              14 (disruptions_mean)
-         
-         205        1192 LOAD_FAST               14 (disruptions_mean)
-                    1194 LOAD_CONST              13 ('shape')
-                    1196 BINARY_SUBSCR
-                    1206 LOAD_FAST                0 (adata)
-                    1208 LOAD_ATTR               14 (var)
-                    1218 LOAD_CONST              14 ('decipher_disruption_shape')
-                    1220 STORE_SUBSCR
-         
-         206        1224 LOAD_FAST               14 (disruptions_mean)
-                    1226 LOAD_CONST              15 ('scale')
-                    1228 BINARY_SUBSCR
-                    1238 LOAD_FAST                0 (adata)
-                    1240 LOAD_ATTR               14 (var)
-                    1250 LOAD_CONST              16 ('decipher_disruption_scale')
-                    1252 STORE_SUBSCR
-         
-         207        1256 LOAD_FAST               14 (disruptions_mean)
-                    1258 LOAD_CONST              17 ('combined')
-                    1260 BINARY_SUBSCR
-                    1270 LOAD_FAST                0 (adata)
-                    1272 LOAD_ATTR               14 (var)
-                    1282 LOAD_CONST              18 ('decipher_disruption_combined')
-                    1284 STORE_SUBSCR
-         
-         208        1288 LOAD_GLOBAL             30 (logger)
-                    1300 LOAD_METHOD             16 (info)
-                    1322 LOAD_CONST              19 ("Added `.var['decipher_disruption_shape']`: shape disruption scores")
-                    1324 PRECALL                  1
-                    1328 CALL                     1
-                    1338 POP_TOP
-         
-         209        1340 LOAD_GLOBAL             30 (logger)
-                    1352 LOAD_METHOD             16 (info)
-                    1374 LOAD_CONST              20 ("Added `.var['decipher_disruption_scale']`: scale disruption scores")
-                    1376 PRECALL                  1
-                    1380 CALL                     1
-                    1390 POP_TOP
-         
-         210        1392 LOAD_GLOBAL             30 (logger)
-                    1404 LOAD_METHOD             16 (info)
-                    1426 LOAD_CONST              21 ("Added `.var['decipher_disruption_combined']`: combined disruption scores")
-                    1428 PRECALL                  1
-                    1432 CALL                     1
-                    1442 POP_TOP
-         
-         212        1444 LOAD_FAST               11 (shape_disruption)
-                    1446 LOAD_ATTR               17 (shape)
-                    1456 LOAD_CONST               9 (0)
-                    1458 BINARY_SUBSCR
-                    1468 STORE_FAST              15 (n_samples)
-         
-         213        1470 LOAD_GLOBAL             21 (NULL + pd)
-                    1482 LOAD_ATTR               11 (DataFrame)
-         
-         215        1492 LOAD_GLOBAL             15 (NULL + np)
-                    1504 LOAD_ATTR               18 (tile)
-                    1514 LOAD_FAST                0 (adata)
-                    1516 LOAD_ATTR                5 (var_names)
-                    1526 LOAD_FAST               15 (n_samples)
-                    1528 PRECALL                  2
-                    1532 CALL                     2
-         
-         216        1542 LOAD_FAST               11 (shape_disruption)
-                    1544 LOAD_METHOD              6 (reshape)
-                    1566 LOAD_CONST               8 (-1)
-                    1568 PRECALL                  1
-                    1572 CALL                     1
-         
-         217        1582 LOAD_FAST               13 (combined_disruption)
-                    1584 LOAD_METHOD              6 (reshape)
-                    1606 LOAD_CONST               8 (-1)
-                    1608 PRECALL                  1
-                    1612 CALL                     1
-         
-         214        1622 LOAD_CONST              22 (('gene', 'shape', 'combined'))
-                    1624 BUILD_CONST_KEY_MAP      3
-         
-         213        1626 PRECALL                  1
-                    1630 CALL                     1
-                    1640 STORE_FAST              16 (disruptions_samples)
-         
-         220        1642 LOAD_FAST               16 (disruptions_samples)
-                    1644 LOAD_FAST                0 (adata)
-                    1646 LOAD_ATTR                2 (uns)
-                    1656 LOAD_CONST               1 ('decipher')
-                    1658 BINARY_SUBSCR
-                    1668 LOAD_CONST              23 ('disruption_scores_samples')
-                    1670 STORE_SUBSCR
-         
-         221        1674 LOAD_FAST               14 (disruptions_mean)
-                    1676 LOAD_FAST                0 (adata)
-                    1678 LOAD_ATTR                2 (uns)
-                    1688 LOAD_CONST               1 ('decipher')
-                    1690 BINARY_SUBSCR
-                    1700 LOAD_CONST              24 ('disruption_scores')
-                    1702 STORE_SUBSCR
-         
-         222        1706 LOAD_GLOBAL             30 (logger)
-                    1718 LOAD_METHOD             16 (info)
-                    1740 LOAD_CONST              25 ("Added `.uns['decipher']['disruption_scores']`: disruption scores")
-                    1742 PRECALL                  1
-                    1746 CALL                     1
-                    1756 POP_TOP
-         
-         223        1758 LOAD_GLOBAL             30 (logger)
-                    1770 LOAD_METHOD             16 (info)
-         
-         224        1792 LOAD_CONST              26 ("Added `.uns['decipher']['disruption_scores_samples']`: disruption scores probabilistic samples")
-         
-         223        1794 PRECALL                  1
-                    1798 CALL                     1
-                    1808 POP_TOP
-                    1810 LOAD_CONST               6 (None)
-                    1812 RETURN_VALUE
+                     558 LOAD_FAST                4 (idx_b)
+                     560 LOAD_CONST               6 (None)
+                     562 LOAD_CONST               6 (None)
+                     564 BUILD_SLICE              2
+                     566 BUILD_TUPLE              2
+                     568 BINARY_SUBSCR
+                     578 STORE_FAST               9 (gene_scales_b)
+         
+         187         580 LOAD_GLOBAL              9 (NULL + len)
+                     592 LOAD_FAST                0 (adata)
+                     594 LOAD_ATTR                5 (var_names)
+                     604 PRECALL                  1
+                     608 CALL                     1
+                     618 STORE_FAST              10 (n_genes)
+         
+         188         620 PUSH_NULL
+                     622 LOAD_FAST                5 (pairwise_distances)
+                     624 LOAD_FAST                6 (beta_a)
+                     626 LOAD_FAST                7 (beta_b)
+                     628 PRECALL                  2
+                     632 CALL                     2
+                     642 STORE_FAST              11 (shape_disruption)
+         
+         189         644 LOAD_FAST               11 (shape_disruption)
+                     646 LOAD_METHOD              6 (reshape)
+                     668 LOAD_CONST               8 (-1)
+                     670 LOAD_FAST               10 (n_genes)
+                     672 PRECALL                  2
+                     676 CALL                     2
+                     686 STORE_FAST              11 (shape_disruption)
+         
+         190         688 LOAD_GLOBAL             15 (NULL + np)
+                     700 LOAD_ATTR                8 (abs)
+                     710 LOAD_GLOBAL             15 (NULL + np)
+                     722 LOAD_ATTR                9 (log)
+                     732 LOAD_FAST                8 (gene_scales_a)
+                     734 PRECALL                  1
+                     738 CALL                     1
+                     748 LOAD_GLOBAL             15 (NULL + np)
+                     760 LOAD_ATTR                9 (log)
+                     770 LOAD_FAST                9 (gene_scales_b)
+                     772 PRECALL                  1
+                     776 CALL                     1
+                     786 BINARY_OP               10 (-)
+                     790 PRECALL                  1
+                     794 CALL                     1
+                     804 STORE_FAST              12 (scale_disruption)
+         
+         191         806 PUSH_NULL
+                     808 LOAD_FAST                5 (pairwise_distances)
+         
+         192         810 LOAD_GLOBAL             15 (NULL + np)
+                     822 LOAD_ATTR                9 (log)
+                     832 LOAD_FAST                8 (gene_scales_a)
+                     834 LOAD_CONST               6 (None)
+                     836 LOAD_CONST               6 (None)
+                     838 LOAD_CONST               6 (None)
+                     840 BUILD_SLICE              2
+                     842 LOAD_CONST               6 (None)
+                     844 BUILD_TUPLE              3
+                     846 BINARY_SUBSCR
+                     856 LOAD_FAST                6 (beta_a)
+                     858 BINARY_OP                5 (*)
+                     862 PRECALL                  1
+                     866 CALL                     1
+         
+         193         876 LOAD_GLOBAL             15 (NULL + np)
+                     888 LOAD_ATTR                9 (log)
+                     898 LOAD_FAST                9 (gene_scales_b)
+                     900 LOAD_CONST               6 (None)
+                     902 LOAD_CONST               6 (None)
+                     904 LOAD_CONST               6 (None)
+                     906 BUILD_SLICE              2
+                     908 LOAD_CONST               6 (None)
+                     910 BUILD_TUPLE              3
+                     912 BINARY_SUBSCR
+                     922 LOAD_FAST                7 (beta_b)
+                     924 BINARY_OP                5 (*)
+                     928 PRECALL                  1
+                     932 CALL                     1
+         
+         191         942 PRECALL                  2
+                     946 CALL                     2
+                     956 STORE_FAST              13 (combined_disruption)
+         
+         195         958 LOAD_FAST               13 (combined_disruption)
+                     960 LOAD_METHOD              6 (reshape)
+                     982 LOAD_CONST               8 (-1)
+                     984 LOAD_FAST               10 (n_genes)
+                     986 PRECALL                  2
+                     990 CALL                     2
+                    1000 STORE_FAST              13 (combined_disruption)
+         
+         196        1002 LOAD_GLOBAL             21 (NULL + pd)
+                    1014 LOAD_ATTR               11 (DataFrame)
+         
+         198        1024 LOAD_FAST                0 (adata)
+                    1026 LOAD_ATTR                5 (var_names)
+         
+         199        1036 LOAD_FAST               11 (shape_disruption)
+                    1038 LOAD_METHOD             12 (mean)
+                    1060 LOAD_CONST               9 (0)
+                    1062 KW_NAMES                10
+                    1064 PRECALL                  1
+                    1068 CALL                     1
+         
+         200        1078 LOAD_FAST               12 (scale_disruption)
+         
+         201        1080 LOAD_FAST               13 (combined_disruption)
+                    1082 LOAD_METHOD             12 (mean)
+                    1104 LOAD_CONST               9 (0)
+                    1106 KW_NAMES                10
+                    1108 PRECALL                  1
+                    1112 CALL                     1
+         
+         197        1122 LOAD_CONST              11 (('gene', 'shape', 'scale', 'combined'))
+                    1124 BUILD_CONST_KEY_MAP      4
+         
+         196        1126 PRECALL                  1
+                    1130 CALL                     1
+         
+         203        1140 LOAD_METHOD             13 (set_index)
+                    1162 LOAD_CONST              12 ('gene')
+                    1164 PRECALL                  1
+                    1168 CALL                     1
+         
+         196        1178 STORE_FAST              14 (disruptions_mean)
+         
+         205        1180 LOAD_FAST               14 (disruptions_mean)
+                    1182 LOAD_CONST              13 ('shape')
+                    1184 BINARY_SUBSCR
+                    1194 LOAD_FAST                0 (adata)
+                    1196 LOAD_ATTR               14 (var)
+                    1206 LOAD_CONST              14 ('decipher_disruption_shape')
+                    1208 STORE_SUBSCR
+         
+         206        1212 LOAD_FAST               14 (disruptions_mean)
+                    1214 LOAD_CONST              15 ('scale')
+                    1216 BINARY_SUBSCR
+                    1226 LOAD_FAST                0 (adata)
+                    1228 LOAD_ATTR               14 (var)
+                    1238 LOAD_CONST              16 ('decipher_disruption_scale')
+                    1240 STORE_SUBSCR
+         
+         207        1244 LOAD_FAST               14 (disruptions_mean)
+                    1246 LOAD_CONST              17 ('combined')
+                    1248 BINARY_SUBSCR
+                    1258 LOAD_FAST                0 (adata)
+                    1260 LOAD_ATTR               14 (var)
+                    1270 LOAD_CONST              18 ('decipher_disruption_combined')
+                    1272 STORE_SUBSCR
+         
+         208        1276 LOAD_GLOBAL             30 (logger)
+                    1288 LOAD_METHOD             16 (info)
+                    1310 LOAD_CONST              19 ("Added `.var['decipher_disruption_shape']`: shape disruption scores")
+                    1312 PRECALL                  1
+                    1316 CALL                     1
+                    1326 POP_TOP
+         
+         209        1328 LOAD_GLOBAL             30 (logger)
+                    1340 LOAD_METHOD             16 (info)
+                    1362 LOAD_CONST              20 ("Added `.var['decipher_disruption_scale']`: scale disruption scores")
+                    1364 PRECALL                  1
+                    1368 CALL                     1
+                    1378 POP_TOP
+         
+         210        1380 LOAD_GLOBAL             30 (logger)
+                    1392 LOAD_METHOD             16 (info)
+                    1414 LOAD_CONST              21 ("Added `.var['decipher_disruption_combined']`: combined disruption scores")
+                    1416 PRECALL                  1
+                    1420 CALL                     1
+                    1430 POP_TOP
+         
+         212        1432 LOAD_FAST               11 (shape_disruption)
+                    1434 LOAD_ATTR               17 (shape)
+                    1444 LOAD_CONST               9 (0)
+                    1446 BINARY_SUBSCR
+                    1456 STORE_FAST              15 (n_samples)
+         
+         213        1458 LOAD_GLOBAL             21 (NULL + pd)
+                    1470 LOAD_ATTR               11 (DataFrame)
+         
+         215        1480 LOAD_GLOBAL             15 (NULL + np)
+                    1492 LOAD_ATTR               18 (tile)
+                    1502 LOAD_FAST                0 (adata)
+                    1504 LOAD_ATTR                5 (var_names)
+                    1514 LOAD_FAST               15 (n_samples)
+                    1516 PRECALL                  2
+                    1520 CALL                     2
+         
+         216        1530 LOAD_FAST               11 (shape_disruption)
+                    1532 LOAD_METHOD              6 (reshape)
+                    1554 LOAD_CONST               8 (-1)
+                    1556 PRECALL                  1
+                    1560 CALL                     1
+         
+         217        1570 LOAD_FAST               13 (combined_disruption)
+                    1572 LOAD_METHOD              6 (reshape)
+                    1594 LOAD_CONST               8 (-1)
+                    1596 PRECALL                  1
+                    1600 CALL                     1
+         
+         214        1610 LOAD_CONST              22 (('gene', 'shape', 'combined'))
+                    1612 BUILD_CONST_KEY_MAP      3
+         
+         213        1614 PRECALL                  1
+                    1618 CALL                     1
+                    1628 STORE_FAST              16 (disruptions_samples)
+         
+         220        1630 LOAD_FAST               16 (disruptions_samples)
+                    1632 LOAD_FAST                0 (adata)
+                    1634 LOAD_ATTR                2 (uns)
+                    1644 LOAD_CONST               1 ('decipher')
+                    1646 BINARY_SUBSCR
+                    1656 LOAD_CONST              23 ('disruption_scores_samples')
+                    1658 STORE_SUBSCR
+         
+         221        1662 LOAD_FAST               14 (disruptions_mean)
+                    1664 LOAD_FAST                0 (adata)
+                    1666 LOAD_ATTR                2 (uns)
+                    1676 LOAD_CONST               1 ('decipher')
+                    1678 BINARY_SUBSCR
+                    1688 LOAD_CONST              24 ('disruption_scores')
+                    1690 STORE_SUBSCR
+         
+         222        1694 LOAD_GLOBAL             30 (logger)
+                    1706 LOAD_METHOD             16 (info)
+                    1728 LOAD_CONST              25 ("Added `.uns['decipher']['disruption_scores']`: disruption scores")
+                    1730 PRECALL                  1
+                    1734 CALL                     1
+                    1744 POP_TOP
+         
+         223        1746 LOAD_GLOBAL             30 (logger)
+                    1758 LOAD_METHOD             16 (info)
+         
+         224        1780 LOAD_CONST              26 ("Added `.uns['decipher']['disruption_scores_samples']`: disruption scores probabilistic samples")
+         
+         223        1782 PRECALL                  1
+                    1786 CALL                     1
+                    1796 POP_TOP
+                    1798 LOAD_CONST               6 (None)
+                    1800 RETURN_VALUE
          consts
             "Compute the disruption scores:\n        - shape: ||beta[0] - beta[1]||_2\n        - scale: | log(s[0]) - log(s[1]) |\n        - combined: || log(beta[0]*s[0]) - log(beta[1]*s[1]) ||\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n    pattern_name_a : str or int, default 0\n        The name or index of the first pattern.\n    pattern_name_b : str or int, default 1\n        The name or index of the second pattern.\n\n    Returns\n    -------\n    `adata.var['decipher_disruption_shape']` : pd.Series\n        The shape disruption scores for each gene.\n    `adata.var['decipher_disruption_scale']` : pd.Series\n        The scale disruption scores for each gene.\n    `adata.var['decipher_disruption_combined']` : pd.Series\n        The combined disruption scores for each gene.\n    `adata.uns['decipher']['disruption_scores']` : pd.DataFrame\n        The disruption scores for each gene.\n    `adata.uns['decipher']['disruption_scores_samples']` : pd.DataFrame\n        The disruption scores for each gene sampled from the posterior.\n    "
             'decipher'
             'basis_decomposition'
             'pattern_names'
             code
                argcount  : 2
@@ -1129,15 +1127,15 @@
                   2
                   -1
                   ('ord', 'axis')
                names      ('np', 'expand_dims', 'linalg', 'norm')
                varnames   ('x', 'y')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
                name       'pairwise_distances'
                firstlineno 163
                lnotab 0x020d2c012c01
             'betas_samples'
             None
             'scales'
             -1
@@ -1155,31 +1153,31 @@
             "Added `.var['decipher_disruption_scale']`: scale disruption scores"
             "Added `.var['decipher_disruption_combined']`: combined disruption scores"
             ('gene', 'shape', 'combined')
             'disruption_scores_samples'
             'disruption_scores'
             "Added `.uns['decipher']['disruption_scores']`: disruption scores"
             "Added `.uns['decipher']['disruption_scores_samples']`: disruption scores probabilistic samples"
-         names      ('type', 'str', 'uns', 'index', 'len', 'var_names', 'reshape', 'np', 'abs', 'log', 'pd', 'DataFrame', 'mean', 'set_index', 'var', 'logger', 'info', 'shape', 'tile')
+         names      ('isinstance', 'str', 'uns', 'index', 'len', 'var_names', 'reshape', 'np', 'abs', 'log', 'pd', 'DataFrame', 'mean', 'set_index', 'var', 'logger', 'info', 'shape', 'tile')
          varnames   ('adata', 'pattern_name_a', 'pattern_name_b', 'idx_a', 'idx_b', 'pairwise_distances', 'beta_a', 'beta_b', 'gene_scales_a', 'gene_scales_b', 'n_genes', 'shape_disruption', 'scale_disruption', 'combined_disruption', 'disruptions_mean', 'n_samples', 'disruptions_samples')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
          name       'disruption_scores'
          firstlineno 124
          lnotab
-            0x021c3001460102ff10033001460102ff10030401040206125201520246
+            0x021c2a01460102ff10032a01460102ff10030401040206125201520246
             014602280118012c0176010401420142fe10042c0116020c012a0102012a
             fc04ff0e0726f902092001200120013401340134021a0116023201280128
             fd04ff1007200120013401220102ff
       (None, 5, 10000, 0.005, 1, 0, -1)
       (0, 1)
    names      ('logging', 'numpy', 'np', 'pandas', 'pd', 'decipher.tools._basis_decomposition.inference', 'InferenceMode', 'decipher.tools._basis_decomposition.run', 'compute_basis_decomposition', 'run_compute_basis_decomposition', 'get_basis', 'decipher.utils', 'is_notebook', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'basis_decomposition', 'disruption_scores')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/basis_decomposition.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/basis_decomposition.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010802080108020c0110040c0220010e0102010cfe1208020102
       01020102010201020102f80868
```

### Comparing `scdecipher-0.1.0/decipher/tools/__pycache__/decipher.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/__pycache__/decipher.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,29 +1,29 @@
 magic:    0xa70d0d0a
-moddate:  0x22985265 (Mon Nov 13 21:41:54 2023 UTC)
-files sz: 12845
+moddate:  0x17282166 (Thu Apr 18 14:03:03 2024 UTC)
+files sz: 14285
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a03640064
       016c045a04640064016c055a06640064016c075a07640064026c086d095a
-      0a0100640064036c046d0b5a0b0100640064046c0c6d0d5a0d6d0e5a0e01
-      00640064056c0f6d105a100100640064066c116d115a110100640064076c
-      126d135a140100640064086c156d165a166d175a170100640064096c186d
-      195a196d1a5a1a6d1b5a1b01006400640a6c1c6d1d5a1d01006400640b6c
+      0a0100640064016c0b5a04640064036c046d0c5a0c0100640064046c0d6d
+      0e5a0e6d0f5a0f0100640064056c106d105a100100640064066c116d125a
+      130100640064076c146d155a156d165a160100640064086c176d185a186d
+      195a196d1a5a1a6d1b5a1b0100640064096c1c6d1d5a1d01006400640a6c
       1e6d1f5a1f6d205a206d215a216d225a220100020065006a230000000000
       0000006524a6010000ab0100000000000000005a25020065006a26000000
-      0000000000640c65006a270000000000000000ac0da6020000ab02000000
-      00000000000100640e84005a28640f84005a2902006517a6000000ab0000
-      00000000000000641064016603641165066a2a0000000000000000660264
-      1284055a2b641a641484015a2c09000900090009000900641b641684015a
-      2d641784005a2e641884005a2f641984005a3064015300
+      0000000000640b65006a270000000000000000ac0ca6020000ab02000000
+      00000000000100641b640e84015a28640f84005a2902006516a6000000ab
+      0000000000000000006410640164116604641265066a2a00000000000000
+      006602641384055a2b641c641584015a2c09000900090009000900641d64
+      1784015a2d641884005a2e641984005a2f641a84005a3064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
@@ -56,323 +56,413 @@
                 52 LOAD_CONST               2 (('pyplot',))
                 54 IMPORT_NAME              8 (matplotlib)
                 56 IMPORT_FROM              9 (pyplot)
                 58 STORE_NAME              10 (plt)
                 60 POP_TOP
    
      9          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               3 (('poutine',))
-                66 IMPORT_NAME              4 (pyro)
-                68 IMPORT_FROM             11 (poutine)
-                70 STORE_NAME              11 (poutine)
-                72 POP_TOP
-   
-    10          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               4 (('SVI', 'Trace_ELBO'))
-                78 IMPORT_NAME             12 (pyro.infer)
-                80 IMPORT_FROM             13 (SVI)
-                82 STORE_NAME              13 (SVI)
-                84 IMPORT_FROM             14 (Trace_ELBO)
-                86 STORE_NAME              14 (Trace_ELBO)
-                88 POP_TOP
-   
-    11          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               5 (('MultiStepLR',))
-                94 IMPORT_NAME             15 (pyro.optim)
-                96 IMPORT_FROM             16 (MultiStepLR)
-                98 STORE_NAME              16 (MultiStepLR)
-               100 POP_TOP
-   
-    12         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               6 (('tqdm',))
-               106 IMPORT_NAME             17 (tqdm)
-               108 IMPORT_FROM             17 (tqdm)
-               110 STORE_NAME              17 (tqdm)
-               112 POP_TOP
-   
-    14         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               7 (('decipher',))
-               118 IMPORT_NAME             18 (decipher.plot.decipher)
-               120 IMPORT_FROM             19 (decipher)
-               122 STORE_NAME              20 (plot_decipher_v)
-               124 POP_TOP
-   
-    15         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST               8 (('Decipher', 'DecipherConfig'))
-               130 IMPORT_NAME             21 (decipher.tools._decipher)
-               132 IMPORT_FROM             22 (Decipher)
-               134 STORE_NAME              22 (Decipher)
-               136 IMPORT_FROM             23 (DecipherConfig)
-               138 STORE_NAME              23 (DecipherConfig)
-               140 POP_TOP
-   
-    16         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST               9 (('decipher_load_model', 'decipher_save_model', 'make_data_loader_from_adata'))
-               146 IMPORT_NAME             24 (decipher.tools._decipher.data)
-               148 IMPORT_FROM             25 (decipher_load_model)
-               150 STORE_NAME              25 (decipher_load_model)
-               152 IMPORT_FROM             26 (decipher_save_model)
-               154 STORE_NAME              26 (decipher_save_model)
-               156 IMPORT_FROM             27 (make_data_loader_from_adata)
-               158 STORE_NAME              27 (make_data_loader_from_adata)
+                64 LOAD_CONST               1 (None)
+                66 IMPORT_NAME             11 (pyro.optim)
+                68 STORE_NAME               4 (pyro)
+   
+    10          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               3 (('poutine',))
+                74 IMPORT_NAME              4 (pyro)
+                76 IMPORT_FROM             12 (poutine)
+                78 STORE_NAME              12 (poutine)
+                80 POP_TOP
+   
+    11          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               4 (('SVI', 'Trace_ELBO'))
+                86 IMPORT_NAME             13 (pyro.infer)
+                88 IMPORT_FROM             14 (SVI)
+                90 STORE_NAME              14 (SVI)
+                92 IMPORT_FROM             15 (Trace_ELBO)
+                94 STORE_NAME              15 (Trace_ELBO)
+                96 POP_TOP
+   
+    12          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               5 (('tqdm',))
+               102 IMPORT_NAME             16 (tqdm)
+               104 IMPORT_FROM             16 (tqdm)
+               106 STORE_NAME              16 (tqdm)
+               108 POP_TOP
+   
+    14         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               6 (('decipher',))
+               114 IMPORT_NAME             17 (decipher.plot.decipher)
+               116 IMPORT_FROM             18 (decipher)
+               118 STORE_NAME              19 (plot_decipher_v)
+               120 POP_TOP
+   
+    15         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST               7 (('Decipher', 'DecipherConfig'))
+               126 IMPORT_NAME             20 (decipher.tools._decipher)
+               128 IMPORT_FROM             21 (Decipher)
+               130 STORE_NAME              21 (Decipher)
+               132 IMPORT_FROM             22 (DecipherConfig)
+               134 STORE_NAME              22 (DecipherConfig)
+               136 POP_TOP
+   
+    16         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST               8 (('decipher_load_model', 'decipher_save_model', 'make_data_loader_from_adata', 'get_dense_X'))
+               142 IMPORT_NAME             23 (decipher.tools._decipher.data)
+               144 IMPORT_FROM             24 (decipher_load_model)
+               146 STORE_NAME              24 (decipher_load_model)
+               148 IMPORT_FROM             25 (decipher_save_model)
+               150 STORE_NAME              25 (decipher_save_model)
+               152 IMPORT_FROM             26 (make_data_loader_from_adata)
+               154 STORE_NAME              26 (make_data_loader_from_adata)
+               156 IMPORT_FROM             27 (get_dense_X)
+               158 STORE_NAME              27 (get_dense_X)
                160 POP_TOP
    
-    21         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              10 (('EarlyStopping',))
+    22         162 LOAD_CONST               0 (0)
+               164 LOAD_CONST               9 (('EarlyStopping',))
                166 IMPORT_NAME             28 (decipher.tools.utils)
                168 IMPORT_FROM             29 (EarlyStopping)
                170 STORE_NAME              29 (EarlyStopping)
                172 POP_TOP
    
-    22         174 LOAD_CONST               0 (0)
-               176 LOAD_CONST              11 (('DECIPHER_GLOBALS', 'GIFMaker', 'is_notebook', 'load_and_show_gif'))
+    23         174 LOAD_CONST               0 (0)
+               176 LOAD_CONST              10 (('DECIPHER_GLOBALS', 'GIFMaker', 'is_notebook', 'load_and_show_gif'))
                178 IMPORT_NAME             30 (decipher.utils)
                180 IMPORT_FROM             31 (DECIPHER_GLOBALS)
                182 STORE_NAME              31 (DECIPHER_GLOBALS)
                184 IMPORT_FROM             32 (GIFMaker)
                186 STORE_NAME              32 (GIFMaker)
                188 IMPORT_FROM             33 (is_notebook)
                190 STORE_NAME              33 (is_notebook)
                192 IMPORT_FROM             34 (load_and_show_gif)
                194 STORE_NAME              34 (load_and_show_gif)
                196 POP_TOP
    
-    24         198 PUSH_NULL
+    25         198 PUSH_NULL
                200 LOAD_NAME                0 (logging)
                202 LOAD_ATTR               35 (getLogger)
                212 LOAD_NAME               36 (__name__)
                214 PRECALL                  1
                218 CALL                     1
                228 STORE_NAME              37 (logger)
    
-    25         230 PUSH_NULL
+    26         230 PUSH_NULL
                232 LOAD_NAME                0 (logging)
                234 LOAD_ATTR               38 (basicConfig)
    
-    26         244 LOAD_CONST              12 ('%(asctime)s | %(levelname)s : %(message)s')
+    27         244 LOAD_CONST              11 ('%(asctime)s | %(levelname)s : %(message)s')
    
-    27         246 LOAD_NAME                0 (logging)
+    28         246 LOAD_NAME                0 (logging)
                248 LOAD_ATTR               39 (INFO)
    
-    25         258 KW_NAMES                13
+    26         258 KW_NAMES                12
                260 PRECALL                  2
                264 CALL                     2
                274 POP_TOP
    
-    31         276 LOAD_CONST              14 (<code object predictive_log_likelihood, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 31>)
-               278 MAKE_FUNCTION            0
-               280 STORE_NAME              40 (predictive_log_likelihood)
+    32         276 LOAD_CONST              27 ((30,))
+               278 LOAD_CONST              14 (<code object predictive_log_likelihood, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 32>)
+               280 MAKE_FUNCTION            1 (defaults)
+               282 STORE_NAME              40 (predictive_log_likelihood)
    
-    47         282 LOAD_CONST              15 (<code object _make_train_val_split, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 47>)
-               284 MAKE_FUNCTION            0
-               286 STORE_NAME              41 (_make_train_val_split)
+    55         284 LOAD_CONST              15 (<code object _make_train_val_split, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 55>)
+               286 MAKE_FUNCTION            0
+               288 STORE_NAME              41 (_make_train_val_split)
    
-    63         288 PUSH_NULL
-               290 LOAD_NAME               23 (DecipherConfig)
-               292 PRECALL                  0
-               296 CALL                     0
+    71         290 PUSH_NULL
+               292 LOAD_NAME               22 (DecipherConfig)
+               294 PRECALL                  0
+               298 CALL                     0
    
-    64         306 LOAD_CONST              16 (-1)
+    72         308 LOAD_CONST              16 (-1)
    
-    65         308 LOAD_CONST               1 (None)
+    73         310 LOAD_CONST               1 (None)
    
-    61         310 BUILD_TUPLE              3
-               312 LOAD_CONST              17 ('adata')
+    74         312 LOAD_CONST              17 ('cpu')
    
-    62         314 LOAD_NAME                6 (sc)
-               316 LOAD_ATTR               42 (AnnData)
+    69         314 BUILD_TUPLE              4
+               316 LOAD_CONST              18 ('adata')
    
-    61         326 BUILD_TUPLE              2
-               328 LOAD_CONST              18 (<code object decipher_train, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 61>)
-               330 MAKE_FUNCTION            5 (defaults, annotations)
-               332 STORE_NAME              43 (decipher_train)
+    70         318 LOAD_NAME                6 (sc)
+               320 LOAD_ATTR               42 (AnnData)
    
-   197         334 LOAD_CONST              26 ((1,))
-               336 LOAD_CONST              20 (<code object rot, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 197>)
-               338 MAKE_FUNCTION            1 (defaults)
-               340 STORE_NAME              44 (rot)
+    69         330 BUILD_TUPLE              2
+               332 LOAD_CONST              19 (<code object decipher_train, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 69>)
+               334 MAKE_FUNCTION            5 (defaults, annotations)
+               336 STORE_NAME              43 (decipher_train)
    
-   205         342 NOP
+   239         338 LOAD_CONST              28 ((1,))
+               340 LOAD_CONST              21 (<code object rot, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 239>)
+               342 MAKE_FUNCTION            1 (defaults)
+               344 STORE_NAME              44 (rot)
    
-   206         344 NOP
+   247         346 NOP
    
-   207         346 NOP
+   248         348 NOP
    
-   208         348 NOP
+   249         350 NOP
    
-   209         350 NOP
+   250         352 NOP
    
-   203         352 LOAD_CONST              27 ((None, None, None, None, True))
-               354 LOAD_CONST              22 (<code object decipher_rotate_space, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 203>)
-               356 MAKE_FUNCTION            1 (defaults)
-               358 STORE_NAME              45 (decipher_rotate_space)
+   251         354 NOP
    
-   295         360 LOAD_CONST              23 (<code object decipher_gene_imputation, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 295>)
-               362 MAKE_FUNCTION            0
-               364 STORE_NAME              46 (decipher_gene_imputation)
+   245         356 LOAD_CONST              29 ((None, None, None, None, True))
+               358 LOAD_CONST              23 (<code object decipher_rotate_space, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 245>)
+               360 MAKE_FUNCTION            1 (defaults)
+               362 STORE_NAME              45 (decipher_rotate_space)
    
-   314         366 LOAD_CONST              24 (<code object decipher_and_gene_covariance, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 314>)
-               368 MAKE_FUNCTION            0
-               370 STORE_NAME              47 (decipher_and_gene_covariance)
+   337         364 LOAD_CONST              24 (<code object decipher_gene_imputation, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 337>)
+               366 MAKE_FUNCTION            0
+               368 STORE_NAME              46 (decipher_gene_imputation)
    
-   332         372 LOAD_CONST              25 (<code object _decipher_to_adata, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 332>)
-               374 MAKE_FUNCTION            0
-               376 STORE_NAME              48 (_decipher_to_adata)
-               378 LOAD_CONST               1 (None)
-               380 RETURN_VALUE
+   356         370 LOAD_CONST              25 (<code object decipher_and_gene_covariance, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 356>)
+               372 MAKE_FUNCTION            0
+               374 STORE_NAME              47 (decipher_and_gene_covariance)
+   
+   378         376 LOAD_CONST              26 (<code object _decipher_to_adata, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 378>)
+               378 MAKE_FUNCTION            0
+               380 STORE_NAME              48 (_decipher_to_adata)
+               382 LOAD_CONST               1 (None)
+               384 RETURN_VALUE
    consts
       0
       None
       ('pyplot',)
       ('poutine',)
       ('SVI', 'Trace_ELBO')
-      ('MultiStepLR',)
       ('tqdm',)
       ('decipher',)
       ('Decipher', 'DecipherConfig')
-      ('decipher_load_model', 'decipher_save_model', 'make_data_loader_from_adata')
+      ('decipher_load_model', 'decipher_save_model', 'make_data_loader_from_adata', 'get_dense_X')
       ('EarlyStopping',)
       ('DECIPHER_GLOBALS', 'GIFMaker', 'is_notebook', 'load_and_show_gif')
       '%(asctime)s | %(levelname)s : %(message)s'
       ('format', 'level')
+      30
       code
-         argcount  : 2
-         nlocals   : 8
-         stacksize : 5
+         argcount  : 3
+         nlocals   : 11
+         stacksize : 9
          flags     : 3
          code
-            0x97007401000000000000000000007c01a6010000ab0100000000000000
-            007402000000000000000000006a0200000000000000006b020000000072
-            1a7407000000000000000000007c017c006a0400000000000000006a0500
-            00000000000000a6020000ab0200000000000000007d017c00a006000000
-            0000000000000000000000000000000000a6000000ab0000000000000000
-            00010064017d027c0144005d9a7d030200740f000000000000000000006a
-            0800000000000000007c006a090000000000000000a6010000ab01000000
-            00000000006a0a00000000000000007c038e007d04740f00000000000000
-            0000006a0b00000000000000007c006a0c00000000000000007c04ac02a6
-            020000ab0200000000000000007d05740f000000000000000000006a0d00
-            000000000000007c0564036701ac04a6020000ab0200000000000000007d
-            060200740f000000000000000000006a0800000000000000007c06a60100
-            00ab0100000000000000006a0a00000000000000007c038e007d077c027c
-            07a00e0000000000000000000000000000000000000000a6000000ab0000
-            00000000000000a00f0000000000000000000000000000000000000000a6
-            000000ab0000000000000000007a0d00007d028c9b7c0274210000000000
-            00000000007c016a110000000000000000a6010000ab0100000000000000
-            007a0b00005300
-          31           0 RESUME                   0
-         
-          33           2 LOAD_GLOBAL              1 (NULL + type)
-                      14 LOAD_FAST                1 (dataloader)
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 LOAD_GLOBAL              2 (sc)
-                      42 LOAD_ATTR                2 (AnnData)
-                      52 COMPARE_OP               2 (==)
-                      58 POP_JUMP_FORWARD_IF_FALSE    26 (to 112)
-         
-          34          60 LOAD_GLOBAL              7 (NULL + make_data_loader_from_adata)
-                      72 LOAD_FAST                1 (dataloader)
-                      74 LOAD_FAST                0 (decipher)
-                      76 LOAD_ATTR                4 (config)
-                      86 LOAD_ATTR                5 (batch_size)
-                      96 PRECALL                  2
-                     100 CALL                     2
-                     110 STORE_FAST               1 (dataloader)
-         
-          36     >>  112 LOAD_FAST                0 (decipher)
-                     114 LOAD_METHOD              6 (eval)
-                     136 PRECALL                  0
-                     140 CALL                     0
-                     150 POP_TOP
-         
-          37         152 LOAD_CONST               1 (0)
-                     154 STORE_FAST               2 (log_likelihood)
-         
-          38         156 LOAD_FAST                1 (dataloader)
-                     158 GET_ITER
-                 >>  160 FOR_ITER               154 (to 470)
-                     162 STORE_FAST               3 (xc)
-         
-          39         164 PUSH_NULL
-                     166 LOAD_GLOBAL             15 (NULL + poutine)
-                     178 LOAD_ATTR                8 (trace)
-                     188 LOAD_FAST                0 (decipher)
-                     190 LOAD_ATTR                9 (guide)
-                     200 PRECALL                  1
-                     204 CALL                     1
-                     214 LOAD_ATTR               10 (get_trace)
-                     224 LOAD_FAST                3 (xc)
-                     226 CALL_FUNCTION_EX         0
-                     228 STORE_FAST               4 (guide_trace)
-         
-          40         230 LOAD_GLOBAL             15 (NULL + poutine)
-                     242 LOAD_ATTR               11 (replay)
-                     252 LOAD_FAST                0 (decipher)
-                     254 LOAD_ATTR               12 (model)
-                     264 LOAD_FAST                4 (guide_trace)
-                     266 KW_NAMES                 2
-                     268 PRECALL                  2
-                     272 CALL                     2
-                     282 STORE_FAST               5 (replayed_model)
-         
-          41         284 LOAD_GLOBAL             15 (NULL + poutine)
-                     296 LOAD_ATTR               13 (block)
-                     306 LOAD_FAST                5 (replayed_model)
-                     308 LOAD_CONST               3 ('x')
-                     310 BUILD_LIST               1
-                     312 KW_NAMES                 4
-                     314 PRECALL                  2
-                     318 CALL                     2
-                     328 STORE_FAST               6 (blocked_replayed_model)
-         
-          42         330 PUSH_NULL
-                     332 LOAD_GLOBAL             15 (NULL + poutine)
-                     344 LOAD_ATTR                8 (trace)
-                     354 LOAD_FAST                6 (blocked_replayed_model)
-                     356 PRECALL                  1
-                     360 CALL                     1
-                     370 LOAD_ATTR               10 (get_trace)
-                     380 LOAD_FAST                3 (xc)
-                     382 CALL_FUNCTION_EX         0
-                     384 STORE_FAST               7 (model_trace)
-         
-          43         386 LOAD_FAST                2 (log_likelihood)
-                     388 LOAD_FAST                7 (model_trace)
-                     390 LOAD_METHOD             14 (log_prob_sum)
-                     412 PRECALL                  0
-                     416 CALL                     0
-                     426 LOAD_METHOD             15 (item)
-                     448 PRECALL                  0
-                     452 CALL                     0
-                     462 BINARY_OP               13 (+=)
-                     466 STORE_FAST               2 (log_likelihood)
-                     468 JUMP_BACKWARD          155 (to 160)
-         
-          44     >>  470 LOAD_FAST                2 (log_likelihood)
-                     472 LOAD_GLOBAL             33 (NULL + len)
-                     484 LOAD_FAST                1 (dataloader)
-                     486 LOAD_ATTR               17 (dataset)
-                     496 PRECALL                  1
-                     500 CALL                     1
-                     510 BINARY_OP               11 (/)
-                     514 RETURN_VALUE
+            0x8700970067007d0389006a0000000000000000006a0100000000000000
+            007d04640189006a0000000000000000005f010000000000000000090074
+            05000000000000000000007c02a6010000ab01000000000000000044005d
+            ae7d0564027d067c0144005d927d0788006601640384087c074400a60000
+            00ab0000000000000000007d0702007407000000000000000000006a0400
+            0000000000000089006a050000000000000000a6010000ab010000000000
+            0000006a0600000000000000007c078e007d080200740700000000000000
+            0000006a0400000000000000007407000000000000000000006a07000000
+            000000000089006a0800000000000000007c08ac04a6020000ab02000000
+            0000000000a6010000ab0100000000000000006a0600000000000000007c
+            078e007d097c067c09a00900000000000000000000000000000000000000
+            00a6000000ab0000000000000000007c08a0090000000000000000000000
+            000000000000000000a6000000ab0000000000000000007a0a00007a0d00
+            007d068c937c03a00a00000000000000000000000000000000000000007c
+            06a6010000ab01000000000000000001008caf09007c0489006a00000000
+            00000000005f0100000000000000006e1123007c0489006a000000000000
+            0000005f0100000000000000007700780359007701741700000000000000
+            0000006a0c00000000000000007417000000000000000000006a0d000000
+            00000000007c03a6010000ab010000000000000000741d00000000000000
+            0000006a0f00000000000000007c02a6010000ab0100000000000000007a
+            0a00006402a6020000ab0200000000000000007d0a7c0aa0100000000000
+            000000000000000000000000000000a6000000ab00000000000000000053
+            00
+                       0 MAKE_CELL                0 (decipher)
+         
+          32           2 RESUME                   0
+         
+          33           4 BUILD_LIST               0
+                       6 STORE_FAST               3 (log_weights)
+         
+          34           8 LOAD_DEREF               0 (decipher)
+                      10 LOAD_ATTR                0 (config)
+                      20 LOAD_ATTR                1 (beta)
+                      30 STORE_FAST               4 (old_beta)
+         
+          35          32 LOAD_CONST               1 (1.0)
+                      34 LOAD_DEREF               0 (decipher)
+                      36 LOAD_ATTR                0 (config)
+                      46 STORE_ATTR               1 (beta)
+         
+          36          56 NOP
+         
+          37          58 LOAD_GLOBAL              5 (NULL + range)
+                      70 LOAD_FAST                2 (n_samples)
+                      72 PRECALL                  1
+                      76 CALL                     1
+                      86 GET_ITER
+                 >>   88 FOR_ITER               174 (to 438)
+                      90 STORE_FAST               5 (i)
+         
+          38          92 LOAD_CONST               2 (0)
+                      94 STORE_FAST               6 (total_log_prob)
+         
+          39          96 LOAD_FAST                1 (dataloader)
+                      98 GET_ITER
+                 >>  100 FOR_ITER               146 (to 394)
+                     102 STORE_FAST               7 (xc)
+         
+          40         104 LOAD_CLOSURE             0 (decipher)
+                     106 BUILD_TUPLE              1
+                     108 LOAD_CONST               3 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 40>)
+                     110 MAKE_FUNCTION            8 (closure)
+                     112 LOAD_FAST                7 (xc)
+                     114 GET_ITER
+                     116 PRECALL                  0
+                     120 CALL                     0
+                     130 STORE_FAST               7 (xc)
+         
+          41         132 PUSH_NULL
+                     134 LOAD_GLOBAL              7 (NULL + poutine)
+                     146 LOAD_ATTR                4 (trace)
+                     156 LOAD_DEREF               0 (decipher)
+                     158 LOAD_ATTR                5 (guide)
+                     168 PRECALL                  1
+                     172 CALL                     1
+                     182 LOAD_ATTR                6 (get_trace)
+                     192 LOAD_FAST                7 (xc)
+                     194 CALL_FUNCTION_EX         0
+                     196 STORE_FAST               8 (guide_trace)
+         
+          42         198 PUSH_NULL
+                     200 LOAD_GLOBAL              7 (NULL + poutine)
+                     212 LOAD_ATTR                4 (trace)
+         
+          43         222 LOAD_GLOBAL              7 (NULL + poutine)
+                     234 LOAD_ATTR                7 (replay)
+                     244 LOAD_DEREF               0 (decipher)
+                     246 LOAD_ATTR                8 (model)
+                     256 LOAD_FAST                8 (guide_trace)
+                     258 KW_NAMES                 4
+                     260 PRECALL                  2
+                     264 CALL                     2
+         
+          42         274 PRECALL                  1
+                     278 CALL                     1
+         
+          44         288 LOAD_ATTR                6 (get_trace)
+                     298 LOAD_FAST                7 (xc)
+         
+          42         300 CALL_FUNCTION_EX         0
+                     302 STORE_FAST               9 (model_trace)
+         
+          45         304 LOAD_FAST                6 (total_log_prob)
+                     306 LOAD_FAST                9 (model_trace)
+                     308 LOAD_METHOD              9 (log_prob_sum)
+                     330 PRECALL                  0
+                     334 CALL                     0
+                     344 LOAD_FAST                8 (guide_trace)
+                     346 LOAD_METHOD              9 (log_prob_sum)
+                     368 PRECALL                  0
+                     372 CALL                     0
+                     382 BINARY_OP               10 (-)
+                     386 BINARY_OP               13 (+=)
+                     390 STORE_FAST               6 (total_log_prob)
+                     392 JUMP_BACKWARD          147 (to 100)
+         
+          46     >>  394 LOAD_FAST                3 (log_weights)
+                     396 LOAD_METHOD             10 (append)
+                     418 LOAD_FAST                6 (total_log_prob)
+                     420 PRECALL                  1
+                     424 CALL                     1
+                     434 POP_TOP
+                     436 JUMP_BACKWARD          175 (to 88)
+         
+          37     >>  438 NOP
+         
+          49         440 LOAD_FAST                4 (old_beta)
+                     442 LOAD_DEREF               0 (decipher)
+                     444 LOAD_ATTR                0 (config)
+                     454 STORE_ATTR               1 (beta)
+                     464 JUMP_FORWARD            17 (to 500)
+                 >>  466 PUSH_EXC_INFO
+                     468 LOAD_FAST                4 (old_beta)
+                     470 LOAD_DEREF               0 (decipher)
+                     472 LOAD_ATTR                0 (config)
+                     482 STORE_ATTR               1 (beta)
+                     492 RERAISE                  0
+                 >>  494 COPY                     3
+                     496 POP_EXCEPT
+                     498 RERAISE                  1
+         
+          51     >>  500 LOAD_GLOBAL             23 (NULL + torch)
+                     512 LOAD_ATTR               12 (logsumexp)
+                     522 LOAD_GLOBAL             23 (NULL + torch)
+                     534 LOAD_ATTR               13 (tensor)
+                     544 LOAD_FAST                3 (log_weights)
+                     546 PRECALL                  1
+                     550 CALL                     1
+                     560 LOAD_GLOBAL             29 (NULL + np)
+                     572 LOAD_ATTR               15 (log)
+                     582 LOAD_FAST                2 (n_samples)
+                     584 PRECALL                  1
+                     588 CALL                     1
+                     598 BINARY_OP               10 (-)
+                     602 LOAD_CONST               2 (0)
+                     604 PRECALL                  2
+                     608 CALL                     2
+                     618 STORE_FAST              10 (log_z)
+         
+          52         620 LOAD_FAST               10 (log_z)
+                     622 LOAD_METHOD             16 (item)
+                     644 PRECALL                  0
+                     648 CALL                     0
+                     658 RETURN_VALUE
+         ExceptionTable:
+           58 to 436 -> 466 [0]
+           466 to 492 -> 494 [1] lasti
          consts
-            'Compute the predictive log likelihood of the decipher model.'
+            None
+            1.0
             0
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 19
+               code
+                  0x9501970067007c005d1c7d017c01a00000000000000000000000000000
+                  0000000000000089026a010000000000000000a6010000ab010000000000
+                  00000091028c1d5300
+                             0 COPY_FREE_VARS           1
+               
+                40           2 RESUME                   0
+                             4 BUILD_LIST               0
+                             6 LOAD_FAST                0 (.0)
+                       >>    8 FOR_ITER                28 (to 66)
+                            10 STORE_FAST               1 (x)
+                            12 LOAD_FAST                1 (x)
+                            14 LOAD_METHOD              0 (to)
+                            36 LOAD_DEREF               2 (decipher)
+                            38 LOAD_ATTR                1 (device)
+                            48 PRECALL                  1
+                            52 CALL                     1
+                            62 LIST_APPEND              2
+                            64 JUMP_BACKWARD           29 (to 8)
+                       >>   66 RETURN_VALUE
+               consts
+               names      ('to', 'device')
+               varnames   ('.0', 'x')
+               freevars   ('decipher',)
+               cellvars   ()
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
+               name       '<listcomp>'
+               firstlineno 40
+               lnotab 0x
             ('trace',)
-            'x'
-            ('expose',)
-         names      ('type', 'sc', 'AnnData', 'make_data_loader_from_adata', 'config', 'batch_size', 'eval', 'poutine', 'trace', 'guide', 'get_trace', 'replay', 'model', 'block', 'log_prob_sum', 'item', 'len', 'dataset')
-         varnames   ('decipher', 'dataloader', 'log_likelihood', 'xc', 'guide_trace', 'replayed_model', 'blocked_replayed_model', 'model_trace')
+         names      ('config', 'beta', 'range', 'poutine', 'trace', 'guide', 'get_trace', 'replay', 'model', 'log_prob_sum', 'append', 'torch', 'logsumexp', 'tensor', 'np', 'log', 'item')
+         varnames   ('decipher', 'dataloader', 'n_samples', 'log_weights', 'old_beta', 'i', 'total_log_prob', 'xc', 'guide_trace', 'model_trace', 'log_z')
          freevars   ()
-         cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         cellvars   ('decipher',)
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       'predictive_log_likelihood'
-         firstlineno 31
-         lnotab 0x02023a013402280104010801420136012e0138015401
+         firstlineno 32
+         lnotab
+            0x040104011801180102012201040108011c014201180134ff0e020cfe04
+            035a012cf7020c3c027801
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000007c017c006a01000000000000000064
@@ -387,101 +477,101 @@
             0700000000000000006a0800000000000000007c006a0700000000000000
             006a0900000000000000007c0519000000000000000000640366023c0000
             007c006a070000000000000000640319000000000000000000a00a000000
             00000000000000000000000000000000006405a6010000ab010000000000
             0000007c006a07000000000000000064033c000000741700000000000000
             0000006a0c000000000000000064067c039b0064079d03a6010000ab0100
             00000000000000010064005300
-          47           0 RESUME                   0
+          55           0 RESUME                   0
          
-          48           2 LOAD_GLOBAL              1 (NULL + int)
+          56           2 LOAD_GLOBAL              1 (NULL + int)
                       14 LOAD_FAST                1 (val_frac)
                       16 LOAD_FAST                0 (adata)
                       18 LOAD_ATTR                1 (shape)
                       28 LOAD_CONST               1 (0)
                       30 BINARY_SUBSCR
                       40 BINARY_OP                5 (*)
                       44 PRECALL                  1
                       48 CALL                     1
                       58 STORE_FAST               3 (n_val)
          
-          49          60 LOAD_GLOBAL              5 (NULL + np)
+          57          60 LOAD_GLOBAL              5 (NULL + np)
                       72 LOAD_ATTR                3 (arange)
                       82 LOAD_FAST                0 (adata)
                       84 LOAD_ATTR                1 (shape)
                       94 LOAD_CONST               1 (0)
                       96 BINARY_SUBSCR
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               4 (cell_idx)
          
-          50         122 LOAD_GLOBAL              4 (np)
+          58         122 LOAD_GLOBAL              4 (np)
                      134 LOAD_ATTR                4 (random)
                      144 LOAD_METHOD              5 (default_rng)
                      166 LOAD_FAST                2 (seed)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 LOAD_METHOD              6 (shuffle)
                      204 LOAD_FAST                4 (cell_idx)
                      206 PRECALL                  1
                      210 CALL                     1
                      220 POP_TOP
          
-          51         222 LOAD_FAST                4 (cell_idx)
+          59         222 LOAD_FAST                4 (cell_idx)
                      224 LOAD_FAST                3 (n_val)
                      226 UNARY_NEGATIVE
                      228 LOAD_CONST               0 (None)
                      230 BUILD_SLICE              2
                      232 BINARY_SUBSCR
                      242 STORE_FAST               5 (val_idx)
          
-          52         244 LOAD_CONST               2 ('train')
+          60         244 LOAD_CONST               2 ('train')
                      246 LOAD_FAST                0 (adata)
                      248 LOAD_ATTR                7 (obs)
                      258 LOAD_CONST               3 ('decipher_split')
                      260 STORE_SUBSCR
          
-          53         264 LOAD_CONST               4 ('validation')
+          61         264 LOAD_CONST               4 ('validation')
                      266 LOAD_FAST                0 (adata)
                      268 LOAD_ATTR                7 (obs)
                      278 LOAD_ATTR                8 (loc)
                      288 LOAD_FAST                0 (adata)
                      290 LOAD_ATTR                7 (obs)
                      300 LOAD_ATTR                9 (index)
                      310 LOAD_FAST                5 (val_idx)
                      312 BINARY_SUBSCR
                      322 LOAD_CONST               3 ('decipher_split')
                      324 BUILD_TUPLE              2
                      326 STORE_SUBSCR
          
-          54         330 LOAD_FAST                0 (adata)
+          62         330 LOAD_FAST                0 (adata)
                      332 LOAD_ATTR                7 (obs)
                      342 LOAD_CONST               3 ('decipher_split')
                      344 BINARY_SUBSCR
                      354 LOAD_METHOD             10 (astype)
                      376 LOAD_CONST               5 ('category')
                      378 PRECALL                  1
                      382 CALL                     1
                      392 LOAD_FAST                0 (adata)
                      394 LOAD_ATTR                7 (obs)
                      404 LOAD_CONST               3 ('decipher_split')
                      406 STORE_SUBSCR
          
-          55         410 LOAD_GLOBAL             23 (NULL + logging)
+          63         410 LOAD_GLOBAL             23 (NULL + logging)
                      422 LOAD_ATTR               12 (info)
          
-          56         432 LOAD_CONST               6 ("Added `.obs['decipher_split']`: the Decipher train/validation split.\n ")
+          64         432 LOAD_CONST               6 ("Added `.obs['decipher_split']`: the Decipher train/validation split.\n ")
          
-          57         434 LOAD_FAST                3 (n_val)
+          65         434 LOAD_FAST                3 (n_val)
          
-          56         436 FORMAT_VALUE             0
+          64         436 FORMAT_VALUE             0
                      438 LOAD_CONST               7 (' cells in validation set.')
                      440 BUILD_STRING             3
          
-          55         442 PRECALL                  1
+          63         442 PRECALL                  1
                      446 CALL                     1
                      456 POP_TOP
                      458 LOAD_CONST               0 (None)
                      460 RETURN_VALUE
          consts
             None
             0
@@ -491,641 +581,898 @@
             'category'
             "Added `.obs['decipher_split']`: the Decipher train/validation split.\n "
             ' cells in validation set.'
          names      ('int', 'shape', 'np', 'arange', 'random', 'default_rng', 'shuffle', 'obs', 'loc', 'index', 'astype', 'logging', 'info')
          varnames   ('adata', 'val_frac', 'seed', 'n_val', 'cell_idx', 'val_idx')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       '_make_train_val_split'
-         firstlineno 47
+         firstlineno 55
          lnotab 0x02013a013e01640116011401420150011601020102ff06ff
       -1
+      'cpu'
       'adata'
       code
-         argcount  : 4
-         nlocals   : 29
-         stacksize : 10
+         argcount  : 5
+         nlocals   : 34
+         stacksize : 17
          flags     : 3
          code
-            0x9700740100000000000000000000a6000000ab00000000000000000072
-            227c0264016b0200000000721c64027d02740200000000000000000000a0
-            0200000000000000000000000000000000000000006403a6010000ab0100
-            0000000000000001007407000000000000000000006a0400000000000000
-            00a6000000ab00000000000000000001007406000000000000000000006a
-            050000000000000000a00600000000000000000000000000000000000000
-            007c016a070000000000000000a6010000ab010000000000000000010074
-            11000000000000000000007c007c016a0900000000000000007c016a0700
-            00000000000000a6030000ab03000000000000000001007c006a0a000000
-            000000000064041900000000000000000064056b02000000007d047c006a
-            0a000000000000000064041900000000000000000064066b02000000007d
-            057c007c046407640785026602190000000000000000007d067c007c0564
-            07640785026602190000000000000000007d077c03800e74170000000000
-            0000000000a6000000ab0000000000000000007d037c01a00c0000000000
-            0000000000000000000000000000007c06a6010000ab0100000000000000
-            000100741b000000000000000000007c067c016a0e0000000000000000a6
-            020000ab0200000000000000007d08741b000000000000000000007c077c
-            016a0e0000000000000000a6020000ab0200000000000000007d09741f00
-            0000000000000000007c01ac08a6010000ab0100000000000000007d0a74
-            06000000000000000000006a100000000000000000a01100000000000000
-            000000000000000000000000007c016a1200000000000000006409640a9c
-            02a6010000ab0100000000000000007d0b742700000000000000000000a6
-            000000ab0000000000000000007d0c7429000000000000000000007c0a6a
-            1500000000000000007c0a6a1600000000000000007c0b7c0ca6040000ab
-            0400000000000000007d0d742f00000000000000000000640bac0ca60100
-            00ab0100000000000000007d0e67007d0f74310000000000000000000064
-            02ac0da6010000ab0100000000000000007d107433000000000000000000
-            007435000000000000000000007c016a1b0000000000000000a6010000ab
-            010000000000000000a6010000ab0100000000000000007d117c11440090
-            015df77d1267007d137c0aa01c0000000000000000000000000000000000
-            000000a6000000ab00000000000000000001007c12640e6b040000000072
-            4a7c0aa01d0000000000000000000000000000000000000000a6000000ab
-            00000000000000000044005d357d14743d000000000000000000007c1474
-            3e000000000000000000006a2000000000000000006a2100000000000000
-            00a6020000ab02000000000000000072147c14a022000000000000000000
-            0000000000000000000000a6000000ab00000000000000000001008c367c
-            0844005d217d1502007c0d6a2300000000000000007c158e007d167c13a0
-            2400000000000000000000000000000000000000007c16a6010000ab0100
-            0000000000000001008c22744b000000000000000000006a260000000000
-            0000007c13a6010000ab010000000000000000744f000000000000000000
-            007c086a280000000000000000a6010000ab0100000000000000007a0b00
-            007d177c0aa0220000000000000000000000000000000000000000a60000
-            00ab00000000000000000001007453000000000000000000007c0a7c09a6
-            020000ab0200000000000000000b007d187c0fa024000000000000000000
-            00000000000000000000007c18a6010000ab01000000000000000001007c
-            11a02a0000000000000000000000000000000000000000640f7c129b0064
-            107c1764119b0464127c1864119b049d06a6010000ab0100000000000000
-            00010002007c107c18a6010000ab01000000000000000072117457000000
-            000000000000006413a6010000ab010000000000000000010001006ecd7c
-            02640e6b040000000072c57c127c027a060000640e6b020000000072bc74
-            59000000000000000000007c0a7c00a6020000ab02000000000000000001
-            00745b000000000000000000007c0066016414641569017c03a4018e0101
-            007c0ea02e0000000000000000000000000000000000000000745f000000
-            000000000000006a300000000000000000a6000000ab0000000000000000
-            00a6010000ab0100000000000000000100740100000000000000000000a6
-            000000ab0000000000000000007243640e64166c316d327d1901007c19a0
-            3300000000000000000000000000000000000000006417ac18a6010000ab
-            01000000000000000001007c19a032000000000000000000000000000000
-            0000000000745f000000000000000000006a300000000000000000a60000
-            00ab000000000000000000a6010000ab01000000000000000001006e1374
-            5f000000000000000000006a340000000000000000a6000000ab00000000
-            00000000000100745f000000000000000000006a350000000000000000a6
-            000000ab000000000000000000010090018cf97401000000000000000000
-            00a6000000ab000000000000000000722e640e64166c316d327d1901007c
-            19a0330000000000000000000000000000000000000000a6000000ab0000
-            0000000000000001007c11a0320000000000000000000000000000000000
-            000000a6000000ab00000000000000000001007459000000000000000000
-            007c0a7c00a6020000ab0200000000000000000100746d00000000000000
-            0000007c007c0aa6020000ab02000000000000000001007c006a37000000
-            0000000000641919000000000000000000641a190000000000000000007d
-            1a747000000000000000000000641b190000000000000000007d1b747200
-            0000000000000000006a3a0000000000000000a03b000000000000000000
-            00000000000000000000007c1b7c1a641ca6030000ab0300000000000000
-            007d1c7c0ea03c00000000000000000000000000000000000000007c1ca6
-            010000ab0100000000000000000100740100000000000000000000a60000
-            00ab000000000000000000720f747b000000000000000000007c1ca60100
-            00ab0100000000000000000100745b000000000000000000007c00660164
-            14641569017c03a4018e0101007c0a7c0f66025300
-          61           0 RESUME                   0
-         
-          95           2 LOAD_GLOBAL              1 (NULL + is_notebook)
-                      14 PRECALL                  0
-                      18 CALL                     0
-                      28 POP_JUMP_FORWARD_IF_FALSE    34 (to 98)
-                      30 LOAD_FAST                2 (plot_every_k_epochs)
-                      32 LOAD_CONST               1 (-1)
-                      34 COMPARE_OP               2 (==)
-                      40 POP_JUMP_FORWARD_IF_FALSE    28 (to 98)
-         
-          96          42 LOAD_CONST               2 (5)
-                      44 STORE_FAST               2 (plot_every_k_epochs)
-         
-          97          46 LOAD_GLOBAL              2 (logger)
-                      58 LOAD_METHOD              2 (info)
-         
-          98          80 LOAD_CONST               3 ('Plotting decipher space every 5 epochs by default. Set `plot_every_k_epoch` to -2 to disable.')
-         
-          97          82 PRECALL                  1
-                      86 CALL                     1
-                      96 POP_TOP
-         
-         102     >>   98 LOAD_GLOBAL              7 (NULL + pyro)
-                     110 LOAD_ATTR                4 (clear_param_store)
-                     120 PRECALL                  0
-                     124 CALL                     0
-                     134 POP_TOP
-         
-         103         136 LOAD_GLOBAL              6 (pyro)
-                     148 LOAD_ATTR                5 (util)
-                     158 LOAD_METHOD              6 (set_rng_seed)
-                     180 LOAD_FAST                1 (decipher_config)
-                     182 LOAD_ATTR                7 (seed)
-                     192 PRECALL                  1
-                     196 CALL                     1
-                     206 POP_TOP
-         
-         105         208 LOAD_GLOBAL             17 (NULL + _make_train_val_split)
-                     220 LOAD_FAST                0 (adata)
-                     222 LOAD_FAST                1 (decipher_config)
-                     224 LOAD_ATTR                9 (val_frac)
-                     234 LOAD_FAST                1 (decipher_config)
-                     236 LOAD_ATTR                7 (seed)
-                     246 PRECALL                  3
-                     250 CALL                     3
-                     260 POP_TOP
-         
-         106         262 LOAD_FAST                0 (adata)
-                     264 LOAD_ATTR               10 (obs)
-                     274 LOAD_CONST               4 ('decipher_split')
-                     276 BINARY_SUBSCR
-                     286 LOAD_CONST               5 ('train')
-                     288 COMPARE_OP               2 (==)
-                     294 STORE_FAST               4 (train_idx)
-         
-         107         296 LOAD_FAST                0 (adata)
-                     298 LOAD_ATTR               10 (obs)
-                     308 LOAD_CONST               4 ('decipher_split')
-                     310 BINARY_SUBSCR
-                     320 LOAD_CONST               6 ('validation')
-                     322 COMPARE_OP               2 (==)
-                     328 STORE_FAST               5 (val_idx)
-         
-         108         330 LOAD_FAST                0 (adata)
-                     332 LOAD_FAST                4 (train_idx)
-                     334 LOAD_CONST               7 (None)
+            0x87049700740100000000000000000000a6000000ab0000000000000000
+            0072227c0264016b0200000000721c64027d027402000000000000000000
+            00a00200000000000000000000000000000000000000006403a6010000ab
+            01000000000000000001007407000000000000000000006a040000000000
+            000000a6000000ab00000000000000000001007406000000000000000000
+            006a050000000000000000a0060000000000000000000000000000000000
+            0000007c016a070000000000000000a6010000ab01000000000000000001
+            007411000000000000000000007c007c016a0900000000000000007c016a
+            070000000000000000a6030000ab03000000000000000001007c006a0a00
+            0000000000000064041900000000000000000064056b02000000007d057c
+            006a0a000000000000000064041900000000000000000064066b02000000
+            007d067c007c056407640785026602190000000000000000007d077c007c
+            066407640785026602190000000000000000007d087c03800e7417000000
+            00000000000000a6000000ab0000000000000000007d037c01a00c000000
+            00000000000000000000000000000000007c07a6010000ab010000000000
+            0000000100741b000000000000000000007c077c016a0e00000000000000
+            006408ac09a6030000ab0300000000000000007d09741b00000000000000
+            0000007c087c016a0e0000000000000000a6020000ab0200000000000000
+            007d0a741f000000000000000000007c01ac0aa6010000ab010000000000
+            0000007d0b7c0ba010000000000000000000000000000000000000000089
+            04a6010000ab01000000000000000001007406000000000000000000006a
+            110000000000000000a01200000000000000000000000000000000000000
+            007c016a130000000000000000640b640c9c02a6010000ab010000000000
+            0000007d0c742900000000000000000000a6000000ab0000000000000000
+            007d0d742b000000000000000000007c0b6a1600000000000000007c0b6a
+            1700000000000000007c0c7c0da6040000ab0400000000000000007d0e74
+            3100000000000000000000640dac0ea6010000ab0100000000000000007d
+            0f67007d107c016a19000000000000000081217c016a1900000000000000
+            00640f6b040000000072167435000000000000000000007c016a19000000
+            0000000000ac10a6010000ab0100000000000000007d116e1d7435000000
+            000000000000007437000000000000000000006411a6010000ab01000000
+            0000000000ac10a6010000ab0100000000000000007d1174390000000000
+            0000000000743b000000000000000000007c016a1e0000000000000000a6
+            010000ab010000000000000000a6010000ab0100000000000000007d1264
+            077d1364077d147c12440090025d937d1567007d167c0ba01f0000000000
+            000000000000000000000000000000a6000000ab00000000000000000001
+            007c15640f6b0400000000724a7c0ba02000000000000000000000000000
+            00000000000000a6000000ab00000000000000000044005d357d17744300
+            0000000000000000007c177444000000000000000000006a230000000000
+            0000006a240000000000000000a6020000ab02000000000000000072147c
+            17a0250000000000000000000000000000000000000000a6000000ab0000
+            0000000000000001008c36744d000000000000000000007c09a6010000ab
+            0100000000000000007d18640f7d19640f7d1a7c0944005db57d1b090088
+            046601641284087c1b4400a6000000ab0000000000000000007d1b02007c
+            0e6a2700000000000000007c1b8e007d1c6e2f2300745000000000000000
+            000000240072227d1d74530000000000000000000064137c1da6020000ab
+            02000000000000000001007c0b7c1066026302590064077d1d7e1d630201
+            0063020100530064077d1d7e1d770177007803590077017c16a02a000000
+            00000000000000000000000000000000007c1ca6010000ab010000000000
+            00000001007c197c1c7a0d00007d197c1a7c1b640f190000000000000000
+            006a2b0000000000000000640f190000000000000000007a0d00007d1a7c
+            12a02c000000000000000000000000000000000000000064147c159b0064
+            15744d000000000000000000007c16a6010000ab0100000000000000009b
+            0064167c189b0064177c197c1a7a0b000064189b0464197c1364189b0464
+            1a7c1464189b049d0ca6010000ab01000000000000000001008cb67c0ba0
+            250000000000000000000000000000000000000000a6000000ab00000000
+            00000000000100745b000000000000000000007c0b7c0aa6020000ab0200
+            000000000000000b007c086a2b0000000000000000640f19000000000000
+            0000007a0b00007d147c10a02a0000000000000000000000000000000000
+            0000007c14a6010000ab01000000000000000001007c12a02c0000000000
+            00000000000000000000000000000064147c159b006415744d0000000000
+            00000000007c16a6010000ab0100000000000000009b0064167c189b0064
+            177c197c1a7a0b000064189b0464197c1364189b04641a7c1464189b049d
+            0ca6010000ab01000000000000000001007c197c1a7a0b00007d1302007c
+            117c14a6010000ab010000000000000000720201006ecd7c02640f6b0400
+            00000072c57c157c027a060000640f6b020000000072bc745d0000000000
+            00000000007c0b7c00a6020000ab0200000000000000000100745f000000
+            000000000000007c006601641b641c69017c03a4018e0101007c0fa03000
+            000000000000000000000000000000000000007463000000000000000000
+            006a320000000000000000a6000000ab000000000000000000a6010000ab
+            0100000000000000000100740100000000000000000000a6000000ab0000
+            000000000000007243640f641d6c336d347d1e01007c1ea0350000000000
+            0000000000000000000000000000006408ac1ea6010000ab010000000000
+            00000001007c1ea034000000000000000000000000000000000000000074
+            63000000000000000000006a320000000000000000a6000000ab00000000
+            0000000000a6010000ab01000000000000000001006e1374630000000000
+            00000000006a360000000000000000a6000000ab00000000000000000001
+            007463000000000000000000006a370000000000000000a6000000ab0000
+            00000000000000010090028c95740100000000000000000000a6000000ab
+            000000000000000000722e640f641d6c336d347d1e01007c1ea035000000
+            0000000000000000000000000000000000a6000000ab0000000000000000
+            0001007c12a0340000000000000000000000000000000000000000a60000
+            00ab00000000000000000001007c11a03800000000000000000000000000
+            00000000000000a6000000ab000000000000000000721a74020000000000
+            0000000000a0020000000000000000000000000000000000000000641fa6
+            010000ab0100000000000000000100745d000000000000000000007c0b7c
+            00a6020000ab02000000000000000001007473000000000000000000007c
+            007c0ba6020000ab02000000000000000001007c006a3a00000000000000
+            006420190000000000000000006421190000000000000000007d1f747600
+            0000000000000000006422190000000000000000007d2074780000000000
+            00000000006a3d0000000000000000a03e00000000000000000000000000
+            000000000000007c20747f000000000000000000007c1fa6010000ab0100
+            000000000000006423a6030000ab0300000000000000007d217c0f6a4000
+            0000000000000072327c0fa0410000000000000000000000000000000000
+            0000007c21a6010000ab0100000000000000000100740100000000000000
+            000000a6000000ab000000000000000000720f7485000000000000000000
+            007c21a6010000ab0100000000000000000100745f000000000000000000
+            007c006601641b641c69017c03a4018e0101007c0b7c1066025300
+                       0 MAKE_CELL                4 (device)
+         
+          69           2 RESUME                   0
+         
+         106           4 LOAD_GLOBAL              1 (NULL + is_notebook)
+                      16 PRECALL                  0
+                      20 CALL                     0
+                      30 POP_JUMP_FORWARD_IF_FALSE    34 (to 100)
+                      32 LOAD_FAST                2 (plot_every_k_epochs)
+                      34 LOAD_CONST               1 (-1)
+                      36 COMPARE_OP               2 (==)
+                      42 POP_JUMP_FORWARD_IF_FALSE    28 (to 100)
+         
+         107          44 LOAD_CONST               2 (5)
+                      46 STORE_FAST               2 (plot_every_k_epochs)
+         
+         108          48 LOAD_GLOBAL              2 (logger)
+                      60 LOAD_METHOD              2 (info)
+         
+         109          82 LOAD_CONST               3 ('Plotting decipher space every 5 epochs by default. Set `plot_every_k_epoch` to -2 to disable.')
+         
+         108          84 PRECALL                  1
+                      88 CALL                     1
+                      98 POP_TOP
+         
+         113     >>  100 LOAD_GLOBAL              7 (NULL + pyro)
+                     112 LOAD_ATTR                4 (clear_param_store)
+                     122 PRECALL                  0
+                     126 CALL                     0
+                     136 POP_TOP
+         
+         114         138 LOAD_GLOBAL              6 (pyro)
+                     150 LOAD_ATTR                5 (util)
+                     160 LOAD_METHOD              6 (set_rng_seed)
+                     182 LOAD_FAST                1 (decipher_config)
+                     184 LOAD_ATTR                7 (seed)
+                     194 PRECALL                  1
+                     198 CALL                     1
+                     208 POP_TOP
+         
+         116         210 LOAD_GLOBAL             17 (NULL + _make_train_val_split)
+                     222 LOAD_FAST                0 (adata)
+                     224 LOAD_FAST                1 (decipher_config)
+                     226 LOAD_ATTR                9 (val_frac)
+                     236 LOAD_FAST                1 (decipher_config)
+                     238 LOAD_ATTR                7 (seed)
+                     248 PRECALL                  3
+                     252 CALL                     3
+                     262 POP_TOP
+         
+         117         264 LOAD_FAST                0 (adata)
+                     266 LOAD_ATTR               10 (obs)
+                     276 LOAD_CONST               4 ('decipher_split')
+                     278 BINARY_SUBSCR
+                     288 LOAD_CONST               5 ('train')
+                     290 COMPARE_OP               2 (==)
+                     296 STORE_FAST               5 (train_idx)
+         
+         118         298 LOAD_FAST                0 (adata)
+                     300 LOAD_ATTR               10 (obs)
+                     310 LOAD_CONST               4 ('decipher_split')
+                     312 BINARY_SUBSCR
+                     322 LOAD_CONST               6 ('validation')
+                     324 COMPARE_OP               2 (==)
+                     330 STORE_FAST               6 (val_idx)
+         
+         119         332 LOAD_FAST                0 (adata)
+                     334 LOAD_FAST                5 (train_idx)
                      336 LOAD_CONST               7 (None)
-                     338 BUILD_SLICE              2
-                     340 BUILD_TUPLE              2
-                     342 BINARY_SUBSCR
-                     352 STORE_FAST               6 (adata_train)
-         
-         109         354 LOAD_FAST                0 (adata)
-                     356 LOAD_FAST                5 (val_idx)
-                     358 LOAD_CONST               7 (None)
+                     338 LOAD_CONST               7 (None)
+                     340 BUILD_SLICE              2
+                     342 BUILD_TUPLE              2
+                     344 BINARY_SUBSCR
+                     354 STORE_FAST               7 (adata_train)
+         
+         120         356 LOAD_FAST                0 (adata)
+                     358 LOAD_FAST                6 (val_idx)
                      360 LOAD_CONST               7 (None)
-                     362 BUILD_SLICE              2
-                     364 BUILD_TUPLE              2
-                     366 BINARY_SUBSCR
-                     376 STORE_FAST               7 (adata_val)
-         
-         111         378 LOAD_FAST                3 (plot_kwargs)
-                     380 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 410)
-         
-         112         382 LOAD_GLOBAL             23 (NULL + dict)
-                     394 PRECALL                  0
-                     398 CALL                     0
-                     408 STORE_FAST               3 (plot_kwargs)
-         
-         114     >>  410 LOAD_FAST                1 (decipher_config)
-                     412 LOAD_METHOD             12 (initialize_from_adata)
-                     434 LOAD_FAST                6 (adata_train)
-                     436 PRECALL                  1
-                     440 CALL                     1
-                     450 POP_TOP
-         
-         116         452 LOAD_GLOBAL             27 (NULL + make_data_loader_from_adata)
-                     464 LOAD_FAST                6 (adata_train)
-                     466 LOAD_FAST                1 (decipher_config)
-                     468 LOAD_ATTR               14 (batch_size)
-                     478 PRECALL                  2
-                     482 CALL                     2
-                     492 STORE_FAST               8 (dataloader_train)
-         
-         117         494 LOAD_GLOBAL             27 (NULL + make_data_loader_from_adata)
-                     506 LOAD_FAST                7 (adata_val)
-                     508 LOAD_FAST                1 (decipher_config)
-                     510 LOAD_ATTR               14 (batch_size)
-                     520 PRECALL                  2
-                     524 CALL                     2
-                     534 STORE_FAST               9 (dataloader_val)
-         
-         119         536 LOAD_GLOBAL             31 (NULL + Decipher)
-         
-         120         548 LOAD_FAST                1 (decipher_config)
-         
-         119         550 KW_NAMES                 8
-                     552 PRECALL                  1
-                     556 CALL                     1
-                     566 STORE_FAST              10 (decipher)
-         
-         122         568 LOAD_GLOBAL              6 (pyro)
-                     580 LOAD_ATTR               16 (optim)
-                     590 LOAD_METHOD             17 (ClippedAdam)
-         
-         124         612 LOAD_FAST                1 (decipher_config)
-                     614 LOAD_ATTR               18 (learning_rate)
-         
-         125         624 LOAD_CONST               9 (0.0001)
-         
-         123         626 LOAD_CONST              10 (('lr', 'weight_decay'))
-                     628 BUILD_CONST_KEY_MAP      2
-         
-         122         630 PRECALL                  1
-                     634 CALL                     1
-                     644 STORE_FAST              11 (optimizer)
-         
-         128         646 LOAD_GLOBAL             39 (NULL + Trace_ELBO)
-                     658 PRECALL                  0
-                     662 CALL                     0
-                     672 STORE_FAST              12 (elbo)
-         
-         129         674 LOAD_GLOBAL             41 (NULL + SVI)
-                     686 LOAD_FAST               10 (decipher)
-                     688 LOAD_ATTR               21 (model)
-                     698 LOAD_FAST               10 (decipher)
-                     700 LOAD_ATTR               22 (guide)
-                     710 LOAD_FAST               11 (optimizer)
-                     712 LOAD_FAST               12 (elbo)
-                     714 PRECALL                  4
-                     718 CALL                     4
-                     728 STORE_FAST              13 (svi)
-         
-         130         730 LOAD_GLOBAL             47 (NULL + GIFMaker)
-                     742 LOAD_CONST              11 (120)
-                     744 KW_NAMES                12
-                     746 PRECALL                  1
-                     750 CALL                     1
-                     760 STORE_FAST              14 (gif_maker)
-         
-         133         762 BUILD_LIST               0
-                     764 STORE_FAST              15 (val_losses)
-         
-         134         766 LOAD_GLOBAL             49 (NULL + EarlyStopping)
-                     778 LOAD_CONST               2 (5)
-                     780 KW_NAMES                13
-                     782 PRECALL                  1
-                     786 CALL                     1
-                     796 STORE_FAST              16 (early_stopping)
-         
-         135         798 LOAD_GLOBAL             51 (NULL + tqdm)
-                     810 LOAD_GLOBAL             53 (NULL + range)
-                     822 LOAD_FAST                1 (decipher_config)
-                     824 LOAD_ATTR               27 (n_epochs)
-                     834 PRECALL                  1
-                     838 CALL                     1
-                     848 PRECALL                  1
-                     852 CALL                     1
-                     862 STORE_FAST              17 (pbar)
-         
-         136         864 LOAD_FAST               17 (pbar)
-                     866 GET_ITER
-                 >>  868 EXTENDED_ARG             1
-                     870 FOR_ITER               503 (to 1878)
-                     872 STORE_FAST              18 (epoch)
-         
-         137         874 BUILD_LIST               0
-                     876 STORE_FAST              19 (train_losses)
-         
-         138         878 LOAD_FAST               10 (decipher)
-                     880 LOAD_METHOD             28 (train)
-                     902 PRECALL                  0
-                     906 CALL                     0
-                     916 POP_TOP
-         
-         139         918 LOAD_FAST               18 (epoch)
-                     920 LOAD_CONST              14 (0)
-                     922 COMPARE_OP               4 (>)
-                     928 POP_JUMP_FORWARD_IF_FALSE    74 (to 1078)
-         
-         143         930 LOAD_FAST               10 (decipher)
-                     932 LOAD_METHOD             29 (modules)
-                     954 PRECALL                  0
-                     958 CALL                     0
-                     968 GET_ITER
-                 >>  970 FOR_ITER                53 (to 1078)
-                     972 STORE_FAST              20 (module)
-         
-         144         974 LOAD_GLOBAL             61 (NULL + isinstance)
-                     986 LOAD_FAST               20 (module)
-                     988 LOAD_GLOBAL             62 (torch)
-                    1000 LOAD_ATTR               32 (nn)
-                    1010 LOAD_ATTR               33 (BatchNorm1d)
-                    1020 PRECALL                  2
-                    1024 CALL                     2
-                    1034 POP_JUMP_FORWARD_IF_FALSE    20 (to 1076)
-         
-         145        1036 LOAD_FAST               20 (module)
-                    1038 LOAD_METHOD             34 (eval)
-                    1060 PRECALL                  0
-                    1064 CALL                     0
-                    1074 POP_TOP
-                 >> 1076 JUMP_BACKWARD           54 (to 970)
-         
-         147     >> 1078 LOAD_FAST                8 (dataloader_train)
-                    1080 GET_ITER
-                 >> 1082 FOR_ITER                33 (to 1150)
-                    1084 STORE_FAST              21 (xc)
-         
-         148        1086 PUSH_NULL
-                    1088 LOAD_FAST               13 (svi)
-                    1090 LOAD_ATTR               35 (step)
-                    1100 LOAD_FAST               21 (xc)
-                    1102 CALL_FUNCTION_EX         0
-                    1104 STORE_FAST              22 (loss)
-         
-         149        1106 LOAD_FAST               19 (train_losses)
-                    1108 LOAD_METHOD             36 (append)
-                    1130 LOAD_FAST               22 (loss)
-                    1132 PRECALL                  1
-                    1136 CALL                     1
-                    1146 POP_TOP
-                    1148 JUMP_BACKWARD           34 (to 1082)
-         
-         151     >> 1150 LOAD_GLOBAL             75 (NULL + np)
-                    1162 LOAD_ATTR               38 (sum)
-                    1172 LOAD_FAST               19 (train_losses)
-                    1174 PRECALL                  1
-                    1178 CALL                     1
-                    1188 LOAD_GLOBAL             79 (NULL + len)
-                    1200 LOAD_FAST                8 (dataloader_train)
-                    1202 LOAD_ATTR               40 (dataset)
-                    1212 PRECALL                  1
-                    1216 CALL                     1
-                    1226 BINARY_OP               11 (/)
-                    1230 STORE_FAST              23 (train_elbo)
-         
-         152        1232 LOAD_FAST               10 (decipher)
-                    1234 LOAD_METHOD             34 (eval)
-                    1256 PRECALL                  0
-                    1260 CALL                     0
-                    1270 POP_TOP
-         
-         153        1272 LOAD_GLOBAL             83 (NULL + predictive_log_likelihood)
-                    1284 LOAD_FAST               10 (decipher)
-                    1286 LOAD_FAST                9 (dataloader_val)
-                    1288 PRECALL                  2
-                    1292 CALL                     2
-                    1302 UNARY_NEGATIVE
-                    1304 STORE_FAST              24 (val_nll)
-         
-         154        1306 LOAD_FAST               15 (val_losses)
-                    1308 LOAD_METHOD             36 (append)
-                    1330 LOAD_FAST               24 (val_nll)
-                    1332 PRECALL                  1
-                    1336 CALL                     1
-                    1346 POP_TOP
-         
-         155        1348 LOAD_FAST               17 (pbar)
-                    1350 LOAD_METHOD             42 (set_description)
-         
-         156        1372 LOAD_CONST              15 ('Epoch ')
-                    1374 LOAD_FAST               18 (epoch)
-                    1376 FORMAT_VALUE             0
-                    1378 LOAD_CONST              16 (' | train elbo: ')
-                    1380 LOAD_FAST               23 (train_elbo)
-                    1382 LOAD_CONST              17 ('.2f')
-                    1384 FORMAT_VALUE             4 (with format)
-                    1386 LOAD_CONST              18 (' | val ll: ')
-                    1388 LOAD_FAST               24 (val_nll)
-                    1390 LOAD_CONST              17 ('.2f')
-                    1392 FORMAT_VALUE             4 (with format)
-                    1394 BUILD_STRING             6
-         
-         155        1396 PRECALL                  1
-                    1400 CALL                     1
-                    1410 POP_TOP
-         
-         158        1412 PUSH_NULL
-                    1414 LOAD_FAST               16 (early_stopping)
-                    1416 LOAD_FAST               24 (val_nll)
-                    1418 PRECALL                  1
-                    1422 CALL                     1
-                    1432 POP_JUMP_FORWARD_IF_FALSE    17 (to 1468)
-         
-         159        1434 LOAD_GLOBAL             87 (NULL + print)
-                    1446 LOAD_CONST              19 ('Early stopping.')
-                    1448 PRECALL                  1
-                    1452 CALL                     1
-                    1462 POP_TOP
-         
-         160        1464 POP_TOP
-                    1466 JUMP_FORWARD           205 (to 1878)
-         
-         162     >> 1468 LOAD_FAST                2 (plot_every_k_epochs)
-                    1470 LOAD_CONST              14 (0)
-                    1472 COMPARE_OP               4 (>)
-                    1478 POP_JUMP_FORWARD_IF_FALSE   197 (to 1874)
-                    1480 LOAD_FAST               18 (epoch)
-                    1482 LOAD_FAST                2 (plot_every_k_epochs)
-                    1484 BINARY_OP                6 (%)
-                    1488 LOAD_CONST              14 (0)
-                    1490 COMPARE_OP               2 (==)
-                    1496 POP_JUMP_FORWARD_IF_FALSE   188 (to 1874)
-         
-         163        1498 LOAD_GLOBAL             89 (NULL + _decipher_to_adata)
-                    1510 LOAD_FAST               10 (decipher)
-                    1512 LOAD_FAST                0 (adata)
-                    1514 PRECALL                  2
-                    1518 CALL                     2
-                    1528 POP_TOP
-         
-         164        1530 LOAD_GLOBAL             91 (NULL + plot_decipher_v)
-                    1542 LOAD_FAST                0 (adata)
-                    1544 BUILD_TUPLE              1
-                    1546 LOAD_CONST              20 ('basis')
-                    1548 LOAD_CONST              21 ('decipher_v')
-                    1550 BUILD_MAP                1
-                    1552 LOAD_FAST                3 (plot_kwargs)
-                    1554 DICT_MERGE               1
-                    1556 CALL_FUNCTION_EX         1
-                    1558 POP_TOP
-         
-         165        1560 LOAD_FAST               14 (gif_maker)
-                    1562 LOAD_METHOD             46 (add_image)
-                    1584 LOAD_GLOBAL             95 (NULL + plt)
-                    1596 LOAD_ATTR               48 (gcf)
-                    1606 PRECALL                  0
-                    1610 CALL                     0
-                    1620 PRECALL                  1
-                    1624 CALL                     1
-                    1634 POP_TOP
-         
-         166        1636 LOAD_GLOBAL              1 (NULL + is_notebook)
-                    1648 PRECALL                  0
-                    1652 CALL                     0
-                    1662 POP_JUMP_FORWARD_IF_FALSE    67 (to 1798)
-         
-         167        1664 LOAD_CONST              14 (0)
-                    1666 LOAD_CONST              22 (('display',))
-                    1668 IMPORT_NAME             49 (IPython.core)
-                    1670 IMPORT_FROM             50 (display)
-                    1672 STORE_FAST              25 (display)
-                    1674 POP_TOP
-         
-         169        1676 LOAD_FAST               25 (display)
-                    1678 LOAD_METHOD             51 (clear_output)
-                    1700 LOAD_CONST              23 (True)
-                    1702 KW_NAMES                24
-                    1704 PRECALL                  1
-                    1708 CALL                     1
-                    1718 POP_TOP
-         
-         170        1720 LOAD_FAST               25 (display)
-                    1722 LOAD_METHOD             50 (display)
-                    1744 LOAD_GLOBAL             95 (NULL + plt)
-                    1756 LOAD_ATTR               48 (gcf)
-                    1766 PRECALL                  0
-                    1770 CALL                     0
-                    1780 PRECALL                  1
-                    1784 CALL                     1
-                    1794 POP_TOP
-                    1796 JUMP_FORWARD            19 (to 1836)
-         
-         172     >> 1798 LOAD_GLOBAL             95 (NULL + plt)
-                    1810 LOAD_ATTR               52 (show)
-                    1820 PRECALL                  0
-                    1824 CALL                     0
-                    1834 POP_TOP
-         
-         173     >> 1836 LOAD_GLOBAL             95 (NULL + plt)
-                    1848 LOAD_ATTR               53 (close)
-                    1858 PRECALL                  0
-                    1862 CALL                     0
-                    1872 POP_TOP
-                 >> 1874 EXTENDED_ARG             1
-                    1876 JUMP_BACKWARD          505 (to 868)
-         
-         175     >> 1878 LOAD_GLOBAL              1 (NULL + is_notebook)
-                    1890 PRECALL                  0
-                    1894 CALL                     0
-                    1904 POP_JUMP_FORWARD_IF_FALSE    46 (to 1998)
-         
-         176        1906 LOAD_CONST              14 (0)
-                    1908 LOAD_CONST              22 (('display',))
-                    1910 IMPORT_NAME             49 (IPython.core)
-                    1912 IMPORT_FROM             50 (display)
-                    1914 STORE_FAST              25 (display)
-                    1916 POP_TOP
-         
-         178        1918 LOAD_FAST               25 (display)
-                    1920 LOAD_METHOD             51 (clear_output)
-                    1942 PRECALL                  0
-                    1946 CALL                     0
-                    1956 POP_TOP
-         
-         179        1958 LOAD_FAST               17 (pbar)
-                    1960 LOAD_METHOD             50 (display)
-                    1982 PRECALL                  0
-                    1986 CALL                     0
-                    1996 POP_TOP
-         
-         181     >> 1998 LOAD_GLOBAL             89 (NULL + _decipher_to_adata)
-                    2010 LOAD_FAST               10 (decipher)
-                    2012 LOAD_FAST                0 (adata)
-                    2014 PRECALL                  2
-                    2018 CALL                     2
-                    2028 POP_TOP
-         
-         182        2030 LOAD_GLOBAL            109 (NULL + decipher_save_model)
-                    2042 LOAD_FAST                0 (adata)
-                    2044 LOAD_FAST               10 (decipher)
-                    2046 PRECALL                  2
-                    2050 CALL                     2
-                    2060 POP_TOP
-         
-         184        2062 LOAD_FAST                0 (adata)
-                    2064 LOAD_ATTR               55 (uns)
-                    2074 LOAD_CONST              25 ('decipher')
-                    2076 BINARY_SUBSCR
-                    2086 LOAD_CONST              26 ('run_id')
-                    2088 BINARY_SUBSCR
-                    2098 STORE_FAST              26 (model_run_id)
-         
-         185        2100 LOAD_GLOBAL            112 (DECIPHER_GLOBALS)
-                    2112 LOAD_CONST              27 ('save_folder')
-                    2114 BINARY_SUBSCR
-                    2124 STORE_FAST              27 (save_folder)
-         
-         186        2126 LOAD_GLOBAL            114 (os)
-                    2138 LOAD_ATTR               58 (path)
-                    2148 LOAD_METHOD             59 (join)
-                    2170 LOAD_FAST               27 (save_folder)
-                    2172 LOAD_FAST               26 (model_run_id)
-                    2174 LOAD_CONST              28 ('decipher_training.gif')
-                    2176 PRECALL                  3
-                    2180 CALL                     3
-                    2190 STORE_FAST              28 (full_path)
-         
-         187        2192 LOAD_FAST               14 (gif_maker)
-                    2194 LOAD_METHOD             60 (save_gif)
-                    2216 LOAD_FAST               28 (full_path)
-                    2218 PRECALL                  1
-                    2222 CALL                     1
-                    2232 POP_TOP
-         
-         189        2234 LOAD_GLOBAL              1 (NULL + is_notebook)
-                    2246 PRECALL                  0
-                    2250 CALL                     0
-                    2260 POP_JUMP_FORWARD_IF_FALSE    15 (to 2292)
-         
-         190        2262 LOAD_GLOBAL            123 (NULL + load_and_show_gif)
-                    2274 LOAD_FAST               28 (full_path)
-                    2276 PRECALL                  1
-                    2280 CALL                     1
-                    2290 POP_TOP
-         
-         192     >> 2292 LOAD_GLOBAL             91 (NULL + plot_decipher_v)
-                    2304 LOAD_FAST                0 (adata)
-                    2306 BUILD_TUPLE              1
-                    2308 LOAD_CONST              20 ('basis')
-                    2310 LOAD_CONST              21 ('decipher_v')
-                    2312 BUILD_MAP                1
-                    2314 LOAD_FAST                3 (plot_kwargs)
-                    2316 DICT_MERGE               1
-                    2318 CALL_FUNCTION_EX         1
-                    2320 POP_TOP
-         
-         194        2322 LOAD_FAST               10 (decipher)
-                    2324 LOAD_FAST               15 (val_losses)
-                    2326 BUILD_TUPLE              2
-                    2328 RETURN_VALUE
+                     362 LOAD_CONST               7 (None)
+                     364 BUILD_SLICE              2
+                     366 BUILD_TUPLE              2
+                     368 BINARY_SUBSCR
+                     378 STORE_FAST               8 (adata_val)
+         
+         122         380 LOAD_FAST                3 (plot_kwargs)
+                     382 POP_JUMP_FORWARD_IF_NOT_NONE    14 (to 412)
+         
+         123         384 LOAD_GLOBAL             23 (NULL + dict)
+                     396 PRECALL                  0
+                     400 CALL                     0
+                     410 STORE_FAST               3 (plot_kwargs)
+         
+         125     >>  412 LOAD_FAST                1 (decipher_config)
+                     414 LOAD_METHOD             12 (initialize_from_adata)
+                     436 LOAD_FAST                7 (adata_train)
+                     438 PRECALL                  1
+                     442 CALL                     1
+                     452 POP_TOP
+         
+         127         454 LOAD_GLOBAL             27 (NULL + make_data_loader_from_adata)
+         
+         128         466 LOAD_FAST                7 (adata_train)
+                     468 LOAD_FAST                1 (decipher_config)
+                     470 LOAD_ATTR               14 (batch_size)
+                     480 LOAD_CONST               8 (True)
+         
+         127         482 KW_NAMES                 9
+                     484 PRECALL                  3
+                     488 CALL                     3
+                     498 STORE_FAST               9 (dataloader_train)
+         
+         130         500 LOAD_GLOBAL             27 (NULL + make_data_loader_from_adata)
+                     512 LOAD_FAST                8 (adata_val)
+                     514 LOAD_FAST                1 (decipher_config)
+                     516 LOAD_ATTR               14 (batch_size)
+                     526 PRECALL                  2
+                     530 CALL                     2
+                     540 STORE_FAST              10 (dataloader_val)
+         
+         132         542 LOAD_GLOBAL             31 (NULL + Decipher)
+         
+         133         554 LOAD_FAST                1 (decipher_config)
+         
+         132         556 KW_NAMES                10
+                     558 PRECALL                  1
+                     562 CALL                     1
+                     572 STORE_FAST              11 (decipher)
+         
+         135         574 LOAD_FAST               11 (decipher)
+                     576 LOAD_METHOD             16 (to)
+                     598 LOAD_DEREF               4 (device)
+                     600 PRECALL                  1
+                     604 CALL                     1
+                     614 POP_TOP
+         
+         137         616 LOAD_GLOBAL              6 (pyro)
+                     628 LOAD_ATTR               17 (optim)
+                     638 LOAD_METHOD             18 (ClippedAdam)
+         
+         139         660 LOAD_FAST                1 (decipher_config)
+                     662 LOAD_ATTR               19 (learning_rate)
+         
+         140         672 LOAD_CONST              11 (0.0001)
+         
+         138         674 LOAD_CONST              12 (('lr', 'weight_decay'))
+                     676 BUILD_CONST_KEY_MAP      2
+         
+         137         678 PRECALL                  1
+                     682 CALL                     1
+                     692 STORE_FAST              12 (optimizer)
+         
+         143         694 LOAD_GLOBAL             41 (NULL + Trace_ELBO)
+                     706 PRECALL                  0
+                     710 CALL                     0
+                     720 STORE_FAST              13 (elbo)
+         
+         144         722 LOAD_GLOBAL             43 (NULL + SVI)
+                     734 LOAD_FAST               11 (decipher)
+                     736 LOAD_ATTR               22 (model)
+                     746 LOAD_FAST               11 (decipher)
+                     748 LOAD_ATTR               23 (guide)
+                     758 LOAD_FAST               12 (optimizer)
+                     760 LOAD_FAST               13 (elbo)
+                     762 PRECALL                  4
+                     766 CALL                     4
+                     776 STORE_FAST              14 (svi)
+         
+         145         778 LOAD_GLOBAL             49 (NULL + GIFMaker)
+                     790 LOAD_CONST              13 (120)
+                     792 KW_NAMES                14
+                     794 PRECALL                  1
+                     798 CALL                     1
+                     808 STORE_FAST              15 (gif_maker)
+         
+         148         810 BUILD_LIST               0
+                     812 STORE_FAST              16 (val_losses)
+         
+         150         814 LOAD_FAST                1 (decipher_config)
+                     816 LOAD_ATTR               25 (early_stopping_patience)
+                     826 POP_JUMP_FORWARD_IF_NONE    33 (to 894)
+         
+         151         828 LOAD_FAST                1 (decipher_config)
+                     830 LOAD_ATTR               25 (early_stopping_patience)
+                     840 LOAD_CONST              15 (0)
+                     842 COMPARE_OP               4 (>)
+                     848 POP_JUMP_FORWARD_IF_FALSE    22 (to 894)
+         
+         153         850 LOAD_GLOBAL             53 (NULL + EarlyStopping)
+                     862 LOAD_FAST                1 (decipher_config)
+                     864 LOAD_ATTR               25 (early_stopping_patience)
+                     874 KW_NAMES                16
+                     876 PRECALL                  1
+                     880 CALL                     1
+                     890 STORE_FAST              17 (early_stopping)
+                     892 JUMP_FORWARD            29 (to 952)
+         
+         155     >>  894 LOAD_GLOBAL             53 (NULL + EarlyStopping)
+                     906 LOAD_GLOBAL             55 (NULL + int)
+                     918 LOAD_CONST              17 (1e+30)
+                     920 PRECALL                  1
+                     924 CALL                     1
+                     934 KW_NAMES                16
+                     936 PRECALL                  1
+                     940 CALL                     1
+                     950 STORE_FAST              17 (early_stopping)
+         
+         157     >>  952 LOAD_GLOBAL             57 (NULL + tqdm)
+                     964 LOAD_GLOBAL             59 (NULL + range)
+                     976 LOAD_FAST                1 (decipher_config)
+                     978 LOAD_ATTR               30 (n_epochs)
+                     988 PRECALL                  1
+                     992 CALL                     1
+                    1002 PRECALL                  1
+                    1006 CALL                     1
+                    1016 STORE_FAST              18 (pbar)
+         
+         158        1018 LOAD_CONST               7 (None)
+                    1020 STORE_FAST              19 (last_train_elbo)
+         
+         159        1022 LOAD_CONST               7 (None)
+                    1024 STORE_FAST              20 (val_nll)
+         
+         160        1026 LOAD_FAST               18 (pbar)
+                    1028 GET_ITER
+                 >> 1030 EXTENDED_ARG             2
+                    1032 FOR_ITER               659 (to 2352)
+                    1034 STORE_FAST              21 (epoch)
+         
+         161        1036 BUILD_LIST               0
+                    1038 STORE_FAST              22 (train_losses)
+         
+         162        1040 LOAD_FAST               11 (decipher)
+                    1042 LOAD_METHOD             31 (train)
+                    1064 PRECALL                  0
+                    1068 CALL                     0
+                    1078 POP_TOP
+         
+         163        1080 LOAD_FAST               21 (epoch)
+                    1082 LOAD_CONST              15 (0)
+                    1084 COMPARE_OP               4 (>)
+                    1090 POP_JUMP_FORWARD_IF_FALSE    74 (to 1240)
+         
+         167        1092 LOAD_FAST               11 (decipher)
+                    1094 LOAD_METHOD             32 (modules)
+                    1116 PRECALL                  0
+                    1120 CALL                     0
+                    1130 GET_ITER
+                 >> 1132 FOR_ITER                53 (to 1240)
+                    1134 STORE_FAST              23 (module)
+         
+         168        1136 LOAD_GLOBAL             67 (NULL + isinstance)
+                    1148 LOAD_FAST               23 (module)
+                    1150 LOAD_GLOBAL             68 (torch)
+                    1162 LOAD_ATTR               35 (nn)
+                    1172 LOAD_ATTR               36 (BatchNorm1d)
+                    1182 PRECALL                  2
+                    1186 CALL                     2
+                    1196 POP_JUMP_FORWARD_IF_FALSE    20 (to 1238)
+         
+         169        1198 LOAD_FAST               23 (module)
+                    1200 LOAD_METHOD             37 (eval)
+                    1222 PRECALL                  0
+                    1226 CALL                     0
+                    1236 POP_TOP
+                 >> 1238 JUMP_BACKWARD           54 (to 1132)
+         
+         171     >> 1240 LOAD_GLOBAL             77 (NULL + len)
+                    1252 LOAD_FAST                9 (dataloader_train)
+                    1254 PRECALL                  1
+                    1258 CALL                     1
+                    1268 STORE_FAST              24 (n_batches)
+         
+         172        1270 LOAD_CONST              15 (0)
+                    1272 STORE_FAST              25 (train_elbo)
+         
+         173        1274 LOAD_CONST              15 (0)
+                    1276 STORE_FAST              26 (train_elbo_n_obs)
+         
+         174        1278 LOAD_FAST                9 (dataloader_train)
+                    1280 GET_ITER
+                 >> 1282 FOR_ITER               181 (to 1646)
+                    1284 STORE_FAST              27 (xc)
+         
+         175        1286 NOP
+         
+         176        1288 LOAD_CLOSURE             4 (device)
+                    1290 BUILD_TUPLE              1
+                    1292 LOAD_CONST              18 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 176>)
+                    1294 MAKE_FUNCTION            8 (closure)
+                    1296 LOAD_FAST               27 (xc)
+                    1298 GET_ITER
+                    1300 PRECALL                  0
+                    1304 CALL                     0
+                    1314 STORE_FAST              27 (xc)
+         
+         177        1316 PUSH_NULL
+                    1318 LOAD_FAST               14 (svi)
+                    1320 LOAD_ATTR               39 (step)
+                    1330 LOAD_FAST               27 (xc)
+                    1332 CALL_FUNCTION_EX         0
+                    1334 STORE_FAST              28 (loss)
+                    1336 JUMP_FORWARD            47 (to 1432)
+                 >> 1338 PUSH_EXC_INFO
+         
+         178        1340 LOAD_GLOBAL             80 (Exception)
+                    1352 CHECK_EXC_MATCH
+                    1354 POP_JUMP_FORWARD_IF_FALSE    34 (to 1424)
+                    1356 STORE_FAST              29 (e)
+         
+         179        1358 LOAD_GLOBAL             83 (NULL + print)
+                    1370 LOAD_CONST              19 ('ERROR')
+                    1372 LOAD_FAST               29 (e)
+                    1374 PRECALL                  2
+                    1378 CALL                     2
+                    1388 POP_TOP
+         
+         180        1390 LOAD_FAST               11 (decipher)
+                    1392 LOAD_FAST               16 (val_losses)
+                    1394 BUILD_TUPLE              2
+                    1396 SWAP                     2
+                    1398 POP_EXCEPT
+                    1400 LOAD_CONST               7 (None)
+                    1402 STORE_FAST              29 (e)
+                    1404 DELETE_FAST             29 (e)
+                    1406 SWAP                     2
+                    1408 POP_TOP
+                    1410 SWAP                     2
+                    1412 POP_TOP
+                    1414 RETURN_VALUE
+                 >> 1416 LOAD_CONST               7 (None)
+                    1418 STORE_FAST              29 (e)
+                    1420 DELETE_FAST             29 (e)
+                    1422 RERAISE                  1
+         
+         178     >> 1424 RERAISE                  0
+                 >> 1426 COPY                     3
+                    1428 POP_EXCEPT
+                    1430 RERAISE                  1
+         
+         181     >> 1432 LOAD_FAST               22 (train_losses)
+                    1434 LOAD_METHOD             42 (append)
+                    1456 LOAD_FAST               28 (loss)
+                    1458 PRECALL                  1
+                    1462 CALL                     1
+                    1472 POP_TOP
+         
+         182        1474 LOAD_FAST               25 (train_elbo)
+                    1476 LOAD_FAST               28 (loss)
+                    1478 BINARY_OP               13 (+=)
+                    1482 STORE_FAST              25 (train_elbo)
+         
+         183        1484 LOAD_FAST               26 (train_elbo_n_obs)
+                    1486 LOAD_FAST               27 (xc)
+                    1488 LOAD_CONST              15 (0)
+                    1490 BINARY_SUBSCR
+                    1500 LOAD_ATTR               43 (shape)
+                    1510 LOAD_CONST              15 (0)
+                    1512 BINARY_SUBSCR
+                    1522 BINARY_OP               13 (+=)
+                    1526 STORE_FAST              26 (train_elbo_n_obs)
+         
+         184        1528 LOAD_FAST               18 (pbar)
+                    1530 LOAD_METHOD             44 (set_description)
+         
+         185        1552 LOAD_CONST              20 ('Epoch ')
+                    1554 LOAD_FAST               21 (epoch)
+                    1556 FORMAT_VALUE             0
+                    1558 LOAD_CONST              21 (' (batch ')
+                    1560 LOAD_GLOBAL             77 (NULL + len)
+                    1572 LOAD_FAST               22 (train_losses)
+                    1574 PRECALL                  1
+                    1578 CALL                     1
+                    1588 FORMAT_VALUE             0
+                    1590 LOAD_CONST              22 ('/')
+                    1592 LOAD_FAST               24 (n_batches)
+                    1594 FORMAT_VALUE             0
+                    1596 LOAD_CONST              23 (') | | train elbo: ')
+         
+         186        1598 LOAD_FAST               25 (train_elbo)
+                    1600 LOAD_FAST               26 (train_elbo_n_obs)
+                    1602 BINARY_OP               11 (/)
+                    1606 LOAD_CONST              24 ('.2f')
+         
+         185        1608 FORMAT_VALUE             4 (with format)
+                    1610 LOAD_CONST              25 (' (last epoch: ')
+         
+         186        1612 LOAD_FAST               19 (last_train_elbo)
+                    1614 LOAD_CONST              24 ('.2f')
+         
+         185        1616 FORMAT_VALUE             4 (with format)
+                    1618 LOAD_CONST              26 (') | val ll: ')
+         
+         187        1620 LOAD_FAST               20 (val_nll)
+                    1622 LOAD_CONST              24 ('.2f')
+         
+         185        1624 FORMAT_VALUE             4 (with format)
+                    1626 BUILD_STRING            12
+         
+         184        1628 PRECALL                  1
+                    1632 CALL                     1
+                    1642 POP_TOP
+                    1644 JUMP_BACKWARD          182 (to 1282)
+         
+         190     >> 1646 LOAD_FAST               11 (decipher)
+                    1648 LOAD_METHOD             37 (eval)
+                    1670 PRECALL                  0
+                    1674 CALL                     0
+                    1684 POP_TOP
+         
+         191        1686 LOAD_GLOBAL             91 (NULL + predictive_log_likelihood)
+                    1698 LOAD_FAST               11 (decipher)
+                    1700 LOAD_FAST               10 (dataloader_val)
+                    1702 PRECALL                  2
+                    1706 CALL                     2
+                    1716 UNARY_NEGATIVE
+                    1718 LOAD_FAST                8 (adata_val)
+                    1720 LOAD_ATTR               43 (shape)
+                    1730 LOAD_CONST              15 (0)
+                    1732 BINARY_SUBSCR
+                    1742 BINARY_OP               11 (/)
+                    1746 STORE_FAST              20 (val_nll)
+         
+         192        1748 LOAD_FAST               16 (val_losses)
+                    1750 LOAD_METHOD             42 (append)
+                    1772 LOAD_FAST               20 (val_nll)
+                    1774 PRECALL                  1
+                    1778 CALL                     1
+                    1788 POP_TOP
+         
+         193        1790 LOAD_FAST               18 (pbar)
+                    1792 LOAD_METHOD             44 (set_description)
+         
+         194        1814 LOAD_CONST              20 ('Epoch ')
+                    1816 LOAD_FAST               21 (epoch)
+                    1818 FORMAT_VALUE             0
+                    1820 LOAD_CONST              21 (' (batch ')
+                    1822 LOAD_GLOBAL             77 (NULL + len)
+                    1834 LOAD_FAST               22 (train_losses)
+                    1836 PRECALL                  1
+                    1840 CALL                     1
+                    1850 FORMAT_VALUE             0
+                    1852 LOAD_CONST              22 ('/')
+                    1854 LOAD_FAST               24 (n_batches)
+                    1856 FORMAT_VALUE             0
+                    1858 LOAD_CONST              23 (') | | train elbo: ')
+         
+         195        1860 LOAD_FAST               25 (train_elbo)
+                    1862 LOAD_FAST               26 (train_elbo_n_obs)
+                    1864 BINARY_OP               11 (/)
+                    1868 LOAD_CONST              24 ('.2f')
+         
+         194        1870 FORMAT_VALUE             4 (with format)
+                    1872 LOAD_CONST              25 (' (last epoch: ')
+         
+         195        1874 LOAD_FAST               19 (last_train_elbo)
+                    1876 LOAD_CONST              24 ('.2f')
+         
+         194        1878 FORMAT_VALUE             4 (with format)
+                    1880 LOAD_CONST              26 (') | val ll: ')
+         
+         196        1882 LOAD_FAST               20 (val_nll)
+                    1884 LOAD_CONST              24 ('.2f')
+         
+         194        1886 FORMAT_VALUE             4 (with format)
+                    1888 BUILD_STRING            12
+         
+         193        1890 PRECALL                  1
+                    1894 CALL                     1
+                    1904 POP_TOP
+         
+         198        1906 LOAD_FAST               25 (train_elbo)
+                    1908 LOAD_FAST               26 (train_elbo_n_obs)
+                    1910 BINARY_OP               11 (/)
+                    1914 STORE_FAST              19 (last_train_elbo)
+         
+         199        1916 PUSH_NULL
+                    1918 LOAD_FAST               17 (early_stopping)
+                    1920 LOAD_FAST               20 (val_nll)
+                    1922 PRECALL                  1
+                    1926 CALL                     1
+                    1936 POP_JUMP_FORWARD_IF_FALSE     2 (to 1942)
+         
+         200        1938 POP_TOP
+                    1940 JUMP_FORWARD           205 (to 2352)
+         
+         202     >> 1942 LOAD_FAST                2 (plot_every_k_epochs)
+                    1944 LOAD_CONST              15 (0)
+                    1946 COMPARE_OP               4 (>)
+                    1952 POP_JUMP_FORWARD_IF_FALSE   197 (to 2348)
+                    1954 LOAD_FAST               21 (epoch)
+                    1956 LOAD_FAST                2 (plot_every_k_epochs)
+                    1958 BINARY_OP                6 (%)
+                    1962 LOAD_CONST              15 (0)
+                    1964 COMPARE_OP               2 (==)
+                    1970 POP_JUMP_FORWARD_IF_FALSE   188 (to 2348)
+         
+         203        1972 LOAD_GLOBAL             93 (NULL + _decipher_to_adata)
+                    1984 LOAD_FAST               11 (decipher)
+                    1986 LOAD_FAST                0 (adata)
+                    1988 PRECALL                  2
+                    1992 CALL                     2
+                    2002 POP_TOP
+         
+         204        2004 LOAD_GLOBAL             95 (NULL + plot_decipher_v)
+                    2016 LOAD_FAST                0 (adata)
+                    2018 BUILD_TUPLE              1
+                    2020 LOAD_CONST              27 ('basis')
+                    2022 LOAD_CONST              28 ('decipher_v')
+                    2024 BUILD_MAP                1
+                    2026 LOAD_FAST                3 (plot_kwargs)
+                    2028 DICT_MERGE               1
+                    2030 CALL_FUNCTION_EX         1
+                    2032 POP_TOP
+         
+         205        2034 LOAD_FAST               15 (gif_maker)
+                    2036 LOAD_METHOD             48 (add_image)
+                    2058 LOAD_GLOBAL             99 (NULL + plt)
+                    2070 LOAD_ATTR               50 (gcf)
+                    2080 PRECALL                  0
+                    2084 CALL                     0
+                    2094 PRECALL                  1
+                    2098 CALL                     1
+                    2108 POP_TOP
+         
+         206        2110 LOAD_GLOBAL              1 (NULL + is_notebook)
+                    2122 PRECALL                  0
+                    2126 CALL                     0
+                    2136 POP_JUMP_FORWARD_IF_FALSE    67 (to 2272)
+         
+         207        2138 LOAD_CONST              15 (0)
+                    2140 LOAD_CONST              29 (('display',))
+                    2142 IMPORT_NAME             51 (IPython.core)
+                    2144 IMPORT_FROM             52 (display)
+                    2146 STORE_FAST              30 (display)
+                    2148 POP_TOP
+         
+         209        2150 LOAD_FAST               30 (display)
+                    2152 LOAD_METHOD             53 (clear_output)
+                    2174 LOAD_CONST               8 (True)
+                    2176 KW_NAMES                30
+                    2178 PRECALL                  1
+                    2182 CALL                     1
+                    2192 POP_TOP
+         
+         210        2194 LOAD_FAST               30 (display)
+                    2196 LOAD_METHOD             52 (display)
+                    2218 LOAD_GLOBAL             99 (NULL + plt)
+                    2230 LOAD_ATTR               50 (gcf)
+                    2240 PRECALL                  0
+                    2244 CALL                     0
+                    2254 PRECALL                  1
+                    2258 CALL                     1
+                    2268 POP_TOP
+                    2270 JUMP_FORWARD            19 (to 2310)
+         
+         212     >> 2272 LOAD_GLOBAL             99 (NULL + plt)
+                    2284 LOAD_ATTR               54 (show)
+                    2294 PRECALL                  0
+                    2298 CALL                     0
+                    2308 POP_TOP
+         
+         213     >> 2310 LOAD_GLOBAL             99 (NULL + plt)
+                    2322 LOAD_ATTR               55 (close)
+                    2332 PRECALL                  0
+                    2336 CALL                     0
+                    2346 POP_TOP
+                 >> 2348 EXTENDED_ARG             2
+                    2350 JUMP_BACKWARD          661 (to 1030)
+         
+         215     >> 2352 LOAD_GLOBAL              1 (NULL + is_notebook)
+                    2364 PRECALL                  0
+                    2368 CALL                     0
+                    2378 POP_JUMP_FORWARD_IF_FALSE    46 (to 2472)
+         
+         216        2380 LOAD_CONST              15 (0)
+                    2382 LOAD_CONST              29 (('display',))
+                    2384 IMPORT_NAME             51 (IPython.core)
+                    2386 IMPORT_FROM             52 (display)
+                    2388 STORE_FAST              30 (display)
+                    2390 POP_TOP
+         
+         218        2392 LOAD_FAST               30 (display)
+                    2394 LOAD_METHOD             53 (clear_output)
+                    2416 PRECALL                  0
+                    2420 CALL                     0
+                    2430 POP_TOP
+         
+         219        2432 LOAD_FAST               18 (pbar)
+                    2434 LOAD_METHOD             52 (display)
+                    2456 PRECALL                  0
+                    2460 CALL                     0
+                    2470 POP_TOP
+         
+         221     >> 2472 LOAD_FAST               17 (early_stopping)
+                    2474 LOAD_METHOD             56 (has_stopped)
+                    2496 PRECALL                  0
+                    2500 CALL                     0
+                    2510 POP_JUMP_FORWARD_IF_FALSE    26 (to 2564)
+         
+         222        2512 LOAD_GLOBAL              2 (logger)
+                    2524 LOAD_METHOD              2 (info)
+                    2546 LOAD_CONST              31 ('Early stopping has been triggered.')
+                    2548 PRECALL                  1
+                    2552 CALL                     1
+                    2562 POP_TOP
+         
+         223     >> 2564 LOAD_GLOBAL             93 (NULL + _decipher_to_adata)
+                    2576 LOAD_FAST               11 (decipher)
+                    2578 LOAD_FAST                0 (adata)
+                    2580 PRECALL                  2
+                    2584 CALL                     2
+                    2594 POP_TOP
+         
+         224        2596 LOAD_GLOBAL            115 (NULL + decipher_save_model)
+                    2608 LOAD_FAST                0 (adata)
+                    2610 LOAD_FAST               11 (decipher)
+                    2612 PRECALL                  2
+                    2616 CALL                     2
+                    2626 POP_TOP
+         
+         226        2628 LOAD_FAST                0 (adata)
+                    2630 LOAD_ATTR               58 (uns)
+                    2640 LOAD_CONST              32 ('decipher')
+                    2642 BINARY_SUBSCR
+                    2652 LOAD_CONST              33 ('run_id')
+                    2654 BINARY_SUBSCR
+                    2664 STORE_FAST              31 (model_run_id)
+         
+         227        2666 LOAD_GLOBAL            118 (DECIPHER_GLOBALS)
+                    2678 LOAD_CONST              34 ('save_folder')
+                    2680 BINARY_SUBSCR
+                    2690 STORE_FAST              32 (save_folder)
+         
+         228        2692 LOAD_GLOBAL            120 (os)
+                    2704 LOAD_ATTR               61 (path)
+                    2714 LOAD_METHOD             62 (join)
+                    2736 LOAD_FAST               32 (save_folder)
+                    2738 LOAD_GLOBAL            127 (NULL + str)
+                    2750 LOAD_FAST               31 (model_run_id)
+                    2752 PRECALL                  1
+                    2756 CALL                     1
+                    2766 LOAD_CONST              35 ('decipher_training.gif')
+                    2768 PRECALL                  3
+                    2772 CALL                     3
+                    2782 STORE_FAST              33 (full_path)
+         
+         229        2784 LOAD_FAST               15 (gif_maker)
+                    2786 LOAD_ATTR               64 (images)
+                    2796 POP_JUMP_FORWARD_IF_FALSE    50 (to 2898)
+         
+         230        2798 LOAD_FAST               15 (gif_maker)
+                    2800 LOAD_METHOD             65 (save_gif)
+                    2822 LOAD_FAST               33 (full_path)
+                    2824 PRECALL                  1
+                    2828 CALL                     1
+                    2838 POP_TOP
+         
+         231        2840 LOAD_GLOBAL              1 (NULL + is_notebook)
+                    2852 PRECALL                  0
+                    2856 CALL                     0
+                    2866 POP_JUMP_FORWARD_IF_FALSE    15 (to 2898)
+         
+         232        2868 LOAD_GLOBAL            133 (NULL + load_and_show_gif)
+                    2880 LOAD_FAST               33 (full_path)
+                    2882 PRECALL                  1
+                    2886 CALL                     1
+                    2896 POP_TOP
+         
+         234     >> 2898 LOAD_GLOBAL             95 (NULL + plot_decipher_v)
+                    2910 LOAD_FAST                0 (adata)
+                    2912 BUILD_TUPLE              1
+                    2914 LOAD_CONST              27 ('basis')
+                    2916 LOAD_CONST              28 ('decipher_v')
+                    2918 BUILD_MAP                1
+                    2920 LOAD_FAST                3 (plot_kwargs)
+                    2922 DICT_MERGE               1
+                    2924 CALL_FUNCTION_EX         1
+                    2926 POP_TOP
+         
+         236        2928 LOAD_FAST               11 (decipher)
+                    2930 LOAD_FAST               16 (val_losses)
+                    2932 BUILD_TUPLE              2
+                    2934 RETURN_VALUE
+         ExceptionTable:
+           1288 to 1334 -> 1338 [2]
+           1338 to 1356 -> 1426 [3] lasti
+           1358 to 1394 -> 1416 [3] lasti
+           1396 to 1396 -> 1426 [3] lasti
+           1416 to 1424 -> 1426 [3] lasti
          consts
-            "Train a decipher model.\n\n    Parameters\n    ----------\n    adata: sc.AnnData\n        The annotated data matrix.\n    decipher_config: DecipherConfig, optional\n        Configuration for the decipher model.\n    plot_every_k_epochs: int, optional\n        If > 0, plot the decipher space every `plot_every_k_epoch` epochs.\n        Default: -1 (no plots).\n    plot_kwargs: dict, optional\n        Additional keyword arguments to pass to `dc.pl.decipher`.\n\n    Returns\n    -------\n    decipher: Decipher\n        The trained decipher model.\n    val_losses: list of float\n        The validation losses at each epoch.\n    `adata.obs['decipher_split']`: categorical\n        The train/validation split.\n    `adata.obsm['decipher_v']`: ndarray\n        The decipher v space.\n    `adata.obsm['decipher_z']`: ndarray\n        The decipher z space.\n    "
+            'Train a decipher model.\n\n    Parameters\n    ----------\n    adata: sc.AnnData\n        The annotated data matrix.\n    decipher_config: DecipherConfig, optional\n        Configuration for the decipher model.\n    plot_every_k_epochs: int, optional\n        If > 0, plot the decipher space every `plot_every_k_epoch` epochs.\n        Default: -1 (no plots).\n    plot_kwargs: dict, optional\n        Additional keyword arguments to pass to `dc.pl.decipher`.\n    device: str, optional\n        The device to use for training. Default: "cpu".\n\n    Returns\n    -------\n    decipher: Decipher\n        The trained decipher model.\n    val_losses: list of float\n        The validation losses at each epoch.\n    `adata.obs[\'decipher_split\']`: categorical\n        The train/validation split.\n    `adata.obsm[\'decipher_v\']`: ndarray\n        The decipher v space.\n    `adata.obsm[\'decipher_z\']`: ndarray\n        The decipher z space.\n    '
             -1
             5
             'Plotting decipher space every 5 epochs by default. Set `plot_every_k_epoch` to -2 to disable.'
             'decipher_split'
             'train'
             'validation'
             None
+            True
+            ('drop_last',)
             ('config',)
             0.0001
             ('lr', 'weight_decay')
             120
             ('dpi',)
-            ('patience',)
             0
+            ('patience',)
+            1e+30
+            code
+               argcount  : 1
+               nlocals   : 2
+               stacksize : 5
+               flags     : 19
+               code
+                  0x9501970067007c005d177d017c01a00000000000000000000000000000
+                  000000000000008902a6010000ab01000000000000000091028c185300
+                             0 COPY_FREE_VARS           1
+               
+               176           2 RESUME                   0
+                             4 BUILD_LIST               0
+                             6 LOAD_FAST                0 (.0)
+                       >>    8 FOR_ITER                23 (to 56)
+                            10 STORE_FAST               1 (x)
+                            12 LOAD_FAST                1 (x)
+                            14 LOAD_METHOD              0 (to)
+                            36 LOAD_DEREF               2 (device)
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 LIST_APPEND              2
+                            54 JUMP_BACKWARD           24 (to 8)
+                       >>   56 RETURN_VALUE
+               consts
+               names      ('to',)
+               varnames   ('.0', 'x')
+               freevars   ('device',)
+               cellvars   ()
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
+               name       '<listcomp>'
+               firstlineno 176
+               lnotab 0x
+            'ERROR'
             'Epoch '
-            ' | train elbo: '
+            ' (batch '
+            '/'
+            ') | | train elbo: '
             '.2f'
-            ' | val ll: '
-            'Early stopping.'
+            ' (last epoch: '
+            ') | val ll: '
             'basis'
             'decipher_v'
             ('display',)
-            True
             ('wait',)
+            'Early stopping has been triggered.'
             'decipher'
             'run_id'
             'save_folder'
             'decipher_training.gif'
-         names      ('is_notebook', 'logger', 'info', 'pyro', 'clear_param_store', 'util', 'set_rng_seed', 'seed', '_make_train_val_split', 'val_frac', 'obs', 'dict', 'initialize_from_adata', 'make_data_loader_from_adata', 'batch_size', 'Decipher', 'optim', 'ClippedAdam', 'learning_rate', 'Trace_ELBO', 'SVI', 'model', 'guide', 'GIFMaker', 'EarlyStopping', 'tqdm', 'range', 'n_epochs', 'train', 'modules', 'isinstance', 'torch', 'nn', 'BatchNorm1d', 'eval', 'step', 'append', 'np', 'sum', 'len', 'dataset', 'predictive_log_likelihood', 'set_description', 'print', '_decipher_to_adata', 'plot_decipher_v', 'add_image', 'plt', 'gcf', 'IPython.core', 'display', 'clear_output', 'show', 'close', 'decipher_save_model', 'uns', 'DECIPHER_GLOBALS', 'os', 'path', 'join', 'save_gif', 'load_and_show_gif')
-         varnames   ('adata', 'decipher_config', 'plot_every_k_epochs', 'plot_kwargs', 'train_idx', 'val_idx', 'adata_train', 'adata_val', 'dataloader_train', 'dataloader_val', 'decipher', 'optimizer', 'elbo', 'svi', 'gif_maker', 'val_losses', 'early_stopping', 'pbar', 'epoch', 'train_losses', 'module', 'xc', 'loss', 'train_elbo', 'val_nll', 'display', 'model_run_id', 'save_folder', 'full_path')
+         names      ('is_notebook', 'logger', 'info', 'pyro', 'clear_param_store', 'util', 'set_rng_seed', 'seed', '_make_train_val_split', 'val_frac', 'obs', 'dict', 'initialize_from_adata', 'make_data_loader_from_adata', 'batch_size', 'Decipher', 'to', 'optim', 'ClippedAdam', 'learning_rate', 'Trace_ELBO', 'SVI', 'model', 'guide', 'GIFMaker', 'early_stopping_patience', 'EarlyStopping', 'int', 'tqdm', 'range', 'n_epochs', 'train', 'modules', 'isinstance', 'torch', 'nn', 'BatchNorm1d', 'eval', 'len', 'step', 'Exception', 'print', 'append', 'shape', 'set_description', 'predictive_log_likelihood', '_decipher_to_adata', 'plot_decipher_v', 'add_image', 'plt', 'gcf', 'IPython.core', 'display', 'clear_output', 'show', 'close', 'has_stopped', 'decipher_save_model', 'uns', 'DECIPHER_GLOBALS', 'os', 'path', 'join', 'str', 'images', 'save_gif', 'load_and_show_gif')
+         varnames   ('adata', 'decipher_config', 'plot_every_k_epochs', 'plot_kwargs', 'device', 'train_idx', 'val_idx', 'adata_train', 'adata_val', 'dataloader_train', 'dataloader_val', 'decipher', 'optimizer', 'elbo', 'svi', 'gif_maker', 'val_losses', 'early_stopping', 'pbar', 'last_train_elbo', 'val_nll', 'epoch', 'train_losses', 'module', 'n_batches', 'train_elbo', 'train_elbo_n_obs', 'xc', 'loss', 'e', 'display', 'model_run_id', 'save_folder', 'full_path')
          freevars   ()
-         cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         cellvars   ('device',)
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       'decipher_train'
-         firstlineno 61
+         firstlineno 69
          lnotab
-            0x022228010401220102ff1005260148023601220122011801180204011c
-            022a022a012a020c0102ff12032c020c0102fe04ff10061c013801200304
-            01200142010a01040128010c042c013e012a02080114012c025201280122
-            012a01180118ff100316011e0104021e0120011e014c011c010c022c014e
-            0226012a021c010c02280128022001200226011a0142012a021c011e021e
-            02
+            0x042528010401220102ff1005260148023601220122011801180204011c
+            022a020c0110ff12032a020c0102ff12032a022c020c0102fe04ff10061c
+            013801200304020e0116022c023a024201040104010a01040128010c042c
+            013e012a021e0104010401080102011c0118011201200122fe08032a010a
+            012c0118012e010aff040104ff040204fe04ff120628013e012a0118012e
+            010aff040104ff040204fe04ff10050a01160104021e0120011e014c011c
+            010c022c014e0226012a021c010c0228012802280134012001200226011a
+            015c010e012a011c011e021e02
       1
       code
          argcount  : 2
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
@@ -1134,28 +1481,28 @@
             0000007403000000000000000000006a0300000000000000007c00a60100
             00ab0100000000000000007403000000000000000000006a040000000000
             0000007c00a6010000ab0100000000000000007c017a0500006702740300
             0000000000000000006a0400000000000000007c00a6010000ab01000000
             00000000000b007403000000000000000000006a0300000000000000007c
             00a6010000ab0100000000000000007c017a05000067026702a6010000ab
             0100000000000000005300
-         197           0 RESUME                   0
+         239           0 RESUME                   0
          
-         198           2 LOAD_FAST                1 (u)
+         240           2 LOAD_FAST                1 (u)
                        4 LOAD_CONST               1 ((-1, 1))
                        6 CONTAINS_OP              1
                        8 POP_JUMP_FORWARD_IF_FALSE    15 (to 40)
          
-         199          10 LOAD_GLOBAL              1 (NULL + ValueError)
+         241          10 LOAD_GLOBAL              1 (NULL + ValueError)
                       22 LOAD_CONST               2 ('u must be -1 or 1')
                       24 PRECALL                  1
                       28 CALL                     1
                       38 RAISE_VARARGS            1
          
-         200     >>   40 LOAD_GLOBAL              3 (NULL + np)
+         242     >>   40 LOAD_GLOBAL              3 (NULL + np)
                       52 LOAD_ATTR                2 (array)
                       62 LOAD_GLOBAL              3 (NULL + np)
                       74 LOAD_ATTR                3 (cos)
                       84 LOAD_FAST                0 (t)
                       86 PRECALL                  1
                       90 CALL                     1
                      100 LOAD_GLOBAL              3 (NULL + np)
@@ -1188,17 +1535,17 @@
             None
             (-1, 1)
             'u must be -1 or 1'
          names      ('ValueError', 'np', 'array', 'cos', 'sin')
          varnames   ('t', 'u')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       'rot'
-         firstlineno 197
+         firstlineno 239
          lnotab 0x020108011e01
       True
       code
          argcount  : 6
          nlocals   : 17
          stacksize : 7
          flags     : 3
@@ -1239,172 +1586,172 @@
                        2 MAKE_CELL                1 (v1_col)
                        4 MAKE_CELL                3 (v2_col)
                        6 MAKE_CELL               17 (v1_obs)
                        8 MAKE_CELL               18 (v1_valid_cells)
                       10 MAKE_CELL               19 (v2_obs)
                       12 MAKE_CELL               20 (v2_valid_cells)
          
-         203          14 RESUME                   0
+         245          14 RESUME                   0
          
-         246          16 LOAD_GLOBAL              1 (NULL + decipher_load_model)
+         288          16 LOAD_GLOBAL              1 (NULL + decipher_load_model)
                       28 LOAD_DEREF               0 (adata)
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               6 (decipher)
          
-         247          46 LOAD_GLOBAL              3 (NULL + _decipher_to_adata)
+         289          46 LOAD_GLOBAL              3 (NULL + _decipher_to_adata)
                       58 LOAD_FAST                6 (decipher)
                       60 LOAD_DEREF               0 (adata)
                       62 PRECALL                  2
                       66 CALL                     2
                       76 POP_TOP
          
-         249          78 LOAD_CLOSURE             0 (adata)
+         291          78 LOAD_CLOSURE             0 (adata)
                       80 BUILD_TUPLE              1
-                      82 LOAD_CONST               1 (<code object process_col_obs, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 249>)
+                      82 LOAD_CONST               1 (<code object process_col_obs, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 291>)
                       84 MAKE_FUNCTION            8 (closure)
                       86 STORE_FAST               7 (process_col_obs)
          
-         260          88 PUSH_NULL
+         302          88 PUSH_NULL
                       90 LOAD_FAST                7 (process_col_obs)
                       92 LOAD_DEREF               1 (v1_col)
                       94 LOAD_FAST                2 (v1_order)
                       96 PRECALL                  2
                      100 CALL                     2
                      110 UNPACK_SEQUENCE          2
                      114 STORE_DEREF             17 (v1_obs)
                      116 STORE_DEREF             18 (v1_valid_cells)
          
-         261         118 PUSH_NULL
+         303         118 PUSH_NULL
                      120 LOAD_FAST                7 (process_col_obs)
                      122 LOAD_DEREF               3 (v2_col)
                      124 LOAD_FAST                4 (v2_order)
                      126 PRECALL                  2
                      130 CALL                     2
                      140 UNPACK_SEQUENCE          2
                      144 STORE_DEREF             19 (v2_obs)
                      146 STORE_DEREF             20 (v2_valid_cells)
          
-         263         148 LOAD_CLOSURE             0 (adata)
+         305         148 LOAD_CLOSURE             0 (adata)
                      150 LOAD_CLOSURE             1 (v1_col)
                      152 LOAD_CLOSURE            17 (v1_obs)
                      154 LOAD_CLOSURE            18 (v1_valid_cells)
                      156 LOAD_CLOSURE             3 (v2_col)
                      158 LOAD_CLOSURE            19 (v2_obs)
                      160 LOAD_CLOSURE            20 (v2_valid_cells)
                      162 BUILD_TUPLE              7
-                     164 LOAD_CONST               2 (<code object score_rotation, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 263>)
+                     164 LOAD_CONST               2 (<code object score_rotation, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 305>)
                      166 MAKE_FUNCTION            8 (closure)
                      168 STORE_FAST               8 (score_rotation)
          
-         274         170 LOAD_DEREF               1 (v1_col)
+         316         170 LOAD_DEREF               1 (v1_col)
                      172 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 178)
                      174 LOAD_DEREF               3 (v2_col)
                      176 POP_JUMP_FORWARD_IF_NONE   196 (to 570)
          
-         275     >>  178 BUILD_LIST               0
+         317     >>  178 BUILD_LIST               0
                      180 STORE_FAST               9 (rotation_scores)
          
-         276         182 LOAD_GLOBAL              5 (NULL + np)
+         318         182 LOAD_GLOBAL              5 (NULL + np)
                      194 LOAD_ATTR                3 (linspace)
                      204 LOAD_CONST               4 (0)
                      206 LOAD_CONST               5 (2)
                      208 LOAD_GLOBAL              4 (np)
                      220 LOAD_ATTR                4 (pi)
                      230 BINARY_OP                5 (*)
                      234 LOAD_CONST               6 (100)
                      236 PRECALL                  3
                      240 CALL                     3
                      250 GET_ITER
                  >>  252 FOR_ITER                55 (to 364)
                      254 STORE_FAST              10 (t)
          
-         277         256 LOAD_CONST               7 ((1, -1))
+         319         256 LOAD_CONST               7 ((1, -1))
                      258 GET_ITER
                  >>  260 FOR_ITER                50 (to 362)
                      262 STORE_FAST              11 (u)
          
-         278         264 LOAD_GLOBAL             11 (NULL + rot)
+         320         264 LOAD_GLOBAL             11 (NULL + rot)
                      276 LOAD_FAST               10 (t)
                      278 LOAD_FAST               11 (u)
                      280 PRECALL                  2
                      284 CALL                     2
                      294 STORE_FAST              12 (rotation)
          
-         279         296 LOAD_FAST                9 (rotation_scores)
+         321         296 LOAD_FAST                9 (rotation_scores)
                      298 LOAD_METHOD              6 (append)
                      320 PUSH_NULL
                      322 LOAD_FAST                8 (score_rotation)
                      324 LOAD_FAST               12 (rotation)
                      326 PRECALL                  1
                      330 CALL                     1
                      340 LOAD_FAST               12 (rotation)
                      342 BUILD_TUPLE              2
                      344 PRECALL                  1
                      348 CALL                     1
                      358 POP_TOP
                      360 JUMP_BACKWARD           51 (to 260)
          
-         277     >>  362 JUMP_BACKWARD           56 (to 252)
+         319     >>  362 JUMP_BACKWARD           56 (to 252)
          
-         280     >>  364 LOAD_GLOBAL             15 (NULL + max)
+         322     >>  364 LOAD_GLOBAL             15 (NULL + max)
                      376 LOAD_FAST                9 (rotation_scores)
-                     378 LOAD_CONST               8 (<code object <lambda>, file "/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py", line 280>)
+                     378 LOAD_CONST               8 (<code object <lambda>, file "/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py", line 322>)
                      380 MAKE_FUNCTION            0
                      382 KW_NAMES                 9
                      384 PRECALL                  2
                      388 CALL                     2
                      398 LOAD_CONST              10 (1)
                      400 BINARY_SUBSCR
                      410 STORE_FAST              13 (best_rotation)
          
-         282         412 LOAD_DEREF               0 (adata)
+         324         412 LOAD_DEREF               0 (adata)
                      414 LOAD_ATTR                8 (obsm)
                      424 LOAD_CONST              11 ('decipher_v')
                      426 BINARY_SUBSCR
                      436 LOAD_METHOD              9 (copy)
                      458 PRECALL                  0
                      462 CALL                     0
                      472 LOAD_DEREF               0 (adata)
                      474 LOAD_ATTR                8 (obsm)
                      484 LOAD_CONST              12 ('decipher_v_not_rotated')
                      486 STORE_SUBSCR
          
-         283         490 LOAD_DEREF               0 (adata)
+         325         490 LOAD_DEREF               0 (adata)
                      492 LOAD_ATTR                8 (obsm)
                      502 LOAD_CONST              11 ('decipher_v')
                      504 BINARY_SUBSCR
                      514 LOAD_FAST               13 (best_rotation)
                      516 BINARY_OP                4 (@)
                      520 LOAD_DEREF               0 (adata)
                      522 LOAD_ATTR                8 (obsm)
                      532 LOAD_CONST              11 ('decipher_v')
                      534 STORE_SUBSCR
          
-         284         538 LOAD_FAST               13 (best_rotation)
+         326         538 LOAD_FAST               13 (best_rotation)
                      540 LOAD_DEREF               0 (adata)
                      542 LOAD_ATTR               10 (uns)
                      552 LOAD_CONST              13 ('decipher')
                      554 BINARY_SUBSCR
                      564 LOAD_CONST              14 ('rotation')
                      566 STORE_SUBSCR
          
-         286     >>  570 LOAD_FAST                5 (auto_flip_decipher_z)
+         328     >>  570 LOAD_FAST                5 (auto_flip_decipher_z)
                      572 POP_JUMP_FORWARD_IF_FALSE   186 (to 946)
          
-         288         574 LOAD_DEREF               0 (adata)
+         330         574 LOAD_DEREF               0 (adata)
                      576 LOAD_ATTR                8 (obsm)
                      586 LOAD_CONST              15 ('decipher_z')
                      588 BINARY_SUBSCR
                      598 LOAD_ATTR               11 (shape)
                      608 LOAD_CONST              10 (1)
                      610 BINARY_SUBSCR
                      620 STORE_FAST              14 (dim_z)
          
-         289         622 LOAD_GLOBAL              5 (NULL + np)
+         331         622 LOAD_GLOBAL              5 (NULL + np)
                      634 LOAD_ATTR               12 (corrcoef)
                      644 LOAD_DEREF               0 (adata)
                      646 LOAD_ATTR                8 (obsm)
                      656 LOAD_CONST              15 ('decipher_z')
                      658 BINARY_SUBSCR
                      668 LOAD_DEREF               0 (adata)
                      670 LOAD_ATTR                8 (obsm)
@@ -1412,15 +1759,15 @@
                      682 BINARY_SUBSCR
                      692 LOAD_CONST              16 (False)
                      694 KW_NAMES                17
                      696 PRECALL                  3
                      700 CALL                     3
                      710 STORE_FAST              15 (z_v_corr)
          
-         290         712 LOAD_GLOBAL              5 (NULL + np)
+         332         712 LOAD_GLOBAL              5 (NULL + np)
                      724 LOAD_ATTR               13 (sign)
                      734 LOAD_FAST               15 (z_v_corr)
                      736 LOAD_CONST               3 (None)
                      738 LOAD_FAST               14 (dim_z)
                      740 BUILD_SLICE              2
                      742 LOAD_FAST               14 (dim_z)
                      744 LOAD_CONST               3 (None)
@@ -1432,40 +1779,40 @@
                      784 KW_NAMES                18
                      786 PRECALL                  1
                      790 CALL                     1
                      800 PRECALL                  1
                      804 CALL                     1
                      814 STORE_FAST              16 (z_sign_correction)
          
-         291         816 LOAD_DEREF               0 (adata)
+         333         816 LOAD_DEREF               0 (adata)
                      818 LOAD_ATTR                8 (obsm)
                      828 LOAD_CONST              15 ('decipher_z')
                      830 BINARY_SUBSCR
                      840 LOAD_METHOD              9 (copy)
                      862 PRECALL                  0
                      866 CALL                     0
                      876 LOAD_DEREF               0 (adata)
                      878 LOAD_ATTR                8 (obsm)
                      888 LOAD_CONST              19 ('decipher_z_not_rotated')
                      890 STORE_SUBSCR
          
-         292         894 LOAD_DEREF               0 (adata)
+         334         894 LOAD_DEREF               0 (adata)
                      896 LOAD_ATTR                8 (obsm)
                      906 LOAD_CONST              15 ('decipher_z')
                      908 BINARY_SUBSCR
                      918 LOAD_FAST               16 (z_sign_correction)
                      920 BINARY_OP                5 (*)
                      924 LOAD_DEREF               0 (adata)
                      926 LOAD_ATTR                8 (obsm)
                      936 LOAD_CONST              15 ('decipher_z')
                      938 STORE_SUBSCR
                      942 LOAD_CONST               3 (None)
                      944 RETURN_VALUE
          
-         286     >>  946 LOAD_CONST               3 (None)
+         328     >>  946 LOAD_CONST               3 (None)
                      948 RETURN_VALUE
          consts
             "Rotate and flip the decipher space v to maximize the correlation of each decipher component\n    with provided columns values from `adata.obs` (e.g. pseudo-time, cell state progression, etc.)\n\n    Parameters\n    ----------\n    adata: sc.AnnData\n       The annotated data matrix.\n    v1_col: str, optional\n        Column name in `adata.obs` to align the first decipher component with.\n        If None, only align the second component (or does not align at all if `v2` is also None).\n    v1_order: list, optional\n        List of values in `adata.obs[v1_col]`. The rotation will attempt to align these values in\n        order along the v1 component. Must be provided if `adata.obs[v1_col]` is not numeric.\n    v2_col: str, optional\n        Column name in `adata.obs` to align the second decipher component with.\n        If None, only align the first component (or does not align at all if `v1` is also None).\n    v2_order: list, optional\n        List of values in `adata.obs[v2_col]`. The rotation will attempt to align these values in\n        order along the v2 component. Must be provided if `adata.obs[v2_col]` is not numeric.\n    auto_flip_decipher_z: bool, default True\n        If True, flip each z to be correlated positively with the components.\n\n    Returns\n    -------\n    `adata.obsm['decipher_v']`: ndarray\n        The decipher v space after rotation.\n    `adata.obsm['decipher_z']`: ndarray\n        The decipher z space after flipping.\n    `adata.uns['decipher']['rotation']`: ndarray\n        The rotation matrix used to rotate the decipher v space.\n    `adata.obsm['decipher_v_not_rotated']`: ndarray\n        The decipher v space before rotation.\n    `adata.obsm['decipher_z_not_rotated']`: ndarray\n        The decipher z space before flipping.\n    "
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
@@ -1481,86 +1828,86 @@
                   007d027c02a0080000000000000000000000000000000000000000a60000
                   00ab0000000000000000000f007d037c027c0319000000000000000000a0
                   010000000000000000000000000000000000000000741200000000000000
                   000000a6010000ab0100000000000000007d027c027c0366025300640353
                   00
                              0 COPY_FREE_VARS           1
                
-               249           2 RESUME                   0
+               291           2 RESUME                   0
                
-               250           4 LOAD_FAST                0 (v_col)
+               292           4 LOAD_FAST                0 (v_col)
                              6 POP_JUMP_FORWARD_IF_NONE   159 (to 326)
                
-               251           8 LOAD_DEREF               4 (adata)
+               293           8 LOAD_DEREF               4 (adata)
                             10 LOAD_ATTR                0 (obs)
                             20 LOAD_FAST                0 (v_col)
                             22 BINARY_SUBSCR
                             32 STORE_FAST               2 (v_obs)
                
-               252          34 LOAD_FAST                1 (v_order)
+               294          34 LOAD_FAST                1 (v_order)
                             36 POP_JUMP_FORWARD_IF_NONE    87 (to 212)
                
-               253          38 LOAD_FAST                2 (v_obs)
+               295          38 LOAD_FAST                2 (v_obs)
                             40 LOAD_METHOD              1 (astype)
                             62 LOAD_CONST               1 ('category')
                             64 PRECALL                  1
                             68 CALL                     1
                             78 LOAD_ATTR                2 (cat)
                             88 LOAD_METHOD              3 (set_categories)
                            110 LOAD_FAST                1 (v_order)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 STORE_FAST               2 (v_obs)
                
-               254         128 LOAD_FAST                2 (v_obs)
+               296         128 LOAD_FAST                2 (v_obs)
                            130 LOAD_ATTR                2 (cat)
                            140 LOAD_ATTR                4 (codes)
                            150 LOAD_METHOD              5 (replace)
                            172 LOAD_CONST               2 (-1)
                            174 LOAD_GLOBAL             12 (np)
                            186 LOAD_ATTR                7 (nan)
                            196 PRECALL                  2
                            200 CALL                     2
                            210 STORE_FAST               2 (v_obs)
                
-               255     >>  212 LOAD_FAST                2 (v_obs)
+               297     >>  212 LOAD_FAST                2 (v_obs)
                            214 LOAD_METHOD              8 (isna)
                            236 PRECALL                  0
                            240 CALL                     0
                            250 UNARY_INVERT
                            252 STORE_FAST               3 (v_valid_cells)
                
-               256         254 LOAD_FAST                2 (v_obs)
+               298         254 LOAD_FAST                2 (v_obs)
                            256 LOAD_FAST                3 (v_valid_cells)
                            258 BINARY_SUBSCR
                            268 LOAD_METHOD              1 (astype)
                            290 LOAD_GLOBAL             18 (float)
                            302 PRECALL                  1
                            306 CALL                     1
                            316 STORE_FAST               2 (v_obs)
                
-               257         318 LOAD_FAST                2 (v_obs)
+               299         318 LOAD_FAST                2 (v_obs)
                            320 LOAD_FAST                3 (v_valid_cells)
                            322 BUILD_TUPLE              2
                            324 RETURN_VALUE
                
-               258     >>  326 LOAD_CONST               3 ((None, None))
+               300     >>  326 LOAD_CONST               3 ((None, None))
                            328 RETURN_VALUE
                consts
                   None
                   'category'
                   -1
                   (None, None)
                names      ('obs', 'astype', 'cat', 'set_categories', 'codes', 'replace', 'np', 'nan', 'isna', 'float')
                varnames   ('v_col', 'v_order', 'v_obs', 'v_valid_cells')
                freevars   ('adata',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
                name       'process_col_obs'
-               firstlineno 249
+               firstlineno 291
                lnotab 0x040104011a0104015a0154012a0140010801
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 8
                flags     : 19
                code
@@ -1577,31 +1924,31 @@
                   000000000000007a0d00007d027c027403000000000000000000006a0300
                   000000000000007403000000000000000000006a0200000000000000007c
                   01890964026602190000000000000000008908a6020000ab020000000000
                   000000640319000000000000000000a6010000ab0100000000000000007a
                   1700007d027c025300
                              0 COPY_FREE_VARS           7
                
-               263           2 RESUME                   0
+               305           2 RESUME                   0
                
-               264           4 LOAD_DEREF               3 (adata)
+               306           4 LOAD_DEREF               3 (adata)
                              6 LOAD_ATTR                0 (obsm)
                             16 LOAD_CONST               1 ('decipher_v')
                             18 BINARY_SUBSCR
                             28 LOAD_FAST                0 (r)
                             30 BINARY_OP                4 (@)
                             34 STORE_FAST               1 (rotated_space)
                
-               265          36 LOAD_CONST               2 (0)
+               307          36 LOAD_CONST               2 (0)
                             38 STORE_FAST               2 (score)
                
-               266          40 LOAD_DEREF               4 (v1_col)
+               308          40 LOAD_DEREF               4 (v1_col)
                             42 POP_JUMP_FORWARD_IF_NONE    94 (to 232)
                
-               267          44 LOAD_FAST                2 (score)
+               309          44 LOAD_FAST                2 (score)
                             46 LOAD_GLOBAL              3 (NULL + np)
                             58 LOAD_ATTR                2 (corrcoef)
                             68 LOAD_FAST                1 (rotated_space)
                             70 LOAD_DEREF               6 (v1_valid_cells)
                             72 LOAD_CONST               2 (0)
                             74 BUILD_TUPLE              2
                             76 BINARY_SUBSCR
@@ -1609,15 +1956,15 @@
                             88 PRECALL                  2
                             92 CALL                     2
                            102 LOAD_CONST               3 ((1, 0))
                            104 BINARY_SUBSCR
                            114 BINARY_OP               13 (+=)
                            118 STORE_FAST               2 (score)
                
-               268         120 LOAD_FAST                2 (score)
+               310         120 LOAD_FAST                2 (score)
                            122 LOAD_GLOBAL              3 (NULL + np)
                            134 LOAD_ATTR                3 (abs)
                            144 LOAD_GLOBAL              3 (NULL + np)
                            156 LOAD_ATTR                2 (corrcoef)
                            166 LOAD_FAST                1 (rotated_space)
                            168 LOAD_DEREF               6 (v1_valid_cells)
                            170 LOAD_CONST               4 (1)
@@ -1629,18 +1976,18 @@
                            200 LOAD_CONST               3 ((1, 0))
                            202 BINARY_SUBSCR
                            212 PRECALL                  1
                            216 CALL                     1
                            226 BINARY_OP               23 (-=)
                            230 STORE_FAST               2 (score)
                
-               269     >>  232 LOAD_DEREF               7 (v2_col)
+               311     >>  232 LOAD_DEREF               7 (v2_col)
                            234 POP_JUMP_FORWARD_IF_NONE    94 (to 424)
                
-               270         236 LOAD_FAST                2 (score)
+               312         236 LOAD_FAST                2 (score)
                            238 LOAD_GLOBAL              3 (NULL + np)
                            250 LOAD_ATTR                2 (corrcoef)
                            260 LOAD_FAST                1 (rotated_space)
                            262 LOAD_DEREF               9 (v2_valid_cells)
                            264 LOAD_CONST               4 (1)
                            266 BUILD_TUPLE              2
                            268 BINARY_SUBSCR
@@ -1648,15 +1995,15 @@
                            280 PRECALL                  2
                            284 CALL                     2
                            294 LOAD_CONST               3 ((1, 0))
                            296 BINARY_SUBSCR
                            306 BINARY_OP               13 (+=)
                            310 STORE_FAST               2 (score)
                
-               271         312 LOAD_FAST                2 (score)
+               313         312 LOAD_FAST                2 (score)
                            314 LOAD_GLOBAL              3 (NULL + np)
                            326 LOAD_ATTR                3 (abs)
                            336 LOAD_GLOBAL              3 (NULL + np)
                            348 LOAD_ATTR                2 (corrcoef)
                            358 LOAD_FAST                1 (rotated_space)
                            360 LOAD_DEREF               9 (v2_valid_cells)
                            362 LOAD_CONST               2 (0)
@@ -1668,56 +2015,56 @@
                            392 LOAD_CONST               3 ((1, 0))
                            394 BINARY_SUBSCR
                            404 PRECALL                  1
                            408 CALL                     1
                            418 BINARY_OP               23 (-=)
                            422 STORE_FAST               2 (score)
                
-               272     >>  424 LOAD_FAST                2 (score)
+               314     >>  424 LOAD_FAST                2 (score)
                            426 RETURN_VALUE
                consts
                   None
                   'decipher_v'
                   0
                   (1, 0)
                   1
                names      ('obsm', 'np', 'corrcoef', 'abs')
                varnames   ('r', 'rotated_space', 'score')
                freevars   ('adata', 'v1_col', 'v1_obs', 'v1_valid_cells', 'v2_col', 'v2_obs', 'v2_valid_cells')
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
                name       'score_rotation'
-               firstlineno 263
+               firstlineno 305
                lnotab 0x04012001040104014c01700104014c017001
             None
             0
             2
             100
             (1, -1)
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 19
                code 0x97007c006401190000000000000000005300
-               280           0 RESUME                   0
+               322           0 RESUME                   0
                              2 LOAD_FAST                0 (x)
                              4 LOAD_CONST               1 (0)
                              6 BINARY_SUBSCR
                             16 RETURN_VALUE
                consts
                   None
                   0
                names      ()
                varnames   ('x',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
                name       '<lambda>'
-               firstlineno 280
+               firstlineno 322
                lnotab 0x
             ('key',)
             1
             'decipher_v'
             'decipher_v_not_rotated'
             'decipher'
             'rotation'
@@ -1726,17 +2073,17 @@
             ('y', 'rowvar')
             ('axis',)
             'decipher_z_not_rotated'
          names      ('decipher_load_model', '_decipher_to_adata', 'np', 'linspace', 'pi', 'rot', 'append', 'max', 'obsm', 'copy', 'uns', 'shape', 'corrcoef', 'sign', 'sum')
          varnames   ('adata', 'v1_col', 'v1_order', 'v2_col', 'v2_order', 'auto_flip_decipher_z', 'decipher', 'process_col_obs', 'score_rotation', 'rotation_scores', 't', 'u', 'rotation', 'best_rotation', 'dim_z', 'z_v_corr', 'z_sign_correction')
          freevars   ()
          cellvars   ('adata', 'v1_col', 'v2_col', 'v1_obs', 'v1_valid_cells', 'v2_obs', 'v2_valid_cells')
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       'decipher_rotate_space'
-         firstlineno 203
+         firstlineno 245
          lnotab
             0x102b1e0120020a0b1e011e02160b080104014a010801200142fe020330
             024e0130012002040230015a0168014e0134fa
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 4
@@ -1745,40 +2092,40 @@
             0x97007401000000000000000000007c00a6010000ab0100000000000000
             007d017c01a00100000000000000000000000000000000000000007c006a
             020000000000000000a00300000000000000000000000000000000000000
             00a6000000ab000000000000000000a6010000ab0100000000000000007d
             027c027c006a04000000000000000064013c000000740b00000000000000
             0000006a0600000000000000006402a6010000ab01000000000000000001
             0064035300
-         295           0 RESUME                   0
+         337           0 RESUME                   0
          
-         308           2 LOAD_GLOBAL              1 (NULL + decipher_load_model)
+         350           2 LOAD_GLOBAL              1 (NULL + decipher_load_model)
                       14 LOAD_FAST                0 (adata)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 STORE_FAST               1 (decipher)
          
-         309          32 LOAD_FAST                1 (decipher)
+         351          32 LOAD_FAST                1 (decipher)
                       34 LOAD_METHOD              1 (impute_gene_expression_numpy)
                       56 LOAD_FAST                0 (adata)
                       58 LOAD_ATTR                2 (X)
                       68 LOAD_METHOD              3 (toarray)
                       90 PRECALL                  0
                       94 CALL                     0
                      104 PRECALL                  1
                      108 CALL                     1
                      118 STORE_FAST               2 (imputed)
          
-         310         120 LOAD_FAST                2 (imputed)
+         352         120 LOAD_FAST                2 (imputed)
                      122 LOAD_FAST                0 (adata)
                      124 LOAD_ATTR                4 (layers)
                      134 LOAD_CONST               1 ('decipher_imputed')
                      136 STORE_SUBSCR
          
-         311         140 LOAD_GLOBAL             11 (NULL + logging)
+         353         140 LOAD_GLOBAL             11 (NULL + logging)
                      152 LOAD_ATTR                6 (info)
                      162 LOAD_CONST               2 ("Added `.layers['imputed']`: the Decipher imputed data.")
                      164 PRECALL                  1
                      168 CALL                     1
                      178 POP_TOP
                      180 LOAD_CONST               3 (None)
                      182 RETURN_VALUE
@@ -1787,17 +2134,17 @@
             'decipher_imputed'
             "Added `.layers['imputed']`: the Decipher imputed data."
             None
          names      ('decipher_load_model', 'impute_gene_expression_numpy', 'X', 'toarray', 'layers', 'logging', 'info')
          varnames   ('adata', 'decipher', 'imputed')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       'decipher_gene_imputation'
-         firstlineno 295
+         firstlineno 337
          lnotab 0x020d1e0158011401
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
@@ -1814,51 +2161,51 @@
             006a0300000000000000007c017c006a0400000000000000006408190000
             000000000000006403ac04a6030000ab03000000000000000064007c006a
             0500000000000000006a0600000000000000006405190000000000000000
             0085027c006a0500000000000000006a0600000000000000006405190000
             00000000000000640085026602190000000000000000007c006a07000000
             000000000064093c0000007411000000000000000000006a090000000000
             000000640aa6010000ab010000000000000000010064005300
-         314           0 RESUME                   0
+         356           0 RESUME                   0
          
-         315           2 LOAD_CONST               1 ('decipher_imputed')
+         357           2 LOAD_CONST               1 ('decipher_imputed')
                        4 LOAD_FAST                0 (adata)
                        6 LOAD_ATTR                0 (layers)
                       16 CONTAINS_OP              1
                       18 POP_JUMP_FORWARD_IF_FALSE    15 (to 50)
          
-         316          20 LOAD_GLOBAL              3 (NULL + decipher_gene_imputation)
+         358          20 LOAD_GLOBAL              3 (NULL + decipher_gene_imputation)
                       32 LOAD_FAST                0 (adata)
                       34 PRECALL                  1
                       38 CALL                     1
                       48 POP_TOP
          
-         317     >>   50 LOAD_FAST                0 (adata)
+         359     >>   50 LOAD_FAST                0 (adata)
                       52 LOAD_ATTR                0 (layers)
                       62 LOAD_CONST               1 ('decipher_imputed')
                       64 BINARY_SUBSCR
                       74 STORE_FAST               1 (gene_expression_imputed)
          
-         318          76 LOAD_GLOBAL              5 (NULL + np)
+         360          76 LOAD_GLOBAL              5 (NULL + np)
                       88 LOAD_ATTR                3 (cov)
          
-         319          98 LOAD_FAST                1 (gene_expression_imputed)
+         361          98 LOAD_FAST                1 (gene_expression_imputed)
          
-         320         100 LOAD_FAST                0 (adata)
+         362         100 LOAD_FAST                0 (adata)
                      102 LOAD_ATTR                4 (obsm)
                      112 LOAD_CONST               2 ('decipher_v')
                      114 BINARY_SUBSCR
          
-         321         124 LOAD_CONST               3 (False)
+         363         124 LOAD_CONST               3 (False)
          
-         318         126 KW_NAMES                 4
+         360         126 KW_NAMES                 4
                      128 PRECALL                  3
                      132 CALL                     3
          
-         322         142 LOAD_CONST               0 (None)
+         364         142 LOAD_CONST               0 (None)
                      144 LOAD_FAST                0 (adata)
                      146 LOAD_ATTR                5 (X)
                      156 LOAD_ATTR                6 (shape)
                      166 LOAD_CONST               5 (1)
                      168 BINARY_SUBSCR
                      178 BUILD_SLICE              2
                      180 LOAD_FAST                0 (adata)
@@ -1866,44 +2213,46 @@
                      192 LOAD_ATTR                6 (shape)
                      202 LOAD_CONST               5 (1)
                      204 BINARY_SUBSCR
                      214 LOAD_CONST               0 (None)
                      216 BUILD_SLICE              2
                      218 BUILD_TUPLE              2
          
-         318         220 BINARY_SUBSCR
+         360         220 BINARY_SUBSCR
                      230 LOAD_FAST                0 (adata)
                      232 LOAD_ATTR                7 (varm)
                      242 LOAD_CONST               6 ('decipher_v_gene_covariance')
                      244 STORE_SUBSCR
          
-         323         248 LOAD_GLOBAL             17 (NULL + logging)
+         365         248 LOAD_GLOBAL             17 (NULL + logging)
                      260 LOAD_ATTR                9 (info)
-                     270 LOAD_CONST               7 ("Added `.varm['decipher_v_gene_covariance']`: the covariance between Decipher v and each gene.")
-                     272 PRECALL                  1
+         
+         366         270 LOAD_CONST               7 ("Added `.varm['decipher_v_gene_covariance']`: the covariance between Decipher v and each gene.")
+         
+         365         272 PRECALL                  1
                      276 CALL                     1
                      286 POP_TOP
          
-         324         288 LOAD_GLOBAL              5 (NULL + np)
+         368         288 LOAD_GLOBAL              5 (NULL + np)
                      300 LOAD_ATTR                3 (cov)
          
-         325         310 LOAD_FAST                1 (gene_expression_imputed)
+         369         310 LOAD_FAST                1 (gene_expression_imputed)
          
-         326         312 LOAD_FAST                0 (adata)
+         370         312 LOAD_FAST                0 (adata)
                      314 LOAD_ATTR                4 (obsm)
                      324 LOAD_CONST               8 ('decipher_z')
                      326 BINARY_SUBSCR
          
-         327         336 LOAD_CONST               3 (False)
+         371         336 LOAD_CONST               3 (False)
          
-         324         338 KW_NAMES                 4
+         368         338 KW_NAMES                 4
                      340 PRECALL                  3
                      344 CALL                     3
          
-         328         354 LOAD_CONST               0 (None)
+         372         354 LOAD_CONST               0 (None)
                      356 LOAD_FAST                0 (adata)
                      358 LOAD_ATTR                5 (X)
                      368 LOAD_ATTR                6 (shape)
                      378 LOAD_CONST               5 (1)
                      380 BINARY_SUBSCR
                      390 BUILD_SLICE              2
                      392 LOAD_FAST                0 (adata)
@@ -1911,24 +2260,26 @@
                      404 LOAD_ATTR                6 (shape)
                      414 LOAD_CONST               5 (1)
                      416 BINARY_SUBSCR
                      426 LOAD_CONST               0 (None)
                      428 BUILD_SLICE              2
                      430 BUILD_TUPLE              2
          
-         324         432 BINARY_SUBSCR
+         368         432 BINARY_SUBSCR
                      442 LOAD_FAST                0 (adata)
                      444 LOAD_ATTR                7 (varm)
                      454 LOAD_CONST               9 ('decipher_z_gene_covariance')
                      456 STORE_SUBSCR
          
-         329         460 LOAD_GLOBAL             17 (NULL + logging)
+         373         460 LOAD_GLOBAL             17 (NULL + logging)
                      472 LOAD_ATTR                9 (info)
-                     482 LOAD_CONST              10 ("Added `.varm['decipher_z_gene_covariance']`: the covariance between Decipher z and each gene.")
-                     484 PRECALL                  1
+         
+         374         482 LOAD_CONST              10 ("Added `.varm['decipher_z_gene_covariance']`: the covariance between Decipher z and each gene.")
+         
+         373         484 PRECALL                  1
                      488 CALL                     1
                      498 POP_TOP
                      500 LOAD_CONST               0 (None)
                      502 RETURN_VALUE
          consts
             None
             'decipher_imputed'
@@ -1941,104 +2292,104 @@
             'decipher_z'
             'decipher_z_gene_covariance'
             "Added `.varm['decipher_z_gene_covariance']`: the covariance between Decipher z and each gene."
          names      ('layers', 'decipher_gene_imputation', 'np', 'cov', 'obsm', 'X', 'shape', 'varm', 'logging', 'info')
          varnames   ('adata', 'gene_expression_imputed')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       'decipher_and_gene_covariance'
-         firstlineno 314
+         firstlineno 356
          lnotab
-            0x020112011e011a0116010201180102fd10044efc1c0528011601020118
-            0102fd10044efc1c05
+            0x020112011e011a0116010201180102fd10044efc1c05160102ff100316
+            010201180102fd10044efc1c05160102ff
       code
          argcount  : 2
          nlocals   : 4
-         stacksize : 4
+         stacksize : 5
          flags     : 3
          code
             0x97007c00a0000000000000000000000000000000000000000000a60000
             00ab00000000000000000001007c00a00100000000000000000000000000
-            000000000000007c016a020000000000000000a003000000000000000000
-            0000000000000000000000a6000000ab000000000000000000a6010000ab
-            0100000000000000005c0200007d027d037c027c016a0400000000000000
-            0064013c0000007c037c016a04000000000000000064023c000000740b00
-            0000000000000000006a0600000000000000006403a6010000ab01000000
-            00000000000100740b000000000000000000006a06000000000000000064
-            04a6010000ab010000000000000000010064055300
-         332           0 RESUME                   0
+            000000000000007405000000000000000000007c01a6010000ab01000000
+            0000000000a6010000ab0100000000000000005c0200007d027d037c027c
+            016a03000000000000000064013c0000007c037c016a0300000000000000
+            0064023c0000007409000000000000000000006a05000000000000000064
+            03a6010000ab01000000000000000001007409000000000000000000006a
+            0500000000000000006404a6010000ab0100000000000000000100640553
+            00
+         378           0 RESUME                   0
          
-         349           2 LOAD_FAST                0 (decipher)
+         395           2 LOAD_FAST                0 (decipher)
                        4 LOAD_METHOD              0 (eval)
                       26 PRECALL                  0
                       30 CALL                     0
                       40 POP_TOP
          
-         350          42 LOAD_FAST                0 (decipher)
+         396          42 LOAD_FAST                0 (decipher)
                       44 LOAD_METHOD              1 (compute_v_z_numpy)
-                      66 LOAD_FAST                1 (adata)
-                      68 LOAD_ATTR                2 (X)
-                      78 LOAD_METHOD              3 (toarray)
-                     100 PRECALL                  0
-                     104 CALL                     0
-                     114 PRECALL                  1
-                     118 CALL                     1
-                     128 UNPACK_SEQUENCE          2
-                     132 STORE_FAST               2 (latent_v)
-                     134 STORE_FAST               3 (latent_z)
+                      66 LOAD_GLOBAL              5 (NULL + get_dense_X)
+                      78 LOAD_FAST                1 (adata)
+                      80 PRECALL                  1
+                      84 CALL                     1
+                      94 PRECALL                  1
+                      98 CALL                     1
+                     108 UNPACK_SEQUENCE          2
+                     112 STORE_FAST               2 (latent_v)
+                     114 STORE_FAST               3 (latent_z)
+         
+         397         116 LOAD_FAST                2 (latent_v)
+                     118 LOAD_FAST                1 (adata)
+                     120 LOAD_ATTR                3 (obsm)
+                     130 LOAD_CONST               1 ('decipher_v')
+                     132 STORE_SUBSCR
          
-         351         136 LOAD_FAST                2 (latent_v)
+         398         136 LOAD_FAST                3 (latent_z)
                      138 LOAD_FAST                1 (adata)
-                     140 LOAD_ATTR                4 (obsm)
-                     150 LOAD_CONST               1 ('decipher_v')
+                     140 LOAD_ATTR                3 (obsm)
+                     150 LOAD_CONST               2 ('decipher_z')
                      152 STORE_SUBSCR
          
-         352         156 LOAD_FAST                3 (latent_z)
-                     158 LOAD_FAST                1 (adata)
-                     160 LOAD_ATTR                4 (obsm)
-                     170 LOAD_CONST               2 ('decipher_z')
-                     172 STORE_SUBSCR
-         
-         353         176 LOAD_GLOBAL             11 (NULL + logging)
-                     188 LOAD_ATTR                6 (info)
-                     198 LOAD_CONST               3 ("Added `.obsm['decipher_v']`: the Decipher v space.")
-                     200 PRECALL                  1
-                     204 CALL                     1
-                     214 POP_TOP
-         
-         354         216 LOAD_GLOBAL             11 (NULL + logging)
-                     228 LOAD_ATTR                6 (info)
-                     238 LOAD_CONST               4 ("Added `.obsm['decipher_z']`: the Decipher z space.")
-                     240 PRECALL                  1
-                     244 CALL                     1
-                     254 POP_TOP
-                     256 LOAD_CONST               5 (None)
-                     258 RETURN_VALUE
+         399         156 LOAD_GLOBAL              9 (NULL + logging)
+                     168 LOAD_ATTR                5 (info)
+                     178 LOAD_CONST               3 ("Added `.obsm['decipher_v']`: the Decipher v space.")
+                     180 PRECALL                  1
+                     184 CALL                     1
+                     194 POP_TOP
+         
+         400         196 LOAD_GLOBAL              9 (NULL + logging)
+                     208 LOAD_ATTR                5 (info)
+                     218 LOAD_CONST               4 ("Added `.obsm['decipher_z']`: the Decipher z space.")
+                     220 PRECALL                  1
+                     224 CALL                     1
+                     234 POP_TOP
+                     236 LOAD_CONST               5 (None)
+                     238 RETURN_VALUE
          consts
             "Compute the decipher v and z spaces from the decipher model. Add them to `adata.obsm`.\n\n    Parameters\n    ----------\n    decipher: Decipher\n        The decipher model.\n    adata: sc.AnnData\n        The annotated data matrix.\n\n    Returns\n    -------\n    `adata.obsm['decipher_v']`: ndarray\n        The decipher v space.\n    `adata.obsm['decipher_z']`: ndarray\n        The decipher z space.\n    "
             'decipher_v'
             'decipher_z'
             "Added `.obsm['decipher_v']`: the Decipher v space."
             "Added `.obsm['decipher_z']`: the Decipher z space."
             None
-         names      ('eval', 'compute_v_z_numpy', 'X', 'toarray', 'obsm', 'logging', 'info')
+         names      ('eval', 'compute_v_z_numpy', 'get_dense_X', 'obsm', 'logging', 'info')
          varnames   ('decipher', 'adata', 'latent_v', 'latent_z')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
          name       '_decipher_to_adata'
-         firstlineno 332
-         lnotab 0x021128015e01140114012801
+         firstlineno 378
+         lnotab 0x021128014a01140114012801
+      (30,)
       (1,)
       (None, None, None, None, True)
-   names      ('logging', 'os', 'numpy', 'np', 'pyro', 'scanpy', 'sc', 'torch', 'matplotlib', 'pyplot', 'plt', 'poutine', 'pyro.infer', 'SVI', 'Trace_ELBO', 'pyro.optim', 'MultiStepLR', 'tqdm', 'decipher.plot.decipher', 'decipher', 'plot_decipher_v', 'decipher.tools._decipher', 'Decipher', 'DecipherConfig', 'decipher.tools._decipher.data', 'decipher_load_model', 'decipher_save_model', 'make_data_loader_from_adata', 'decipher.tools.utils', 'EarlyStopping', 'decipher.utils', 'DECIPHER_GLOBALS', 'GIFMaker', 'is_notebook', 'load_and_show_gif', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'predictive_log_likelihood', '_make_train_val_split', 'AnnData', 'decipher_train', 'rot', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance', '_decipher_to_adata')
+   names      ('logging', 'os', 'numpy', 'np', 'pyro', 'scanpy', 'sc', 'torch', 'matplotlib', 'pyplot', 'plt', 'pyro.optim', 'poutine', 'pyro.infer', 'SVI', 'Trace_ELBO', 'tqdm', 'decipher.plot.decipher', 'decipher', 'plot_decipher_v', 'decipher.tools._decipher', 'Decipher', 'DecipherConfig', 'decipher.tools._decipher.data', 'decipher_load_model', 'decipher_save_model', 'make_data_loader_from_adata', 'get_dense_X', 'decipher.tools.utils', 'EarlyStopping', 'decipher.utils', 'DECIPHER_GLOBALS', 'GIFMaker', 'is_notebook', 'load_and_show_gif', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'predictive_log_likelihood', '_make_train_val_split', 'AnnData', 'decipher_train', 'rot', 'decipher_rotate_space', 'decipher_gene_imputation', 'decipher_and_gene_covariance', '_decipher_to_adata')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/decipher.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/decipher.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010801080208010801080108010c010c0110010c010c020c0110
-      0114050c01180220010e0102010cfe1206061006101201020102fc04010c
-      ff087f00090808020102010201020102fa085c06130612
+      0x00ff02010801080208010801080108010c0108010c0110010c020c0110
+      0118060c01180220010e0102010cfe12060817061012010201020102fb04
+      010cff087f002b0808020102010201020102fa085c06130616
```

### Comparing `scdecipher-0.1.0/decipher/tools/__pycache__/trajectory_inference.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/__pycache__/trajectory_inference.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 19292
+moddate:  0x2d222166 (Thu Apr 18 13:37:49 2024 UTC)
+files sz: 19329
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a03640064
@@ -93,78 +93,78 @@
     15         150 KW_NAMES                 5
                152 PRECALL                  2
                156 CALL                     2
                166 POP_TOP
    
     21         168 PUSH_NULL
                170 LOAD_BUILD_CLASS
-               172 LOAD_CONST               6 (<code object Trajectory, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 21>)
+               172 LOAD_CONST               6 (<code object Trajectory, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 21>)
                174 MAKE_FUNCTION            0
                176 LOAD_CONST               7 ('Trajectory')
                178 PRECALL                  2
                182 CALL                     2
                192 STORE_NAME              23 (Trajectory)
    
     92         194 PUSH_NULL
                196 LOAD_BUILD_CLASS
-               198 LOAD_CONST               8 (<code object TConfig, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 92>)
+               198 LOAD_CONST               8 (<code object TConfig, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 92>)
                200 MAKE_FUNCTION            0
                202 LOAD_CONST               9 ('TConfig')
                204 PRECALL                  2
                208 CALL                     2
                218 STORE_NAME              24 (TConfig)
    
    182         220 LOAD_CONST              25 ((1.0, 10, 0, 'decipher_z'))
-               222 LOAD_CONST              13 (<code object cell_clusters, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 182>)
+               222 LOAD_CONST              13 (<code object cell_clusters, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 182>)
                224 MAKE_FUNCTION            1 (defaults)
                226 STORE_NAME              25 (cell_clusters)
    
    241         228 NOP
    
    242         230 NOP
    
    243         232 NOP
    
    237         234 LOAD_CONST              26 ((0.3, 10, 'decipher_clusters'))
-               236 LOAD_CONST              16 (<code object _subset_cells_and_clusters, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 237>)
+               236 LOAD_CONST              16 (<code object _subset_cells_and_clusters, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 237>)
                238 MAKE_FUNCTION            1 (defaults)
                240 STORE_NAME              26 (_subset_cells_and_clusters)
    
    266         242 NOP
    
    267         244 NOP
    
    268         246 NOP
    
    269         248 NOP
    
    270         250 NOP
    
    263         252 LOAD_CONST              27 ((None, None, 0.3, 'decipher_clusters', 10))
-               254 LOAD_CONST              17 (<code object find_cluster_with_marker, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 263>)
+               254 LOAD_CONST              17 (<code object find_cluster_with_marker, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 263>)
                256 MAKE_FUNCTION            1 (defaults)
                258 STORE_NAME              27 (find_cluster_with_marker)
    
    313         260 LOAD_CONST              18 (50)
    
    314         262 LOAD_CONST              15 ('decipher_clusters')
    
    310         264 LOAD_CONST              19 (('point_density', 'cluster_key'))
                266 BUILD_CONST_KEY_MAP      2
-               268 LOAD_CONST              20 (<code object trajectories, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 310>)
+               268 LOAD_CONST              20 (<code object trajectories, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 310>)
                270 MAKE_FUNCTION            2 (kwdefaults)
                272 STORE_NAME              28 (trajectories)
    
-   399         274 LOAD_CONST              28 ((10,))
-               276 LOAD_CONST              21 (<code object decipher_time, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 399>)
+   402         274 LOAD_CONST              28 ((10,))
+               276 LOAD_CONST              21 (<code object decipher_time, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 402>)
                278 MAKE_FUNCTION            1 (defaults)
                280 STORE_NAME              29 (decipher_time)
    
-   435         282 LOAD_CONST              29 ((10000, 100))
-               284 LOAD_CONST              24 (<code object gene_patterns, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 435>)
+   438         282 LOAD_CONST              29 ((10000, 100))
+               284 LOAD_CONST              24 (<code object gene_patterns, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 438>)
                286 MAKE_FUNCTION            1 (defaults)
                288 STORE_NAME              30 (gene_patterns)
                290 LOAD_CONST               1 (None)
                292 RETURN_VALUE
    consts
       0
       None
@@ -188,34 +188,34 @@
                        8 STORE_NAME               2 (__qualname__)
          
           26          10 NOP
          
           27          12 NOP
          
           22          14 LOAD_CONST              10 ((50, 'decipher_v'))
-                      16 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 22>)
+                      16 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 22>)
                       18 MAKE_FUNCTION            1 (defaults)
                       20 STORE_NAME               3 (__init__)
          
           47          22 LOAD_CONST              11 ((100,))
-                      24 LOAD_CONST               5 (<code object _linspace, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 47>)
+                      24 LOAD_CONST               5 (<code object _linspace, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 47>)
                       26 MAKE_FUNCTION            1 (defaults)
                       28 STORE_NAME               4 (_linspace)
          
-          58          30 LOAD_CONST               6 (<code object at_time, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 58>)
+          58          30 LOAD_CONST               6 (<code object at_time, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 58>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               5 (at_time)
          
-          71          36 LOAD_CONST               7 (<code object to_dict, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 71>)
+          71          36 LOAD_CONST               7 (<code object to_dict, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 71>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               6 (to_dict)
          
           81          42 LOAD_NAME                7 (staticmethod)
          
-          82          44 LOAD_CONST               8 (<code object from_dict, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 81>)
+          82          44 LOAD_CONST               8 (<code object from_dict, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 81>)
                       46 MAKE_FUNCTION            0
          
           81          48 PRECALL                  0
                       52 CALL                     0
          
           82          62 STORE_NAME               8 (from_dict)
                       64 LOAD_CONST               9 (None)
@@ -352,15 +352,15 @@
                   None
                   1
                   -1
                names      ('_point_density', 'cluster_ids', 'np', 'array', 'zip', 'linalg', 'norm', 'append', 'cumsum', 'cumulative_length', 'cluster_locations', 'int', 'n_points', 'rep_key', '_linspace', 'trajectory_latent', 'trajectory_time')
                varnames   ('self', 'cluster_locations', 'cluster_ids', 'point_density', 'rep_key', 'distances', 's', 'e', 'v', 'd', 'cumulative_length')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       '__init__'
                firstlineno 22
                lnotab 0x02070e010e01280104013a010a013e012c0228020e010e014e010e02
             100
             code
                argcount  : 2
                nlocals   : 8
@@ -437,15 +437,15 @@
                   None
                   -1
                   0
                names      ('cumulative_length', 'np', 'linspace', 'append', 'at_time', 'array', 'astype', 'float32')
                varnames   ('self', 'num', 'total_length', 'times', 'res', 't', 'trajectory_latent', 'trajectory_time')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       '_linspace'
                firstlineno 47
                lnotab 0x02011a012c0104010801520162010402
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 5
@@ -548,15 +548,15 @@
                   None
                   0
                   1
                names      ('cumulative_length', 'cluster_locations')
                varnames   ('self', 't', 'i')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       'at_time'
                firstlineno 58
                lnotab 0x0201040122010aff22020c0124013aff08042002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
@@ -595,15 +595,15 @@
                consts
                   None
                   ('cluster_locations', 'cluster_ids', 'points', 'times', 'density', 'rep_key')
                names      ('dict', 'cluster_locations', 'cluster_ids', 'trajectory_latent', 'trajectory_time', '_point_density', 'rep_key')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       'to_dict'
                firstlineno 71
                lnotab 0x02010c010c010c010c010c010c010cfa
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
@@ -647,26 +647,26 @@
                   'density'
                   'rep_key'
                   ('point_density', 'rep_key')
                names      ('Trajectory',)
                varnames   ('d', 'trajectory')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       'from_dict'
                firstlineno 81
                lnotab 0x02020c010e010e010e010efc1206
             None
             (50, 'decipher_v')
             (100,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_linspace', 'at_time', 'to_dict', 'staticmethod', 'from_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'Trajectory'
          firstlineno 21
          lnotab 0x0a05020102fb0819080b060d060a020104ff0e01
       'Trajectory'
       code
          argcount  : 0
          nlocals   : 0
@@ -701,28 +701,28 @@
          
          130          28 LOAD_CONST              11 ((None, None, None, None, None, 0.3, 10))
                       30 LOAD_CONST               5 ('name')
          
          132          32 LOAD_NAME                4 (str)
          
          130          34 BUILD_TUPLE              2
-                      36 LOAD_CONST               6 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 130>)
+                      36 LOAD_CONST               6 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 130>)
                       38 MAKE_FUNCTION            5 (defaults, annotations)
                       40 STORE_NAME               5 (__init__)
          
          150          42 LOAD_CONST              12 (('decipher_clusters',))
-                      44 LOAD_CONST               8 (<code object _compute_cluster_id, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 150>)
+                      44 LOAD_CONST               8 (<code object _compute_cluster_id, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 150>)
                       46 MAKE_FUNCTION            1 (defaults)
                       48 STORE_NAME               6 (_compute_cluster_id)
          
-         175          50 LOAD_CONST               9 (<code object get_start_cluster_id, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 175>)
+         175          50 LOAD_CONST               9 (<code object get_start_cluster_id, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 175>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME               7 (get_start_cluster_id)
          
-         178          56 LOAD_CONST              10 (<code object get_end_cluster_id, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 178>)
+         178          56 LOAD_CONST              10 (<code object get_end_cluster_id, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 178>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME               8 (get_end_cluster_id)
                       62 LOAD_CONST               2 (None)
                       64 RETURN_VALUE
          consts
             'TConfig'
             'A class to configure the computation of a trajectory.\n\n    The user can define a trajectory in different ways:\n    - by providing the start and end clusters of the trajectory: `start_cluster_or_marker` and\n      `end_cluster_or_marker`. These can be either cluster ids or marker genes. If they are marker\n      genes, the cluster with the highest expression of the marker gene is selected. Then, the\n      trajectory is computed as the shortest path between the two clusters in the minimum spanning\n      tree of the clusters.\n    - by providing a list of cluster ids: `cluster_ids_list`. Then, the trajectory is the path\n      connecting the clusters in the order of the list.\n\n    Parameters\n    ----------\n    name : str\n        The name of the trajectory. It is used as a key to store the trajectory in the AnnData.\n    start_cluster_or_marker : str, optional\n        The start cluster id or marker gene. If it is a marker gene, the cluster with the highest\n        expression of the marker gene is selected. If it is a cluster id, it is used as is.\n    end_cluster_or_marker : str, optional\n        The end cluster id or marker gene. If it is a marker gene, the cluster with the highest\n        expression of the marker gene is selected. If it is a cluster id, it is used as is.\n    subset_col : str, optional\n        The column in `adata.obs` to subset on. If None, no subsetting is performed.\n    subset_val : str, optional\n        The value in subset_column to subset on. If None, no subsetting is performed.\n    cluster_ids_list : list, optional\n        A list of cluster ids. If provided, the trajectory is the path connecting the clusters in\n        the order of the list. `start_cluster_or_marker` and `end_cluster_or_marker` are ignored.\n    subset_percent_per_cluster : float, default 0.3\n        When subsetting the cells, each cluster must have at least this proportion of cells from\n        the subset to not be discarded. This is useful to remove clusters with too few cells from\n        the subset.\n    min_cell_per_cluster : int, default 10\n        When subsetting the cells, each cluster must have at least this number of cells from the\n        subset to not be discarded. See `subset_percent_per_cluster`.\n    '
@@ -777,15 +777,15 @@
                            116 RETURN_VALUE
                consts
                   None
                names      ('name', '_start_cluster', '_end_cluster', 'subset_column', 'subset_value', 'subset_percent_per_cluster', 'min_cell_per_cluster', 'cluster_ids_list')
                varnames   ('self', 'name', 'start_cluster_or_marker', 'end_cluster_or_marker', 'subset_col', 'subset_val', 'cluster_ids_list', 'subset_percent_per_cluster', 'min_cell_per_cluster')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       '__init__'
                firstlineno 130
                lnotab 0x020b0e010e010e010e010e010e010e01
             'decipher_clusters'
             code
                argcount  : 4
                nlocals   : 5
@@ -841,15 +841,15 @@
                consts
                   None
                   ('subset_column', 'subset_value', 'subset_min_percent_per_cluster', 'cluster_key', 'min_cell_per_cluster')
                names      ('obs', 'values', 'find_cluster_with_marker', 'subset_column', 'subset_value', 'subset_percent_per_cluster', 'min_cell_per_cluster')
                varnames   ('self', 'adata', 'cluster_input', 'cluster_key', 'cluster_id')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       '_compute_cluster_id'
                firstlineno 150
                lnotab 0x0209280204030c01020102010c010c010c0102010cf91209
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -869,15 +869,15 @@
                             54 RETURN_VALUE
                consts
                   None
                names      ('_compute_cluster_id', '_start_cluster')
                varnames   ('self', 'adata')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       'get_start_cluster_id'
                firstlineno 175
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -897,25 +897,25 @@
                             54 RETURN_VALUE
                consts
                   None
                names      ('_compute_cluster_id', '_end_cluster')
                varnames   ('self', 'adata')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       'get_end_cluster_id'
                firstlineno 178
                lnotab 0x0201
             (None, None, None, None, None, 0.3, 10)
             ('decipher_clusters',)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', '_compute_cluster_id', 'get_start_cluster_id', 'get_end_cluster_id')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'TConfig'
          firstlineno 92
          lnotab 0x0a01042802010201020102010201020102f7040202fe081408190603
       'TConfig'
       1.0
       10
       'decipher_z'
@@ -1058,15 +1058,15 @@
             'decipher_clusters'
             "Added `.obs['decipher_clusters']`: the cluster labels."
             None
          names      ('logger', 'info', 'sc', 'pp', 'neighbors', 'tl', 'leiden', 'pd', 'Categorical', 'obs', 'logging')
          varnames   ('adata', 'leiden_resolution', 'n_neighbors', 'seed', 'rep_key', 'neighbors_key', 'cluster_key')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'cell_clusters'
          firstlineno 182
          lnotab
             0x021b34010a010a0122010aff10032c01020102010201020102fb120722
             010aff10032c01020102010201020102fb12074e02
       0.3
       'decipher_clusters'
@@ -1077,16 +1077,16 @@
          flags     : 3
          code
             0x97007c006a0000000000000000007c017c056702190000000000000000
             00a0010000000000000000000000000000000000000000a6000000ab0000
             000000000000007d066401640267027c065f0200000000000000007c0664
             01190000000000000000007c026b02000000007c0664033c0000007c06a0
             0300000000000000000000000000000000000000006402a6010000ab0100
-            00000000000000a0040000000000000000000000000000000000000000a6
-            000000ab0000000000000000006403190000000000000000007c036b0400
+            00000000000000640319000000000000000000a004000000000000000000
+            0000000000000000000000a6000000ab0000000000000000007c036b0400
             0000007d077c06a003000000000000000000000000000000000000000064
             02a6010000ab010000000000000000640319000000000000000000a00500
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007c046b04000000007d087c077c087a0100007d097c097c09190000
             000000000000006a0600000000000000007d097c06640219000000000000
             000000a00700000000000000000000000000000000000000007c09a60100
             00ab0100000000000000007d0a7c007c0a190000000000000000007d0b7c
@@ -1120,19 +1120,19 @@
                      112 STORE_SUBSCR
          
          250         116 LOAD_FAST                6 (data)
                      118 LOAD_METHOD              3 (groupby)
                      140 LOAD_CONST               2 ('cluster')
                      142 PRECALL                  1
                      146 CALL                     1
-                     156 LOAD_METHOD              4 (mean)
-                     178 PRECALL                  0
-                     182 CALL                     0
-                     192 LOAD_CONST               3 ('in_subset')
-                     194 BINARY_SUBSCR
+                     156 LOAD_CONST               3 ('in_subset')
+                     158 BINARY_SUBSCR
+                     168 LOAD_METHOD              4 (mean)
+                     190 PRECALL                  0
+                     194 CALL                     0
                      204 LOAD_FAST                3 (subset_min_percent_per_cluster)
                      206 COMPARE_OP               4 (>)
                      212 STORE_FAST               7 (valid_p)
          
          252         214 LOAD_FAST                6 (data)
                      216 LOAD_METHOD              3 (groupby)
                      238 LOAD_CONST               2 ('cluster')
@@ -1179,15 +1179,15 @@
             'subset'
             'cluster'
             'in_subset'
          names      ('obs', 'copy', 'columns', 'groupby', 'mean', 'sum', 'index', 'isin')
          varnames   ('adata', 'subset_column', 'subset_value', 'subset_min_percent_per_cluster', 'min_cell_per_cluster', 'cluster_key', 'data', 'valid_p', 'valid_n', 'valid_clusters', 'cell_mask', 'adata_subset')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       '_subset_cells_and_clusters'
          firstlineno 237
          lnotab 0x0208420112011e03620262010a011a0236031001
       code
          argcount  : 7
          nlocals   : 8
          stacksize : 8
@@ -1287,15 +1287,15 @@
             0
             False
             ('by', 'ascending')
          names      ('_subset_cells_and_clusters', 'pd', 'DataFrame', 'X', 'toarray', 'obs', 'values', 'groupby', 'mean', 'sort_values', 'index')
          varnames   ('adata', 'marker', 'subset_column', 'subset_value', 'subset_min_percent_per_cluster', 'cluster_key', 'min_cell_per_cluster', 'marker_data')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'find_cluster_with_marker'
          firstlineno 263
          lnotab 0x021e04010c010201020102010201020102fa12086a012a024e012e01
       50
       ('point_density', 'cluster_key')
       code
          argcount  : 1
@@ -1609,15 +1609,15 @@
                     1186 POP_TOP
          
          389        1188 LOAD_GLOBAL             41 (NULL + np)
                     1200 LOAD_ATTR               21 (array)
          
          390        1210 LOAD_CLOSURE            27 (cluster_locations)
                     1212 BUILD_TUPLE              1
-                    1214 LOAD_CONST              16 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py", line 390>)
+                    1214 LOAD_CONST              16 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py", line 390>)
                     1216 MAKE_FUNCTION            8 (closure)
                     1218 LOAD_FAST               11 (t_cluster_ids)
                     1220 GET_ITER
                     1222 PRECALL                  0
                     1226 CALL                     0
          
          389        1236 PRECALL                  1
@@ -1630,37 +1630,40 @@
                     1298 CALL                     1
          
          389        1308 STORE_FAST              25 (t_cluster_locations)
          
          392        1310 LOAD_GLOBAL             77 (NULL + Trajectory)
          
          393        1322 LOAD_FAST               25 (t_cluster_locations)
-                    1324 LOAD_FAST               11 (t_cluster_ids)
-                    1326 LOAD_FAST                1 (point_density)
-                    1328 LOAD_FAST                4 (rep_key)
+         
+         394        1324 LOAD_FAST               11 (t_cluster_ids)
+         
+         395        1326 LOAD_FAST                1 (point_density)
+         
+         396        1328 LOAD_FAST                4 (rep_key)
          
          392        1330 KW_NAMES                17
                     1332 PRECALL                  4
                     1336 CALL                     4
                     1346 STORE_FAST              26 (trajectory)
          
-         395        1348 LOAD_FAST               26 (trajectory)
+         398        1348 LOAD_FAST               26 (trajectory)
                     1350 LOAD_METHOD             39 (to_dict)
                     1372 PRECALL                  0
                     1376 CALL                     0
                     1386 LOAD_FAST                0 (adata)
                     1388 LOAD_ATTR               40 (uns)
                     1398 LOAD_CONST              18 ('decipher')
                     1400 BINARY_SUBSCR
                     1410 LOAD_FAST                5 (uns_key)
                     1412 BINARY_SUBSCR
                     1422 LOAD_FAST                7 (t_name)
                     1424 STORE_SUBSCR
          
-         396        1428 LOAD_GLOBAL             69 (NULL + logging)
+         399        1428 LOAD_GLOBAL             69 (NULL + logging)
                     1440 LOAD_ATTR               35 (info)
                     1450 LOAD_CONST              19 ('Added trajectory ')
                     1452 LOAD_FAST                7 (t_name)
                     1454 FORMAT_VALUE             0
                     1456 LOAD_CONST              20 (" to `adata.uns['decipher']['")
                     1458 LOAD_FAST                5 (uns_key)
                     1460 FORMAT_VALUE             0
@@ -1720,35 +1723,35 @@
                consts
                   0
                   1
                names      ('loc',)
                varnames   ('.0', 'cluster_id')
                freevars   ('cluster_locations',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
                name       '<listcomp>'
                firstlineno 390
                lnotab 0x
             ('point_density', 'rep_key')
             'decipher'
             'Added trajectory '
             " to `adata.uns['decipher']['"
             "']`."
          names      ('create_decipher_uns_key', 'name', 'subset_column', '_subset_cells_and_clusters', 'subset_value', 'subset_percent_per_cluster', 'min_cell_per_cluster', 'pd', 'DataFrame', 'obsm', 'obs', 'values', 'groupby', 'count', 'mean', 'cluster_ids_list', 'nx', 'Graph', 'iterrows', 'add_node', 'np', 'array', 'scipy', 'spatial', 'distance', 'euclidean', 'itertools', 'combinations', 'nodes', 'add_edge', 'minimum_spanning_tree', 'get_start_cluster_id', 'get_end_cluster_id', 'shortest_path', 'logging', 'info', 'astype', 'float32', 'Trajectory', 'to_dict', 'uns')
          varnames   ('adata', 'point_density', 'cluster_key', 'trajectory_configs', 'rep_key', 'uns_key', 't_config', 't_name', 'adata_subset', 'cells_locations', 'valid_clusters', 't_cluster_ids', 'graph', 'i', 'x', 'y', 'distance_func', 'n1', 'n2', 'n1_data', 'n2_data', 'distance', 'tree', 'start_cluster_id', 'end_cluster_id', 't_cluster_locations', 'trajectory')
          freevars   ()
          cellvars   ('cluster_locations',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'trajectories'
          firstlineno 310
          lnotab
             0x0420040104011e020a010e010e010c0102010c010c010c010c0102fa14
             0904023e012a036aff02034e0110020e011202260148015c022c01400134
-            013001320128022a012a022c02360116011aff0e023afe02030c0108ff12
-            0350013ace
+            013001320128022a012a022c02360116011aff0e023afe02030c01020102
+            01020102fc120650013acb
       code
          argcount  : 2
          nlocals   : 10
          stacksize : 6
          flags     : 3
          code
             0x9700640164026c006d017d02010064037d037404000000000000000000
@@ -1766,118 +1769,118 @@
             0a00000000000000007c07a6010000ab0100000000000000006401190000
             000000000000007d097c06a00b0000000000000000000000000000000000
             0000007c006a0c0000000000000000640b190000000000000000007c0919
             000000000000000000a6010000ab0100000000000000007c006a04000000
             00000000006a0d00000000000000007c08640466023c0000008cbb741d00
             0000000000000000006a0f0000000000000000640ca6010000ab01000000
             00000000000100640d5300
-         399           0 RESUME                   0
+         402           0 RESUME                   0
          
-         417           2 LOAD_CONST               1 (0)
+         420           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('KNeighborsRegressor',))
                        6 IMPORT_NAME              0 (sklearn.neighbors)
                        8 IMPORT_FROM              1 (KNeighborsRegressor)
                       10 STORE_FAST               2 (KNeighborsRegressor)
                       12 POP_TOP
          
-         419          14 LOAD_CONST               3 ('decipher_clusters')
+         422          14 LOAD_CONST               3 ('decipher_clusters')
                       16 STORE_FAST               3 (cluster_key)
          
-         420          18 LOAD_GLOBAL              4 (np)
+         423          18 LOAD_GLOBAL              4 (np)
                       30 LOAD_ATTR                3 (nan)
                       40 LOAD_FAST                0 (adata)
                       42 LOAD_ATTR                4 (obs)
                       52 LOAD_CONST               4 ('decipher_time')
                       54 STORE_SUBSCR
          
-         421          58 LOAD_FAST                0 (adata)
+         424          58 LOAD_FAST                0 (adata)
                       60 LOAD_ATTR                5 (uns)
                       70 LOAD_CONST               5 ('decipher')
                       72 BINARY_SUBSCR
                       82 LOAD_CONST               6 ('trajectories')
                       84 BINARY_SUBSCR
                       94 LOAD_METHOD              6 (items)
                      116 PRECALL                  0
                      120 CALL                     0
                      130 GET_ITER
                  >>  132 FOR_ITER               186 (to 506)
                      134 UNPACK_SEQUENCE          2
                      138 STORE_FAST               4 (name)
                      140 STORE_FAST               5 (trajectory)
          
-         422         142 PUSH_NULL
+         425         142 PUSH_NULL
                      144 LOAD_FAST                2 (KNeighborsRegressor)
                      146 LOAD_FAST                1 (n_neighbors)
                      148 KW_NAMES                 7
                      150 PRECALL                  1
                      154 CALL                     1
                      164 STORE_FAST               6 (knn)
          
-         423         166 LOAD_FAST                6 (knn)
+         426         166 LOAD_FAST                6 (knn)
                      168 LOAD_METHOD              7 (fit)
                      190 LOAD_FAST                5 (trajectory)
                      192 LOAD_CONST               8 ('points')
                      194 BINARY_SUBSCR
                      204 LOAD_FAST                5 (trajectory)
                      206 LOAD_CONST               9 ('times')
                      208 BINARY_SUBSCR
                      218 PRECALL                  2
                      222 CALL                     2
                      232 POP_TOP
          
-         424         234 LOAD_FAST                0 (adata)
+         427         234 LOAD_FAST                0 (adata)
                      236 LOAD_ATTR                4 (obs)
                      246 LOAD_FAST                3 (cluster_key)
                      248 BINARY_SUBSCR
                      258 LOAD_METHOD              8 (isin)
                      280 LOAD_FAST                5 (trajectory)
                      282 LOAD_CONST              10 ('cluster_ids')
                      284 BINARY_SUBSCR
                      294 PRECALL                  1
                      298 CALL                     1
                      308 STORE_FAST               7 (is_on_trajectory)
          
-         425         310 LOAD_FAST                0 (adata)
+         428         310 LOAD_FAST                0 (adata)
                      312 LOAD_ATTR                4 (obs)
                      322 LOAD_FAST                7 (is_on_trajectory)
                      324 BINARY_SUBSCR
                      334 LOAD_ATTR                9 (index)
                      344 STORE_FAST               8 (cells_on_trajectory_index)
          
-         426         346 LOAD_GLOBAL              5 (NULL + np)
+         429         346 LOAD_GLOBAL              5 (NULL + np)
                      358 LOAD_ATTR               10 (where)
                      368 LOAD_FAST                7 (is_on_trajectory)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 LOAD_CONST               1 (0)
                      386 BINARY_SUBSCR
                      396 STORE_FAST               9 (cells_on_trajectory_idx)
          
-         428         398 LOAD_FAST                6 (knn)
+         431         398 LOAD_FAST                6 (knn)
                      400 LOAD_METHOD             11 (predict)
          
-         429         422 LOAD_FAST                0 (adata)
+         432         422 LOAD_FAST                0 (adata)
                      424 LOAD_ATTR               12 (obsm)
                      434 LOAD_CONST              11 ('decipher_v')
                      436 BINARY_SUBSCR
                      446 LOAD_FAST                9 (cells_on_trajectory_idx)
                      448 BINARY_SUBSCR
          
-         428         458 PRECALL                  1
+         431         458 PRECALL                  1
                      462 CALL                     1
                      472 LOAD_FAST                0 (adata)
                      474 LOAD_ATTR                4 (obs)
                      484 LOAD_ATTR               13 (loc)
                      494 LOAD_FAST                8 (cells_on_trajectory_index)
                      496 LOAD_CONST               4 ('decipher_time')
                      498 BUILD_TUPLE              2
                      500 STORE_SUBSCR
                      504 JUMP_BACKWARD          187 (to 132)
          
-         432     >>  506 LOAD_GLOBAL             29 (NULL + logging)
+         435     >>  506 LOAD_GLOBAL             29 (NULL + logging)
                      518 LOAD_ATTR               15 (info)
                      528 LOAD_CONST              12 ("Added `.obs['decipher_time']`: the decipher time of each cell.")
                      530 PRECALL                  1
                      534 CALL                     1
                      544 POP_TOP
                      546 LOAD_CONST              13 (None)
                      548 RETURN_VALUE
@@ -1896,17 +1899,17 @@
             'decipher_v'
             "Added `.obs['decipher_time']`: the decipher time of each cell."
             None
          names      ('sklearn.neighbors', 'KNeighborsRegressor', 'np', 'nan', 'obs', 'uns', 'items', 'fit', 'isin', 'index', 'where', 'predict', 'obsm', 'loc', 'logging', 'info')
          varnames   ('adata', 'n_neighbors', 'KNeighborsRegressor', 'cluster_key', 'name', 'trajectory', 'knn', 'is_on_trajectory', 'cells_on_trajectory_index', 'cells_on_trajectory_idx')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'decipher_time'
-         firstlineno 399
+         firstlineno 402
          lnotab 0x02120c02040128015401180144014c0124013402180124ff3004
       10000
       100
       code
          argcount  : 3
          nlocals   : 13
          stacksize : 6
@@ -1953,147 +1956,147 @@
             00ab0300000000000000007c0b640e3c0000007407000000000000000000
             006a1300000000000000007c0c640f640cac0da6030000ab030000000000
             0000007c0b64103c0000007c0ca014000000000000000000000000000000
             0000000000640cac0da6010000ab0100000000000000007c0b64113c0000
             0069007c0ba50164057c076901a5017c006a010000000000000000640219
             0000000000000000007c03190000000000000000007c053c00000090028c
             4464125300
-         435           0 RESUME                   0
+         438           0 RESUME                   0
          
-         461           2 LOAD_CONST               1 ('gene_patterns')
+         464           2 LOAD_CONST               1 ('gene_patterns')
                        4 STORE_FAST               3 (uns_decipher_key)
          
-         462           6 LOAD_GLOBAL              1 (NULL + decipher_load_model)
+         465           6 LOAD_GLOBAL              1 (NULL + decipher_load_model)
                       18 LOAD_FAST                0 (adata)
                       20 PRECALL                  1
                       24 CALL                     1
                       34 STORE_FAST               4 (model)
          
-         463          36 LOAD_FAST                3 (uns_decipher_key)
+         466          36 LOAD_FAST                3 (uns_decipher_key)
                       38 LOAD_FAST                0 (adata)
                       40 LOAD_ATTR                1 (uns)
                       50 LOAD_CONST               2 ('decipher')
                       52 BINARY_SUBSCR
                       62 CONTAINS_OP              1
                       64 POP_JUMP_FORWARD_IF_FALSE    28 (to 122)
          
-         464          66 LOAD_GLOBAL              5 (NULL + dict)
+         467          66 LOAD_GLOBAL              5 (NULL + dict)
                       78 PRECALL                  0
                       82 CALL                     0
                       92 LOAD_FAST                0 (adata)
                       94 LOAD_ATTR                1 (uns)
                      104 LOAD_CONST               2 ('decipher')
                      106 BINARY_SUBSCR
                      116 LOAD_FAST                3 (uns_decipher_key)
                      118 STORE_SUBSCR
          
-         466     >>  122 LOAD_FAST                0 (adata)
+         469     >>  122 LOAD_FAST                0 (adata)
                      124 LOAD_ATTR                1 (uns)
                      134 LOAD_CONST               2 ('decipher')
                      136 BINARY_SUBSCR
                      146 LOAD_CONST               3 ('trajectories')
                      148 BINARY_SUBSCR
                      158 GET_ITER
                  >>  160 EXTENDED_ARG             2
                      162 FOR_ITER               578 (to 1320)
                      164 STORE_FAST               5 (t_name)
          
-         467         166 LOAD_FAST                0 (adata)
+         470         166 LOAD_FAST                0 (adata)
                      168 LOAD_ATTR                1 (uns)
                      178 LOAD_CONST               2 ('decipher')
                      180 BINARY_SUBSCR
                      190 LOAD_CONST               3 ('trajectories')
                      192 BINARY_SUBSCR
                      202 LOAD_FAST                5 (t_name)
                      204 BINARY_SUBSCR
                      214 LOAD_CONST               4 ('points')
                      216 BINARY_SUBSCR
                      226 STORE_FAST               6 (t_points)
          
-         468         228 LOAD_FAST                0 (adata)
+         471         228 LOAD_FAST                0 (adata)
                      230 LOAD_ATTR                1 (uns)
                      240 LOAD_CONST               2 ('decipher')
                      242 BINARY_SUBSCR
                      252 LOAD_CONST               3 ('trajectories')
                      254 BINARY_SUBSCR
                      264 LOAD_FAST                5 (t_name)
                      266 BINARY_SUBSCR
                      276 LOAD_CONST               5 ('times')
                      278 BINARY_SUBSCR
                      288 STORE_FAST               7 (t_times)
          
-         470         290 LOAD_CONST               6 ('rotation')
+         473         290 LOAD_CONST               6 ('rotation')
                      292 LOAD_FAST                0 (adata)
                      294 LOAD_ATTR                1 (uns)
                      304 LOAD_CONST               2 ('decipher')
                      306 BINARY_SUBSCR
                      316 CONTAINS_OP              0
                      318 POP_JUMP_FORWARD_IF_FALSE    51 (to 422)
          
-         472         320 LOAD_FAST                6 (t_points)
+         475         320 LOAD_FAST                6 (t_points)
                      322 LOAD_GLOBAL              6 (np)
                      334 LOAD_ATTR                4 (linalg)
                      344 LOAD_METHOD              5 (inv)
                      366 LOAD_FAST                0 (adata)
                      368 LOAD_ATTR                1 (uns)
                      378 LOAD_CONST               2 ('decipher')
                      380 BINARY_SUBSCR
                      390 LOAD_CONST               6 ('rotation')
                      392 BINARY_SUBSCR
                      402 PRECALL                  1
                      406 CALL                     1
                      416 BINARY_OP                4 (@)
                      420 STORE_FAST               6 (t_points)
          
-         474     >>  422 LOAD_GLOBAL             13 (NULL + torch)
+         477     >>  422 LOAD_GLOBAL             13 (NULL + torch)
                      434 LOAD_ATTR                7 (FloatTensor)
                      444 LOAD_FAST                6 (t_points)
                      446 PRECALL                  1
                      450 CALL                     1
                      460 STORE_FAST               6 (t_points)
          
-         475         462 LOAD_FAST                4 (model)
+         478         462 LOAD_FAST                4 (model)
                      464 LOAD_METHOD              8 (decoder_v_to_z)
                      486 LOAD_FAST                6 (t_points)
                      488 PRECALL                  1
                      492 CALL                     1
                      502 UNPACK_SEQUENCE          2
                      506 STORE_FAST               8 (z_mean)
                      508 STORE_FAST               9 (z_scale)
          
-         476         510 LOAD_GLOBAL             12 (torch)
+         479         510 LOAD_GLOBAL             12 (torch)
                      522 LOAD_ATTR                9 (nn)
                      532 LOAD_ATTR               10 (functional)
                      542 LOAD_METHOD             11 (softplus)
                      564 LOAD_FAST                9 (z_scale)
                      566 PRECALL                  1
                      570 CALL                     1
                      580 STORE_FAST               9 (z_scale)
          
-         478         582 LOAD_GLOBAL             12 (torch)
+         481         582 LOAD_GLOBAL             12 (torch)
                      594 LOAD_ATTR               12 (distributions)
                      604 LOAD_METHOD             13 (Normal)
                      626 LOAD_FAST                8 (z_mean)
                      628 LOAD_FAST                9 (z_scale)
                      630 PRECALL                  2
                      634 CALL                     2
                      644 LOAD_METHOD             14 (sample)
                      666 LOAD_FAST                2 (n_samples)
                      668 BUILD_TUPLE              1
                      670 KW_NAMES                 7
                      672 PRECALL                  1
                      676 CALL                     1
                      686 STORE_FAST              10 (z_samples)
          
-         480         688 LOAD_GLOBAL              5 (NULL + dict)
+         483         688 LOAD_GLOBAL              5 (NULL + dict)
                      700 PRECALL                  0
                      704 CALL                     0
                      714 STORE_FAST              11 (gene_patterns)
          
-         482         716 LOAD_GLOBAL             12 (torch)
+         485         716 LOAD_GLOBAL             12 (torch)
                      728 LOAD_ATTR                9 (nn)
                      738 LOAD_ATTR               10 (functional)
                      748 LOAD_METHOD             15 (softmax)
                      770 LOAD_FAST                4 (model)
                      772 LOAD_METHOD             16 (decoder_z_to_x)
                      794 LOAD_FAST                8 (z_mean)
                      796 PRECALL                  1
@@ -2105,23 +2108,23 @@
                      828 LOAD_METHOD             17 (detach)
                      850 PRECALL                  0
                      854 CALL                     0
                      864 LOAD_METHOD             18 (numpy)
                      886 PRECALL                  0
                      890 CALL                     0
          
-         483         900 LOAD_FAST                1 (l_scale)
+         486         900 LOAD_FAST                1 (l_scale)
          
-         482         902 BINARY_OP                5 (*)
+         485         902 BINARY_OP                5 (*)
          
-         481         906 LOAD_FAST               11 (gene_patterns)
+         484         906 LOAD_FAST               11 (gene_patterns)
                      908 LOAD_CONST              10 ('mean')
                      910 STORE_SUBSCR
          
-         487         914 LOAD_GLOBAL             12 (torch)
+         490         914 LOAD_GLOBAL             12 (torch)
                      926 LOAD_ATTR                9 (nn)
                      936 LOAD_ATTR               10 (functional)
                      946 LOAD_METHOD             15 (softmax)
                      968 LOAD_FAST                4 (model)
                      970 LOAD_METHOD             16 (decoder_z_to_x)
                      992 LOAD_FAST               10 (z_samples)
                      994 PRECALL                  1
@@ -2133,77 +2136,77 @@
                     1026 LOAD_METHOD             17 (detach)
                     1048 PRECALL                  0
                     1052 CALL                     0
                     1062 LOAD_METHOD             18 (numpy)
                     1084 PRECALL                  0
                     1088 CALL                     0
          
-         488        1098 LOAD_FAST                1 (l_scale)
+         491        1098 LOAD_FAST                1 (l_scale)
          
-         487        1100 BINARY_OP                5 (*)
+         490        1100 BINARY_OP                5 (*)
          
-         486        1104 STORE_FAST              12 (gene_expression_samples)
+         489        1104 STORE_FAST              12 (gene_expression_samples)
          
-         490        1106 LOAD_GLOBAL              7 (NULL + np)
+         493        1106 LOAD_GLOBAL              7 (NULL + np)
                     1118 LOAD_ATTR               19 (quantile)
                     1128 LOAD_FAST               12 (gene_expression_samples)
                     1130 LOAD_CONST              11 (0.25)
                     1132 LOAD_CONST              12 (0)
                     1134 KW_NAMES                13
                     1136 PRECALL                  3
                     1140 CALL                     3
                     1150 LOAD_FAST               11 (gene_patterns)
                     1152 LOAD_CONST              14 ('q25')
                     1154 STORE_SUBSCR
          
-         491        1158 LOAD_GLOBAL              7 (NULL + np)
+         494        1158 LOAD_GLOBAL              7 (NULL + np)
                     1170 LOAD_ATTR               19 (quantile)
                     1180 LOAD_FAST               12 (gene_expression_samples)
                     1182 LOAD_CONST              15 (0.75)
                     1184 LOAD_CONST              12 (0)
                     1186 KW_NAMES                13
                     1188 PRECALL                  3
                     1192 CALL                     3
                     1202 LOAD_FAST               11 (gene_patterns)
                     1204 LOAD_CONST              16 ('q75')
                     1206 STORE_SUBSCR
          
-         494        1210 LOAD_FAST               12 (gene_expression_samples)
+         497        1210 LOAD_FAST               12 (gene_expression_samples)
                     1212 LOAD_METHOD             20 (mean)
                     1234 LOAD_CONST              12 (0)
                     1236 KW_NAMES                13
                     1238 PRECALL                  1
                     1242 CALL                     1
                     1252 LOAD_FAST               11 (gene_patterns)
                     1254 LOAD_CONST              17 ('mean2')
                     1256 STORE_SUBSCR
          
-         496        1260 BUILD_MAP                0
+         499        1260 BUILD_MAP                0
          
-         497        1262 LOAD_FAST               11 (gene_patterns)
+         500        1262 LOAD_FAST               11 (gene_patterns)
          
-         496        1264 DICT_UPDATE              1
+         499        1264 DICT_UPDATE              1
          
-         498        1266 LOAD_CONST               5 ('times')
+         501        1266 LOAD_CONST               5 ('times')
                     1268 LOAD_FAST                7 (t_times)
          
-         496        1270 BUILD_MAP                1
+         499        1270 BUILD_MAP                1
                     1272 DICT_UPDATE              1
                     1274 LOAD_FAST                0 (adata)
                     1276 LOAD_ATTR                1 (uns)
                     1286 LOAD_CONST               2 ('decipher')
                     1288 BINARY_SUBSCR
                     1298 LOAD_FAST                3 (uns_decipher_key)
                     1300 BINARY_SUBSCR
                     1310 LOAD_FAST                5 (t_name)
                     1312 STORE_SUBSCR
                     1316 EXTENDED_ARG             2
                     1318 JUMP_BACKWARD          580 (to 160)
          
-         466     >> 1320 LOAD_CONST              18 (None)
+         469     >> 1320 LOAD_CONST              18 (None)
                     1322 RETURN_VALUE
          consts
             'Compute the gene patterns for each trajectory.\n\n    The trajectories\' points are sent through the decoders, thus defining distributions over the\n    gene expression. The gene patterns are computed by sampling from these distribution.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix. The trajectories should have been computed and stored in\n        `adata.uns["decipher"]["trajectories"]`.\n    l_scale : float\n        The library size scaling factor.\n    n_samples : int\n        The number of samples to draw from the decoder to compute the gene pattern statistics.\n\n    Returns\n    -------\n    `adata.uns["decipher"]["gene_patterns"]`: dict\n        The gene patterns for each trajectory.\n        - trajectory_name: dict\n            - `mean`: the mean gene expression pattern\n            - `q25`: the 25% quantile of the gene expression pattern\n            - `q75`: the 75% quantile of the gene expression pattern\n            - `times`: the times of the trajectory\n    '
             'gene_patterns'
             'decipher'
             'trajectories'
             'points'
@@ -2221,30 +2224,30 @@
             'q75'
             'mean2'
             None
          names      ('decipher_load_model', 'uns', 'dict', 'np', 'linalg', 'inv', 'torch', 'FloatTensor', 'decoder_v_to_z', 'nn', 'functional', 'softplus', 'distributions', 'Normal', 'sample', 'softmax', 'decoder_z_to_x', 'detach', 'numpy', 'quantile', 'mean')
          varnames   ('adata', 'l_scale', 'n_samples', 'uns_decipher_key', 'model', 't_name', 't_points', 't_times', 'z_mean', 'z_scale', 'z_samples', 'gene_patterns', 'gene_expression_samples')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
          name       'gene_patterns'
-         firstlineno 435
+         firstlineno 438
          lnotab
             0x021a04011e011e0138022c013e013e021e0266022801300148026a021c
             02b80102ff04ff0806b80102ff04ff0204340134033202020102ff020204
             fe32e2
       (1.0, 10, 0, 'decipher_z')
       (0.3, 10, 'decipher_clusters')
       (None, None, 0.3, 'decipher_clusters', 10)
       (10,)
       (10000, 100)
    names      ('itertools', 'logging', 'networkx', 'nx', 'numpy', 'np', 'pandas', 'pd', 'scanpy', 'sc', 'scipy.spatial', 'scipy', 'torch.nn.functional', 'torch', 'decipher.tools._decipher.data', 'decipher_load_model', 'decipher.utils', 'create_decipher_uns_key', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'Trajectory', 'TConfig', 'cell_clusters', '_subset_cells_and_clusters', 'find_cluster_with_marker', 'trajectories', 'decipher_time', 'gene_patterns')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/trajectory_inference.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/trajectory_inference.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080108020801080108010801080108020c010c0220010e0102
       010cfe12061a471a5a083b0201020102fa081d020102010201020102f908
-      32020102fc0a590824
+      32020102fc0a5c0824
```

### Comparing `scdecipher-0.1.0/decipher/tools/__pycache__/utils.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/__pycache__/utils.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
+moddate:  0x7d19d665 (Wed Feb 21 15:40:45 2024 UTC)
 files sz: 1282
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
@@ -14,15 +14,15 @@
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (numpy)
                  8 STORE_NAME               1 (np)
    
      4          10 PUSH_NULL
                 12 LOAD_BUILD_CLASS
-                14 LOAD_CONST               2 (<code object EarlyStopping, file "/Users/achille/Documents/decipher-pip/decipher/tools/utils.py", line 4>)
+                14 LOAD_CONST               2 (<code object EarlyStopping, file "/Users/achille/Documents/decipher_dev/decipher/tools/utils.py", line 4>)
                 16 MAKE_FUNCTION            0
                 18 LOAD_CONST               3 ('EarlyStopping')
                 20 PRECALL                  2
                 24 CALL                     2
                 34 STORE_NAME               2 (EarlyStopping)
                 36 LOAD_CONST               1 (None)
                 38 RETURN_VALUE
@@ -43,23 +43,23 @@
                        6 LOAD_CONST               0 ('EarlyStopping')
                        8 STORE_NAME               2 (__qualname__)
          
            5          10 LOAD_CONST               1 ('Keeps track of when the loss does not improve after a given patience.\n\n    Useful to stop training when the validation loss does not improve anymore.\n\n    Parameters\n    ----------\n    patience : int\n        How long to wait after the last validation loss improvement.\n\n    Examples\n    --------\n    >>> n_epochs = 100\n    >>> early_stopping = EarlyStopping(patience=5)\n    >>> for epoch in range(n_epochs):\n    >>>     # train\n    >>>     validation_loss = ...\n    >>>     if early_stopping(validation_loss):\n    >>>         break\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           25          14 LOAD_CONST               7 ((5,))
-                      16 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/utils.py", line 25>)
+                      16 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/utils.py", line 25>)
                       18 MAKE_FUNCTION            1 (defaults)
                       20 STORE_NAME               4 (__init__)
          
-          31          22 LOAD_CONST               4 (<code object __call__, file "/Users/achille/Documents/decipher-pip/decipher/tools/utils.py", line 31>)
+          31          22 LOAD_CONST               4 (<code object __call__, file "/Users/achille/Documents/decipher_dev/decipher/tools/utils.py", line 31>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (__call__)
          
-          43          28 LOAD_CONST               5 (<code object has_stopped, file "/Users/achille/Documents/decipher-pip/decipher/tools/utils.py", line 43>)
+          43          28 LOAD_CONST               5 (<code object has_stopped, file "/Users/achille/Documents/decipher_dev/decipher/tools/utils.py", line 43>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (has_stopped)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'EarlyStopping'
             'Keeps track of when the loss does not improve after a given patience.\n\n    Useful to stop training when the validation loss does not improve anymore.\n\n    Parameters\n    ----------\n    patience : int\n        How long to wait after the last validation loss improvement.\n\n    Examples\n    --------\n    >>> n_epochs = 100\n    >>> early_stopping = EarlyStopping(patience=5)\n    >>> for epoch in range(n_epochs):\n    >>>     # train\n    >>>     validation_loss = ...\n    >>>     if early_stopping(validation_loss):\n    >>>         break\n    '
@@ -97,15 +97,15 @@
                   None
                   0
                   False
                names      ('patience', 'counter', 'early_stop', 'np', 'inf', 'validation_loss_min')
                varnames   ('self', 'patience')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/utils.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/utils.py'
                name       '__init__'
                firstlineno 25
                lnotab 0x02010e010e010e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -160,15 +160,15 @@
                   0
                   1
                   True
                names      ('validation_loss_min', 'counter', 'patience', 'early_stop')
                varnames   ('self', 'validation_loss')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/utils.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/utils.py'
                name       '__call__'
                firstlineno 31
                lnotab 0x020216010e011002200120010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
@@ -181,30 +181,30 @@
                             14 RETURN_VALUE
                consts
                   'Returns True if the stopping condition has been met.'
                names      ('early_stop',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/utils.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/utils.py'
                name       'has_stopped'
                firstlineno 43
                lnotab 0x0202
             None
             (5,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '__call__', 'has_stopped')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/utils.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/utils.py'
          name       'EarlyStopping'
          firstlineno 4
          lnotab 0x0a0104140806060c
       'EarlyStopping'
    names      ('numpy', 'np', 'EarlyStopping')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/utils.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/utils.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010803
```

### Comparing `scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/inference.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/inference.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
+moddate:  0x2d222166 (Thu Apr 18 13:37:49 2024 UTC)
 files sz: 1456
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -22,23 +22,23 @@
      3          14 LOAD_CONST               0 (0)
                 16 LOAD_CONST               2 (None)
                 18 IMPORT_NAME              2 (pyro)
                 20 STORE_NAME               2 (pyro)
    
      6          22 PUSH_NULL
                 24 LOAD_BUILD_CLASS
-                26 LOAD_CONST               3 (<code object InferenceMode, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/inference.py", line 6>)
+                26 LOAD_CONST               3 (<code object InferenceMode, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/inference.py", line 6>)
                 28 MAKE_FUNCTION            0
                 30 LOAD_CONST               4 ('InferenceMode')
                 32 LOAD_NAME                1 (Enum)
                 34 PRECALL                  3
                 38 CALL                     3
                 48 STORE_NAME               3 (InferenceMode)
    
-    13          50 LOAD_CONST               5 (<code object get_inference_guide, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/inference.py", line 13>)
+    13          50 LOAD_CONST               5 (<code object get_inference_guide, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/inference.py", line 13>)
                 52 MAKE_FUNCTION            0
                 54 STORE_NAME               4 (get_inference_guide)
                 56 LOAD_CONST               2 (None)
                 58 RETURN_VALUE
    consts
       0
       ('Enum',)
@@ -77,15 +77,15 @@
             2
             3
             None
          names      ('__name__', '__module__', '__qualname__', 'POINT_ESTIMATE', 'GAUSSIAN', 'GAUSSIAN_BETA_ONLY', 'GAUSSIAN_BASIS_ONLY')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/inference.py'
          name       'InferenceMode'
          firstlineno 6
          lnotab 0x0a01040104010401
       'InferenceMode'
       code
          argcount  : 2
          nlocals   : 3
@@ -304,21 +304,21 @@
             ('expose',)
             0.2
             ('init_scale',)
          names      ('InferenceMode', 'GAUSSIAN', 'pyro', 'infer', 'autoguide', 'AutoNormal', 'GAUSSIAN_BETA_ONLY', 'AutoGuideList', 'append', 'AutoDelta', 'poutine', 'block', 'GAUSSIAN_BASIS_ONLY', 'POINT_ESTIMATE')
          varnames   ('model', 'inference_mode', 'guide')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/inference.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/inference.py'
          name       'get_inference_guide'
          firstlineno 13
          lnotab
             0x020320014c03200148011801360142ff0eff10051801360144ff10ff14
             07200148011801360142ff0eff1005b00320014802
    names      ('enum', 'Enum', 'pyro', 'InferenceMode', 'get_inference_guide')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/inference.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/inference.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0208031c07
```

### Comparing `scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/model.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/model.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,21 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 4219
+moddate:  0xa2222166 (Thu Apr 18 13:39:46 2024 UTC)
+files sz: 4184
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064016c025a03640064016c045a04640064
-      016c056d065a070100640064016c085a08640064026c096d0a5a0a010002
-      00470064038400640465046a0b00000000000000006a0a00000000000000
-      00a6030000ab0300000000000000005a0c0200470064058400640665086a
-      0b00000000000000006a0d0000000000000000a6030000ab030000000000
-      0000005a0e64015300
+      016c056d065a070100640064016c085a080200470064028400640365046a
+      0900000000000000006a0a0000000000000000a6030000ab030000000000
+      0000005a0b0200470064048400640565086a0900000000000000006a0c00
+      00000000000000a6030000ab0300000000000000005a0d64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (numpy)
                  8 STORE_NAME               1 (np)
    
@@ -38,76 +37,68 @@
                 36 POP_TOP
    
      5          38 LOAD_CONST               0 (0)
                 40 LOAD_CONST               1 (None)
                 42 IMPORT_NAME              8 (torch)
                 44 STORE_NAME               8 (torch)
    
-     6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               2 (('PyroModule',))
-                50 IMPORT_NAME              9 (pyro.nn)
-                52 IMPORT_FROM             10 (PyroModule)
-                54 STORE_NAME              10 (PyroModule)
-                56 POP_TOP
+     8          46 PUSH_NULL
+                48 LOAD_BUILD_CLASS
+                50 LOAD_CONST               2 (<code object RealFunction, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 8>)
+                52 MAKE_FUNCTION            0
+                54 LOAD_CONST               3 ('RealFunction')
+                56 LOAD_NAME                4 (pyro)
+                58 LOAD_ATTR                9 (nn)
+                68 LOAD_ATTR               10 (PyroModule)
+                78 PRECALL                  3
+                82 CALL                     3
+                92 STORE_NAME              11 (RealFunction)
    
-     9          58 PUSH_NULL
-                60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               3 (<code object RealFunction, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 9>)
-                64 MAKE_FUNCTION            0
-                66 LOAD_CONST               4 ('RealFunction')
-                68 LOAD_NAME                4 (pyro)
-                70 LOAD_ATTR               11 (nn)
-                80 LOAD_ATTR               10 (PyroModule)
-                90 PRECALL                  3
-                94 CALL                     3
-               104 STORE_NAME              12 (RealFunction)
-   
-    48         106 PUSH_NULL
-               108 LOAD_BUILD_CLASS
-               110 LOAD_CONST               5 (<code object BasisDecomposition, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 48>)
-               112 MAKE_FUNCTION            0
-               114 LOAD_CONST               6 ('BasisDecomposition')
-               116 LOAD_NAME                8 (torch)
-               118 LOAD_ATTR               11 (nn)
-               128 LOAD_ATTR               13 (Module)
-               138 PRECALL                  3
-               142 CALL                     3
-               152 STORE_NAME              14 (BasisDecomposition)
-               154 LOAD_CONST               1 (None)
-               156 RETURN_VALUE
+    47          94 PUSH_NULL
+                96 LOAD_BUILD_CLASS
+                98 LOAD_CONST               4 (<code object BasisDecomposition, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 47>)
+               100 MAKE_FUNCTION            0
+               102 LOAD_CONST               5 ('BasisDecomposition')
+               104 LOAD_NAME                8 (torch)
+               106 LOAD_ATTR                9 (nn)
+               116 LOAD_ATTR               12 (Module)
+               126 PRECALL                  3
+               130 CALL                     3
+               140 STORE_NAME              13 (BasisDecomposition)
+               142 LOAD_CONST               1 (None)
+               144 RETURN_VALUE
    consts
       0
       None
-      ('PyroModule',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a02640164029c01880066016403840a5a0364
             0484005a04880078015a055300
                        0 MAKE_CELL                0 (__class__)
          
-           9           2 RESUME                   0
+           8           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('RealFunction')
                       10 STORE_NAME               2 (__qualname__)
          
-          10          12 LOAD_CONST               1 (False)
+           9          12 LOAD_CONST               1 (False)
                       14 LOAD_CONST               2 (('sigmoid_output',))
                       16 BUILD_CONST_KEY_MAP      1
                       18 LOAD_CLOSURE             0 (__class__)
                       20 BUILD_TUPLE              1
-                      22 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 10>)
+                      22 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 9>)
                       24 MAKE_FUNCTION           10 (kwdefaults, closure)
                       26 STORE_NAME               3 (__init__)
          
-          35          28 LOAD_CONST               4 (<code object forward, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 35>)
+          34          28 LOAD_CONST               4 (<code object forward, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 34>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               4 (forward)
                       34 LOAD_CLOSURE             0 (__class__)
                       36 COPY                     1
                       38 STORE_NAME               5 (__classcell__)
                       40 RETURN_VALUE
          consts
@@ -152,42 +143,42 @@
                   00000000007c0064067c089b009d027c047c0819000000000000000000a6
                   030000ab03000000000000000001008c1d7410000000000000000000006a
                   060000000000000000a01700000000000000000000000000000000000000
                   00a6000000ab0000000000000000007c005f180000000000000000640053
                   00
                              0 COPY_FREE_VARS           1
                
-                10           2 RESUME                   0
+                 9           2 RESUME                   0
                
-                11           4 LOAD_GLOBAL              1 (NULL + super)
+                10           4 LOAD_GLOBAL              1 (NULL + super)
                             16 LOAD_GLOBAL              2 (RealFunction)
                             28 LOAD_FAST                0 (self)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 LOAD_METHOD              2 (__init__)
                             66 PRECALL                  0
                             70 CALL                     0
                             80 POP_TOP
                
-                12          82 LOAD_CONST               1 (1)
+                11          82 LOAD_CONST               1 (1)
                             84 BUILD_LIST               1
                             86 LOAD_FAST                2 (hidden_dims)
                             88 LIST_EXTEND              1
                             90 LOAD_CONST               1 (1)
                             92 LIST_APPEND              1
                             94 STORE_FAST               3 (dimensions)
                
-                13          96 LOAD_FAST                1 (sigmoid_output)
+                12          96 LOAD_FAST                1 (sigmoid_output)
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (sigmoid_output)
                
-                14         110 BUILD_LIST               0
+                13         110 BUILD_LIST               0
                            112 STORE_FAST               4 (layers)
                
-                15         114 LOAD_GLOBAL              9 (NULL + zip)
+                14         114 LOAD_GLOBAL              9 (NULL + zip)
                            126 LOAD_FAST                3 (dimensions)
                            128 LOAD_FAST                3 (dimensions)
                            130 LOAD_CONST               1 (1)
                            132 LOAD_CONST               0 (None)
                            134 BUILD_SLICE              2
                            136 BINARY_SUBSCR
                            146 PRECALL                  2
@@ -195,137 +186,137 @@
                            160 GET_ITER
                        >>  162 EXTENDED_ARG             1
                            164 FOR_ITER               311 (to 788)
                            166 UNPACK_SEQUENCE          2
                            170 STORE_FAST               5 (in_features)
                            172 STORE_FAST               6 (out_features)
                
-                16         174 LOAD_GLOBAL             11 (NULL + pyro)
+                15         174 LOAD_GLOBAL             11 (NULL + pyro)
                            186 LOAD_ATTR                6 (nn)
                            196 LOAD_ATTR                7 (PyroModule)
                            206 LOAD_GLOBAL             16 (torch)
                            218 LOAD_ATTR                6 (nn)
                            228 LOAD_ATTR                9 (Linear)
                            238 BINARY_SUBSCR
                            248 LOAD_FAST                5 (in_features)
                            250 LOAD_FAST                6 (out_features)
                            252 PRECALL                  2
                            256 CALL                     2
                            266 STORE_FAST               7 (layer)
                
-                17         268 LOAD_GLOBAL             10 (pyro)
+                16         268 LOAD_GLOBAL             10 (pyro)
                            280 LOAD_ATTR                6 (nn)
                            290 LOAD_METHOD             10 (PyroSample)
                
-                18         312 LOAD_GLOBAL             23 (NULL + dist)
+                17         312 LOAD_GLOBAL             23 (NULL + dist)
                            324 LOAD_ATTR               12 (Normal)
                            334 LOAD_CONST               2 (0.0)
                            336 LOAD_CONST               3 (1.0)
                            338 LOAD_FAST                5 (in_features)
                            340 LOAD_CONST               4 (0.5)
                            342 BINARY_OP                8 (**)
                            346 BINARY_OP               11 (/)
                            350 PRECALL                  2
                            354 CALL                     2
                
-                19         364 LOAD_METHOD             13 (expand)
+                18         364 LOAD_METHOD             13 (expand)
                            386 LOAD_GLOBAL             17 (NULL + torch)
                            398 LOAD_ATTR               14 (Size)
                            408 LOAD_FAST                6 (out_features)
                            410 LOAD_FAST                5 (in_features)
                            412 BUILD_LIST               2
                            414 PRECALL                  1
                            418 CALL                     1
                            428 PRECALL                  1
                            432 CALL                     1
                
-                20         442 LOAD_METHOD             15 (to_event)
+                19         442 LOAD_METHOD             15 (to_event)
                            464 LOAD_CONST               5 (2)
                            466 PRECALL                  1
                            470 CALL                     1
                
-                17         480 PRECALL                  1
+                16         480 PRECALL                  1
                            484 CALL                     1
                            494 LOAD_FAST                7 (layer)
                            496 STORE_ATTR              16 (weight)
                
-                22         506 LOAD_GLOBAL             10 (pyro)
+                21         506 LOAD_GLOBAL             10 (pyro)
                            518 LOAD_ATTR                6 (nn)
                            528 LOAD_METHOD             10 (PyroSample)
                
-                23         550 LOAD_GLOBAL             23 (NULL + dist)
+                22         550 LOAD_GLOBAL             23 (NULL + dist)
                            562 LOAD_ATTR               12 (Normal)
                            572 LOAD_CONST               2 (0.0)
                            574 LOAD_CONST               3 (1.0)
                            576 LOAD_FAST                5 (in_features)
                            578 LOAD_CONST               4 (0.5)
                            580 BINARY_OP                8 (**)
                            584 BINARY_OP               11 (/)
                            588 PRECALL                  2
                            592 CALL                     2
                
-                24         602 LOAD_METHOD             13 (expand)
+                23         602 LOAD_METHOD             13 (expand)
                            624 LOAD_GLOBAL             17 (NULL + torch)
                            636 LOAD_ATTR               14 (Size)
                            646 LOAD_FAST                6 (out_features)
                            648 BUILD_LIST               1
                            650 PRECALL                  1
                            654 CALL                     1
                            664 PRECALL                  1
                            668 CALL                     1
                
-                25         678 LOAD_METHOD             15 (to_event)
+                24         678 LOAD_METHOD             15 (to_event)
                            700 LOAD_CONST               1 (1)
                            702 PRECALL                  1
                            706 CALL                     1
                
-                22         716 PRECALL                  1
+                21         716 PRECALL                  1
                            720 CALL                     1
                            730 LOAD_FAST                7 (layer)
                            732 STORE_ATTR              17 (bias)
                
-                27         742 LOAD_FAST                4 (layers)
+                26         742 LOAD_FAST                4 (layers)
                            744 LOAD_METHOD             18 (append)
                            766 LOAD_FAST                7 (layer)
                            768 PRECALL                  1
                            772 CALL                     1
                            782 POP_TOP
                            784 EXTENDED_ARG             1
                            786 JUMP_BACKWARD          313 (to 162)
                
-                29     >>  788 LOAD_FAST                4 (layers)
+                28     >>  788 LOAD_FAST                4 (layers)
                            790 LOAD_FAST                0 (self)
                            792 STORE_ATTR              19 (layers)
                
-                30         802 LOAD_GLOBAL             41 (NULL + range)
+                29         802 LOAD_GLOBAL             41 (NULL + range)
                            814 LOAD_GLOBAL             43 (NULL + len)
                            826 LOAD_FAST                4 (layers)
                            828 PRECALL                  1
                            832 CALL                     1
                            842 PRECALL                  1
                            846 CALL                     1
                            856 GET_ITER
                        >>  858 FOR_ITER                28 (to 916)
                            860 STORE_FAST               8 (i)
                
-                31         862 LOAD_GLOBAL             45 (NULL + setattr)
+                30         862 LOAD_GLOBAL             45 (NULL + setattr)
                            874 LOAD_FAST                0 (self)
                            876 LOAD_CONST               6 ('layer_')
                            878 LOAD_FAST                8 (i)
                            880 FORMAT_VALUE             0
                            882 BUILD_STRING             2
                            884 LOAD_FAST                4 (layers)
                            886 LOAD_FAST                8 (i)
                            888 BINARY_SUBSCR
                            898 PRECALL                  3
                            902 CALL                     3
                            912 POP_TOP
                            914 JUMP_BACKWARD           29 (to 858)
                
-                33     >>  916 LOAD_GLOBAL             16 (torch)
+                32     >>  916 LOAD_GLOBAL             16 (torch)
                            928 LOAD_ATTR                6 (nn)
                            938 LOAD_METHOD             23 (Tanh)
                            960 PRECALL                  0
                            964 CALL                     0
                            974 LOAD_FAST                0 (self)
                            976 STORE_ATTR              24 (activation)
                            986 LOAD_CONST               0 (None)
@@ -338,17 +329,17 @@
                   0.5
                   2
                   'layer_'
                names      ('super', 'RealFunction', '__init__', 'sigmoid_output', 'zip', 'pyro', 'nn', 'PyroModule', 'torch', 'Linear', 'PyroSample', 'dist', 'Normal', 'expand', 'Size', 'to_event', 'weight', 'bias', 'append', 'layers', 'range', 'len', 'setattr', 'Tanh', 'activation')
                varnames   ('self', 'sigmoid_output', 'hidden_dims', 'dimensions', 'layers', 'in_features', 'out_features', 'layer', 'i')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       '__init__'
-               firstlineno 10
+               firstlineno 9
                lnotab
                   0x04014e010e010e0104013c015e012c0134014e0126fd1a052c0134014c
                   0126fd1a052e020e013c013602
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 7
@@ -363,63 +354,63 @@
                   017c00a00500000000000000000000000000000000000000007c01a60100
                   00ab0100000000000000007d018c367409000000000000000000007c0064
                   037405000000000000000000007c006a030000000000000000a6010000ab
                   01000000000000000064027a0a00009b009d02a6020000ab020000000000
                   0000007d0302007c037c01a6010000ab0100000000000000007d017c006a
                   0600000000000000007214740f000000000000000000006a080000000000
                   0000007c01a6010000ab0100000000000000007d017c015300
-                35           0 RESUME                   0
+                34           0 RESUME                   0
                
-                36           2 LOAD_FAST                1 (x)
+                35           2 LOAD_FAST                1 (x)
                              4 LOAD_METHOD              0 (view)
                             26 LOAD_CONST               1 ((-1, 1))
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               1 (x)
                
-                37          44 LOAD_GLOBAL              3 (NULL + range)
+                36          44 LOAD_GLOBAL              3 (NULL + range)
                             56 LOAD_GLOBAL              5 (NULL + len)
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                3 (layers)
                             80 PRECALL                  1
                             84 CALL                     1
                             94 LOAD_CONST               2 (1)
                             96 BINARY_OP               10 (-)
                            100 PRECALL                  1
                            104 CALL                     1
                            114 GET_ITER
                        >>  116 FOR_ITER                53 (to 224)
                            118 STORE_FAST               2 (i)
                
-                38         120 LOAD_GLOBAL              9 (NULL + getattr)
+                37         120 LOAD_GLOBAL              9 (NULL + getattr)
                            132 LOAD_FAST                0 (self)
                            134 LOAD_CONST               3 ('layer_')
                            136 LOAD_FAST                2 (i)
                            138 FORMAT_VALUE             0
                            140 BUILD_STRING             2
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_FAST               3 (layer)
                
-                39         158 PUSH_NULL
+                38         158 PUSH_NULL
                            160 LOAD_FAST                3 (layer)
                            162 LOAD_FAST                1 (x)
                            164 PRECALL                  1
                            168 CALL                     1
                            178 STORE_FAST               1 (x)
                
-                40         180 LOAD_FAST                0 (self)
+                39         180 LOAD_FAST                0 (self)
                            182 LOAD_METHOD              5 (activation)
                            204 LOAD_FAST                1 (x)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 STORE_FAST               1 (x)
                            222 JUMP_BACKWARD           54 (to 116)
                
-                41     >>  224 LOAD_GLOBAL              9 (NULL + getattr)
+                40     >>  224 LOAD_GLOBAL              9 (NULL + getattr)
                            236 LOAD_FAST                0 (self)
                            238 LOAD_CONST               3 ('layer_')
                            240 LOAD_GLOBAL              5 (NULL + len)
                            252 LOAD_FAST                0 (self)
                            254 LOAD_ATTR                3 (layers)
                            264 PRECALL                  1
                            268 CALL                     1
@@ -427,110 +418,110 @@
                            280 BINARY_OP               10 (-)
                            284 FORMAT_VALUE             0
                            286 BUILD_STRING             2
                            288 PRECALL                  2
                            292 CALL                     2
                            302 STORE_FAST               3 (layer)
                
-                42         304 PUSH_NULL
+                41         304 PUSH_NULL
                            306 LOAD_FAST                3 (layer)
                            308 LOAD_FAST                1 (x)
                            310 PRECALL                  1
                            314 CALL                     1
                            324 STORE_FAST               1 (x)
                
-                43         326 LOAD_FAST                0 (self)
+                42         326 LOAD_FAST                0 (self)
                            328 LOAD_ATTR                6 (sigmoid_output)
                            338 POP_JUMP_FORWARD_IF_FALSE    20 (to 380)
                
-                44         340 LOAD_GLOBAL             15 (NULL + torch)
+                43         340 LOAD_GLOBAL             15 (NULL + torch)
                            352 LOAD_ATTR                8 (sigmoid)
                            362 LOAD_FAST                1 (x)
                            364 PRECALL                  1
                            368 CALL                     1
                            378 STORE_FAST               1 (x)
                
-                45     >>  380 LOAD_FAST                1 (x)
+                44     >>  380 LOAD_FAST                1 (x)
                            382 RETURN_VALUE
                consts
                   None
                   (-1, 1)
                   1
                   'layer_'
                names      ('view', 'range', 'len', 'layers', 'getattr', 'activation', 'sigmoid_output', 'torch', 'sigmoid')
                varnames   ('self', 'x', 'i', 'layer')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       'forward'
-               firstlineno 35
+               firstlineno 34
                lnotab 0x02012a014c01260116012c01500116010e012801
          names      ('__name__', '__module__', '__qualname__', '__init__', 'forward', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
          name       'RealFunction'
-         firstlineno 9
+         firstlineno 8
          lnotab 0x0c011019
       'RealFunction'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a02640a88006601640484095a036504640584
             00a6000000ab0000000000000000005a05650464068400a6000000ab0000
             000000000000005a06640784005a07640884005a08640984005a09880078
             015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-          48           2 RESUME                   0
+          47           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('BasisDecomposition')
                       10 STORE_NAME               2 (__qualname__)
          
-          49          12 LOAD_CONST              10 ((2, 1.0, True))
+          48          12 LOAD_CONST              10 ((2, 1.0, True))
                       14 LOAD_CLOSURE             0 (__class__)
                       16 BUILD_TUPLE              1
-                      18 LOAD_CONST               4 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 49>)
+                      18 LOAD_CONST               4 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 48>)
                       20 MAKE_FUNCTION            9 (defaults, closure)
                       22 STORE_NAME               3 (__init__)
          
-          66          24 LOAD_NAME                4 (property)
+          65          24 LOAD_NAME                4 (property)
          
-          67          26 LOAD_CONST               5 (<code object gene_scales, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 66>)
+          66          26 LOAD_CONST               5 (<code object gene_scales, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 65>)
                       28 MAKE_FUNCTION            0
          
-          66          30 PRECALL                  0
+          65          30 PRECALL                  0
                       34 CALL                     0
          
-          67          44 STORE_NAME               5 (gene_scales)
+          66          44 STORE_NAME               5 (gene_scales)
          
-          70          46 LOAD_NAME                4 (property)
+          69          46 LOAD_NAME                4 (property)
          
-          71          48 LOAD_CONST               6 (<code object std, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 70>)
+          70          48 LOAD_CONST               6 (<code object std, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 69>)
                       50 MAKE_FUNCTION            0
          
-          70          52 PRECALL                  0
+          69          52 PRECALL                  0
                       56 CALL                     0
          
-          71          66 STORE_NAME               6 (std)
+          70          66 STORE_NAME               6 (std)
          
-          74          68 LOAD_CONST               7 (<code object forward, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 74>)
+          73          68 LOAD_CONST               7 (<code object forward, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 73>)
                       70 MAKE_FUNCTION            0
                       72 STORE_NAME               7 (forward)
          
-         113          74 LOAD_CONST               8 (<code object get_basis, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 113>)
+         112          74 LOAD_CONST               8 (<code object get_basis, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 112>)
                       76 MAKE_FUNCTION            0
                       78 STORE_NAME               8 (get_basis)
          
-         120          80 LOAD_CONST               9 (<code object show_basis, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 120>)
+         119          80 LOAD_CONST               9 (<code object show_basis, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 119>)
                       82 MAKE_FUNCTION            0
                       84 STORE_NAME               9 (show_basis)
                       86 LOAD_CLOSURE             0 (__class__)
                       88 COPY                     1
                       90 STORE_NAME              10 (__classcell__)
                       92 RETURN_VALUE
          consts
@@ -556,83 +547,83 @@
                   00000000007c0289005f0c00000000000000007c0189005f020000000000
                   0000007c0489005f0d0000000000000000640289005f0e00000000000000
                   00640089005f0f0000000000000000640089005f10000000000000000064
                   005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
-                49           4 RESUME                   0
+                48           4 RESUME                   0
                
-                50           6 LOAD_GLOBAL              1 (NULL + super)
+                49           6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_METHOD              1 (__init__)
                             54 PRECALL                  0
                             58 CALL                     0
                             68 POP_TOP
                
-                51          70 LOAD_FAST                1 (K)
+                50          70 LOAD_FAST                1 (K)
                             72 LOAD_DEREF               0 (self)
                             74 STORE_ATTR               2 (K)
                
-                52          84 LOAD_FAST                5 (normalized_mode)
+                51          84 LOAD_FAST                5 (normalized_mode)
                             86 LOAD_DEREF               0 (self)
                             88 STORE_ATTR               3 (normalized_mode)
                
-                54          98 LOAD_GLOBAL              9 (NULL + pyro)
+                53          98 LOAD_GLOBAL              9 (NULL + pyro)
                            110 LOAD_ATTR                5 (nn)
                            120 LOAD_ATTR                6 (PyroModule)
                            130 LOAD_GLOBAL             14 (torch)
                            142 LOAD_ATTR                5 (nn)
                            152 LOAD_ATTR                8 (ModuleList)
                            162 BINARY_SUBSCR
                
-                55         172 LOAD_CLOSURE             0 (self)
+                54         172 LOAD_CLOSURE             0 (self)
                            174 BUILD_TUPLE              1
-                           176 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 55>)
+                           176 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 54>)
                            178 MAKE_FUNCTION            8 (closure)
                            180 LOAD_GLOBAL             19 (NULL + range)
                            192 LOAD_DEREF               0 (self)
                            194 LOAD_ATTR                2 (K)
                            204 PRECALL                  1
                            208 CALL                     1
                            218 GET_ITER
                            220 PRECALL                  0
                            224 CALL                     0
                
-                54         234 PRECALL                  1
+                53         234 PRECALL                  1
                            238 CALL                     1
                            248 LOAD_DEREF               0 (self)
                            250 STORE_ATTR              10 (trajectory_basis)
                
-                57         260 LOAD_FAST                3 (n_conditions)
+                56         260 LOAD_FAST                3 (n_conditions)
                            262 LOAD_DEREF               0 (self)
                            264 STORE_ATTR              11 (n_conditions)
                
-                58         274 LOAD_FAST                2 (n_genes)
+                57         274 LOAD_FAST                2 (n_genes)
                            276 LOAD_DEREF               0 (self)
                            278 STORE_ATTR              12 (n_genes)
                
-                59         288 LOAD_FAST                1 (K)
+                58         288 LOAD_FAST                1 (K)
                            290 LOAD_DEREF               0 (self)
                            292 STORE_ATTR               2 (K)
                
-                60         302 LOAD_FAST                4 (beta_prior)
+                59         302 LOAD_FAST                4 (beta_prior)
                            304 LOAD_DEREF               0 (self)
                            306 STORE_ATTR              13 (beta_prior)
                
-                62         316 LOAD_CONST               2 (True)
+                61         316 LOAD_CONST               2 (True)
                            318 LOAD_DEREF               0 (self)
                            320 STORE_ATTR              14 (return_basis)
                
-                63         330 LOAD_CONST               0 (None)
+                62         330 LOAD_CONST               0 (None)
                            332 LOAD_DEREF               0 (self)
                            334 STORE_ATTR              15 (_last_basis)
                
-                64         344 LOAD_CONST               0 (None)
+                63         344 LOAD_CONST               0 (None)
                            346 LOAD_DEREF               0 (self)
                            348 STORE_ATTR              16 (_last_patterns)
                            358 LOAD_CONST               0 (None)
                            360 RETURN_VALUE
                consts
                   None
                   code
@@ -642,15 +633,15 @@
                      flags     : 19
                      code
                         0x9501970067007c005d197d017401000000000000000000006400640089
                         026a010000000000000000ac01a6030000ab03000000000000000091028c
                         1a5300
                                    0 COPY_FREE_VARS           1
                      
-                      55           2 RESUME                   0
+                      54           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                25 (to 60)
                                   10 STORE_FAST               1 (_)
                                   12 LOAD_GLOBAL              1 (NULL + RealFunction)
                                   24 LOAD_CONST               0 (32)
                                   26 LOAD_CONST               0 (32)
@@ -665,41 +656,41 @@
                      consts
                         32
                         ('sigmoid_output',)
                      names      ('RealFunction', 'normalized_mode')
                      varnames   ('.0', '_')
                      freevars   ('self',)
                      cellvars   ()
-                     filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+                     filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                      name       '<listcomp>'
-                     firstlineno 55
+                     firstlineno 54
                      lnotab 0x
                   True
                names      ('super', '__init__', 'K', 'normalized_mode', 'pyro', 'nn', 'PyroModule', 'torch', 'ModuleList', 'range', 'trajectory_basis', 'n_conditions', 'n_genes', 'beta_prior', 'return_basis', '_last_basis', '_last_patterns')
                varnames   ('self', 'K', 'n_genes', 'n_conditions', 'beta_prior', 'normalized_mode')
                freevars   ('__class__',)
                cellvars   ('self',)
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       '__init__'
-               firstlineno 49
+               firstlineno 48
                lnotab 0x060140010e010e024a013eff1a030e010e010e010e020e010e01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 9
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000006a03000000000000000064017401000000000000000000
                   006a0400000000000000007c006a0500000000000000007c006a06000000
                   0000000000a6020000ab020000000000000000a6020000ab020000000000
                   000000a6010000ab0100000000000000005300
-                66           0 RESUME                   0
+                65           0 RESUME                   0
                
-                68           2 LOAD_GLOBAL              1 (NULL + torch)
+                67           2 LOAD_GLOBAL              1 (NULL + torch)
                             14 LOAD_ATTR                1 (exp)
                             24 LOAD_GLOBAL              5 (NULL + pyro)
                             36 LOAD_ATTR                3 (param)
                             46 LOAD_CONST               1 ('gene_scale')
                             48 LOAD_GLOBAL              1 (NULL + torch)
                             60 LOAD_ATTR                4 (zeros)
                             70 LOAD_FAST                0 (self)
@@ -716,31 +707,31 @@
                consts
                   None
                   'gene_scale'
                names      ('torch', 'exp', 'pyro', 'param', 'zeros', 'n_conditions', 'n_genes')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       'gene_scales'
-               firstlineno 66
+               firstlineno 65
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007405000000
                   000000000000006a03000000000000000064017401000000000000000000
                   006a0400000000000000006402a6010000ab010000000000000000a60200
                   00ab020000000000000000a6010000ab0100000000000000005300
-                70           0 RESUME                   0
+                69           0 RESUME                   0
                
-                72           2 LOAD_GLOBAL              1 (NULL + torch)
+                71           2 LOAD_GLOBAL              1 (NULL + torch)
                             14 LOAD_ATTR                1 (exp)
                             24 LOAD_GLOBAL              5 (NULL + pyro)
                             36 LOAD_ATTR                3 (param)
                             46 LOAD_CONST               1 ('std')
                             48 LOAD_GLOBAL              1 (NULL + torch)
                             60 LOAD_ATTR                4 (zeros)
                             70 LOAD_CONST               2 (1)
@@ -755,17 +746,17 @@
                   None
                   'std'
                   1
                names      ('torch', 'exp', 'pyro', 'param', 'zeros')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       'std'
-               firstlineno 70
+               firstlineno 69
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 11
                stacksize : 10
                flags     : 3
                code
@@ -804,193 +795,193 @@
                   020000ab02000000000000000001006e0b23003100730477027803590077
                   010100590001000100640064006400a6020000ab02000000000000000001
                   006e0b230031007304770278035900770101005900010001006400640064
                   00a6020000ab02000000000000000001006e0b2300310073047702780359
                   00770101005900010001007c037c005f1700000000000000007c077c005f
                   1800000000000000007c006a19000000000000000072027c0353007c0753
                   00
-                74           0 RESUME                   0
+                73           0 RESUME                   0
                
-                75           2 LOAD_FAST                0 (self)
+                74           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (get_basis)
                             26 LOAD_FAST                1 (times)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               3 (basis)
                
-                77          44 LOAD_FAST                0 (self)
+                76          44 LOAD_FAST                0 (self)
                             46 LOAD_ATTR                1 (normalized_mode)
                             56 POP_JUMP_FORWARD_IF_TRUE   103 (to 264)
                
-                78          58 LOAD_GLOBAL              5 (NULL + pyro)
+                77          58 LOAD_GLOBAL              5 (NULL + pyro)
                             70 LOAD_ATTR                3 (sample)
                
-                79          80 LOAD_CONST               1 ('beta')
+                78          80 LOAD_CONST               1 ('beta')
                
-                80          82 LOAD_GLOBAL              9 (NULL + dist)
+                79          82 LOAD_GLOBAL              9 (NULL + dist)
                             94 LOAD_ATTR                5 (Exponential)
                            104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (beta_prior)
                            116 PRECALL                  1
                            120 CALL                     1
                
-                81         130 LOAD_METHOD              7 (expand)
+                80         130 LOAD_METHOD              7 (expand)
                            152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR                8 (n_conditions)
                            164 LOAD_FAST                0 (self)
                            166 LOAD_ATTR                9 (n_genes)
                            176 LOAD_FAST                0 (self)
                            178 LOAD_ATTR               10 (K)
                            188 BUILD_LIST               3
                            190 PRECALL                  1
                            194 CALL                     1
                
-                82         204 LOAD_METHOD             11 (to_event)
+                81         204 LOAD_METHOD             11 (to_event)
                            226 LOAD_CONST               2 (3)
                            228 PRECALL                  1
                            232 CALL                     1
                
-                78         242 PRECALL                  2
+                77         242 PRECALL                  2
                            246 CALL                     2
                            256 STORE_FAST               4 (betas)
                
-                84         258 LOAD_CONST               3 (0.1)
+                83         258 LOAD_CONST               3 (0.1)
                            260 STORE_FAST               5 (std)
                            262 JUMP_FORWARD           179 (to 622)
                
-                86     >>  264 LOAD_GLOBAL              5 (NULL + pyro)
+                85     >>  264 LOAD_GLOBAL              5 (NULL + pyro)
                            276 LOAD_ATTR                3 (sample)
                
-                87         286 LOAD_CONST               1 ('beta')
+                86         286 LOAD_CONST               1 ('beta')
                
-                88         288 LOAD_GLOBAL              9 (NULL + dist)
+                87         288 LOAD_GLOBAL              9 (NULL + dist)
                            300 LOAD_ATTR               12 (Dirichlet)
                            310 LOAD_GLOBAL             27 (NULL + torch)
                            322 LOAD_ATTR               14 (ones)
                            332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR               10 (K)
                            344 PRECALL                  1
                            348 CALL                     1
                            358 LOAD_FAST                0 (self)
                            360 LOAD_ATTR                6 (beta_prior)
                            370 BINARY_OP                5 (*)
                            374 PRECALL                  1
                            378 CALL                     1
                
-                89         388 LOAD_METHOD              7 (expand)
+                88         388 LOAD_METHOD              7 (expand)
                            410 LOAD_GLOBAL             27 (NULL + torch)
                            422 LOAD_ATTR               15 (Size)
                            432 LOAD_FAST                0 (self)
                            434 LOAD_ATTR                8 (n_conditions)
                            444 LOAD_FAST                0 (self)
                            446 LOAD_ATTR                9 (n_genes)
                            456 BUILD_LIST               2
                            458 PRECALL                  1
                            462 CALL                     1
                            472 PRECALL                  1
                            476 CALL                     1
                
-                90         486 LOAD_METHOD             11 (to_event)
+                89         486 LOAD_METHOD             11 (to_event)
                            508 LOAD_CONST               4 (2)
                            510 PRECALL                  1
                            514 CALL                     1
                
-                86         524 PRECALL                  2
+                85         524 PRECALL                  2
                            528 CALL                     2
                            538 STORE_FAST               4 (betas)
                
-                92         540 LOAD_FAST                0 (self)
+                91         540 LOAD_FAST                0 (self)
                            542 LOAD_ATTR               16 (gene_scales)
                            552 LOAD_METHOD             17 (unsqueeze)
                            574 LOAD_CONST               5 (-1)
                            576 PRECALL                  1
                            580 CALL                     1
                            590 STORE_FAST               6 (gene_scales)
                
-                93         592 LOAD_FAST                4 (betas)
+                92         592 LOAD_FAST                4 (betas)
                            594 LOAD_FAST                6 (gene_scales)
                            596 BINARY_OP                5 (*)
                            600 STORE_FAST               4 (betas)
                
-                94         602 LOAD_FAST                0 (self)
+                93         602 LOAD_FAST                0 (self)
                            604 LOAD_ATTR               18 (std)
                            614 LOAD_FAST                6 (gene_scales)
                            616 BINARY_OP                5 (*)
                            620 STORE_FAST               5 (std)
                
-                96     >>  622 LOAD_GLOBAL             27 (NULL + torch)
+                95     >>  622 LOAD_GLOBAL             27 (NULL + torch)
                            634 LOAD_ATTR               19 (einsum)
                            644 LOAD_CONST               6 ('cgk, tk -> cgt')
                            646 LOAD_FAST                4 (betas)
                            648 LOAD_FAST                3 (basis)
                            650 PRECALL                  3
                            654 CALL                     3
                            664 STORE_FAST               7 (gene_patterns)
                
-                98         666 LOAD_GLOBAL              5 (NULL + pyro)
+                97         666 LOAD_GLOBAL              5 (NULL + pyro)
                            678 LOAD_ATTR               20 (plate)
                            688 LOAD_CONST               7 ('t')
                            690 LOAD_GLOBAL             43 (NULL + len)
                            702 LOAD_FAST                1 (times)
                            704 PRECALL                  1
                            708 CALL                     1
                            718 LOAD_CONST               5 (-1)
                            720 KW_NAMES                 8
                            722 PRECALL                  3
                            726 CALL                     3
                            736 STORE_FAST               8 (t_axis)
                
-                99         738 LOAD_GLOBAL              5 (NULL + pyro)
+                98         738 LOAD_GLOBAL              5 (NULL + pyro)
                            750 LOAD_ATTR               20 (plate)
                            760 LOAD_CONST               9 ('g')
                            762 LOAD_FAST                0 (self)
                            764 LOAD_ATTR                9 (n_genes)
                            774 LOAD_CONST              10 (-2)
                            776 KW_NAMES                 8
                            778 PRECALL                  3
                            782 CALL                     3
                            792 STORE_FAST               9 (gene_axis)
                
-               100         794 LOAD_GLOBAL              5 (NULL + pyro)
+                99         794 LOAD_GLOBAL              5 (NULL + pyro)
                            806 LOAD_ATTR               20 (plate)
                            816 LOAD_CONST              11 ('c')
                            818 LOAD_FAST                0 (self)
                            820 LOAD_ATTR                8 (n_conditions)
                            830 LOAD_CONST              12 (-3)
                            832 KW_NAMES                 8
                            834 PRECALL                  3
                            838 CALL                     3
                            848 STORE_FAST              10 (c_axis)
                
-               102         850 LOAD_FAST               10 (c_axis)
+               101         850 LOAD_FAST               10 (c_axis)
                            852 BEFORE_WITH
                            854 POP_TOP
                            856 LOAD_FAST                9 (gene_axis)
                            858 BEFORE_WITH
                            860 POP_TOP
                            862 LOAD_FAST                8 (t_axis)
                            864 BEFORE_WITH
                            866 POP_TOP
                
-               103         868 LOAD_GLOBAL              5 (NULL + pyro)
+               102         868 LOAD_GLOBAL              5 (NULL + pyro)
                            880 LOAD_ATTR                3 (sample)
                            890 LOAD_CONST              13 ('obs')
                            892 LOAD_GLOBAL              9 (NULL + dist)
                            904 LOAD_ATTR               22 (Normal)
                            914 LOAD_FAST                7 (gene_patterns)
                            916 LOAD_FAST                5 (std)
                            918 PRECALL                  2
                            922 CALL                     2
                            932 LOAD_FAST                2 (data)
                            934 KW_NAMES                14
                            936 PRECALL                  3
                            940 CALL                     3
                            950 POP_TOP
                
-               102         952 LOAD_CONST               0 (None)
+               101         952 LOAD_CONST               0 (None)
                            954 LOAD_CONST               0 (None)
                            956 LOAD_CONST               0 (None)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                            974 JUMP_FORWARD            11 (to 998)
                        >>  976 PUSH_EXC_INFO
@@ -1037,30 +1028,30 @@
                           1078 POP_EXCEPT
                           1080 RERAISE                  1
                        >> 1082 POP_TOP
                           1084 POP_EXCEPT
                           1086 POP_TOP
                           1088 POP_TOP
                
-               105     >> 1090 LOAD_FAST                3 (basis)
+               104     >> 1090 LOAD_FAST                3 (basis)
                           1092 LOAD_FAST                0 (self)
                           1094 STORE_ATTR              23 (_last_basis)
                
-               106        1104 LOAD_FAST                7 (gene_patterns)
+               105        1104 LOAD_FAST                7 (gene_patterns)
                           1106 LOAD_FAST                0 (self)
                           1108 STORE_ATTR              24 (_last_patterns)
                
-               108        1118 LOAD_FAST                0 (self)
+               107        1118 LOAD_FAST                0 (self)
                           1120 LOAD_ATTR               25 (return_basis)
                           1130 POP_JUMP_FORWARD_IF_FALSE     2 (to 1136)
                
-               109        1132 LOAD_FAST                3 (basis)
+               108        1132 LOAD_FAST                3 (basis)
                           1134 RETURN_VALUE
                
-               111     >> 1136 LOAD_FAST                7 (gene_patterns)
+               110     >> 1136 LOAD_FAST                7 (gene_patterns)
                           1138 RETURN_VALUE
                ExceptionTable:
                  854 to 858 -> 1068 [1] lasti
                  860 to 864 -> 1022 [2] lasti
                  866 to 950 -> 976 [3] lasti
                  952 to 974 -> 1022 [2] lasti
                  976 to 982 -> 984 [5] lasti
@@ -1090,17 +1081,17 @@
                   -3
                   'obs'
                   ('obs',)
                names      ('get_basis', 'normalized_mode', 'pyro', 'sample', 'dist', 'Exponential', 'beta_prior', 'expand', 'n_conditions', 'n_genes', 'K', 'to_event', 'Dirichlet', 'torch', 'ones', 'Size', 'gene_scales', 'unsqueeze', 'std', 'einsum', 'plate', 'len', 'Normal', '_last_basis', '_last_patterns', 'return_basis')
                varnames   ('self', 'times', 'data', 'basis', 'betas', 'std', 'gene_scales', 'gene_patterns', 't_axis', 'gene_axis', 'c_axis')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       'forward'
-               firstlineno 74
+               firstlineno 73
                lnotab
                   0x02012a020e011601020130014a0126fc10060602160102016401620126
                   fc100634010a0114022c02480138013802120154ff8a030e010e020e0104
                   02
             code
                argcount  : 2
                nlocals   : 3
@@ -1109,59 +1100,59 @@
                code
                   0x8701970088016601640184087c006a0000000000000000004400a60000
                   00ab0000000000000000007d02640284007c024400a6000000ab00000000
                   00000000007d027403000000000000000000006a0200000000000000007c
                   026403ac04a6020000ab0200000000000000007d027c025300
                              0 MAKE_CELL                1 (times)
                
-               113           2 RESUME                   0
+               112           2 RESUME                   0
                
-               115           4 LOAD_CLOSURE             1 (times)
+               114           4 LOAD_CLOSURE             1 (times)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 115>)
+                             8 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 114>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 LOAD_FAST                0 (self)
                             14 LOAD_ATTR                0 (trajectory_basis)
                             24 GET_ITER
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               2 (basis)
                
-               116          42 LOAD_CONST               2 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 116>)
+               115          42 LOAD_CONST               2 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 115>)
                             44 MAKE_FUNCTION            0
                             46 LOAD_FAST                2 (basis)
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               2 (basis)
                
-               117          66 LOAD_GLOBAL              3 (NULL + torch)
+               116          66 LOAD_GLOBAL              3 (NULL + torch)
                             78 LOAD_ATTR                2 (cat)
                             88 LOAD_FAST                2 (basis)
                             90 LOAD_CONST               3 (1)
                             92 KW_NAMES                 4
                             94 PRECALL                  2
                             98 CALL                     2
                            108 STORE_FAST               2 (basis)
                
-               118         110 LOAD_FAST                2 (basis)
+               117         110 LOAD_FAST                2 (basis)
                            112 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x9501970067007c005d0d7d0102007c018902a6010000ab010000000000
                         00000091028c0e5300
                                    0 COPY_FREE_VARS           1
                      
-                     115           2 RESUME                   0
+                     114           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                13 (to 36)
                                   10 STORE_FAST               1 (trajectory)
                                   12 PUSH_NULL
                                   14 LOAD_FAST                1 (trajectory)
                                   16 LOAD_DEREF               2 (times)
@@ -1171,28 +1162,28 @@
                                   34 JUMP_BACKWARD           14 (to 8)
                              >>   36 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'trajectory')
                      freevars   ('times',)
                      cellvars   ()
-                     filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+                     filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                      name       '<listcomp>'
-                     firstlineno 115
+                     firstlineno 114
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d1c7d017c017c01a00000000000000000000000000000
                         00000000000000a6000000ab00000000000000000064007a0000007a0b00
                         0091028c1d5300
-                     116           0 RESUME                   0
+                     115           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                28 (to 64)
                                    8 STORE_FAST               1 (b)
                                   10 LOAD_FAST                1 (b)
                                   12 LOAD_FAST                1 (b)
                                   14 LOAD_METHOD              0 (max)
@@ -1206,27 +1197,27 @@
                              >>   64 RETURN_VALUE
                      consts
                         1e-06
                      names      ('max',)
                      varnames   ('.0', 'b')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+                     filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                      name       '<listcomp>'
-                     firstlineno 116
+                     firstlineno 115
                      lnotab 0x
                   1
                   ('dim',)
                names      ('trajectory_basis', 'torch', 'cat')
                varnames   ('self', 'times', 'basis')
                freevars   ()
                cellvars   ('times',)
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       'get_basis'
-               firstlineno 113
+               firstlineno 112
                lnotab 0x0402260118012c01
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
@@ -1234,44 +1225,44 @@
                   01640184087c006a0200000000000000004400a6000000ab000000000000
                   000000a6010000ab0100000000000000006a0300000000000000007d0274
                   09000000000000000000006a0500000000000000007c02a6010000ab0100
                   000000000000007d037c03a0060000000000000000000000000000000000
                   000000a6000000ab000000000000000000010064005300
                              0 MAKE_CELL                1 (times)
                
-               120           2 RESUME                   0
+               119           2 RESUME                   0
                
-               122           4 LOAD_GLOBAL              1 (NULL + np)
+               121           4 LOAD_GLOBAL              1 (NULL + np)
                             16 LOAD_ATTR                1 (array)
                
-               123          26 LOAD_CLOSURE             1 (times)
+               122          26 LOAD_CLOSURE             1 (times)
                             28 BUILD_TUPLE              1
-                            30 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py", line 123>)
+                            30 LOAD_CONST               1 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py", line 122>)
                             32 MAKE_FUNCTION            8 (closure)
                             34 LOAD_FAST                0 (self)
                             36 LOAD_ATTR                2 (trajectory_basis)
                             46 GET_ITER
                             48 PRECALL                  0
                             52 CALL                     0
                
-               122          62 PRECALL                  1
+               121          62 PRECALL                  1
                             66 CALL                     1
                
-               124          76 LOAD_ATTR                3 (T)
+               123          76 LOAD_ATTR                3 (T)
                
-               122          86 STORE_FAST               2 (basis)
+               121          86 STORE_FAST               2 (basis)
                
-               126          88 LOAD_GLOBAL              9 (NULL + pd)
+               125          88 LOAD_GLOBAL              9 (NULL + pd)
                            100 LOAD_ATTR                5 (DataFrame)
                            110 LOAD_FAST                2 (basis)
                            112 PRECALL                  1
                            116 CALL                     1
                            126 STORE_FAST               3 (data)
                
-               127         128 LOAD_FAST                3 (data)
+               126         128 LOAD_FAST                3 (data)
                            130 LOAD_METHOD              6 (plot)
                            152 PRECALL                  0
                            156 CALL                     0
                            166 POP_TOP
                            168 LOAD_CONST               0 (None)
                            170 RETURN_VALUE
                consts
@@ -1285,15 +1276,15 @@
                         0x9501970067007c005d447d0102007c018902a6010000ab010000000000
                         000000a0000000000000000000000000000000000000000000a6000000ab
                         000000000000000000a00100000000000000000000000000000000000000
                         00a6000000ab000000000000000000a00200000000000000000000000000
                         000000000000006400a6010000ab01000000000000000091028c455300
                                    0 COPY_FREE_VARS           1
                      
-                     123           2 RESUME                   0
+                     122           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                68 (to 146)
                                   10 STORE_FAST               1 (trajectory)
                                   12 PUSH_NULL
                                   14 LOAD_FAST                1 (trajectory)
                                   16 LOAD_DEREF               2 (times)
@@ -1314,37 +1305,37 @@
                              >>  146 RETURN_VALUE
                      consts
                         -1
                      names      ('detach', 'numpy', 'reshape')
                      varnames   ('.0', 'trajectory')
                      freevars   ('times',)
                      cellvars   ()
-                     filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+                     filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                      name       '<listcomp>'
-                     firstlineno 123
+                     firstlineno 122
                      lnotab 0x
                names      ('np', 'array', 'trajectory_basis', 'T', 'pd', 'DataFrame', 'plot')
                varnames   ('self', 'times', 'basis', 'data')
                freevars   ()
                cellvars   ('times',)
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
                name       'show_basis'
-               firstlineno 120
+               firstlineno 119
                lnotab 0x0402160124ff0e020afe02042801
             (2, 1.0, True)
          names      ('__name__', '__module__', '__qualname__', '__init__', 'property', 'gene_scales', 'std', 'forward', 'get_basis', 'show_basis', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
          name       'BasisDecomposition'
-         firstlineno 48
+         firstlineno 47
          lnotab 0x0c010c11020104ff0e010203020104ff0e01020306270607
       'BasisDecomposition'
-   names      ('numpy', 'np', 'pandas', 'pd', 'pyro', 'pyro.distributions', 'distributions', 'dist', 'torch', 'pyro.nn', 'PyroModule', 'nn', 'RealFunction', 'Module', 'BasisDecomposition')
+   names      ('numpy', 'np', 'pandas', 'pd', 'pyro', 'pyro.distributions', 'distributions', 'dist', 'torch', 'nn', 'PyroModule', 'RealFunction', 'Module', 'BasisDecomposition')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/model.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/model.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010801080108010c0108010c033027
+   lnotab 0x00ff02010801080108010c0108033027
```

### Comparing `scdecipher-0.1.0/decipher/tools/_basis_decomposition/__pycache__/run.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/_basis_decomposition/__pycache__/run.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 3880
+moddate:  0x86212166 (Thu Apr 18 13:35:02 2024 UTC)
+files sz: 3878
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a020100640064016c035a04640064016c055a
@@ -99,28 +99,28 @@
     23         132 NOP
    
     24         134 NOP
    
     25         136 NOP
    
     15         138 LOAD_CONST              18 ((5, 0.001, 10000, 1.0, 1, True, None, -1))
-               140 LOAD_CONST              14 (<code object compute_basis_decomposition, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py", line 15>)
+               140 LOAD_CONST              14 (<code object compute_basis_decomposition, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py", line 15>)
                142 MAKE_FUNCTION            1 (defaults)
                144 STORE_NAME              19 (compute_basis_decomposition)
    
-    89         146 LOAD_CONST              15 (<code object get_basis, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py", line 89>)
+    89         146 LOAD_CONST              15 (<code object get_basis, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py", line 89>)
                148 MAKE_FUNCTION            0
                150 STORE_NAME              20 (get_basis)
    
    104         152 LOAD_CONST              19 ((None,))
-               154 LOAD_CONST              16 (<code object _plot_basis, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py", line 104>)
+               154 LOAD_CONST              16 (<code object _plot_basis, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py", line 104>)
                156 MAKE_FUNCTION            1 (defaults)
                158 STORE_NAME              21 (_plot_basis)
    
-   114         160 LOAD_CONST              17 (<code object summary, file "/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py", line 114>)
+   114         160 LOAD_CONST              17 (<code object summary, file "/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py", line 114>)
                162 MAKE_FUNCTION            0
                164 STORE_NAME              22 (summary)
                166 LOAD_CONST               1 (None)
                168 RETURN_VALUE
    consts
       0
       None
@@ -557,15 +557,15 @@
             ('beta', '_RETURN', 'obs')
             ('guide', 'num_samples', 'return_sites')
             '_RETURN'
          names      ('pyro', 'set_rng_seed', 'torch', 'FloatTensor', 'BasisDecomposition', 'shape', 'get_inference_guide', 'optim', 'Adam', 'SVI', 'Trace_ELBO', 'clear_param_store', 'np', 'linspace', 'mean', 'EarlyStopping', 'tqdm', 'range', 'step', '_last_patterns', 'item', 'set_description', 'append', 'IPython.core', 'display', '_last_basis', 'detach', 'numpy', 'plt', 'figure', '_plot_basis', 'clear_output', 'gcf', 'close', 'return_basis', 'Predictive', 'gene_scales', 'squeeze', 'summary')
          varnames   ('gene_patterns', 'inference_mode', 'n_basis', 'lr', 'n_iter', 'beta_prior', 'seed', 'normalized_mode', 'times', 'plot_every_k_epochs', 'model', 'guide', 'adam', 'svi', 'num_iterations', 'gene_patterns_mean', 'gene_patterns_raw', 'losses', 'early_stopping', 'pbar', 'epoch', 'loss', 'reconstruction', 'reconstruction_rel', 'display', 'basis', 'predictive', 'samples', 'gene_scales')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py'
          name       'compute_basis_decomposition'
          firstlineno 15
          lnotab
             0x020c280128010c01020118011801020102fb1207200142013e02260104
             010401680328022e0104010a020401200138010a022c0162013401180112
             ff10032a01160104021e010c0256012a011e012c014c012a020e010c0108
             ff1203180120013a011e02
@@ -663,15 +663,15 @@
             ('guide', 'num_samples', 'return_sites')
             '_RETURN'
             'mean'
          names      ('torch', 'FloatTensor', 'return_basis', 'Predictive', 'summary', 'detach', 'numpy')
          varnames   ('model', 'guide', 'gene_patterns', 'times', 'return_basis_value', 'predictive', 'samples', 'bases')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py'
          name       'get_basis'
          firstlineno 89
          lnotab 0x0201280128010e010e010c0108ff120318011e0164010e01
       code
          argcount  : 2
          nlocals   : 3
          stacksize : 8
@@ -737,15 +737,15 @@
             'basis %d'
             3
             ('c', 'label', 'linewidth')
          names      ('range', 'shape', 'plt', 'plot')
          varnames   ('bases', 'colors', 'i')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py'
          name       '_plot_basis'
          firstlineno 104
          lnotab 0x020138011601160116010e0102fc14ff
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
@@ -801,23 +801,23 @@
             None
             0
             ('mean', 'std', 'values')
          names      ('items', 'torch', 'mean', 'std')
          varnames   ('samples', 'site_stats', 'k', 'v')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py'
          name       'summary'
          firstlineno 114
          lnotab 0x0201040132022801280102fd0e05
       (5, 0.001, 10000, 1.0, 1, True, None, -1)
       (None,)
    names      ('matplotlib.pyplot', 'pyplot', 'plt', 'numpy', 'np', 'pyro', 'pyro.infer', 'pyro.optim', 'torch', 'Predictive', 'SVI', 'Trace_ELBO', 'tqdm', 'decipher.tools._basis_decomposition.inference', 'get_inference_guide', 'decipher.tools._basis_decomposition.model', 'BasisDecomposition', 'decipher.tools.utils', 'EarlyStopping', 'compute_basis_decomposition', 'get_basis', '_plot_basis', 'summary')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_basis_decomposition/run.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_basis_decomposition/run.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010801080108010801080114010c020c010c010c06020102
       010201020102010201020102f6084a060f080a
```

### Comparing `scdecipher-0.1.0/decipher/tools/_basis_decomposition/inference.py` & `scdecipher-0.1.2/decipher/tools/_basis_decomposition/inference.py`

 * *Files identical despite different names*

### Comparing `scdecipher-0.1.0/decipher/tools/_basis_decomposition/model.py` & `scdecipher-0.1.2/decipher/tools/_basis_decomposition/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import numpy as np
 import pandas as pd
 import pyro
 import pyro.distributions as dist
 import torch
-from pyro.nn import PyroModule
 
 
 class RealFunction(pyro.nn.PyroModule):
     def __init__(self, *hidden_dims, sigmoid_output=False):
         super(RealFunction, self).__init__()
         dimensions = [1, *hidden_dims, 1]
         self.sigmoid_output = sigmoid_output
         layers = []
         for in_features, out_features in zip(dimensions, dimensions[1:]):
             layer = pyro.nn.PyroModule[torch.nn.Linear](in_features, out_features)
             layer.weight = pyro.nn.PyroSample(
-                dist.Normal(0.0, 1.0 / in_features ** 0.5)
+                dist.Normal(0.0, 1.0 / in_features**0.5)
                 .expand(torch.Size([out_features, in_features]))
                 .to_event(2)
             )
             layer.bias = pyro.nn.PyroSample(
-                dist.Normal(0.0, 1.0 / in_features ** 0.5)
+                dist.Normal(0.0, 1.0 / in_features**0.5)
                 .expand(torch.Size([out_features]))
                 .to_event(1)
             )
             layers.append(layer)
 
         self.layers = layers
         for i in range(len(layers)):
```

### Comparing `scdecipher-0.1.0/decipher/tools/_basis_decomposition/run.py` & `scdecipher-0.1.2/decipher/tools/_basis_decomposition/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     losses = []
     early_stopping = EarlyStopping(patience=100)
     pbar = tqdm(range(num_iterations))
     for epoch in pbar:
         # calculate the loss and take a gradient step
         loss = svi.step(times, gene_patterns)
         reconstruction = ((model._last_patterns - gene_patterns) ** 2).mean().item()
-        reconstruction_rel = reconstruction / (gene_patterns ** 2).mean()
+        reconstruction_rel = reconstruction / (gene_patterns**2).mean()
         pbar.set_description(
             "Loss: %.1f - Relative Error: %.2f%%" % (loss, reconstruction_rel * 100)
         )
         losses.append(loss)
         if early_stopping(loss):
             break
```

### Comparing `scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/data.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/data.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,23 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 3280
+moddate:  0x2d222166 (Thu Apr 18 13:37:49 2024 UTC)
+files sz: 3549
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      016c035a03640064016c045a04640064016c055a04640064016c065a0464
-      0064026c076d085a086d095a090100640064036c0a6d0b5a0b6d0c5a0c01
-      00020065006a0d0000000000000000650ea6010000ab0100000000000000
-      005a0f020065006a100000000000000000640465006a1100000000000000
-      00ac05a6020000ab0200000000000000000100640c640684015a12640d64
-      0884015a13640984005a14640e640b84015a1564015300
+      016c035a04640064016c055a05640064016c065a06640064016c075a0664
+      0064016c085a06640064016c095a06640064026c0a6d0b5a0b6d0c5a0c01
+      00640064036c0d6d0e5a0e6d0f5a0f0100020065006a1000000000000000
+      006511a6010000ab0100000000000000005a12020065006a130000000000
+      000000640465006a140000000000000000ac05a6020000ab020000000000
+      0000000100640684005a15640d640784015a16640e640984015a17640a84
+      005a18640f640c84015a1964015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (logging)
                  8 STORE_NAME               0 (logging)
    
@@ -29,141 +30,197 @@
      3          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               1 (None)
                 22 IMPORT_NAME              2 (time)
                 24 STORE_NAME               2 (time)
    
      5          26 LOAD_CONST               0 (0)
                 28 LOAD_CONST               1 (None)
-                30 IMPORT_NAME              3 (randomname)
-                32 STORE_NAME               3 (randomname)
+                30 IMPORT_NAME              3 (numpy)
+                32 STORE_NAME               4 (np)
    
      6          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               1 (None)
-                38 IMPORT_NAME              4 (torch)
-                40 STORE_NAME               4 (torch)
+                38 IMPORT_NAME              5 (randomname)
+                40 STORE_NAME               5 (randomname)
    
      7          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               1 (None)
-                46 IMPORT_NAME              5 (torch.nn.functional)
-                48 STORE_NAME               4 (torch)
+                46 IMPORT_NAME              6 (torch)
+                48 STORE_NAME               6 (torch)
    
      8          50 LOAD_CONST               0 (0)
                 52 LOAD_CONST               1 (None)
-                54 IMPORT_NAME              6 (torch.utils.data)
-                56 STORE_NAME               4 (torch)
+                54 IMPORT_NAME              7 (torch.distributions)
+                56 STORE_NAME               6 (torch)
    
-    10          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               2 (('Decipher', 'DecipherConfig'))
-                62 IMPORT_NAME              7 (decipher.tools._decipher)
-                64 IMPORT_FROM              8 (Decipher)
-                66 STORE_NAME               8 (Decipher)
-                68 IMPORT_FROM              9 (DecipherConfig)
-                70 STORE_NAME               9 (DecipherConfig)
-                72 POP_TOP
-   
-    11          74 LOAD_CONST               0 (0)
-                76 LOAD_CONST               3 (('DECIPHER_GLOBALS', 'create_decipher_uns_key'))
-                78 IMPORT_NAME             10 (decipher.utils)
-                80 IMPORT_FROM             11 (DECIPHER_GLOBALS)
-                82 STORE_NAME              11 (DECIPHER_GLOBALS)
-                84 IMPORT_FROM             12 (create_decipher_uns_key)
-                86 STORE_NAME              12 (create_decipher_uns_key)
+     9          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               1 (None)
+                62 IMPORT_NAME              8 (torch.nn.functional)
+                64 STORE_NAME               6 (torch)
+   
+    10          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               1 (None)
+                70 IMPORT_NAME              9 (torch.utils.data)
+                72 STORE_NAME               6 (torch)
+   
+    12          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               2 (('Decipher', 'DecipherConfig'))
+                78 IMPORT_NAME             10 (decipher.tools._decipher)
+                80 IMPORT_FROM             11 (Decipher)
+                82 STORE_NAME              11 (Decipher)
+                84 IMPORT_FROM             12 (DecipherConfig)
+                86 STORE_NAME              12 (DecipherConfig)
                 88 POP_TOP
    
-    13          90 PUSH_NULL
-                92 LOAD_NAME                0 (logging)
-                94 LOAD_ATTR               13 (getLogger)
-               104 LOAD_NAME               14 (__name__)
-               106 PRECALL                  1
-               110 CALL                     1
-               120 STORE_NAME              15 (logger)
-   
-    14         122 PUSH_NULL
-               124 LOAD_NAME                0 (logging)
-               126 LOAD_ATTR               16 (basicConfig)
-   
-    15         136 LOAD_CONST               4 ('%(asctime)s | %(levelname)s : %(message)s')
-   
-    16         138 LOAD_NAME                0 (logging)
-               140 LOAD_ATTR               17 (INFO)
-   
-    14         150 KW_NAMES                 5
-               152 PRECALL                  2
-               156 CALL                     2
-               166 POP_TOP
-   
-    20         168 LOAD_CONST              12 ((None,))
-               170 LOAD_CONST               6 (<code object get_random_name, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py", line 20>)
-               172 MAKE_FUNCTION            1 (defaults)
-               174 STORE_NAME              18 (get_random_name)
-   
-    31         176 LOAD_CONST              13 ((False,))
-               178 LOAD_CONST               8 (<code object decipher_save_model, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py", line 31>)
-               180 MAKE_FUNCTION            1 (defaults)
-               182 STORE_NAME              19 (decipher_save_model)
+    13          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               3 (('DECIPHER_GLOBALS', 'create_decipher_uns_key'))
+                94 IMPORT_NAME             13 (decipher.utils)
+                96 IMPORT_FROM             14 (DECIPHER_GLOBALS)
+                98 STORE_NAME              14 (DECIPHER_GLOBALS)
+               100 IMPORT_FROM             15 (create_decipher_uns_key)
+               102 STORE_NAME              15 (create_decipher_uns_key)
+               104 POP_TOP
+   
+    15         106 PUSH_NULL
+               108 LOAD_NAME                0 (logging)
+               110 LOAD_ATTR               16 (getLogger)
+               120 LOAD_NAME               17 (__name__)
+               122 PRECALL                  1
+               126 CALL                     1
+               136 STORE_NAME              18 (logger)
+   
+    16         138 PUSH_NULL
+               140 LOAD_NAME                0 (logging)
+               142 LOAD_ATTR               19 (basicConfig)
+   
+    17         152 LOAD_CONST               4 ('%(asctime)s | %(levelname)s : %(message)s')
+   
+    18         154 LOAD_NAME                0 (logging)
+               156 LOAD_ATTR               20 (INFO)
+   
+    16         166 KW_NAMES                 5
+               168 PRECALL                  2
+               172 CALL                     2
+               182 POP_TOP
    
-    52         184 LOAD_CONST               9 (<code object decipher_load_model, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py", line 52>)
+    22         184 LOAD_CONST               6 (<code object get_dense_X, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py", line 22>)
                186 MAKE_FUNCTION            0
-               188 STORE_NAME              20 (decipher_load_model)
+               188 STORE_NAME              21 (get_dense_X)
    
-    81         190 LOAD_CONST              14 ((64, None))
-               192 LOAD_CONST              11 (<code object make_data_loader_from_adata, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py", line 81>)
+    29         190 LOAD_CONST              13 ((None,))
+               192 LOAD_CONST               7 (<code object get_random_name, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py", line 29>)
                194 MAKE_FUNCTION            1 (defaults)
-               196 STORE_NAME              21 (make_data_loader_from_adata)
-               198 LOAD_CONST               1 (None)
-               200 RETURN_VALUE
+               196 STORE_NAME              22 (get_random_name)
+   
+    40         198 LOAD_CONST              14 ((False,))
+               200 LOAD_CONST               9 (<code object decipher_save_model, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py", line 40>)
+               202 MAKE_FUNCTION            1 (defaults)
+               204 STORE_NAME              23 (decipher_save_model)
+   
+    61         206 LOAD_CONST              10 (<code object decipher_load_model, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py", line 61>)
+               208 MAKE_FUNCTION            0
+               210 STORE_NAME              24 (decipher_load_model)
+   
+    90         212 LOAD_CONST              15 ((64, None))
+               214 LOAD_CONST              12 (<code object make_data_loader_from_adata, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py", line 90>)
+               216 MAKE_FUNCTION            1 (defaults)
+               218 STORE_NAME              25 (make_data_loader_from_adata)
+               220 LOAD_CONST               1 (None)
+               222 RETURN_VALUE
    consts
       0
       None
       ('Decipher', 'DecipherConfig')
       ('DECIPHER_GLOBALS', 'create_decipher_uns_key')
       '%(asctime)s | %(levelname)s : %(message)s'
       ('format', 'level')
       code
          argcount  : 1
+         nlocals   : 1
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007c006a010000000000000000740400
+            0000000000000000006a030000000000000000a6020000ab020000000000
+            00000072077c006a01000000000000000053007c006a0100000000000000
+            00a0040000000000000000000000000000000000000000a6000000ab0000
+            000000000000005300
+          22           0 RESUME                   0
+         
+          23           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                      14 LOAD_FAST                0 (adata)
+                      16 LOAD_ATTR                1 (X)
+                      26 LOAD_GLOBAL              4 (np)
+                      38 LOAD_ATTR                3 (ndarray)
+                      48 PRECALL                  2
+                      52 CALL                     2
+                      62 POP_JUMP_FORWARD_IF_FALSE     7 (to 78)
+         
+          24          64 LOAD_FAST                0 (adata)
+                      66 LOAD_ATTR                1 (X)
+                      76 RETURN_VALUE
+         
+          26     >>   78 LOAD_FAST                0 (adata)
+                      80 LOAD_ATTR                1 (X)
+                      90 LOAD_METHOD              4 (toarray)
+                     112 PRECALL                  0
+                     116 CALL                     0
+                     126 RETURN_VALUE
+         consts
+            None
+         names      ('isinstance', 'X', 'np', 'ndarray', 'toarray')
+         varnames   ('adata',)
+         freevars   ()
+         cellvars   ()
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py'
+         name       'get_dense_X'
+         firstlineno 22
+         lnotab 0x02013e010e02
+      code
+         argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a01000000000000000067006401a2
             0164026403670267006404a2017c00ac05a6040000ab0400000000000000
             007d017405000000000000000000006a0300000000000000006406a60100
             00ab0100000000000000007d027c029b0064077c019b009d035300
-          20           0 RESUME                   0
+          29           0 RESUME                   0
          
-          21           2 LOAD_GLOBAL              1 (NULL + randomname)
+          30           2 LOAD_GLOBAL              1 (NULL + randomname)
                       14 LOAD_ATTR                1 (generate)
          
-          22          24 BUILD_LIST               0
+          31          24 BUILD_LIST               0
                       26 LOAD_CONST               1 (('a/algorithms', 'a/food', 'a/physics'))
                       28 LIST_EXTEND              1
          
-          23          30 LOAD_CONST               2 ('a/colors')
+          32          30 LOAD_CONST               2 ('a/colors')
                       32 LOAD_CONST               3 ('a/emotions')
                       34 BUILD_LIST               2
          
-          24          36 BUILD_LIST               0
+          33          36 BUILD_LIST               0
                       38 LOAD_CONST               4 (('n/algorithms', 'n/food', 'a/physics'))
                       40 LIST_EXTEND              1
          
-          25          42 LOAD_FAST                0 (seed)
+          34          42 LOAD_FAST                0 (seed)
          
-          21          44 KW_NAMES                 5
+          30          44 KW_NAMES                 5
                       46 PRECALL                  4
                       50 CALL                     4
                       60 STORE_FAST               1 (name)
          
-          27          62 LOAD_GLOBAL              5 (NULL + time)
+          36          62 LOAD_GLOBAL              5 (NULL + time)
                       74 LOAD_ATTR                3 (strftime)
                       84 LOAD_CONST               6 ('%Y-%m-%d-%H-%M-%S')
                       86 PRECALL                  1
                       90 CALL                     1
                      100 STORE_FAST               2 (datetime_str)
          
-          28         102 LOAD_FAST                2 (datetime_str)
+          37         102 LOAD_FAST                2 (datetime_str)
                      104 FORMAT_VALUE             0
                      106 LOAD_CONST               7 ('-')
                      108 LOAD_FAST                1 (name)
                      110 FORMAT_VALUE             0
                      112 BUILD_STRING             3
                      114 RETURN_VALUE
          consts
@@ -175,17 +232,17 @@
             ('seed',)
             '%Y-%m-%d-%H-%M-%S'
             '-'
          names      ('randomname', 'generate', 'time', 'strftime')
          varnames   ('seed', 'name', 'datetime_str')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py'
          name       'get_random_name'
-         firstlineno 20
+         firstlineno 29
          lnotab 0x0201160106010601060102fc12062801
       False
       code
          argcount  : 3
          nlocals   : 6
          stacksize : 7
          flags     : 3
@@ -214,59 +271,59 @@
             00000000000000a6000000ab000000000000000000740e00000000000000
             0000006a080000000000000000a009000000000000000000000000000000
             00000000007c05640aa6020000ab020000000000000000a6020000ab0200
             0000000000000001007c016a0e0000000000000000a00f00000000000000
             00000000000000000000000000a6000000ab0000000000000000007c006a
             010000000000000000640219000000000000000000640b3c000000640053
             00
-          31           0 RESUME                   0
+          40           0 RESUME                   0
          
-          32           2 LOAD_GLOBAL              1 (NULL + create_decipher_uns_key)
+          41           2 LOAD_GLOBAL              1 (NULL + create_decipher_uns_key)
                       14 LOAD_FAST                0 (adata)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          34          32 LOAD_CONST               1 ('run_id_history')
+          43          32 LOAD_CONST               1 ('run_id_history')
                       34 LOAD_FAST                0 (adata)
                       36 LOAD_ATTR                1 (uns)
                       46 LOAD_CONST               2 ('decipher')
                       48 BINARY_SUBSCR
                       58 CONTAINS_OP              1
                       60 POP_JUMP_FORWARD_IF_FALSE    16 (to 94)
          
-          35          62 BUILD_LIST               0
+          44          62 BUILD_LIST               0
                       64 LOAD_FAST                0 (adata)
                       66 LOAD_ATTR                1 (uns)
                       76 LOAD_CONST               2 ('decipher')
                       78 BINARY_SUBSCR
                       88 LOAD_CONST               1 ('run_id_history')
                       90 STORE_SUBSCR
          
-          37     >>   94 LOAD_CONST               3 ('run_id')
+          46     >>   94 LOAD_CONST               3 ('run_id')
                       96 LOAD_FAST                0 (adata)
                       98 LOAD_ATTR                1 (uns)
                      108 LOAD_CONST               2 ('decipher')
                      110 BINARY_SUBSCR
                      120 CONTAINS_OP              1
                      122 POP_JUMP_FORWARD_IF_TRUE     2 (to 128)
                      124 LOAD_FAST                2 (overwrite)
                      126 POP_JUMP_FORWARD_IF_TRUE   125 (to 378)
          
-          38     >>  128 LOAD_GLOBAL              5 (NULL + get_random_name)
+          47     >>  128 LOAD_GLOBAL              5 (NULL + get_random_name)
                      140 PRECALL                  0
                      144 CALL                     0
                      154 LOAD_FAST                0 (adata)
                      156 LOAD_ATTR                1 (uns)
                      166 LOAD_CONST               2 ('decipher')
                      168 BINARY_SUBSCR
                      178 LOAD_CONST               3 ('run_id')
                      180 STORE_SUBSCR
          
-          39         184 LOAD_FAST                0 (adata)
+          48         184 LOAD_FAST                0 (adata)
                      186 LOAD_ATTR                1 (uns)
                      196 LOAD_CONST               2 ('decipher')
                      198 BINARY_SUBSCR
                      208 LOAD_CONST               1 ('run_id_history')
                      210 BINARY_SUBSCR
                      220 LOAD_METHOD              3 (append)
                      242 LOAD_FAST                0 (adata)
@@ -275,15 +332,15 @@
                      256 BINARY_SUBSCR
                      266 LOAD_CONST               3 ('run_id')
                      268 BINARY_SUBSCR
                      278 PRECALL                  1
                      282 CALL                     1
                      292 POP_TOP
          
-          40         294 LOAD_GLOBAL              9 (NULL + logging)
+          49         294 LOAD_GLOBAL              9 (NULL + logging)
                      306 LOAD_ATTR                5 (info)
                      316 LOAD_CONST               4 ('Saving decipher model with run_id ')
                      318 LOAD_FAST                0 (adata)
                      320 LOAD_ATTR                1 (uns)
                      330 LOAD_CONST               2 ('decipher')
                      332 BINARY_SUBSCR
                      342 LOAD_CONST               3 ('run_id')
@@ -292,53 +349,53 @@
                      356 LOAD_CONST               5 ('.')
                      358 BUILD_STRING             3
                      360 PRECALL                  1
                      364 CALL                     1
                      374 POP_TOP
                      376 JUMP_FORWARD            20 (to 418)
          
-          42     >>  378 LOAD_GLOBAL              9 (NULL + logging)
+          51     >>  378 LOAD_GLOBAL              9 (NULL + logging)
                      390 LOAD_ATTR                5 (info)
                      400 LOAD_CONST               6 ('Overwriting existing decipher model.')
                      402 PRECALL                  1
                      406 CALL                     1
                      416 POP_TOP
          
-          44     >>  418 LOAD_FAST                0 (adata)
+          53     >>  418 LOAD_FAST                0 (adata)
                      420 LOAD_ATTR                1 (uns)
                      430 LOAD_CONST               2 ('decipher')
                      432 BINARY_SUBSCR
                      442 LOAD_CONST               3 ('run_id')
                      444 BINARY_SUBSCR
                      454 STORE_FAST               3 (model_run_id)
          
-          45         456 LOAD_GLOBAL             12 (DECIPHER_GLOBALS)
+          54         456 LOAD_GLOBAL             12 (DECIPHER_GLOBALS)
                      468 LOAD_CONST               7 ('save_folder')
                      470 BINARY_SUBSCR
                      480 STORE_FAST               4 (save_folder)
          
-          46         482 LOAD_GLOBAL             14 (os)
+          55         482 LOAD_GLOBAL             14 (os)
                      494 LOAD_ATTR                8 (path)
                      504 LOAD_METHOD              9 (join)
                      526 LOAD_FAST                4 (save_folder)
                      528 LOAD_FAST                3 (model_run_id)
                      530 PRECALL                  2
                      534 CALL                     2
                      544 STORE_FAST               5 (full_path)
          
-          47         546 LOAD_GLOBAL             15 (NULL + os)
+          56         546 LOAD_GLOBAL             15 (NULL + os)
                      558 LOAD_ATTR               10 (makedirs)
                      568 LOAD_FAST                5 (full_path)
                      570 LOAD_CONST               8 (True)
                      572 KW_NAMES                 9
                      574 PRECALL                  2
                      578 CALL                     2
                      588 POP_TOP
          
-          48         590 LOAD_GLOBAL             23 (NULL + torch)
+          57         590 LOAD_GLOBAL             23 (NULL + torch)
                      602 LOAD_ATTR               12 (save)
                      612 LOAD_FAST                1 (model)
                      614 LOAD_METHOD             13 (state_dict)
                      636 PRECALL                  0
                      640 CALL                     0
                      650 LOAD_GLOBAL             14 (os)
                      662 LOAD_ATTR                8 (path)
@@ -347,15 +404,15 @@
                      696 LOAD_CONST              10 ('decipher_model.pt')
                      698 PRECALL                  2
                      702 CALL                     2
                      712 PRECALL                  2
                      716 CALL                     2
                      726 POP_TOP
          
-          49         728 LOAD_FAST                1 (model)
+          58         728 LOAD_FAST                1 (model)
                      730 LOAD_ATTR               14 (config)
                      740 LOAD_METHOD             15 (to_dict)
                      762 PRECALL                  0
                      766 CALL                     0
                      776 LOAD_FAST                0 (adata)
                      778 LOAD_ATTR                1 (uns)
                      788 LOAD_CONST               2 ('decipher')
@@ -377,17 +434,17 @@
             ('exist_ok',)
             'decipher_model.pt'
             'config'
          names      ('create_decipher_uns_key', 'uns', 'get_random_name', 'append', 'logging', 'info', 'DECIPHER_GLOBALS', 'os', 'path', 'join', 'makedirs', 'torch', 'save', 'state_dict', 'config', 'to_dict')
          varnames   ('adata', 'model', 'overwrite', 'model_run_id', 'save_folder', 'full_path')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py'
          name       'decipher_save_model'
-         firstlineno 31
+         firstlineno 40
          lnotab 0x02011e021e012002220138016e015402280226011a0140012c018a01
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 8
          flags     : 3
          code
@@ -404,78 +461,78 @@
             000000000000007d057c02a0090000000000000000000000000000000000
             0000007415000000000000000000006a0b0000000000000000740c000000
             000000000000006a070000000000000000a0080000000000000000000000
             0000000000000000007c056406a6020000ab020000000000000000a60100
             00ab010000000000000000a6010000ab01000000000000000001007c02a0
             0c0000000000000000000000000000000000000000a6000000ab00000000
             000000000001007c025300
-          52           0 RESUME                   0
+          61           0 RESUME                   0
          
-          67           2 LOAD_GLOBAL              1 (NULL + create_decipher_uns_key)
+          76           2 LOAD_GLOBAL              1 (NULL + create_decipher_uns_key)
                       14 LOAD_FAST                0 (adata)
                       16 PRECALL                  1
                       20 CALL                     1
                       30 POP_TOP
          
-          68          32 LOAD_CONST               1 ('run_id')
+          77          32 LOAD_CONST               1 ('run_id')
                       34 LOAD_FAST                0 (adata)
                       36 LOAD_ATTR                1 (uns)
                       46 LOAD_CONST               2 ('decipher')
                       48 BINARY_SUBSCR
                       58 CONTAINS_OP              1
                       60 POP_JUMP_FORWARD_IF_FALSE    15 (to 92)
          
-          69          62 LOAD_GLOBAL              5 (NULL + ValueError)
+          78          62 LOAD_GLOBAL              5 (NULL + ValueError)
                       74 LOAD_CONST               3 ('No decipher model has been saved for this AnnData object.')
                       76 PRECALL                  1
                       80 CALL                     1
                       90 RAISE_VARARGS            1
          
-          71     >>   92 LOAD_GLOBAL              7 (NULL + DecipherConfig)
+          80     >>   92 LOAD_GLOBAL              7 (NULL + DecipherConfig)
                      104 LOAD_CONST               7 (())
                      106 BUILD_MAP                0
                      108 LOAD_FAST                0 (adata)
                      110 LOAD_ATTR                1 (uns)
                      120 LOAD_CONST               2 ('decipher')
                      122 BINARY_SUBSCR
                      132 LOAD_CONST               4 ('config')
                      134 BINARY_SUBSCR
                      144 DICT_MERGE               1
                      146 CALL_FUNCTION_EX         1
                      148 STORE_FAST               1 (model_config)
          
-          72         150 LOAD_GLOBAL              9 (NULL + Decipher)
+          81         150 LOAD_GLOBAL              9 (NULL + Decipher)
                      162 LOAD_FAST                1 (model_config)
                      164 PRECALL                  1
                      168 CALL                     1
                      178 STORE_FAST               2 (model)
          
-          73         180 LOAD_FAST                0 (adata)
+          82         180 LOAD_FAST                0 (adata)
                      182 LOAD_ATTR                1 (uns)
                      192 LOAD_CONST               2 ('decipher')
                      194 BINARY_SUBSCR
                      204 LOAD_CONST               1 ('run_id')
                      206 BINARY_SUBSCR
                      216 STORE_FAST               3 (model_run_id)
          
-          74         218 LOAD_GLOBAL             10 (DECIPHER_GLOBALS)
+          83         218 LOAD_GLOBAL             10 (DECIPHER_GLOBALS)
                      230 LOAD_CONST               5 ('save_folder')
                      232 BINARY_SUBSCR
                      242 STORE_FAST               4 (save_folder)
          
-          75         244 LOAD_GLOBAL             12 (os)
+          84         244 LOAD_GLOBAL             12 (os)
                      256 LOAD_ATTR                7 (path)
                      266 LOAD_METHOD              8 (join)
                      288 LOAD_FAST                4 (save_folder)
                      290 LOAD_FAST                3 (model_run_id)
                      292 PRECALL                  2
                      296 CALL                     2
                      306 STORE_FAST               5 (full_path)
          
-          76         308 LOAD_FAST                2 (model)
+          85         308 LOAD_FAST                2 (model)
                      310 LOAD_METHOD              9 (load_state_dict)
                      332 LOAD_GLOBAL             21 (NULL + torch)
                      344 LOAD_ATTR               11 (load)
                      354 LOAD_GLOBAL             12 (os)
                      366 LOAD_ATTR                7 (path)
                      376 LOAD_METHOD              8 (join)
                      398 LOAD_FAST                5 (full_path)
@@ -484,201 +541,206 @@
                      406 CALL                     2
                      416 PRECALL                  1
                      420 CALL                     1
                      430 PRECALL                  1
                      434 CALL                     1
                      444 POP_TOP
          
-          77         446 LOAD_FAST                2 (model)
+          86         446 LOAD_FAST                2 (model)
                      448 LOAD_METHOD             12 (eval)
                      470 PRECALL                  0
                      474 CALL                     0
                      484 POP_TOP
          
-          78         486 LOAD_FAST                2 (model)
+          87         486 LOAD_FAST                2 (model)
                      488 RETURN_VALUE
          consts
             'Load a decipher model whose name is stored in the given AnnData.\n\n    `adata.uns["decipher"]["run_id"]` must be set to the name of the decipher model to load.\n\n    Parameters\n    ----------\n    adata : sc.AnnData\n        The annotated data matrix.\n\n    Returns\n    -------\n    model : Decipher\n        The decipher model.\n    '
             'run_id'
             'decipher'
             'No decipher model has been saved for this AnnData object.'
             'config'
             'save_folder'
             'decipher_model.pt'
             ()
          names      ('create_decipher_uns_key', 'uns', 'ValueError', 'DecipherConfig', 'Decipher', 'DECIPHER_GLOBALS', 'os', 'path', 'join', 'load_state_dict', 'torch', 'load', 'eval')
          varnames   ('adata', 'model_config', 'model', 'model_run_id', 'save_folder', 'full_path')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py'
          name       'decipher_load_model'
-         firstlineno 52
+         firstlineno 61
          lnotab 0x020f1e011e011e023a011e0126011a0140018a012801
       64
       code
          argcount  : 3
-         nlocals   : 10
+         nlocals   : 11
          stacksize : 6
-         flags     : 3
+         flags     : 11
          code
-            0x97007401000000000000000000006a0100000000000000007c006a0200
-            00000000000000a0030000000000000000000000000000000000000000a6
-            000000ab000000000000000000a6010000ab0100000000000000007d037c
-            0367017d0467007d057c02800267007d027c0244005da07d067401000000
-            000000000000006a0400000000000000007c006a0500000000000000007c
-            0619000000000000000000a0060000000000000000000000000000000000
-            0000006401a6010000ab0100000000000000006a0700000000000000006a
-            0800000000000000006a090000000000000000a6010000ab010000000000
-            000000a00a0000000000000000000000000000000000000000a6000000ab
-            0000000000000000007d077400000000000000000000006a0b0000000000
-            0000006a0c0000000000000000a00d000000000000000000000000000000
-            00000000007c07a6010000ab010000000000000000a00e00000000000000
-            00000000000000000000000000a6000000ab0000000000000000007d087c
-            05a00f00000000000000000000000000000000000000007c08a6010000ab
-            01000000000000000001008ca17c05722b7401000000000000000000006a
-            0700000000000000007c056402ac03a6020000ab0200000000000000007d
-            097c04a00f00000000000000000000000000000000000000007c09a60100
-            00ab01000000000000000001007400000000000000000000006a10000000
-            00000000006a110000000000000000a01200000000000000000000000000
-            000000000000007401000000000000000000006a1000000000000000006a
-            1100000000000000006a1300000000000000007c048e007c016404ac05a6
-            030000ab0300000000000000005300
-          81           0 RESUME                   0
+            0x97007401000000000000000000006a0100000000000000007405000000
+            000000000000007c00a6010000ab010000000000000000a6010000ab0100
+            000000000000007d047c0467017d0567007d067c02800267007d027c0244
+            005da07d077401000000000000000000006a0300000000000000007c006a
+            0400000000000000007c0719000000000000000000a00500000000000000
+            000000000000000000000000006402a6010000ab0100000000000000006a
+            0600000000000000006a0700000000000000006a080000000000000000a6
+            010000ab010000000000000000a009000000000000000000000000000000
+            0000000000a6000000ab0000000000000000007d08740000000000000000
+            0000006a0a00000000000000006a0b0000000000000000a00c0000000000
+            0000000000000000000000000000007c08a6010000ab0100000000000000
+            00a00d0000000000000000000000000000000000000000a6000000ab0000
+            000000000000007d097c06a00e0000000000000000000000000000000000
+            0000007c09a6010000ab01000000000000000001008ca17c06722b740100
+            0000000000000000006a0600000000000000007c066403ac04a6020000ab
+            0200000000000000007d0a7c05a00e000000000000000000000000000000
+            00000000007c0aa6010000ab010000000000000000010074010000000000
+            00000000006a0f00000000000000006a1000000000000000006a11000000
+            00000000007401000000000000000000006a0f00000000000000006a1000
+            000000000000006a1200000000000000007c058e0066017c01640564069c
+            027c03a4018e015300
+          90           0 RESUME                   0
          
-          82           2 LOAD_GLOBAL              1 (NULL + torch)
+          92           2 LOAD_GLOBAL              1 (NULL + torch)
                       14 LOAD_ATTR                1 (FloatTensor)
-                      24 LOAD_FAST                0 (adata)
-                      26 LOAD_ATTR                2 (X)
-                      36 LOAD_METHOD              3 (todense)
-                      58 PRECALL                  0
-                      62 CALL                     0
-                      72 PRECALL                  1
-                      76 CALL                     1
-                      86 STORE_FAST               3 (genes)
-         
-          83          88 LOAD_FAST                3 (genes)
-                      90 BUILD_LIST               1
-                      92 STORE_FAST               4 (params)
-         
-          84          94 BUILD_LIST               0
-                      96 STORE_FAST               5 (context_tensors)
-         
-          85          98 LOAD_FAST                2 (context_discrete_keys)
-                     100 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 106)
-         
-          86         102 BUILD_LIST               0
-                     104 STORE_FAST               2 (context_discrete_keys)
-         
-          88     >>  106 LOAD_FAST                2 (context_discrete_keys)
-                     108 GET_ITER
-                 >>  110 FOR_ITER               160 (to 432)
-                     112 STORE_FAST               6 (key)
-         
-          89         114 LOAD_GLOBAL              1 (NULL + torch)
-                     126 LOAD_ATTR                4 (IntTensor)
-                     136 LOAD_FAST                0 (adata)
-                     138 LOAD_ATTR                5 (obs)
-                     148 LOAD_FAST                6 (key)
-                     150 BINARY_SUBSCR
-                     160 LOAD_METHOD              6 (astype)
-                     182 LOAD_CONST               1 ('category')
-                     184 PRECALL                  1
-                     188 CALL                     1
-                     198 LOAD_ATTR                7 (cat)
-                     208 LOAD_ATTR                8 (codes)
-                     218 LOAD_ATTR                9 (values)
-                     228 PRECALL                  1
-                     232 CALL                     1
-                     242 LOAD_METHOD             10 (long)
-                     264 PRECALL                  0
-                     268 CALL                     0
-                     278 STORE_FAST               7 (t)
-         
-          90         280 LOAD_GLOBAL              0 (torch)
-                     292 LOAD_ATTR               11 (nn)
-                     302 LOAD_ATTR               12 (functional)
-                     312 LOAD_METHOD             13 (one_hot)
-                     334 LOAD_FAST                7 (t)
-                     336 PRECALL                  1
-                     340 CALL                     1
-                     350 LOAD_METHOD             14 (float)
-                     372 PRECALL                  0
-                     376 CALL                     0
-                     386 STORE_FAST               8 (encoded)
-         
-          91         388 LOAD_FAST                5 (context_tensors)
-                     390 LOAD_METHOD             15 (append)
-                     412 LOAD_FAST                8 (encoded)
-                     414 PRECALL                  1
-                     418 CALL                     1
-                     428 POP_TOP
-                     430 JUMP_BACKWARD          161 (to 110)
-         
-          93     >>  432 LOAD_FAST                5 (context_tensors)
-                     434 POP_JUMP_FORWARD_IF_FALSE    43 (to 522)
-         
-          94         436 LOAD_GLOBAL              1 (NULL + torch)
-                     448 LOAD_ATTR                7 (cat)
-                     458 LOAD_FAST                5 (context_tensors)
-                     460 LOAD_CONST               2 (-1)
-                     462 KW_NAMES                 3
-                     464 PRECALL                  2
-                     468 CALL                     2
-                     478 STORE_FAST               9 (context)
-         
-          95         480 LOAD_FAST                4 (params)
-                     482 LOAD_METHOD             15 (append)
-                     504 LOAD_FAST                9 (context)
-                     506 PRECALL                  1
-                     510 CALL                     1
-                     520 POP_TOP
-         
-          97     >>  522 LOAD_GLOBAL              0 (torch)
-                     534 LOAD_ATTR               16 (utils)
-                     544 LOAD_ATTR               17 (data)
-                     554 LOAD_METHOD             18 (DataLoader)
-         
-          98         576 LOAD_GLOBAL              1 (NULL + torch)
-                     588 LOAD_ATTR               16 (utils)
-                     598 LOAD_ATTR               17 (data)
-                     608 LOAD_ATTR               19 (TensorDataset)
-                     618 LOAD_FAST                4 (params)
-                     620 CALL_FUNCTION_EX         0
-         
-          99         622 LOAD_FAST                1 (batch_size)
-         
-         100         624 LOAD_CONST               4 (True)
-         
-          97         626 KW_NAMES                 5
-                     628 PRECALL                  3
-                     632 CALL                     3
-                     642 RETURN_VALUE
+                      24 LOAD_GLOBAL              5 (NULL + get_dense_X)
+                      36 LOAD_FAST                0 (adata)
+                      38 PRECALL                  1
+                      42 CALL                     1
+                      52 PRECALL                  1
+                      56 CALL                     1
+                      66 STORE_FAST               4 (genes)
+         
+          93          68 LOAD_FAST                4 (genes)
+                      70 BUILD_LIST               1
+                      72 STORE_FAST               5 (params)
+         
+          94          74 BUILD_LIST               0
+                      76 STORE_FAST               6 (context_tensors)
+         
+          95          78 LOAD_FAST                2 (context_discrete_keys)
+                      80 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 86)
+         
+          96          82 BUILD_LIST               0
+                      84 STORE_FAST               2 (context_discrete_keys)
+         
+          98     >>   86 LOAD_FAST                2 (context_discrete_keys)
+                      88 GET_ITER
+                 >>   90 FOR_ITER               160 (to 412)
+                      92 STORE_FAST               7 (key)
+         
+          99          94 LOAD_GLOBAL              1 (NULL + torch)
+                     106 LOAD_ATTR                3 (IntTensor)
+                     116 LOAD_FAST                0 (adata)
+                     118 LOAD_ATTR                4 (obs)
+                     128 LOAD_FAST                7 (key)
+                     130 BINARY_SUBSCR
+                     140 LOAD_METHOD              5 (astype)
+                     162 LOAD_CONST               2 ('category')
+                     164 PRECALL                  1
+                     168 CALL                     1
+                     178 LOAD_ATTR                6 (cat)
+                     188 LOAD_ATTR                7 (codes)
+                     198 LOAD_ATTR                8 (values)
+                     208 PRECALL                  1
+                     212 CALL                     1
+                     222 LOAD_METHOD              9 (long)
+                     244 PRECALL                  0
+                     248 CALL                     0
+                     258 STORE_FAST               8 (t)
+         
+         100         260 LOAD_GLOBAL              0 (torch)
+                     272 LOAD_ATTR               10 (nn)
+                     282 LOAD_ATTR               11 (functional)
+                     292 LOAD_METHOD             12 (one_hot)
+                     314 LOAD_FAST                8 (t)
+                     316 PRECALL                  1
+                     320 CALL                     1
+                     330 LOAD_METHOD             13 (float)
+                     352 PRECALL                  0
+                     356 CALL                     0
+                     366 STORE_FAST               9 (encoded)
+         
+         101         368 LOAD_FAST                6 (context_tensors)
+                     370 LOAD_METHOD             14 (append)
+                     392 LOAD_FAST                9 (encoded)
+                     394 PRECALL                  1
+                     398 CALL                     1
+                     408 POP_TOP
+                     410 JUMP_BACKWARD          161 (to 90)
+         
+         103     >>  412 LOAD_FAST                6 (context_tensors)
+                     414 POP_JUMP_FORWARD_IF_FALSE    43 (to 502)
+         
+         104         416 LOAD_GLOBAL              1 (NULL + torch)
+                     428 LOAD_ATTR                6 (cat)
+                     438 LOAD_FAST                6 (context_tensors)
+                     440 LOAD_CONST               3 (-1)
+                     442 KW_NAMES                 4
+                     444 PRECALL                  2
+                     448 CALL                     2
+                     458 STORE_FAST              10 (context)
+         
+         105         460 LOAD_FAST                5 (params)
+                     462 LOAD_METHOD             14 (append)
+                     484 LOAD_FAST               10 (context)
+                     486 PRECALL                  1
+                     490 CALL                     1
+                     500 POP_TOP
+         
+         107     >>  502 LOAD_GLOBAL              1 (NULL + torch)
+                     514 LOAD_ATTR               15 (utils)
+                     524 LOAD_ATTR               16 (data)
+                     534 LOAD_ATTR               17 (DataLoader)
+         
+         108         544 LOAD_GLOBAL              1 (NULL + torch)
+                     556 LOAD_ATTR               15 (utils)
+                     566 LOAD_ATTR               16 (data)
+                     576 LOAD_ATTR               18 (TensorDataset)
+                     586 LOAD_FAST                5 (params)
+                     588 CALL_FUNCTION_EX         0
+         
+         107         590 BUILD_TUPLE              1
+         
+         109         592 LOAD_FAST                1 (batch_size)
+         
+         110         594 LOAD_CONST               5 (True)
+         
+         107         596 LOAD_CONST               6 (('batch_size', 'shuffle'))
+                     598 BUILD_CONST_KEY_MAP      2
+         
+         111         600 LOAD_FAST                3 (kwargs)
+         
+         107         602 DICT_MERGE               1
+                     604 CALL_FUNCTION_EX         1
+                     606 RETURN_VALUE
          consts
+            'Create a PyTorch DataLoader from an AnnData object.'
             None
             'category'
             -1
             ('dim',)
             True
             ('batch_size', 'shuffle')
-         names      ('torch', 'FloatTensor', 'X', 'todense', 'IntTensor', 'obs', 'astype', 'cat', 'codes', 'values', 'long', 'nn', 'functional', 'one_hot', 'float', 'append', 'utils', 'data', 'DataLoader', 'TensorDataset')
-         varnames   ('adata', 'batch_size', 'context_discrete_keys', 'genes', 'params', 'context_tensors', 'key', 't', 'encoded', 'context')
+         names      ('torch', 'FloatTensor', 'get_dense_X', 'IntTensor', 'obs', 'astype', 'cat', 'codes', 'values', 'long', 'nn', 'functional', 'one_hot', 'float', 'append', 'utils', 'data', 'DataLoader', 'TensorDataset')
+         varnames   ('adata', 'batch_size', 'context_discrete_keys', 'kwargs', 'genes', 'params', 'context_tensors', 'key', 't', 'encoded', 'context')
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py'
          name       'make_data_loader_from_adata'
-         firstlineno 81
+         firstlineno 90
          lnotab
-            0x0201560106010401040104020801a6016c012c0204012c012a0236012e
-            01020102fd
+            0x0202420106010401040104020801a6016c012c0204012c012a022a012e
+            ff0202020102fd040402fc
       (None,)
       (False,)
       (64, None)
-   names      ('logging', 'os', 'time', 'randomname', 'torch', 'torch.nn.functional', 'torch.utils.data', 'decipher.tools._decipher', 'Decipher', 'DecipherConfig', 'decipher.utils', 'DECIPHER_GLOBALS', 'create_decipher_uns_key', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'get_random_name', 'decipher_save_model', 'decipher_load_model', 'make_data_loader_from_adata')
+   names      ('logging', 'os', 'time', 'numpy', 'np', 'randomname', 'torch', 'torch.distributions', 'torch.nn.functional', 'torch.utils.data', 'decipher.tools._decipher', 'Decipher', 'DecipherConfig', 'decipher.utils', 'DECIPHER_GLOBALS', 'create_decipher_uns_key', 'getLogger', '__name__', 'logger', 'basicConfig', 'INFO', 'get_dense_X', 'get_random_name', 'decipher_save_model', 'decipher_load_model', 'make_data_loader_from_adata')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/data.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/data.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010801080208010801080108021001100220010e0102010c
-      fe1206080b0815061d
+      0x00ff02010801080108020801080108010801080108021001100220010e
+      0102010cfe12060607080b0815061d
```

### Comparing `scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/decipher.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/decipher.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,25 +1,25 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
-files sz: 6399
+moddate:  0x16232166 (Thu Apr 18 13:41:42 2024 UTC)
+files sz: 6596
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c006d015a010100640064036c026d
-      035a036d045a040100640064016c055a06640064016c075a07640064016c
-      086d095a0a0100640064016c0b6d0c5a0c0100640064016c0d5a0d640064
-      016c0e6d0f5a0f0100640064016c105a0d640064046c116d125a12010064
-      0064056c136d145a146d155a150100640064066c166d175a170100020065
-      016407ac08a6010000ab0100000000000000000200470064098400640aa6
-      020000ab020000000000000000a6000000ab0000000000000000005a1802
-      004700640b8400640c650f6a190000000000000000a6030000ab03000000
-      00000000005a1a64015300
+      035a036d045a046d055a050100640064016c065a07640064016c085a0864
+      0064016c096d0a5a0b0100640064016c0c6d0d5a0d0100640064016c0e5a
+      0e640064016c0f6d105a100100640064016c115a0e640064046c126d135a
+      130100640064056c146d155a156d165a160100640064066c176d185a1801
+      00020065016407ac08a6010000ab01000000000000000002004700640984
+      00640aa6020000ab020000000000000000a6000000ab0000000000000000
+      005a1902004700640b8400640c65106a1a0000000000000000a6030000ab
+      0300000000000000005a1b64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (dataclasses)
                  8 STORE_NAME               0 (dataclasses)
    
@@ -27,123 +27,125 @@
                 12 LOAD_CONST               2 (('dataclass',))
                 14 IMPORT_NAME              0 (dataclasses)
                 16 IMPORT_FROM              1 (dataclass)
                 18 STORE_NAME               1 (dataclass)
                 20 POP_TOP
    
      3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               3 (('Sequence', 'Union'))
+                24 LOAD_CONST               3 (('Optional', 'Sequence', 'Union'))
                 26 IMPORT_NAME              2 (typing)
-                28 IMPORT_FROM              3 (Sequence)
-                30 STORE_NAME               3 (Sequence)
-                32 IMPORT_FROM              4 (Union)
-                34 STORE_NAME               4 (Union)
-                36 POP_TOP
+                28 IMPORT_FROM              3 (Optional)
+                30 STORE_NAME               3 (Optional)
+                32 IMPORT_FROM              4 (Sequence)
+                34 STORE_NAME               4 (Sequence)
+                36 IMPORT_FROM              5 (Union)
+                38 STORE_NAME               5 (Union)
+                40 POP_TOP
    
-     5          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               1 (None)
-                42 IMPORT_NAME              5 (numpy)
-                44 STORE_NAME               6 (np)
+     5          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               1 (None)
+                46 IMPORT_NAME              6 (numpy)
+                48 STORE_NAME               7 (np)
    
-     6          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               1 (None)
-                50 IMPORT_NAME              7 (pyro)
-                52 STORE_NAME               7 (pyro)
+     6          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               1 (None)
+                54 IMPORT_NAME              8 (pyro)
+                56 STORE_NAME               8 (pyro)
    
-     7          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               1 (None)
-                58 IMPORT_NAME              8 (pyro.distributions)
-                60 IMPORT_FROM              9 (distributions)
-                62 STORE_NAME              10 (dist)
-                64 POP_TOP
+     7          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               1 (None)
+                62 IMPORT_NAME              9 (pyro.distributions)
+                64 IMPORT_FROM             10 (distributions)
+                66 STORE_NAME              11 (dist)
+                68 POP_TOP
    
-     8          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               1 (None)
-                70 IMPORT_NAME             11 (pyro.poutine)
-                72 IMPORT_FROM             12 (poutine)
-                74 STORE_NAME              12 (poutine)
-                76 POP_TOP
+     8          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               1 (None)
+                74 IMPORT_NAME             12 (pyro.poutine)
+                76 IMPORT_FROM             13 (poutine)
+                78 STORE_NAME              13 (poutine)
+                80 POP_TOP
    
-     9          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               1 (None)
-                82 IMPORT_NAME             13 (torch)
-                84 STORE_NAME              13 (torch)
+     9          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               1 (None)
+                86 IMPORT_NAME             14 (torch)
+                88 STORE_NAME              14 (torch)
    
-    10          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               1 (None)
-                90 IMPORT_NAME             14 (torch.nn)
-                92 IMPORT_FROM             15 (nn)
-                94 STORE_NAME              15 (nn)
-                96 POP_TOP
+    10          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               1 (None)
+                94 IMPORT_NAME             15 (torch.nn)
+                96 IMPORT_FROM             16 (nn)
+                98 STORE_NAME              16 (nn)
+               100 POP_TOP
    
-    11          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               1 (None)
-               102 IMPORT_NAME             16 (torch.utils.data)
-               104 STORE_NAME              13 (torch)
+    11         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               1 (None)
+               106 IMPORT_NAME             17 (torch.utils.data)
+               108 STORE_NAME              14 (torch)
    
-    12         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               4 (('constraints',))
-               110 IMPORT_NAME             17 (torch.distributions)
-               112 IMPORT_FROM             18 (constraints)
-               114 STORE_NAME              18 (constraints)
-               116 POP_TOP
+    12         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               4 (('constraints',))
+               114 IMPORT_NAME             18 (torch.distributions)
+               116 IMPORT_FROM             19 (constraints)
+               118 STORE_NAME              19 (constraints)
+               120 POP_TOP
    
-    13         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               5 (('softmax', 'softplus'))
-               122 IMPORT_NAME             19 (torch.nn.functional)
-               124 IMPORT_FROM             20 (softmax)
-               126 STORE_NAME              20 (softmax)
-               128 IMPORT_FROM             21 (softplus)
-               130 STORE_NAME              21 (softplus)
-               132 POP_TOP
+    13         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST               5 (('softmax', 'softplus'))
+               126 IMPORT_NAME             20 (torch.nn.functional)
+               128 IMPORT_FROM             21 (softmax)
+               130 STORE_NAME              21 (softmax)
+               132 IMPORT_FROM             22 (softplus)
+               134 STORE_NAME              22 (softplus)
+               136 POP_TOP
    
-    15         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST               6 (('ConditionalDenseNN',))
-               138 IMPORT_NAME             22 (decipher.tools._decipher.module)
-               140 IMPORT_FROM             23 (ConditionalDenseNN)
-               142 STORE_NAME              23 (ConditionalDenseNN)
-               144 POP_TOP
+    15         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST               6 (('ConditionalDenseNN',))
+               142 IMPORT_NAME             23 (decipher.tools._decipher.module)
+               144 IMPORT_FROM             24 (ConditionalDenseNN)
+               146 STORE_NAME              24 (ConditionalDenseNN)
+               148 POP_TOP
    
-    18         146 PUSH_NULL
-               148 LOAD_NAME                1 (dataclass)
-               150 LOAD_CONST               7 (True)
-               152 KW_NAMES                 8
-               154 PRECALL                  1
-               158 CALL                     1
+    18         150 PUSH_NULL
+               152 LOAD_NAME                1 (dataclass)
+               154 LOAD_CONST               7 (True)
+               156 KW_NAMES                 8
+               158 PRECALL                  1
+               162 CALL                     1
    
-    19         168 PUSH_NULL
-               170 LOAD_BUILD_CLASS
-               172 LOAD_CONST               9 (<code object DecipherConfig, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 18>)
-               174 MAKE_FUNCTION            0
-               176 LOAD_CONST              10 ('DecipherConfig')
-               178 PRECALL                  2
-               182 CALL                     2
+    19         172 PUSH_NULL
+               174 LOAD_BUILD_CLASS
+               176 LOAD_CONST               9 (<code object DecipherConfig, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 18>)
+               178 MAKE_FUNCTION            0
+               180 LOAD_CONST              10 ('DecipherConfig')
+               182 PRECALL                  2
+               186 CALL                     2
    
-    18         192 PRECALL                  0
-               196 CALL                     0
+    18         196 PRECALL                  0
+               200 CALL                     0
    
-    19         206 STORE_NAME              24 (DecipherConfig)
+    19         210 STORE_NAME              25 (DecipherConfig)
    
-    51         208 PUSH_NULL
-               210 LOAD_BUILD_CLASS
-               212 LOAD_CONST              11 (<code object Decipher, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 51>)
-               214 MAKE_FUNCTION            0
-               216 LOAD_CONST              12 ('Decipher')
-               218 LOAD_NAME               15 (nn)
-               220 LOAD_ATTR               25 (Module)
-               230 PRECALL                  3
-               234 CALL                     3
-               244 STORE_NAME              26 (Decipher)
-               246 LOAD_CONST               1 (None)
-               248 RETURN_VALUE
+    52         212 PUSH_NULL
+               214 LOAD_BUILD_CLASS
+               216 LOAD_CONST              11 (<code object Decipher, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 52>)
+               218 MAKE_FUNCTION            0
+               220 LOAD_CONST              12 ('Decipher')
+               222 LOAD_NAME               16 (nn)
+               224 LOAD_ATTR               26 (Module)
+               234 PRECALL                  3
+               238 CALL                     3
+               248 STORE_NAME              27 (Decipher)
+               250 LOAD_CONST               1 (None)
+               252 RETURN_VALUE
    consts
       0
       None
       ('dataclass',)
-      ('Sequence', 'Union')
+      ('Optional', 'Sequence', 'Union')
       ('constraints',)
       ('softmax', 'softplus')
       ('ConditionalDenseNN',)
       True
       ('unsafe_hash',)
       code
          argcount  : 0
@@ -152,18 +154,18 @@
          flags     : 0
          code
             0x970065005a0164005a02550064015a036504650564023c00000064035a
             066504650564043c00000064055a076508650564063c00000002006509a6
             000000ab0000000000000000005a0a6508650564073c00000064085a0b65
             0c650564093c000000640a5a0d65046505640b3c000000640c5a0e650c65
             05640d3c00000064085a0f650c6505640e3c000000640f5a106504650564
-            103c00000064115a116504650564123c00000064135a126504650564143c
-            00000064135a136504650564153c00000064165a146515650564173c0000
-            0064185a166517650564193c000000641a84005a18641b84005a19641353
-            00
+            103c00000064115a116504650564123c00000064015a1265136504190000
+            00000000000000650564133c00000064145a146504650564153c00000064
+            145a156504650564163c00000064175a166517650564183c00000064195a
+            1865196505641a3c000000641b84005a1a641c84005a1b64145300
           18           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DecipherConfig')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
@@ -229,58 +231,67 @@
           30         140 LOAD_CONST              15 (64)
                      142 STORE_NAME              16 (batch_size)
                      144 LOAD_NAME                4 (int)
                      146 LOAD_NAME                5 (__annotations__)
                      148 LOAD_CONST              16 ('batch_size')
                      150 STORE_SUBSCR
          
-          31         154 LOAD_CONST              17 (100)
+          31         154 LOAD_CONST              17 (1000)
                      156 STORE_NAME              17 (n_epochs)
                      158 LOAD_NAME                4 (int)
                      160 LOAD_NAME                5 (__annotations__)
                      162 LOAD_CONST              18 ('n_epochs')
                      164 STORE_SUBSCR
          
-          33         168 LOAD_CONST              19 (None)
-                     170 STORE_NAME              18 (dim_genes)
-                     172 LOAD_NAME                4 (int)
-                     174 LOAD_NAME                5 (__annotations__)
-                     176 LOAD_CONST              20 ('dim_genes')
-                     178 STORE_SUBSCR
-         
-          34         182 LOAD_CONST              19 (None)
-                     184 STORE_NAME              19 (n_cells)
-                     186 LOAD_NAME                4 (int)
-                     188 LOAD_NAME                5 (__annotations__)
-                     190 LOAD_CONST              21 ('n_cells')
-                     192 STORE_SUBSCR
-         
-          35         196 LOAD_CONST              22 ('normal')
-                     198 STORE_NAME              20 (prior)
-                     200 LOAD_NAME               21 (str)
-                     202 LOAD_NAME                5 (__annotations__)
-                     204 LOAD_CONST              23 ('prior')
-                     206 STORE_SUBSCR
-         
-          37         210 LOAD_CONST              24 (False)
-                     212 STORE_NAME              22 (_initialized_from_adata)
-                     214 LOAD_NAME               23 (bool)
-                     216 LOAD_NAME                5 (__annotations__)
-                     218 LOAD_CONST              25 ('_initialized_from_adata')
-                     220 STORE_SUBSCR
-         
-          39         224 LOAD_CONST              26 (<code object initialize_from_adata, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 39>)
-                     226 MAKE_FUNCTION            0
-                     228 STORE_NAME              24 (initialize_from_adata)
-         
-          44         230 LOAD_CONST              27 (<code object to_dict, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 44>)
-                     232 MAKE_FUNCTION            0
-                     234 STORE_NAME              25 (to_dict)
-                     236 LOAD_CONST              19 (None)
-                     238 RETURN_VALUE
+          32         168 LOAD_CONST               1 (10)
+                     170 STORE_NAME              18 (early_stopping_patience)
+                     172 LOAD_NAME               19 (Optional)
+                     174 LOAD_NAME                4 (int)
+                     176 BINARY_SUBSCR
+                     186 LOAD_NAME                5 (__annotations__)
+                     188 LOAD_CONST              19 ('early_stopping_patience')
+                     190 STORE_SUBSCR
+         
+          34         194 LOAD_CONST              20 (None)
+                     196 STORE_NAME              20 (dim_genes)
+                     198 LOAD_NAME                4 (int)
+                     200 LOAD_NAME                5 (__annotations__)
+                     202 LOAD_CONST              21 ('dim_genes')
+                     204 STORE_SUBSCR
+         
+          35         208 LOAD_CONST              20 (None)
+                     210 STORE_NAME              21 (n_cells)
+                     212 LOAD_NAME                4 (int)
+                     214 LOAD_NAME                5 (__annotations__)
+                     216 LOAD_CONST              22 ('n_cells')
+                     218 STORE_SUBSCR
+         
+          36         222 LOAD_CONST              23 ('normal')
+                     224 STORE_NAME              22 (prior)
+                     226 LOAD_NAME               23 (str)
+                     228 LOAD_NAME                5 (__annotations__)
+                     230 LOAD_CONST              24 ('prior')
+                     232 STORE_SUBSCR
+         
+          38         236 LOAD_CONST              25 (False)
+                     238 STORE_NAME              24 (_initialized_from_adata)
+                     240 LOAD_NAME               25 (bool)
+                     242 LOAD_NAME                5 (__annotations__)
+                     244 LOAD_CONST              26 ('_initialized_from_adata')
+                     246 STORE_SUBSCR
+         
+          40         250 LOAD_CONST              27 (<code object initialize_from_adata, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 40>)
+                     252 MAKE_FUNCTION            0
+                     254 STORE_NAME              26 (initialize_from_adata)
+         
+          45         256 LOAD_CONST              28 (<code object to_dict, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 45>)
+                     258 MAKE_FUNCTION            0
+                     260 STORE_NAME              27 (to_dict)
+                     262 LOAD_CONST              20 (None)
+                     264 RETURN_VALUE
          consts
             'DecipherConfig'
             10
             'dim_z'
             2
             'dim_v'
             (64,)
@@ -291,16 +302,17 @@
             0
             'seed'
             0.005
             'learning_rate'
             'val_frac'
             64
             'batch_size'
-            100
+            1000
             'n_epochs'
+            'early_stopping_patience'
             None
             'dim_genes'
             'n_cells'
             'normal'
             'prior'
             False
             '_initialized_from_adata'
@@ -310,752 +322,794 @@
                stacksize : 2
                flags     : 3
                code
                   0x97007c016a0000000000000000006401190000000000000000007c005f
                   0100000000000000007c016a000000000000000000640219000000000000
                   0000007c005f02000000000000000064037c005f03000000000000000064
                   005300
-                39           0 RESUME                   0
+                40           0 RESUME                   0
                
-                40           2 LOAD_FAST                1 (adata)
+                41           2 LOAD_FAST                1 (adata)
                              4 LOAD_ATTR                0 (shape)
                             14 LOAD_CONST               1 (1)
                             16 BINARY_SUBSCR
                             26 LOAD_FAST                0 (self)
                             28 STORE_ATTR               1 (dim_genes)
                
-                41          38 LOAD_FAST                1 (adata)
+                42          38 LOAD_FAST                1 (adata)
                             40 LOAD_ATTR                0 (shape)
                             50 LOAD_CONST               2 (0)
                             52 BINARY_SUBSCR
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               2 (n_cells)
                
-                42          74 LOAD_CONST               3 (True)
+                43          74 LOAD_CONST               3 (True)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               3 (_initialized_from_adata)
                             88 LOAD_CONST               0 (None)
                             90 RETURN_VALUE
                consts
                   None
                   1
                   0
                   True
                names      ('shape', 'dim_genes', 'n_cells', '_initialized_from_adata')
                varnames   ('self', 'adata')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       'initialize_from_adata'
-               firstlineno 39
+               firstlineno 40
                lnotab 0x020124012401
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c00a60100
                   00ab0100000000000000007d017405000000000000000000007c01640119
                   000000000000000000a6010000ab0100000000000000007c0164013c0000
                   007405000000000000000000007c01640219000000000000000000a60100
                   00ab0100000000000000007c0164023c0000007c015300
-                44           0 RESUME                   0
+                45           0 RESUME                   0
                
-                45           2 LOAD_GLOBAL              1 (NULL + dataclasses)
+                46           2 LOAD_GLOBAL              1 (NULL + dataclasses)
                             14 LOAD_ATTR                1 (asdict)
                             24 LOAD_FAST                0 (self)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (res)
                
-                46          42 LOAD_GLOBAL              5 (NULL + list)
+                47          42 LOAD_GLOBAL              5 (NULL + list)
                             54 LOAD_FAST                1 (res)
                             56 LOAD_CONST               1 ('layers_v_to_z')
                             58 BINARY_SUBSCR
                             68 PRECALL                  1
                             72 CALL                     1
                             82 LOAD_FAST                1 (res)
                             84 LOAD_CONST               1 ('layers_v_to_z')
                             86 STORE_SUBSCR
                
-                47          90 LOAD_GLOBAL              5 (NULL + list)
+                48          90 LOAD_GLOBAL              5 (NULL + list)
                            102 LOAD_FAST                1 (res)
                            104 LOAD_CONST               2 ('layers_z_to_x')
                            106 BINARY_SUBSCR
                            116 PRECALL                  1
                            120 CALL                     1
                            130 LOAD_FAST                1 (res)
                            132 LOAD_CONST               2 ('layers_z_to_x')
                            134 STORE_SUBSCR
                
-                48         138 LOAD_FAST                1 (res)
+                49         138 LOAD_FAST                1 (res)
                            140 RETURN_VALUE
                consts
                   None
                   'layers_v_to_z'
                   'layers_z_to_x'
                names      ('dataclasses', 'asdict', 'list')
                varnames   ('self', 'res')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       'to_dict'
-               firstlineno 44
+               firstlineno 45
                lnotab 0x0201280130013001
-         names      ('__name__', '__module__', '__qualname__', 'dim_z', 'int', '__annotations__', 'dim_v', 'layers_v_to_z', 'Sequence', 'tuple', 'layers_z_to_x', 'beta', 'float', 'seed', 'learning_rate', 'val_frac', 'batch_size', 'n_epochs', 'dim_genes', 'n_cells', 'prior', 'str', '_initialized_from_adata', 'bool', 'initialize_from_adata', 'to_dict')
+         names      ('__name__', '__module__', '__qualname__', 'dim_z', 'int', '__annotations__', 'dim_v', 'layers_v_to_z', 'Sequence', 'tuple', 'layers_z_to_x', 'beta', 'float', 'seed', 'learning_rate', 'val_frac', 'batch_size', 'n_epochs', 'early_stopping_patience', 'Optional', 'dim_genes', 'n_cells', 'prior', 'str', '_initialized_from_adata', 'bool', 'initialize_from_adata', 'to_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
          name       'DecipherConfig'
          firstlineno 18
          lnotab
-            0x0c020e010e010e011e020e010e020e010e010e010e020e010e010e020e
-            020605
+            0x0c020e010e010e011e020e010e020e010e010e010e011a020e010e010e
+            020e020605
       'DecipherConfig'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a0264015a0302006504a6000000ab00000000
             000000000066016402650565046506660219000000000000000000660288
-            0066016403840d5a07640a640584015a08640a640684015a096407650a6a
-            0b00000000000000006602640884045a0c640984005a0d880078015a0e53
-            00
+            0066016403840d5a07650864048400a6000000ab0000000000000000005a
+            09640b640684015a0a640b640784015a0b6408650c6a0d00000000000000
+            006602640984045a0e640a84005a0f880078015a105300
                        0 MAKE_CELL                0 (__class__)
          
-          51           2 RESUME                   0
+          52           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Decipher')
                       10 STORE_NAME               2 (__qualname__)
          
-          52          12 LOAD_CONST               1 ('Decipher _decipher for single-cell data.\n\n    Parameters\n    ----------\n    config : DecipherConfig or dict\n        Configuration for the decipher _decipher.\n    ')
+          53          12 LOAD_CONST               1 ('Decipher _decipher for single-cell data.\n\n    Parameters\n    ----------\n    config : DecipherConfig or dict\n        Configuration for the decipher _decipher.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          62          16 PUSH_NULL
+          63          16 PUSH_NULL
                       18 LOAD_NAME                4 (DecipherConfig)
                       20 PRECALL                  0
                       24 CALL                     0
          
-          60          34 BUILD_TUPLE              1
+          61          34 BUILD_TUPLE              1
                       36 LOAD_CONST               2 ('config')
          
-          62          38 LOAD_NAME                5 (Union)
+          63          38 LOAD_NAME                5 (Union)
                       40 LOAD_NAME                4 (DecipherConfig)
                       42 LOAD_NAME                6 (dict)
                       44 BUILD_TUPLE              2
                       46 BINARY_SUBSCR
          
-          60          56 BUILD_TUPLE              2
+          61          56 BUILD_TUPLE              2
                       58 LOAD_CLOSURE             0 (__class__)
                       60 BUILD_TUPLE              1
-                      62 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 60>)
+                      62 LOAD_CONST               3 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 61>)
                       64 MAKE_FUNCTION           13 (defaults, annotations, closure)
                       66 STORE_NAME               7 (__init__)
          
-          94          68 LOAD_CONST              10 ((None,))
-                      70 LOAD_CONST               5 (<code object model, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 94>)
-                      72 MAKE_FUNCTION            1 (defaults)
-                      74 STORE_NAME               8 (model)
-         
-         130          76 LOAD_CONST              10 ((None,))
-                      78 LOAD_CONST               6 (<code object guide, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 130>)
-                      80 MAKE_FUNCTION            1 (defaults)
-                      82 STORE_NAME               9 (guide)
-         
-         153          84 LOAD_CONST               7 ('x')
-                      86 LOAD_NAME               10 (np)
-                      88 LOAD_ATTR               11 (array)
-                      98 BUILD_TUPLE              2
-                     100 LOAD_CONST               8 (<code object compute_v_z_numpy, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 153>)
-                     102 MAKE_FUNCTION            4 (annotations)
-                     104 STORE_NAME              12 (compute_v_z_numpy)
-         
-         177         106 LOAD_CONST               9 (<code object impute_gene_expression_numpy, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py", line 177>)
-                     108 MAKE_FUNCTION            0
-                     110 STORE_NAME              13 (impute_gene_expression_numpy)
-                     112 LOAD_CLOSURE             0 (__class__)
-                     114 COPY                     1
-                     116 STORE_NAME              14 (__classcell__)
-                     118 RETURN_VALUE
+          97          68 LOAD_NAME                8 (property)
+         
+          98          70 LOAD_CONST               4 (<code object device, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 97>)
+                      72 MAKE_FUNCTION            0
+         
+          97          74 PRECALL                  0
+                      78 CALL                     0
+         
+          98          88 STORE_NAME               9 (device)
+         
+         101          90 LOAD_CONST              11 ((None,))
+                      92 LOAD_CONST               6 (<code object model, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 101>)
+                      94 MAKE_FUNCTION            1 (defaults)
+                      96 STORE_NAME              10 (model)
+         
+         137          98 LOAD_CONST              11 ((None,))
+                     100 LOAD_CONST               7 (<code object guide, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 137>)
+                     102 MAKE_FUNCTION            1 (defaults)
+                     104 STORE_NAME              11 (guide)
+         
+         160         106 LOAD_CONST               8 ('x')
+                     108 LOAD_NAME               12 (np)
+                     110 LOAD_ATTR               13 (array)
+                     120 BUILD_TUPLE              2
+                     122 LOAD_CONST               9 (<code object compute_v_z_numpy, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 160>)
+                     124 MAKE_FUNCTION            4 (annotations)
+                     126 STORE_NAME              14 (compute_v_z_numpy)
+         
+         184         128 LOAD_CONST              10 (<code object impute_gene_expression_numpy, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py", line 184>)
+                     130 MAKE_FUNCTION            0
+                     132 STORE_NAME              15 (impute_gene_expression_numpy)
+                     134 LOAD_CLOSURE             0 (__class__)
+                     136 COPY                     1
+                     138 STORE_NAME              16 (__classcell__)
+                     140 RETURN_VALUE
          consts
             'Decipher'
             'Decipher _decipher for single-cell data.\n\n    Parameters\n    ----------\n    config : DecipherConfig or dict\n        Configuration for the decipher _decipher.\n    '
             'config'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 6
                flags     : 3
                code
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a0010000000000000000000000000000000000000000a6000000ab0000
-                  0000000000000001007405000000000000000000007c01a6010000ab0100
-                  000000000000007406000000000000000000006b0200000000720c740900
-                  000000000000000000640669007c01a4018e017d017c016a050000000000
-                  000000730f740d000000000000000000006401a6010000ab010000000000
-                  00000082017c017c005f0700000000000000007411000000000000000000
-                  007c006a0700000000000000006a0900000000000000007c006a07000000
-                  00000000006a0a00000000000000007c006a0700000000000000006a0b00
-                  00000000000000670164027a050000a6030000ab0300000000000000007c
-                  005f0c00000000000000007411000000000000000000007c006a07000000
-                  00000000006a0b00000000000000007c016a0d00000000000000007c006a
-                  0700000000000000006a0e00000000000000006701a6030000ab03000000
-                  00000000007c005f0f00000000000000007411000000000000000000007c
-                  006a0700000000000000006a0e0000000000000000640367017c006a0700
-                  000000000000006a0b0000000000000000670164027a050000a6030000ab
-                  0300000000000000007c005f100000000000000000741100000000000000
-                  0000007c006a0700000000000000006a0e00000000000000007c006a0700
-                  000000000000006a0b00000000000000007a000000640367017c006a0700
-                  000000000000006a0900000000000000007c006a0700000000000000006a
-                  0900000000000000006702a6030000ab0300000000000000007c005f1100
-                  0000000000000064047c005f12000000000000000064007c005f13000000
-                  00000000007429000000000000000000006405a6010000ab010000000000
-                  000000010064005300
+                  0000000000000001007405000000000000000000007c0174060000000000
+                  0000000000a6020000ab020000000000000000720c740900000000000000
+                  000000640669007c01a4018e017d017c016a050000000000000000730f74
+                  0d000000000000000000006401a6010000ab01000000000000000082017c
+                  017c005f0700000000000000007411000000000000000000006a09000000
+                  00000000007415000000000000000000006a0b00000000000000006402a6
+                  010000ab010000000000000000a6010000ab0100000000000000007c005f
+                  0c0000000000000000741b000000000000000000007c006a070000000000
+                  0000006a0e00000000000000007c006a0700000000000000006a0f000000
+                  00000000007c006a0700000000000000006a100000000000000000670164
+                  037a050000a6030000ab0300000000000000007c005f1100000000000000
+                  00741b000000000000000000007c006a0700000000000000006a10000000
+                  00000000007c016a1200000000000000007c006a0700000000000000006a
+                  1300000000000000006701a6030000ab0300000000000000007c005f1400
+                  00000000000000741b000000000000000000007c006a0700000000000000
+                  006a130000000000000000640467017c006a0700000000000000006a1000
+                  00000000000000670164037a050000a6030000ab0300000000000000007c
+                  005f150000000000000000741b000000000000000000007c006a07000000
+                  00000000006a1300000000000000007c006a0700000000000000006a1000
+                  000000000000007a000000640467017c006a0700000000000000006a0e00
+                  000000000000007c006a0700000000000000006a0e000000000000000067
+                  02a6030000ab0300000000000000007c005f16000000000000000064057c
+                  005f17000000000000000064007c005f18000000000000000064005300
                              0 COPY_FREE_VARS           1
                
-                60           2 RESUME                   0
+                61           2 RESUME                   0
                
-                64           4 LOAD_GLOBAL              1 (NULL + super)
+                65           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (__init__)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 POP_TOP
                
-                65          68 LOAD_GLOBAL              5 (NULL + type)
+                66          68 LOAD_GLOBAL              5 (NULL + isinstance)
                             80 LOAD_FAST                1 (config)
-                            82 PRECALL                  1
-                            86 CALL                     1
-                            96 LOAD_GLOBAL              6 (dict)
-                           108 COMPARE_OP               2 (==)
-                           114 POP_JUMP_FORWARD_IF_FALSE    12 (to 140)
-               
-                66         116 LOAD_GLOBAL              9 (NULL + DecipherConfig)
-                           128 LOAD_CONST               6 (())
-                           130 BUILD_MAP                0
-                           132 LOAD_FAST                1 (config)
-                           134 DICT_MERGE               1
-                           136 CALL_FUNCTION_EX         1
-                           138 STORE_FAST               1 (config)
-               
-                68     >>  140 LOAD_FAST                1 (config)
-                           142 LOAD_ATTR                5 (_initialized_from_adata)
-                           152 POP_JUMP_FORWARD_IF_TRUE    15 (to 184)
-               
-                69         154 LOAD_GLOBAL             13 (NULL + ValueError)
-               
-                70         166 LOAD_CONST               1 ('DecipherConfig must be initialized from an AnnData object, use `DecipherConfig.initialize_from_adata(adata)` to do so.')
-               
-                69         168 PRECALL                  1
-                           172 CALL                     1
-                           182 RAISE_VARARGS            1
-               
-                74     >>  184 LOAD_FAST                1 (config)
-                           186 LOAD_FAST                0 (self)
-                           188 STORE_ATTR               7 (config)
-               
-                76         198 LOAD_GLOBAL             17 (NULL + ConditionalDenseNN)
-               
-                77         210 LOAD_FAST                0 (self)
-                           212 LOAD_ATTR                7 (config)
-                           222 LOAD_ATTR                9 (dim_v)
-                           232 LOAD_FAST                0 (self)
-                           234 LOAD_ATTR                7 (config)
-                           244 LOAD_ATTR               10 (layers_v_to_z)
-                           254 LOAD_FAST                0 (self)
-                           256 LOAD_ATTR                7 (config)
-                           266 LOAD_ATTR               11 (dim_z)
-                           276 BUILD_LIST               1
-                           278 LOAD_CONST               2 (2)
-                           280 BINARY_OP                5 (*)
-               
-                76         284 PRECALL                  3
-                           288 CALL                     3
-                           298 LOAD_FAST                0 (self)
-                           300 STORE_ATTR              12 (decoder_v_to_z)
-               
-                79         310 LOAD_GLOBAL             17 (NULL + ConditionalDenseNN)
-               
-                80         322 LOAD_FAST                0 (self)
-                           324 LOAD_ATTR                7 (config)
-                           334 LOAD_ATTR               11 (dim_z)
-                           344 LOAD_FAST                1 (config)
-                           346 LOAD_ATTR               13 (layers_z_to_x)
-                           356 LOAD_FAST                0 (self)
-                           358 LOAD_ATTR                7 (config)
-                           368 LOAD_ATTR               14 (dim_genes)
-                           378 BUILD_LIST               1
-               
-                79         380 PRECALL                  3
-                           384 CALL                     3
-                           394 LOAD_FAST                0 (self)
-                           396 STORE_ATTR              15 (decoder_z_to_x)
-               
-                82         406 LOAD_GLOBAL             17 (NULL + ConditionalDenseNN)
-               
-                83         418 LOAD_FAST                0 (self)
-                           420 LOAD_ATTR                7 (config)
-                           430 LOAD_ATTR               14 (dim_genes)
-                           440 LOAD_CONST               3 (128)
-                           442 BUILD_LIST               1
-                           444 LOAD_FAST                0 (self)
-                           446 LOAD_ATTR                7 (config)
-                           456 LOAD_ATTR               11 (dim_z)
-                           466 BUILD_LIST               1
-                           468 LOAD_CONST               2 (2)
-                           470 BINARY_OP                5 (*)
-               
-                82         474 PRECALL                  3
-                           478 CALL                     3
-                           488 LOAD_FAST                0 (self)
-                           490 STORE_ATTR              16 (encoder_x_to_z)
-               
-                85         500 LOAD_GLOBAL             17 (NULL + ConditionalDenseNN)
-               
-                86         512 LOAD_FAST                0 (self)
-                           514 LOAD_ATTR                7 (config)
-                           524 LOAD_ATTR               14 (dim_genes)
-                           534 LOAD_FAST                0 (self)
-                           536 LOAD_ATTR                7 (config)
-                           546 LOAD_ATTR               11 (dim_z)
-                           556 BINARY_OP                0 (+)
-                           560 LOAD_CONST               3 (128)
-                           562 BUILD_LIST               1
-                           564 LOAD_FAST                0 (self)
-                           566 LOAD_ATTR                7 (config)
-                           576 LOAD_ATTR                9 (dim_v)
-                           586 LOAD_FAST                0 (self)
-                           588 LOAD_ATTR                7 (config)
-                           598 LOAD_ATTR                9 (dim_v)
-                           608 BUILD_LIST               2
-               
-                85         610 PRECALL                  3
-                           614 CALL                     3
-                           624 LOAD_FAST                0 (self)
-                           626 STORE_ATTR              17 (encoder_zx_to_v)
-               
-                89         636 LOAD_CONST               4 (1e-05)
-                           638 LOAD_FAST                0 (self)
-                           640 STORE_ATTR              18 (_epsilon)
-               
-                91         650 LOAD_CONST               0 (None)
-                           652 LOAD_FAST                0 (self)
-                           654 STORE_ATTR              19 (theta)
-               
-                92         664 LOAD_GLOBAL             41 (NULL + print)
-                           676 LOAD_CONST               5 ('V5')
-                           678 PRECALL                  1
-                           682 CALL                     1
-                           692 POP_TOP
-                           694 LOAD_CONST               0 (None)
-                           696 RETURN_VALUE
+                            82 LOAD_GLOBAL              6 (dict)
+                            94 PRECALL                  2
+                            98 CALL                     2
+                           108 POP_JUMP_FORWARD_IF_FALSE    12 (to 134)
+               
+                67         110 LOAD_GLOBAL              9 (NULL + DecipherConfig)
+                           122 LOAD_CONST               6 (())
+                           124 BUILD_MAP                0
+                           126 LOAD_FAST                1 (config)
+                           128 DICT_MERGE               1
+                           130 CALL_FUNCTION_EX         1
+                           132 STORE_FAST               1 (config)
+               
+                69     >>  134 LOAD_FAST                1 (config)
+                           136 LOAD_ATTR                5 (_initialized_from_adata)
+                           146 POP_JUMP_FORWARD_IF_TRUE    15 (to 178)
+               
+                70         148 LOAD_GLOBAL             13 (NULL + ValueError)
+               
+                71         160 LOAD_CONST               1 ('DecipherConfig must be initialized from an AnnData object, use `DecipherConfig.initialize_from_adata(adata)` to do so.')
+               
+                70         162 PRECALL                  1
+                           166 CALL                     1
+                           176 RAISE_VARARGS            1
+               
+                75     >>  178 LOAD_FAST                1 (config)
+                           180 LOAD_FAST                0 (self)
+                           182 STORE_ATTR               7 (config)
+               
+                76         192 LOAD_GLOBAL             17 (NULL + nn)
+                           204 LOAD_ATTR                9 (Parameter)
+                           214 LOAD_GLOBAL             21 (NULL + torch)
+                           226 LOAD_ATTR               11 (empty)
+                           236 LOAD_CONST               2 (0)
+                           238 PRECALL                  1
+                           242 CALL                     1
+                           252 PRECALL                  1
+                           256 CALL                     1
+                           266 LOAD_FAST                0 (self)
+                           268 STORE_ATTR              12 (dummy_param)
+               
+                78         278 LOAD_GLOBAL             27 (NULL + ConditionalDenseNN)
+               
+                79         290 LOAD_FAST                0 (self)
+                           292 LOAD_ATTR                7 (config)
+                           302 LOAD_ATTR               14 (dim_v)
+                           312 LOAD_FAST                0 (self)
+                           314 LOAD_ATTR                7 (config)
+                           324 LOAD_ATTR               15 (layers_v_to_z)
+                           334 LOAD_FAST                0 (self)
+                           336 LOAD_ATTR                7 (config)
+                           346 LOAD_ATTR               16 (dim_z)
+                           356 BUILD_LIST               1
+                           358 LOAD_CONST               3 (2)
+                           360 BINARY_OP                5 (*)
+               
+                78         364 PRECALL                  3
+                           368 CALL                     3
+                           378 LOAD_FAST                0 (self)
+                           380 STORE_ATTR              17 (decoder_v_to_z)
+               
+                81         390 LOAD_GLOBAL             27 (NULL + ConditionalDenseNN)
+               
+                82         402 LOAD_FAST                0 (self)
+                           404 LOAD_ATTR                7 (config)
+                           414 LOAD_ATTR               16 (dim_z)
+                           424 LOAD_FAST                1 (config)
+                           426 LOAD_ATTR               18 (layers_z_to_x)
+                           436 LOAD_FAST                0 (self)
+                           438 LOAD_ATTR                7 (config)
+                           448 LOAD_ATTR               19 (dim_genes)
+                           458 BUILD_LIST               1
+               
+                81         460 PRECALL                  3
+                           464 CALL                     3
+                           474 LOAD_FAST                0 (self)
+                           476 STORE_ATTR              20 (decoder_z_to_x)
+               
+                84         486 LOAD_GLOBAL             27 (NULL + ConditionalDenseNN)
+               
+                85         498 LOAD_FAST                0 (self)
+                           500 LOAD_ATTR                7 (config)
+                           510 LOAD_ATTR               19 (dim_genes)
+                           520 LOAD_CONST               4 (128)
+                           522 BUILD_LIST               1
+                           524 LOAD_FAST                0 (self)
+                           526 LOAD_ATTR                7 (config)
+                           536 LOAD_ATTR               16 (dim_z)
+                           546 BUILD_LIST               1
+                           548 LOAD_CONST               3 (2)
+                           550 BINARY_OP                5 (*)
+               
+                84         554 PRECALL                  3
+                           558 CALL                     3
+                           568 LOAD_FAST                0 (self)
+                           570 STORE_ATTR              21 (encoder_x_to_z)
+               
+                87         580 LOAD_GLOBAL             27 (NULL + ConditionalDenseNN)
+               
+                88         592 LOAD_FAST                0 (self)
+                           594 LOAD_ATTR                7 (config)
+                           604 LOAD_ATTR               19 (dim_genes)
+                           614 LOAD_FAST                0 (self)
+                           616 LOAD_ATTR                7 (config)
+                           626 LOAD_ATTR               16 (dim_z)
+                           636 BINARY_OP                0 (+)
+               
+                89         640 LOAD_CONST               4 (128)
+                           642 BUILD_LIST               1
+               
+                90         644 LOAD_FAST                0 (self)
+                           646 LOAD_ATTR                7 (config)
+                           656 LOAD_ATTR               14 (dim_v)
+                           666 LOAD_FAST                0 (self)
+                           668 LOAD_ATTR                7 (config)
+                           678 LOAD_ATTR               14 (dim_v)
+                           688 BUILD_LIST               2
+               
+                87         690 PRECALL                  3
+                           694 CALL                     3
+                           704 LOAD_FAST                0 (self)
+                           706 STORE_ATTR              22 (encoder_zx_to_v)
+               
+                93         716 LOAD_CONST               5 (1e-05)
+                           718 LOAD_FAST                0 (self)
+                           720 STORE_ATTR              23 (_epsilon)
+               
+                95         730 LOAD_CONST               0 (None)
+                           732 LOAD_FAST                0 (self)
+                           734 STORE_ATTR              24 (theta)
+                           744 LOAD_CONST               0 (None)
+                           746 RETURN_VALUE
                consts
                   None
                   'DecipherConfig must be initialized from an AnnData object, use `DecipherConfig.initialize_from_adata(adata)` to do so.'
+                  0
                   2
                   128
                   1e-05
-                  'V5'
                   ()
-               names      ('super', '__init__', 'type', 'dict', 'DecipherConfig', '_initialized_from_adata', 'ValueError', 'config', 'ConditionalDenseNN', 'dim_v', 'layers_v_to_z', 'dim_z', 'decoder_v_to_z', 'layers_z_to_x', 'dim_genes', 'decoder_z_to_x', 'encoder_x_to_z', 'encoder_zx_to_v', '_epsilon', 'theta', 'print')
+               names      ('super', '__init__', 'isinstance', 'dict', 'DecipherConfig', '_initialized_from_adata', 'ValueError', 'config', 'nn', 'Parameter', 'torch', 'empty', 'dummy_param', 'ConditionalDenseNN', 'dim_v', 'layers_v_to_z', 'dim_z', 'decoder_v_to_z', 'layers_z_to_x', 'dim_genes', 'decoder_z_to_x', 'encoder_x_to_z', 'encoder_zx_to_v', '_epsilon', 'theta')
                varnames   ('self', 'config')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       '__init__'
-               firstlineno 60
+               firstlineno 61
                lnotab
-                  0x04044001300118020e010c0102ff10050e020c014aff1a030c013aff1a
-                  030c0138ff1a030c0162ff1a040e020e01
+                  0x040440012a0118020e010c0102ff10050e0156020c014aff1a030c013a
+                  ff1a030c0138ff1a030c01300104012efd1a060e02
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 1
+               flags     : 3
+               code 0x97007c006a0000000000000000006a0100000000000000005300
+                97           0 RESUME                   0
+               
+                99           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (dummy_param)
+                            14 LOAD_ATTR                1 (device)
+                            24 RETURN_VALUE
+               consts
+                  None
+               names      ('dummy_param', 'device')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
+               name       'device'
+               firstlineno 97
+               lnotab 0x0202
             None
             code
                argcount  : 3
                nlocals   : 12
                stacksize : 9
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c00a6
                   020000ab02000000000000000001007401000000000000000000006a0200
-                  00000000000000640264037c01a003000000000000000000000000000000
-                  00000000007c006a0400000000000000006a050000000000000000a60100
-                  00ab0100000000000000007a050000740c000000000000000000006a0700
-                  00000000000000ac04a6030000ab0300000000000000007c005f08000000
-                  00000000007401000000000000000000006a090000000000000000640574
-                  15000000000000000000007c01a6010000ab010000000000000000a60200
-                  00ab020000000000000000350001007417000000000000000000006a0c00
-                  000000000000006403ac06a6010000ab0100000000000000003500010074
-                  17000000000000000000006a0c00000000000000007c006a040000000000
-                  0000006a0d0000000000000000ac06a6010000ab01000000000000000035
-                  0001007c006a0400000000000000006a0e000000000000000064076b0200
-                  0000007246741f000000000000000000006a10000000000000000064087c
-                  01a00300000000000000000000000000000000000000007c006a04000000
-                  00000000006a110000000000000000a6010000ab010000000000000000a6
-                  020000ab020000000000000000a012000000000000000000000000000000
-                  00000000006409a6010000ab0100000000000000007d036e687c006a0400
-                  000000000000006a0e0000000000000000640a6b02000000007249741f00
-                  0000000000000000006a130000000000000000640b7c01a0030000000000
-                  0000000000000000000000000000007c006a0400000000000000006a1100
-                  00000000000000a6010000ab010000000000000000640c7a050000a60200
+                  0000000000000064027c01a0030000000000000000000000000000000000
+                  0000007c006a0400000000000000006a050000000000000000a6010000ab
+                  010000000000000000740c000000000000000000006a0700000000000000
+                  00ac03a6030000ab0300000000000000007c005f08000000000000000074
+                  01000000000000000000006a090000000000000000640474150000000000
+                  00000000007c01a6010000ab010000000000000000a6020000ab02000000
+                  0000000000350001007417000000000000000000006a0c00000000000000
+                  006405ac06a6010000ab0100000000000000003500010074170000000000
+                  00000000006a0c00000000000000007c006a0400000000000000006a0d00
+                  00000000000000ac06a6010000ab010000000000000000350001007c006a
+                  0400000000000000006a0e000000000000000064076b0200000000724674
+                  1f000000000000000000006a10000000000000000064087c01a003000000
+                  00000000000000000000000000000000007c006a0400000000000000006a
+                  110000000000000000a6010000ab010000000000000000a6020000ab0200
+                  00000000000000a012000000000000000000000000000000000000000064
+                  09a6010000ab0100000000000000007d036e687c006a0400000000000000
+                  006a0e0000000000000000640a6b02000000007249741f00000000000000
+                  0000006a130000000000000000640b7c01a0030000000000000000000000
+                  0000000000000000007c006a0400000000000000006a1100000000000000
+                  00a6010000ab010000000000000000640c7a050000a6020000ab02000000
+                  0000000000a01200000000000000000000000000000000000000006409a6
+                  010000ab0100000000000000007d036e0f74290000000000000000000064
+                  0da6010000ab01000000000000000082017401000000000000000000006a
+                  150000000000000000640e7c03a6020000ab0200000000000000007d0464
+                  0064006400a6020000ab02000000000000000001006e0b23003100730477
+                  0278035900770101005900010001007c00a0160000000000000000000000
+                  0000000000000000007c047c02ac0fa6020000ab0200000000000000005c
+                  0200007d057d06742f000000000000000000007c06a6010000ab01000000
+                  00000000007d067401000000000000000000006a15000000000000000064
+                  10741f000000000000000000006a1000000000000000007c057c06a60200
                   00ab020000000000000000a0120000000000000000000000000000000000
-                  0000006409a6010000ab0100000000000000007d036e0f74290000000000
-                  0000000000640da6010000ab010000000000000000820174010000000000
-                  00000000006a150000000000000000640e7c03a6020000ab020000000000
-                  0000007d04640064006400a6020000ab02000000000000000001006e0b23
-                  0031007304770278035900770101005900010001007c00a0160000000000
-                  0000000000000000000000000000007c047c02ac0fa6020000ab02000000
-                  00000000005c0200007d057d06742f000000000000000000007c06a60100
-                  00ab0100000000000000007d067401000000000000000000006a15000000
-                  00000000006410741f000000000000000000006a1000000000000000007c
-                  057c06a6020000ab020000000000000000a0120000000000000000000000
-                  0000000000000000006409a6010000ab010000000000000000a6020000ab
-                  0200000000000000007d077c00a018000000000000000000000000000000
-                  00000000007c077c02ac0fa6020000ab0200000000000000007d08743300
-                  0000000000000000007c086411ac12a6020000ab0200000000000000007d
-                  087c01a01a000000000000000000000000000000000000000064116413ac
-                  14a6020000ab0200000000000000007d097437000000000000000000006a
-                  1c00000000000000007c097c087a0500007c006a1d00000000000000007a
-                  000000a6010000ab0100000000000000007437000000000000000000006a
-                  1c00000000000000007c006a0800000000000000007c006a1d0000000000
-                  0000007a000000a6010000ab0100000000000000007a0a00007d0a741f00
-                  0000000000000000006a1e00000000000000007c006a0800000000000000
-                  007c0aac15a6020000ab0200000000000000007d0b740100000000000000
-                  0000006a15000000000000000064167c0ba0120000000000000000000000
-                  0000000000000000006409a6010000ab0100000000000000007c01ac17a6
-                  030000ab0300000000000000000100640064006400a6020000ab02000000
-                  000000000001006e0b230031007304770278035900770101005900010001
-                  00640064006400a6020000ab020000000000000000010064005300230031
-                  0073047702780359007701010059000100010064005300
-                94           0 RESUME                   0
+                  0000006409a6010000ab010000000000000000a6020000ab020000000000
+                  0000007d077c00a01800000000000000000000000000000000000000007c
+                  077c02ac0fa6020000ab0200000000000000007d08743300000000000000
+                  0000007c086411ac12a6020000ab0200000000000000007d087c01a01a00
+                  0000000000000000000000000000000000000064116413ac14a6020000ab
+                  0200000000000000007d097437000000000000000000006a1c0000000000
+                  0000007c097c087a0500007c006a1d00000000000000007a000000a60100
+                  00ab0100000000000000007437000000000000000000006a1c0000000000
+                  0000007c006a0800000000000000007c006a1d00000000000000007a0000
+                  00a6010000ab0100000000000000007a0a00007d0a741f00000000000000
+                  0000006a1e00000000000000007c006a0800000000000000007c006a1d00
+                  000000000000007a0000007c0aac15a6020000ab0200000000000000007d
+                  0b7401000000000000000000006a15000000000000000064167c0ba01200
+                  000000000000000000000000000000000000006409a6010000ab01000000
+                  00000000007c01ac17a6030000ab03000000000000000001006400640064
+                  00a6020000ab02000000000000000001006e0b2300310073047702780359
+                  0077010100590001000100640064006400a6020000ab0200000000000000
+                  000100640053002300310073047702780359007701010059000100010064
+                  005300
+               101           0 RESUME                   0
                
-                95           2 LOAD_GLOBAL              1 (NULL + pyro)
+               102           2 LOAD_GLOBAL              1 (NULL + pyro)
                             14 LOAD_ATTR                1 (module)
                             24 LOAD_CONST               1 ('decipher')
                             26 LOAD_FAST                0 (self)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_TOP
                
-                97          44 LOAD_GLOBAL              1 (NULL + pyro)
+               104          44 LOAD_GLOBAL              1 (NULL + pyro)
                             56 LOAD_ATTR                2 (param)
                
-                98          66 LOAD_CONST               2 ('inverse_dispersion')
+               105          66 LOAD_CONST               2 ('theta')
                
-                99          68 LOAD_CONST               3 (1.0)
-                            70 LOAD_FAST                1 (x)
-                            72 LOAD_METHOD              3 (new_ones)
-                            94 LOAD_FAST                0 (self)
-                            96 LOAD_ATTR                4 (config)
-                           106 LOAD_ATTR                5 (dim_genes)
-                           116 PRECALL                  1
-                           120 CALL                     1
-                           130 BINARY_OP                5 (*)
-               
-               100         134 LOAD_GLOBAL             12 (constraints)
-                           146 LOAD_ATTR                7 (positive)
-               
-                97         156 KW_NAMES                 4
-                           158 PRECALL                  3
-                           162 CALL                     3
-                           172 LOAD_FAST                0 (self)
-                           174 STORE_ATTR               8 (theta)
-               
-               103         184 LOAD_GLOBAL              1 (NULL + pyro)
-                           196 LOAD_ATTR                9 (plate)
-                           206 LOAD_CONST               5 ('batch')
-                           208 LOAD_GLOBAL             21 (NULL + len)
-                           220 LOAD_FAST                1 (x)
-                           222 PRECALL                  1
-                           226 CALL                     1
-                           236 PRECALL                  2
-                           240 CALL                     2
-                           250 BEFORE_WITH
-                           252 POP_TOP
-                           254 LOAD_GLOBAL             23 (NULL + poutine)
-                           266 LOAD_ATTR               12 (scale)
-                           276 LOAD_CONST               3 (1.0)
-                           278 KW_NAMES                 6
-                           280 PRECALL                  1
-                           284 CALL                     1
-                           294 BEFORE_WITH
-                           296 POP_TOP
-               
-               104         298 LOAD_GLOBAL             23 (NULL + poutine)
-                           310 LOAD_ATTR               12 (scale)
-                           320 LOAD_FAST                0 (self)
-                           322 LOAD_ATTR                4 (config)
-                           332 LOAD_ATTR               13 (beta)
-                           342 KW_NAMES                 6
-                           344 PRECALL                  1
-                           348 CALL                     1
-                           358 BEFORE_WITH
-                           360 POP_TOP
-               
-               105         362 LOAD_FAST                0 (self)
-                           364 LOAD_ATTR                4 (config)
-                           374 LOAD_ATTR               14 (prior)
-                           384 LOAD_CONST               7 ('normal')
-                           386 COMPARE_OP               2 (==)
-                           392 POP_JUMP_FORWARD_IF_FALSE    70 (to 534)
-               
-               106         394 LOAD_GLOBAL             31 (NULL + dist)
-                           406 LOAD_ATTR               16 (Normal)
-                           416 LOAD_CONST               8 (0)
-                           418 LOAD_FAST                1 (x)
-                           420 LOAD_METHOD              3 (new_ones)
-                           442 LOAD_FAST                0 (self)
-                           444 LOAD_ATTR                4 (config)
-                           454 LOAD_ATTR               17 (dim_v)
-                           464 PRECALL                  1
-                           468 CALL                     1
-                           478 PRECALL                  2
-                           482 CALL                     2
-                           492 LOAD_METHOD             18 (to_event)
-                           514 LOAD_CONST               9 (1)
-                           516 PRECALL                  1
-                           520 CALL                     1
-                           530 STORE_FAST               3 (prior)
-                           532 JUMP_FORWARD           104 (to 742)
-               
-               107     >>  534 LOAD_FAST                0 (self)
-                           536 LOAD_ATTR                4 (config)
-                           546 LOAD_ATTR               14 (prior)
-                           556 LOAD_CONST              10 ('gamma')
-                           558 COMPARE_OP               2 (==)
-                           564 POP_JUMP_FORWARD_IF_FALSE    73 (to 712)
-               
-               108         566 LOAD_GLOBAL             31 (NULL + dist)
-                           578 LOAD_ATTR               19 (Gamma)
-                           588 LOAD_CONST              11 (0.3)
-                           590 LOAD_FAST                1 (x)
-                           592 LOAD_METHOD              3 (new_ones)
-                           614 LOAD_FAST                0 (self)
-                           616 LOAD_ATTR                4 (config)
-                           626 LOAD_ATTR               17 (dim_v)
-                           636 PRECALL                  1
-                           640 CALL                     1
-                           650 LOAD_CONST              12 (0.8)
-                           652 BINARY_OP                5 (*)
-                           656 PRECALL                  2
-                           660 CALL                     2
-                           670 LOAD_METHOD             18 (to_event)
-                           692 LOAD_CONST               9 (1)
-                           694 PRECALL                  1
-                           698 CALL                     1
-                           708 STORE_FAST               3 (prior)
-                           710 JUMP_FORWARD            15 (to 742)
-               
-               110     >>  712 LOAD_GLOBAL             41 (NULL + ValueError)
-                           724 LOAD_CONST              13 ('Invalid prior, must be normal or gamma')
-                           726 PRECALL                  1
-                           730 CALL                     1
-                           740 RAISE_VARARGS            1
-               
-               111     >>  742 LOAD_GLOBAL              1 (NULL + pyro)
-                           754 LOAD_ATTR               21 (sample)
-                           764 LOAD_CONST              14 ('v')
-                           766 LOAD_FAST                3 (prior)
-                           768 PRECALL                  2
-                           772 CALL                     2
-                           782 STORE_FAST               4 (v)
-               
-               104         784 LOAD_CONST               0 (None)
-                           786 LOAD_CONST               0 (None)
-                           788 LOAD_CONST               0 (None)
-                           790 PRECALL                  2
-                           794 CALL                     2
-                           804 POP_TOP
-                           806 JUMP_FORWARD            11 (to 830)
-                       >>  808 PUSH_EXC_INFO
-                           810 WITH_EXCEPT_START
-                           812 POP_JUMP_FORWARD_IF_TRUE     4 (to 822)
-                           814 RERAISE                  2
-                       >>  816 COPY                     3
+               106          68 LOAD_FAST                1 (x)
+                            70 LOAD_METHOD              3 (new_ones)
+                            92 LOAD_FAST                0 (self)
+                            94 LOAD_ATTR                4 (config)
+                           104 LOAD_ATTR                5 (dim_genes)
+                           114 PRECALL                  1
+                           118 CALL                     1
+               
+               107         128 LOAD_GLOBAL             12 (constraints)
+                           140 LOAD_ATTR                7 (positive)
+               
+               104         150 KW_NAMES                 3
+                           152 PRECALL                  3
+                           156 CALL                     3
+                           166 LOAD_FAST                0 (self)
+                           168 STORE_ATTR               8 (theta)
+               
+               110         178 LOAD_GLOBAL              1 (NULL + pyro)
+                           190 LOAD_ATTR                9 (plate)
+                           200 LOAD_CONST               4 ('batch')
+                           202 LOAD_GLOBAL             21 (NULL + len)
+                           214 LOAD_FAST                1 (x)
+                           216 PRECALL                  1
+                           220 CALL                     1
+                           230 PRECALL                  2
+                           234 CALL                     2
+                           244 BEFORE_WITH
+                           246 POP_TOP
+                           248 LOAD_GLOBAL             23 (NULL + poutine)
+                           260 LOAD_ATTR               12 (scale)
+                           270 LOAD_CONST               5 (1.0)
+                           272 KW_NAMES                 6
+                           274 PRECALL                  1
+                           278 CALL                     1
+                           288 BEFORE_WITH
+                           290 POP_TOP
+               
+               111         292 LOAD_GLOBAL             23 (NULL + poutine)
+                           304 LOAD_ATTR               12 (scale)
+                           314 LOAD_FAST                0 (self)
+                           316 LOAD_ATTR                4 (config)
+                           326 LOAD_ATTR               13 (beta)
+                           336 KW_NAMES                 6
+                           338 PRECALL                  1
+                           342 CALL                     1
+                           352 BEFORE_WITH
+                           354 POP_TOP
+               
+               112         356 LOAD_FAST                0 (self)
+                           358 LOAD_ATTR                4 (config)
+                           368 LOAD_ATTR               14 (prior)
+                           378 LOAD_CONST               7 ('normal')
+                           380 COMPARE_OP               2 (==)
+                           386 POP_JUMP_FORWARD_IF_FALSE    70 (to 528)
+               
+               113         388 LOAD_GLOBAL             31 (NULL + dist)
+                           400 LOAD_ATTR               16 (Normal)
+                           410 LOAD_CONST               8 (0)
+                           412 LOAD_FAST                1 (x)
+                           414 LOAD_METHOD              3 (new_ones)
+                           436 LOAD_FAST                0 (self)
+                           438 LOAD_ATTR                4 (config)
+                           448 LOAD_ATTR               17 (dim_v)
+                           458 PRECALL                  1
+                           462 CALL                     1
+                           472 PRECALL                  2
+                           476 CALL                     2
+                           486 LOAD_METHOD             18 (to_event)
+                           508 LOAD_CONST               9 (1)
+                           510 PRECALL                  1
+                           514 CALL                     1
+                           524 STORE_FAST               3 (prior)
+                           526 JUMP_FORWARD           104 (to 736)
+               
+               114     >>  528 LOAD_FAST                0 (self)
+                           530 LOAD_ATTR                4 (config)
+                           540 LOAD_ATTR               14 (prior)
+                           550 LOAD_CONST              10 ('gamma')
+                           552 COMPARE_OP               2 (==)
+                           558 POP_JUMP_FORWARD_IF_FALSE    73 (to 706)
+               
+               115         560 LOAD_GLOBAL             31 (NULL + dist)
+                           572 LOAD_ATTR               19 (Gamma)
+                           582 LOAD_CONST              11 (0.3)
+                           584 LOAD_FAST                1 (x)
+                           586 LOAD_METHOD              3 (new_ones)
+                           608 LOAD_FAST                0 (self)
+                           610 LOAD_ATTR                4 (config)
+                           620 LOAD_ATTR               17 (dim_v)
+                           630 PRECALL                  1
+                           634 CALL                     1
+                           644 LOAD_CONST              12 (0.8)
+                           646 BINARY_OP                5 (*)
+                           650 PRECALL                  2
+                           654 CALL                     2
+                           664 LOAD_METHOD             18 (to_event)
+                           686 LOAD_CONST               9 (1)
+                           688 PRECALL                  1
+                           692 CALL                     1
+                           702 STORE_FAST               3 (prior)
+                           704 JUMP_FORWARD            15 (to 736)
+               
+               117     >>  706 LOAD_GLOBAL             41 (NULL + ValueError)
+                           718 LOAD_CONST              13 ('Invalid prior, must be normal or gamma')
+                           720 PRECALL                  1
+                           724 CALL                     1
+                           734 RAISE_VARARGS            1
+               
+               118     >>  736 LOAD_GLOBAL              1 (NULL + pyro)
+                           748 LOAD_ATTR               21 (sample)
+                           758 LOAD_CONST              14 ('v')
+                           760 LOAD_FAST                3 (prior)
+                           762 PRECALL                  2
+                           766 CALL                     2
+                           776 STORE_FAST               4 (v)
+               
+               111         778 LOAD_CONST               0 (None)
+                           780 LOAD_CONST               0 (None)
+                           782 LOAD_CONST               0 (None)
+                           784 PRECALL                  2
+                           788 CALL                     2
+                           798 POP_TOP
+                           800 JUMP_FORWARD            11 (to 824)
+                       >>  802 PUSH_EXC_INFO
+                           804 WITH_EXCEPT_START
+                           806 POP_JUMP_FORWARD_IF_TRUE     4 (to 816)
+                           808 RERAISE                  2
+                       >>  810 COPY                     3
+                           812 POP_EXCEPT
+                           814 RERAISE                  1
+                       >>  816 POP_TOP
                            818 POP_EXCEPT
-                           820 RERAISE                  1
-                       >>  822 POP_TOP
-                           824 POP_EXCEPT
-                           826 POP_TOP
-                           828 POP_TOP
-               
-               113     >>  830 LOAD_FAST                0 (self)
-                           832 LOAD_METHOD             22 (decoder_v_to_z)
-                           854 LOAD_FAST                4 (v)
-                           856 LOAD_FAST                2 (context)
-                           858 KW_NAMES                15
-                           860 PRECALL                  2
-                           864 CALL                     2
-                           874 UNPACK_SEQUENCE          2
-                           878 STORE_FAST               5 (z_loc)
-                           880 STORE_FAST               6 (z_scale)
+                           820 POP_TOP
+                           822 POP_TOP
                
-               114         882 LOAD_GLOBAL             47 (NULL + softplus)
-                           894 LOAD_FAST                6 (z_scale)
-                           896 PRECALL                  1
-                           900 CALL                     1
-                           910 STORE_FAST               6 (z_scale)
-               
-               115         912 LOAD_GLOBAL              1 (NULL + pyro)
-                           924 LOAD_ATTR               21 (sample)
-                           934 LOAD_CONST              16 ('z')
-                           936 LOAD_GLOBAL             31 (NULL + dist)
-                           948 LOAD_ATTR               16 (Normal)
-                           958 LOAD_FAST                5 (z_loc)
-                           960 LOAD_FAST                6 (z_scale)
-                           962 PRECALL                  2
-                           966 CALL                     2
-                           976 LOAD_METHOD             18 (to_event)
-                           998 LOAD_CONST               9 (1)
-                          1000 PRECALL                  1
-                          1004 CALL                     1
-                          1014 PRECALL                  2
-                          1018 CALL                     2
-                          1028 STORE_FAST               7 (z)
-               
-               117        1030 LOAD_FAST                0 (self)
-                          1032 LOAD_METHOD             24 (decoder_z_to_x)
-                          1054 LOAD_FAST                7 (z)
-                          1056 LOAD_FAST                2 (context)
-                          1058 KW_NAMES                15
-                          1060 PRECALL                  2
-                          1064 CALL                     2
-                          1074 STORE_FAST               8 (mu)
-               
-               118        1076 LOAD_GLOBAL             51 (NULL + softmax)
-                          1088 LOAD_FAST                8 (mu)
-                          1090 LOAD_CONST              17 (-1)
-                          1092 KW_NAMES                18
-                          1094 PRECALL                  2
-                          1098 CALL                     2
-                          1108 STORE_FAST               8 (mu)
-               
-               119        1110 LOAD_FAST                1 (x)
-                          1112 LOAD_METHOD             26 (sum)
-                          1134 LOAD_CONST              17 (-1)
-                          1136 LOAD_CONST              19 (True)
-                          1138 KW_NAMES                20
-                          1140 PRECALL                  2
-                          1144 CALL                     2
-                          1154 STORE_FAST               9 (library_size)
-               
-               123        1156 LOAD_GLOBAL             55 (NULL + torch)
-                          1168 LOAD_ATTR               28 (log)
-                          1178 LOAD_FAST                9 (library_size)
-                          1180 LOAD_FAST                8 (mu)
-                          1182 BINARY_OP                5 (*)
-                          1186 LOAD_FAST                0 (self)
-                          1188 LOAD_ATTR               29 (_epsilon)
-                          1198 BINARY_OP                0 (+)
-                          1202 PRECALL                  1
-                          1206 CALL                     1
-                          1216 LOAD_GLOBAL             55 (NULL + torch)
-                          1228 LOAD_ATTR               28 (log)
-               
-               124        1238 LOAD_FAST                0 (self)
-                          1240 LOAD_ATTR                8 (theta)
-                          1250 LOAD_FAST                0 (self)
-                          1252 LOAD_ATTR               29 (_epsilon)
-                          1262 BINARY_OP                0 (+)
-               
-               123        1266 PRECALL                  1
-                          1270 CALL                     1
-                          1280 BINARY_OP               10 (-)
-                          1284 STORE_FAST              10 (logit)
-               
-               127        1286 LOAD_GLOBAL             31 (NULL + dist)
-                          1298 LOAD_ATTR               30 (NegativeBinomial)
-                          1308 LOAD_FAST                0 (self)
-                          1310 LOAD_ATTR                8 (theta)
-                          1320 LOAD_FAST               10 (logit)
-                          1322 KW_NAMES                21
-                          1324 PRECALL                  2
-                          1328 CALL                     2
-                          1338 STORE_FAST              11 (x_dist)
-               
-               128        1340 LOAD_GLOBAL              1 (NULL + pyro)
-                          1352 LOAD_ATTR               21 (sample)
-                          1362 LOAD_CONST              22 ('x')
-                          1364 LOAD_FAST               11 (x_dist)
-                          1366 LOAD_METHOD             18 (to_event)
-                          1388 LOAD_CONST               9 (1)
-                          1390 PRECALL                  1
-                          1394 CALL                     1
-                          1404 LOAD_FAST                1 (x)
-                          1406 KW_NAMES                23
-                          1408 PRECALL                  3
-                          1412 CALL                     3
-                          1422 POP_TOP
-               
-               103        1424 LOAD_CONST               0 (None)
-                          1426 LOAD_CONST               0 (None)
-                          1428 LOAD_CONST               0 (None)
-                          1430 PRECALL                  2
-                          1434 CALL                     2
-                          1444 POP_TOP
-                          1446 JUMP_FORWARD            11 (to 1470)
-                       >> 1448 PUSH_EXC_INFO
-                          1450 WITH_EXCEPT_START
-                          1452 POP_JUMP_FORWARD_IF_TRUE     4 (to 1462)
-                          1454 RERAISE                  2
-                       >> 1456 COPY                     3
-                          1458 POP_EXCEPT
-                          1460 RERAISE                  1
-                       >> 1462 POP_TOP
-                          1464 POP_EXCEPT
-                          1466 POP_TOP
-                          1468 POP_TOP
-                       >> 1470 LOAD_CONST               0 (None)
-                          1472 LOAD_CONST               0 (None)
-                          1474 LOAD_CONST               0 (None)
-                          1476 PRECALL                  2
-                          1480 CALL                     2
-                          1490 POP_TOP
-                          1492 LOAD_CONST               0 (None)
-                          1494 RETURN_VALUE
-                       >> 1496 PUSH_EXC_INFO
-                          1498 WITH_EXCEPT_START
-                          1500 POP_JUMP_FORWARD_IF_TRUE     4 (to 1510)
-                          1502 RERAISE                  2
-                       >> 1504 COPY                     3
-                          1506 POP_EXCEPT
-                          1508 RERAISE                  1
-                       >> 1510 POP_TOP
-                          1512 POP_EXCEPT
-                          1514 POP_TOP
-                          1516 POP_TOP
-                          1518 LOAD_CONST               0 (None)
-                          1520 RETURN_VALUE
+               120     >>  824 LOAD_FAST                0 (self)
+                           826 LOAD_METHOD             22 (decoder_v_to_z)
+                           848 LOAD_FAST                4 (v)
+                           850 LOAD_FAST                2 (context)
+                           852 KW_NAMES                15
+                           854 PRECALL                  2
+                           858 CALL                     2
+                           868 UNPACK_SEQUENCE          2
+                           872 STORE_FAST               5 (z_loc)
+                           874 STORE_FAST               6 (z_scale)
+               
+               121         876 LOAD_GLOBAL             47 (NULL + softplus)
+                           888 LOAD_FAST                6 (z_scale)
+                           890 PRECALL                  1
+                           894 CALL                     1
+                           904 STORE_FAST               6 (z_scale)
+               
+               122         906 LOAD_GLOBAL              1 (NULL + pyro)
+                           918 LOAD_ATTR               21 (sample)
+                           928 LOAD_CONST              16 ('z')
+                           930 LOAD_GLOBAL             31 (NULL + dist)
+                           942 LOAD_ATTR               16 (Normal)
+                           952 LOAD_FAST                5 (z_loc)
+                           954 LOAD_FAST                6 (z_scale)
+                           956 PRECALL                  2
+                           960 CALL                     2
+                           970 LOAD_METHOD             18 (to_event)
+                           992 LOAD_CONST               9 (1)
+                           994 PRECALL                  1
+                           998 CALL                     1
+                          1008 PRECALL                  2
+                          1012 CALL                     2
+                          1022 STORE_FAST               7 (z)
+               
+               124        1024 LOAD_FAST                0 (self)
+                          1026 LOAD_METHOD             24 (decoder_z_to_x)
+                          1048 LOAD_FAST                7 (z)
+                          1050 LOAD_FAST                2 (context)
+                          1052 KW_NAMES                15
+                          1054 PRECALL                  2
+                          1058 CALL                     2
+                          1068 STORE_FAST               8 (mu)
+               
+               125        1070 LOAD_GLOBAL             51 (NULL + softmax)
+                          1082 LOAD_FAST                8 (mu)
+                          1084 LOAD_CONST              17 (-1)
+                          1086 KW_NAMES                18
+                          1088 PRECALL                  2
+                          1092 CALL                     2
+                          1102 STORE_FAST               8 (mu)
+               
+               126        1104 LOAD_FAST                1 (x)
+                          1106 LOAD_METHOD             26 (sum)
+                          1128 LOAD_CONST              17 (-1)
+                          1130 LOAD_CONST              19 (True)
+                          1132 KW_NAMES                20
+                          1134 PRECALL                  2
+                          1138 CALL                     2
+                          1148 STORE_FAST               9 (library_size)
+               
+               130        1150 LOAD_GLOBAL             55 (NULL + torch)
+                          1162 LOAD_ATTR               28 (log)
+                          1172 LOAD_FAST                9 (library_size)
+                          1174 LOAD_FAST                8 (mu)
+                          1176 BINARY_OP                5 (*)
+                          1180 LOAD_FAST                0 (self)
+                          1182 LOAD_ATTR               29 (_epsilon)
+                          1192 BINARY_OP                0 (+)
+                          1196 PRECALL                  1
+                          1200 CALL                     1
+                          1210 LOAD_GLOBAL             55 (NULL + torch)
+                          1222 LOAD_ATTR               28 (log)
+               
+               131        1232 LOAD_FAST                0 (self)
+                          1234 LOAD_ATTR                8 (theta)
+                          1244 LOAD_FAST                0 (self)
+                          1246 LOAD_ATTR               29 (_epsilon)
+                          1256 BINARY_OP                0 (+)
+               
+               130        1260 PRECALL                  1
+                          1264 CALL                     1
+                          1274 BINARY_OP               10 (-)
+                          1278 STORE_FAST              10 (logit)
+               
+               134        1280 LOAD_GLOBAL             31 (NULL + dist)
+                          1292 LOAD_ATTR               30 (NegativeBinomial)
+                          1302 LOAD_FAST                0 (self)
+                          1304 LOAD_ATTR                8 (theta)
+                          1314 LOAD_FAST                0 (self)
+                          1316 LOAD_ATTR               29 (_epsilon)
+                          1326 BINARY_OP                0 (+)
+                          1330 LOAD_FAST               10 (logit)
+                          1332 KW_NAMES                21
+                          1334 PRECALL                  2
+                          1338 CALL                     2
+                          1348 STORE_FAST              11 (x_dist)
+               
+               135        1350 LOAD_GLOBAL              1 (NULL + pyro)
+                          1362 LOAD_ATTR               21 (sample)
+                          1372 LOAD_CONST              22 ('x')
+                          1374 LOAD_FAST               11 (x_dist)
+                          1376 LOAD_METHOD             18 (to_event)
+                          1398 LOAD_CONST               9 (1)
+                          1400 PRECALL                  1
+                          1404 CALL                     1
+                          1414 LOAD_FAST                1 (x)
+                          1416 KW_NAMES                23
+                          1418 PRECALL                  3
+                          1422 CALL                     3
+                          1432 POP_TOP
+               
+               110        1434 LOAD_CONST               0 (None)
+                          1436 LOAD_CONST               0 (None)
+                          1438 LOAD_CONST               0 (None)
+                          1440 PRECALL                  2
+                          1444 CALL                     2
+                          1454 POP_TOP
+                          1456 JUMP_FORWARD            11 (to 1480)
+                       >> 1458 PUSH_EXC_INFO
+                          1460 WITH_EXCEPT_START
+                          1462 POP_JUMP_FORWARD_IF_TRUE     4 (to 1472)
+                          1464 RERAISE                  2
+                       >> 1466 COPY                     3
+                          1468 POP_EXCEPT
+                          1470 RERAISE                  1
+                       >> 1472 POP_TOP
+                          1474 POP_EXCEPT
+                          1476 POP_TOP
+                          1478 POP_TOP
+                       >> 1480 LOAD_CONST               0 (None)
+                          1482 LOAD_CONST               0 (None)
+                          1484 LOAD_CONST               0 (None)
+                          1486 PRECALL                  2
+                          1490 CALL                     2
+                          1500 POP_TOP
+                          1502 LOAD_CONST               0 (None)
+                          1504 RETURN_VALUE
+                       >> 1506 PUSH_EXC_INFO
+                          1508 WITH_EXCEPT_START
+                          1510 POP_JUMP_FORWARD_IF_TRUE     4 (to 1520)
+                          1512 RERAISE                  2
+                       >> 1514 COPY                     3
+                          1516 POP_EXCEPT
+                          1518 RERAISE                  1
+                       >> 1520 POP_TOP
+                          1522 POP_EXCEPT
+                          1524 POP_TOP
+                          1526 POP_TOP
+                          1528 LOAD_CONST               0 (None)
+                          1530 RETURN_VALUE
                ExceptionTable:
-                 252 to 294 -> 1496 [1] lasti
-                 296 to 358 -> 1448 [2] lasti
-                 360 to 782 -> 808 [3] lasti
-                 784 to 806 -> 1448 [2] lasti
-                 808 to 814 -> 816 [5] lasti
-                 816 to 820 -> 1448 [2] lasti
-                 822 to 822 -> 816 [5] lasti
-                 824 to 1422 -> 1448 [2] lasti
-                 1424 to 1446 -> 1496 [1] lasti
-                 1448 to 1454 -> 1456 [4] lasti
-                 1456 to 1460 -> 1496 [1] lasti
-                 1462 to 1462 -> 1456 [4] lasti
-                 1464 to 1468 -> 1496 [1] lasti
-                 1496 to 1502 -> 1504 [3] lasti
-                 1510 to 1510 -> 1504 [3] lasti
+                 246 to 288 -> 1506 [1] lasti
+                 290 to 352 -> 1458 [2] lasti
+                 354 to 776 -> 802 [3] lasti
+                 778 to 800 -> 1458 [2] lasti
+                 802 to 808 -> 810 [5] lasti
+                 810 to 814 -> 1458 [2] lasti
+                 816 to 816 -> 810 [5] lasti
+                 818 to 1432 -> 1458 [2] lasti
+                 1434 to 1456 -> 1506 [1] lasti
+                 1458 to 1464 -> 1466 [4] lasti
+                 1466 to 1470 -> 1506 [1] lasti
+                 1472 to 1472 -> 1466 [4] lasti
+                 1474 to 1478 -> 1506 [1] lasti
+                 1506 to 1512 -> 1514 [3] lasti
+                 1520 to 1520 -> 1514 [3] lasti
                consts
                   None
                   'decipher'
-                  'inverse_dispersion'
-                  1.0
+                  'theta'
                   ('constraint',)
                   'batch'
+                  1.0
                   ('scale',)
                   'normal'
                   0
                   1
                   'gamma'
                   0.3
                   0.8
@@ -1070,20 +1124,20 @@
                   ('total_count', 'logits')
                   'x'
                   ('obs',)
                names      ('pyro', 'module', 'param', 'new_ones', 'config', 'dim_genes', 'constraints', 'positive', 'theta', 'plate', 'len', 'poutine', 'scale', 'beta', 'prior', 'dist', 'Normal', 'dim_v', 'to_event', 'Gamma', 'ValueError', 'sample', 'decoder_v_to_z', 'softplus', 'decoder_z_to_x', 'softmax', 'sum', 'torch', 'log', '_epsilon', 'NegativeBinomial')
                varnames   ('self', 'x', 'context', 'prior', 'v', 'z_loc', 'z_scale', 'z', 'mu', 'library_size', 'logit', 'x_dist')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       'model'
-               firstlineno 94
+               firstlineno 101
                lnotab
-                  0x02012a0216010201420116fd1c067201400120018c01200192021e012a
-                  f92e0934011e0176022e0122012e0452011cff1404360154e7
+                  0x02012a02160102013c0116fd1c067201400120018c01200192021e012a
+                  f92e0934011e0176022e0122012e0452011cff1404460154e7
             code
                argcount  : 3
                nlocals   : 11
                stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000006a01000000000000000064017c00a6
@@ -1119,25 +1173,25 @@
                   00ab01000000000000000082017401000000000000000000006a0d000000
                   0000000000640e7c0aa6020000ab02000000000000000001006400640064
                   00a6020000ab02000000000000000001006e0b2300310073047702780359
                   0077010100590001000100640064006400a6020000ab0200000000000000
                   0001006e0b23003100730477027803590077010100590001000100640064
                   006400a6020000ab02000000000000000001006e0b230031007304770278
                   035900770101005900010001007c037c087c047c0966045300
-               130           0 RESUME                   0
+               137           0 RESUME                   0
                
-               131           2 LOAD_GLOBAL              1 (NULL + pyro)
+               138           2 LOAD_GLOBAL              1 (NULL + pyro)
                             14 LOAD_ATTR                1 (module)
                             24 LOAD_CONST               1 ('decipher')
                             26 LOAD_FAST                0 (self)
                             28 PRECALL                  2
                             32 CALL                     2
                             42 POP_TOP
                
-               132          44 LOAD_GLOBAL              1 (NULL + pyro)
+               139          44 LOAD_GLOBAL              1 (NULL + pyro)
                             56 LOAD_ATTR                2 (plate)
                             66 LOAD_CONST               2 ('batch')
                             68 LOAD_GLOBAL              7 (NULL + len)
                             80 LOAD_FAST                1 (x)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 PRECALL                  2
@@ -1149,105 +1203,105 @@
                            136 LOAD_CONST               3 (1.0)
                            138 KW_NAMES                 4
                            140 PRECALL                  1
                            144 CALL                     1
                            154 BEFORE_WITH
                            156 POP_TOP
                
-               133         158 LOAD_GLOBAL             13 (NULL + torch)
+               140         158 LOAD_GLOBAL             13 (NULL + torch)
                            170 LOAD_ATTR                7 (log1p)
                            180 LOAD_FAST                1 (x)
                            182 PRECALL                  1
                            186 CALL                     1
                            196 STORE_FAST               1 (x)
                
-               135         198 LOAD_FAST                0 (self)
+               142         198 LOAD_FAST                0 (self)
                            200 LOAD_METHOD              8 (encoder_x_to_z)
                            222 LOAD_FAST                1 (x)
                            224 LOAD_FAST                2 (context)
                            226 KW_NAMES                 5
                            228 PRECALL                  2
                            232 CALL                     2
                            242 UNPACK_SEQUENCE          2
                            246 STORE_FAST               3 (z_loc)
                            248 STORE_FAST               4 (z_scale)
                
-               136         250 LOAD_GLOBAL             19 (NULL + softplus)
+               143         250 LOAD_GLOBAL             19 (NULL + softplus)
                            262 LOAD_FAST                4 (z_scale)
                            264 PRECALL                  1
                            268 CALL                     1
                            278 STORE_FAST               4 (z_scale)
                
-               137         280 LOAD_GLOBAL             21 (NULL + dist)
+               144         280 LOAD_GLOBAL             21 (NULL + dist)
                            292 LOAD_ATTR               11 (Normal)
                            302 LOAD_FAST                3 (z_loc)
                            304 LOAD_FAST                4 (z_scale)
                            306 PRECALL                  2
                            310 CALL                     2
                            320 LOAD_METHOD             12 (to_event)
                            342 LOAD_CONST               6 (1)
                            344 PRECALL                  1
                            348 CALL                     1
                            358 STORE_FAST               5 (posterior_z)
                
-               138         360 LOAD_GLOBAL              1 (NULL + pyro)
+               145         360 LOAD_GLOBAL              1 (NULL + pyro)
                            372 LOAD_ATTR               13 (sample)
                            382 LOAD_CONST               7 ('z')
                            384 LOAD_FAST                5 (posterior_z)
                            386 PRECALL                  2
                            390 CALL                     2
                            400 STORE_FAST               6 (z)
                
-               140         402 LOAD_GLOBAL             13 (NULL + torch)
+               147         402 LOAD_GLOBAL             13 (NULL + torch)
                            414 LOAD_ATTR               14 (cat)
                            424 LOAD_FAST                6 (z)
                            426 LOAD_FAST                1 (x)
                            428 BUILD_LIST               2
                            430 LOAD_CONST               8 (-1)
                            432 KW_NAMES                 9
                            434 PRECALL                  2
                            438 CALL                     2
                            448 STORE_FAST               7 (zx)
                
-               141         450 LOAD_FAST                0 (self)
+               148         450 LOAD_FAST                0 (self)
                            452 LOAD_METHOD             15 (encoder_zx_to_v)
                            474 LOAD_FAST                7 (zx)
                            476 LOAD_FAST                2 (context)
                            478 KW_NAMES                 5
                            480 PRECALL                  2
                            484 CALL                     2
                            494 UNPACK_SEQUENCE          2
                            498 STORE_FAST               8 (v_loc)
                            500 STORE_FAST               9 (v_scale)
                
-               142         502 LOAD_GLOBAL             19 (NULL + softplus)
+               149         502 LOAD_GLOBAL             19 (NULL + softplus)
                            514 LOAD_FAST                9 (v_scale)
                            516 PRECALL                  1
                            520 CALL                     1
                            530 STORE_FAST               9 (v_scale)
                
-               143         532 LOAD_GLOBAL              9 (NULL + poutine)
+               150         532 LOAD_GLOBAL              9 (NULL + poutine)
                            544 LOAD_ATTR                5 (scale)
                            554 LOAD_FAST                0 (self)
                            556 LOAD_ATTR               16 (config)
                            566 LOAD_ATTR               17 (beta)
                            576 KW_NAMES                 4
                            578 PRECALL                  1
                            582 CALL                     1
                            592 BEFORE_WITH
                            594 POP_TOP
                
-               144         596 LOAD_FAST                0 (self)
+               151         596 LOAD_FAST                0 (self)
                            598 LOAD_ATTR               16 (config)
                            608 LOAD_ATTR               18 (prior)
                            618 LOAD_CONST              10 ('gamma')
                            620 COMPARE_OP               2 (==)
                            626 POP_JUMP_FORWARD_IF_FALSE    54 (to 736)
                
-               145         628 LOAD_GLOBAL             21 (NULL + dist)
+               152         628 LOAD_GLOBAL             21 (NULL + dist)
                            640 LOAD_ATTR               19 (Gamma)
                            650 LOAD_GLOBAL             19 (NULL + softplus)
                            662 LOAD_FAST                8 (v_loc)
                            664 PRECALL                  1
                            668 CALL                     1
                            678 LOAD_FAST                9 (v_scale)
                            680 PRECALL                  2
@@ -1255,55 +1309,55 @@
                            694 LOAD_METHOD             12 (to_event)
                            716 LOAD_CONST               6 (1)
                            718 PRECALL                  1
                            722 CALL                     1
                            732 STORE_FAST              10 (posterior_v)
                            734 JUMP_FORWARD            88 (to 912)
                
-               146     >>  736 LOAD_FAST                0 (self)
+               153     >>  736 LOAD_FAST                0 (self)
                            738 LOAD_ATTR               16 (config)
                            748 LOAD_ATTR               18 (prior)
                            758 LOAD_CONST              11 ('normal')
                            760 COMPARE_OP               2 (==)
                            766 POP_JUMP_FORWARD_IF_TRUE    16 (to 800)
                            768 LOAD_FAST                0 (self)
                            770 LOAD_ATTR               16 (config)
                            780 LOAD_ATTR               18 (prior)
                            790 LOAD_CONST              12 ('student-normal')
                            792 COMPARE_OP               2 (==)
                            798 POP_JUMP_FORWARD_IF_FALSE    41 (to 882)
                
-               147     >>  800 LOAD_GLOBAL             21 (NULL + dist)
+               154     >>  800 LOAD_GLOBAL             21 (NULL + dist)
                            812 LOAD_ATTR               11 (Normal)
                            822 LOAD_FAST                8 (v_loc)
                            824 LOAD_FAST                9 (v_scale)
                            826 PRECALL                  2
                            830 CALL                     2
                            840 LOAD_METHOD             12 (to_event)
                            862 LOAD_CONST               6 (1)
                            864 PRECALL                  1
                            868 CALL                     1
                            878 STORE_FAST              10 (posterior_v)
                            880 JUMP_FORWARD            15 (to 912)
                
-               149     >>  882 LOAD_GLOBAL             41 (NULL + ValueError)
+               156     >>  882 LOAD_GLOBAL             41 (NULL + ValueError)
                            894 LOAD_CONST              13 ('Invalid prior, must be normal or gamma')
                            896 PRECALL                  1
                            900 CALL                     1
                            910 RAISE_VARARGS            1
                
-               150     >>  912 LOAD_GLOBAL              1 (NULL + pyro)
+               157     >>  912 LOAD_GLOBAL              1 (NULL + pyro)
                            924 LOAD_ATTR               13 (sample)
                            934 LOAD_CONST              14 ('v')
                            936 LOAD_FAST               10 (posterior_v)
                            938 PRECALL                  2
                            942 CALL                     2
                            952 POP_TOP
                
-               143         954 LOAD_CONST               0 (None)
+               150         954 LOAD_CONST               0 (None)
                            956 LOAD_CONST               0 (None)
                            958 LOAD_CONST               0 (None)
                            960 PRECALL                  2
                            964 CALL                     2
                            974 POP_TOP
                            976 JUMP_FORWARD            11 (to 1000)
                        >>  978 PUSH_EXC_INFO
@@ -1314,15 +1368,15 @@
                            988 POP_EXCEPT
                            990 RERAISE                  1
                        >>  992 POP_TOP
                            994 POP_EXCEPT
                            996 POP_TOP
                            998 POP_TOP
                
-               132     >> 1000 LOAD_CONST               0 (None)
+               139     >> 1000 LOAD_CONST               0 (None)
                           1002 LOAD_CONST               0 (None)
                           1004 LOAD_CONST               0 (None)
                           1006 PRECALL                  2
                           1010 CALL                     2
                           1020 POP_TOP
                           1022 JUMP_FORWARD            11 (to 1046)
                        >> 1024 PUSH_EXC_INFO
@@ -1351,15 +1405,15 @@
                           1080 POP_EXCEPT
                           1082 RERAISE                  1
                        >> 1084 POP_TOP
                           1086 POP_EXCEPT
                           1088 POP_TOP
                           1090 POP_TOP
                
-               151     >> 1092 LOAD_FAST                3 (z_loc)
+               158     >> 1092 LOAD_FAST                3 (z_loc)
                           1094 LOAD_FAST                8 (v_loc)
                           1096 LOAD_FAST                4 (z_scale)
                           1098 LOAD_FAST                9 (v_scale)
                           1100 BUILD_TUPLE              4
                           1102 RETURN_VALUE
                ExceptionTable:
                  112 to 154 -> 1070 [1] lasti
@@ -1393,17 +1447,17 @@
                   'student-normal'
                   'Invalid prior, must be normal or gamma'
                   'v'
                names      ('pyro', 'module', 'plate', 'len', 'poutine', 'scale', 'torch', 'log1p', 'encoder_x_to_z', 'softplus', 'dist', 'Normal', 'to_event', 'sample', 'cat', 'encoder_zx_to_v', 'config', 'beta', 'prior', 'Gamma', 'ValueError')
                varnames   ('self', 'x', 'context', 'z_loc', 'z_scale', 'posterior_z', 'z', 'zx', 'v_loc', 'v_scale', 'posterior_v')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       'guide'
-               firstlineno 130
+               firstlineno 137
                lnotab
                   0x02012a017201280234011e0150012a02300134011e01400120016c0140
                   0152021e012af92ef55c13
             'x'
             code
                argcount  : 2
                nlocals   : 6
@@ -1422,72 +1476,72 @@
                   0000000000000000000000000000007c04a6010000ab0100000000000000
                   005c0200007d057d037c05a00a0000000000000000000000000000000000
                   000000a6000000ab000000000000000000a00b0000000000000000000000
                   000000000000000000a6000000ab0000000000000000007c02a00a000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00a00b0000000000000000000000000000000000000000a6000000ab0000
                   0000000000000066025300
-               153           0 RESUME                   0
+               160           0 RESUME                   0
                
-               168           2 LOAD_GLOBAL              1 (NULL + type)
+               175           2 LOAD_GLOBAL              1 (NULL + type)
                             14 LOAD_FAST                1 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_GLOBAL              2 (np)
                             42 LOAD_ATTR                2 (ndarray)
                             52 COMPARE_OP               2 (==)
                             58 POP_JUMP_FORWARD_IF_FALSE    32 (to 124)
                
-               169          60 LOAD_GLOBAL              7 (NULL + torch)
+               176          60 LOAD_GLOBAL              7 (NULL + torch)
                             72 LOAD_ATTR                4 (tensor)
                             82 LOAD_FAST                1 (x)
                             84 LOAD_GLOBAL              6 (torch)
                             96 LOAD_ATTR                5 (float32)
                            106 KW_NAMES                 1
                            108 PRECALL                  2
                            112 CALL                     2
                            122 STORE_FAST               1 (x)
                
-               171     >>  124 LOAD_GLOBAL              7 (NULL + torch)
+               178     >>  124 LOAD_GLOBAL              7 (NULL + torch)
                            136 LOAD_ATTR                6 (log1p)
                            146 LOAD_FAST                1 (x)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 STORE_FAST               1 (x)
                
-               172         164 LOAD_FAST                0 (self)
+               179         164 LOAD_FAST                0 (self)
                            166 LOAD_METHOD              7 (encoder_x_to_z)
                            188 LOAD_FAST                1 (x)
                            190 PRECALL                  1
                            194 CALL                     1
                            204 UNPACK_SEQUENCE          2
                            208 STORE_FAST               2 (z_loc)
                            210 STORE_FAST               3 (_)
                
-               173         212 LOAD_GLOBAL              7 (NULL + torch)
+               180         212 LOAD_GLOBAL              7 (NULL + torch)
                            224 LOAD_ATTR                8 (cat)
                            234 LOAD_FAST                2 (z_loc)
                            236 LOAD_FAST                1 (x)
                            238 BUILD_LIST               2
                            240 LOAD_CONST               2 (-1)
                            242 KW_NAMES                 3
                            244 PRECALL                  2
                            248 CALL                     2
                            258 STORE_FAST               4 (zx)
                
-               174         260 LOAD_FAST                0 (self)
+               181         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              9 (encoder_zx_to_v)
                            284 LOAD_FAST                4 (zx)
                            286 PRECALL                  1
                            290 CALL                     1
                            300 UNPACK_SEQUENCE          2
                            304 STORE_FAST               5 (v_loc)
                            306 STORE_FAST               3 (_)
                
-               175         308 LOAD_FAST                5 (v_loc)
+               182         308 LOAD_FAST                5 (v_loc)
                            310 LOAD_METHOD             10 (detach)
                            332 PRECALL                  0
                            336 CALL                     0
                            346 LOAD_METHOD             11 (numpy)
                            368 PRECALL                  0
                            372 CALL                     0
                            382 LOAD_FAST                2 (z_loc)
@@ -1504,17 +1558,17 @@
                   ('dtype',)
                   -1
                   ('dim',)
                names      ('type', 'np', 'ndarray', 'torch', 'tensor', 'float32', 'log1p', 'encoder_x_to_z', 'cat', 'encoder_zx_to_v', 'detach', 'numpy')
                varnames   ('self', 'x', 'z_loc', '_', 'zx', 'v_loc')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       'compute_v_z_numpy'
-               firstlineno 153
+               firstlineno 160
                lnotab 0x020f3a0140022801300130013001
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 4
                flags     : 3
                code
@@ -1527,71 +1581,71 @@
                   0700000000000000000000000000000000000000007c02a6010000ab0100
                   000000000000007d047411000000000000000000007c046402ac03a60200
                   00ab0200000000000000007d047c01a00900000000000000000000000000
                   0000000000000064026404ac05a6020000ab0200000000000000007d057c
                   057c047a050000a00a0000000000000000000000000000000000000000a6
                   000000ab000000000000000000a00b000000000000000000000000000000
                   0000000000a6000000ab0000000000000000005300
-               177           0 RESUME                   0
+               184           0 RESUME                   0
                
-               178           2 LOAD_GLOBAL              1 (NULL + type)
+               185           2 LOAD_GLOBAL              1 (NULL + type)
                             14 LOAD_FAST                1 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 LOAD_GLOBAL              2 (np)
                             42 LOAD_ATTR                2 (ndarray)
                             52 COMPARE_OP               2 (==)
                             58 POP_JUMP_FORWARD_IF_FALSE    32 (to 124)
                
-               179          60 LOAD_GLOBAL              7 (NULL + torch)
+               186          60 LOAD_GLOBAL              7 (NULL + torch)
                             72 LOAD_ATTR                4 (tensor)
                             82 LOAD_FAST                1 (x)
                             84 LOAD_GLOBAL              6 (torch)
                             96 LOAD_ATTR                5 (float32)
                            106 KW_NAMES                 1
                            108 PRECALL                  2
                            112 CALL                     2
                            122 STORE_FAST               1 (x)
                
-               180     >>  124 LOAD_FAST                0 (self)
+               187     >>  124 LOAD_FAST                0 (self)
                            126 LOAD_METHOD              6 (guide)
                            148 LOAD_FAST                1 (x)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 UNPACK_SEQUENCE          4
                            168 STORE_FAST               2 (z_loc)
                            170 STORE_FAST               3 (_)
                            172 STORE_FAST               3 (_)
                            174 STORE_FAST               3 (_)
                
-               181         176 LOAD_FAST                0 (self)
+               188         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD              7 (decoder_z_to_x)
                            200 LOAD_FAST                2 (z_loc)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 STORE_FAST               4 (mu)
                
-               182         218 LOAD_GLOBAL             17 (NULL + softmax)
+               189         218 LOAD_GLOBAL             17 (NULL + softmax)
                            230 LOAD_FAST                4 (mu)
                            232 LOAD_CONST               2 (-1)
                            234 KW_NAMES                 3
                            236 PRECALL                  2
                            240 CALL                     2
                            250 STORE_FAST               4 (mu)
                
-               183         252 LOAD_FAST                1 (x)
+               190         252 LOAD_FAST                1 (x)
                            254 LOAD_METHOD              9 (sum)
                            276 LOAD_CONST               2 (-1)
                            278 LOAD_CONST               4 (True)
                            280 KW_NAMES                 5
                            282 PRECALL                  2
                            286 CALL                     2
                            296 STORE_FAST               5 (library_size)
                
-               184         298 LOAD_FAST                5 (library_size)
+               191         298 LOAD_FAST                5 (library_size)
                            300 LOAD_FAST                4 (mu)
                            302 BINARY_OP                5 (*)
                            306 LOAD_METHOD             10 (detach)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_METHOD             11 (numpy)
                            364 PRECALL                  0
@@ -1604,31 +1658,31 @@
                   ('dim',)
                   True
                   ('axis', 'keepdim')
                names      ('type', 'np', 'ndarray', 'torch', 'tensor', 'float32', 'guide', 'decoder_z_to_x', 'softmax', 'sum', 'detach', 'numpy')
                varnames   ('self', 'x', 'z_loc', '_', 'mu', 'library_size')
                freevars   ()
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
                name       'impute_gene_expression_numpy'
-               firstlineno 177
+               firstlineno 184
                lnotab 0x02013a01400134012a0122012e01
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'DecipherConfig', 'Union', 'dict', '__init__', 'model', 'guide', 'np', 'array', 'compute_v_z_numpy', 'impute_gene_expression_numpy', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'DecipherConfig', 'Union', 'dict', '__init__', 'property', 'device', 'model', 'guide', 'np', 'array', 'compute_v_z_numpy', 'impute_gene_expression_numpy', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
          name       'Decipher'
-         firstlineno 51
-         lnotab 0x0c01040a12fe040212fe0c22082408171618
+         firstlineno 52
+         lnotab 0x0c01040a12fe040212fe0c24020104ff0e010203082408171618
       'Decipher'
-   names      ('dataclasses', 'dataclass', 'typing', 'Sequence', 'Union', 'numpy', 'np', 'pyro', 'pyro.distributions', 'distributions', 'dist', 'pyro.poutine', 'poutine', 'torch', 'torch.nn', 'nn', 'torch.utils.data', 'torch.distributions', 'constraints', 'torch.nn.functional', 'softmax', 'softplus', 'decipher.tools._decipher.module', 'ConditionalDenseNN', 'DecipherConfig', 'Module', 'Decipher')
+   names      ('dataclasses', 'dataclass', 'typing', 'Optional', 'Sequence', 'Union', 'numpy', 'np', 'pyro', 'pyro.distributions', 'distributions', 'dist', 'pyro.poutine', 'poutine', 'torch', 'torch.nn', 'nn', 'torch.utils.data', 'torch.distributions', 'constraints', 'torch.nn.functional', 'softmax', 'softplus', 'decipher.tools._decipher.module', 'ConditionalDenseNN', 'DecipherConfig', 'Module', 'Decipher')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/decipher.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/decipher.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010c011002080108010c010c0108010c0108010c0110020c
-      03160118ff0e010220
+      0x00ff020108010c011402080108010c010c0108010c0108010c0110020c
+      03160118ff0e010221
```

### Comparing `scdecipher-0.1.0/decipher/tools/_decipher/__pycache__/module.cpython-311.pyc` & `scdecipher-0.1.2/decipher/tools/_decipher/__pycache__/module.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x214d5265 (Mon Nov 13 16:21:53 2023 UTC)
+moddate:  0x2d222166 (Thu Apr 18 13:37:49 2024 UTC)
 files sz: 3793
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -35,15 +35,15 @@
                 34 IMPORT_NAME              5 (torch.nn)
                 36 IMPORT_FROM              6 (nn)
                 38 STORE_NAME               6 (nn)
                 40 POP_TOP
    
      8          42 PUSH_NULL
                 44 LOAD_BUILD_CLASS
-                46 LOAD_CONST               3 (<code object ConditionalDenseNN, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py", line 8>)
+                46 LOAD_CONST               3 (<code object ConditionalDenseNN, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py", line 8>)
                 48 MAKE_FUNCTION            0
                 50 LOAD_CONST               4 ('ConditionalDenseNN')
                 52 LOAD_NAME                4 (torch)
                 54 LOAD_ATTR                6 (nn)
                 64 LOAD_ATTR                7 (Module)
                 74 PRECALL                  3
                 78 CALL                     3
@@ -110,20 +110,20 @@
           34         100 LOAD_CONST               9 ('deep_context_injection')
          
           40         102 LOAD_NAME                9 (bool)
          
           34         104 BUILD_TUPLE             10
                      106 LOAD_CLOSURE             0 (__class__)
                      108 BUILD_TUPLE              1
-                     110 LOAD_CONST              10 (<code object __init__, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py", line 34>)
+                     110 LOAD_CONST              10 (<code object __init__, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py", line 34>)
                      112 MAKE_FUNCTION           13 (defaults, annotations, closure)
                      114 STORE_NAME              10 (__init__)
          
           81         116 LOAD_CONST              13 ((None,))
-                     118 LOAD_CONST              12 (<code object forward, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py", line 81>)
+                     118 LOAD_CONST              12 (<code object forward, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py", line 81>)
                      120 MAKE_FUNCTION            1 (defaults)
                      122 STORE_NAME              11 (forward)
                      124 LOAD_CLOSURE             0 (__class__)
                      126 COPY                     1
                      128 STORE_NAME              12 (__classcell__)
                      130 RETURN_VALUE
          consts
@@ -250,15 +250,15 @@
                            298 PRECALL                  1
                            302 CALL                     1
                            312 BUILD_TUPLE              2
                            314 PRECALL                  1
                            318 CALL                     1
                            328 STORE_FAST               7 (indices)
                
-                55         330 LOAD_CONST               2 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py", line 55>)
+                55         330 LOAD_CONST               2 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py", line 55>)
                            332 MAKE_FUNCTION            0
                            334 LOAD_GLOBAL             29 (NULL + zip)
                            346 LOAD_FAST                7 (indices)
                            348 LOAD_CONST               0 (None)
                            350 LOAD_CONST               3 (-1)
                            352 BUILD_SLICE              2
                            354 BINARY_SUBSCR
@@ -463,25 +463,25 @@
                                   48 JUMP_BACKWARD           22 (to 6)
                              >>   50 RETURN_VALUE
                      consts
                      names      ('slice',)
                      varnames   ('.0', 's', 'e')
                      freevars   ()
                      cellvars   ()
-                     filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py'
+                     filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py'
                      name       '<listcomp>'
                      firstlineno 55
                      lnotab 0x
                   -1
                   1
                names      ('super', '__init__', 'input_dim', 'context_dim', 'hidden_dims', 'output_dims', 'deep_context_injection', 'len', 'n_output_layers', 'sum', 'output_total_dim', 'np', 'concatenate', 'cumsum', 'zip', 'output_slices', 'append', 'torch', 'nn', 'Linear', 'BatchNorm1d', 'range', 'ModuleList', 'layers', 'f', 'batch_norms')
                varnames   ('self', 'input_dim', 'hidden_dims', 'output_dims', 'context_dim', 'deep_context_injection', 'activation', 'indices', 'deep_context_dim', 'layers', 'batch_norms', 'i')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py'
                name       '__init__'
                firstlineno 34
                lnotab
                   0x040940020e010e010e010e010e01320132035c015e0320010401040120
                   0178015a013e01180162ff10035c0218015aff1204760248020e01
             None
             code
@@ -654,15 +654,15 @@
                
                101         648 LOAD_DEREF               5 (h)
                            650 RETURN_VALUE
                
                104     >>  652 LOAD_GLOBAL             31 (NULL + tuple)
                            664 LOAD_CLOSURE             5 (h)
                            666 BUILD_TUPLE              1
-                           668 LOAD_CONST               5 (<code object <listcomp>, file "/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py", line 104>)
+                           668 LOAD_CONST               5 (<code object <listcomp>, file "/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py", line 104>)
                            670 MAKE_FUNCTION            8 (closure)
                            672 LOAD_FAST                0 (self)
                            674 LOAD_ATTR               16 (output_slices)
                            684 GET_ITER
                            686 PRECALL                  0
                            690 CALL                     0
                            700 PRECALL                  1
@@ -699,41 +699,41 @@
                              >>   34 RETURN_VALUE
                      consts
                         Ellipsis
                      names      ()
                      varnames   ('.0', 's')
                      freevars   ('h',)
                      cellvars   ()
-                     filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py'
+                     filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py'
                      name       '<listcomp>'
                      firstlineno 104
                      lnotab 0x
                names      ('expand', 'size', 'enumerate', 'layers', 'context_dim', 'deep_context_injection', 'torch', 'cat', 'len', 'batch_norms', 'f', 'n_output_layers', 'reshape', 'list', 'output_total_dim', 'tuple', 'output_slices')
                varnames   ('self', 'x', 'context', 'i', 'layer')
                freevars   ()
                cellvars   ('h',)
-               filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py'
+               filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py'
                name       'forward'
                firstlineno 81
                lnotab
                   0x040104028c020401320130013001160136012c012c02160104028a0216
                   010403
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'torch', 'nn', 'ReLU', 'int', 'Sequence', 'bool', '__init__', 'forward', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py'
+         filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py'
          name       'ConditionalDenseNN'
          firstlineno 8
          lnotab
             0x0c01041d02010201020130f9040202fe02030efd020402fc020502fb02
             0602fa0c2f
       'ConditionalDenseNN'
    names      ('typing', 'Sequence', 'numpy', 'np', 'torch', 'torch.nn', 'nn', 'Module', 'ConditionalDenseNN')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/Users/achille/Documents/decipher-pip/decipher/tools/_decipher/module.py'
+   filename   '/Users/achille/Documents/decipher_dev/decipher/tools/_decipher/module.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c02080108010c03
```

### Comparing `scdecipher-0.1.0/decipher/tools/_decipher/data.py` & `scdecipher-0.1.2/decipher/tools/_decipher/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 import logging
 import os
 import time
 
+import numpy as np
 import randomname
 import torch
+import torch.distributions
 import torch.nn.functional
 import torch.utils.data
 
 from decipher.tools._decipher import Decipher, DecipherConfig
 from decipher.utils import DECIPHER_GLOBALS, create_decipher_uns_key
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s : %(message)s",
     level=logging.INFO,
 )
 
 
+def get_dense_X(adata):
+    if isinstance(adata.X, np.ndarray):
+        return adata.X
+    else:
+        return adata.X.toarray()
+
+
 def get_random_name(seed=None):
     name = randomname.generate(
         ["a/algorithms", "a/food", "a/physics"],
         ["a/colors", "a/emotions"],
         ["n/algorithms", "n/food", "a/physics"],
         seed=seed,
     )
@@ -74,16 +83,17 @@
     save_folder = DECIPHER_GLOBALS["save_folder"]
     full_path = os.path.join(save_folder, model_run_id)
     model.load_state_dict(torch.load(os.path.join(full_path, "decipher_model.pt")))
     model.eval()
     return model
 
 
-def make_data_loader_from_adata(adata, batch_size=64, context_discrete_keys=None):
-    genes = torch.FloatTensor(adata.X.todense())
+def make_data_loader_from_adata(adata, batch_size=64, context_discrete_keys=None, **kwargs):
+    """Create a PyTorch DataLoader from an AnnData object."""
+    genes = torch.FloatTensor(get_dense_X(adata))
     params = [genes]
     context_tensors = []
     if context_discrete_keys is None:
         context_discrete_keys = []
 
     for key in context_discrete_keys:
         t = torch.IntTensor(adata.obs[key].astype("category").cat.codes.values).long()
@@ -94,8 +104,9 @@
         context = torch.cat(context_tensors, dim=-1)
         params.append(context)
 
     return torch.utils.data.DataLoader(
         torch.utils.data.TensorDataset(*params),
         batch_size=batch_size,
         shuffle=True,
+        **kwargs,
     )
```

### Comparing `scdecipher-0.1.0/decipher/tools/_decipher/decipher.py` & `scdecipher-0.1.2/decipher/tools/_decipher/decipher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 from dataclasses import dataclass
-from typing import Sequence, Union
+from typing import Optional, Sequence, Union
 
 import numpy as np
 import pyro
 import pyro.distributions as dist
 import pyro.poutine as poutine
 import torch
 import torch.nn as nn
@@ -24,15 +24,16 @@
 
     beta: float = 1e-1
     seed: int = 0
 
     learning_rate: float = 5e-3
     val_frac: float = 0.1
     batch_size: int = 64
-    n_epochs: int = 100
+    n_epochs: int = 1000
+    early_stopping_patience: Optional[int] = 10
 
     dim_genes: int = None
     n_cells: int = None
     prior: str = "normal"
 
     _initialized_from_adata: bool = False
 
@@ -58,49 +59,55 @@
     """
 
     def __init__(
         self,
         config: Union[DecipherConfig, dict] = DecipherConfig(),
     ):
         super().__init__()
-        if type(config) == dict:
+        if isinstance(config, dict):
             config = DecipherConfig(**config)
 
         if not config._initialized_from_adata:
             raise ValueError(
                 "DecipherConfig must be initialized from an AnnData object, "
                 "use `DecipherConfig.initialize_from_adata(adata)` to do so."
             )
 
         self.config = config
+        self.dummy_param = nn.Parameter(torch.empty(0))
 
         self.decoder_v_to_z = ConditionalDenseNN(
             self.config.dim_v, self.config.layers_v_to_z, [self.config.dim_z] * 2
         )
         self.decoder_z_to_x = ConditionalDenseNN(
             self.config.dim_z, config.layers_z_to_x, [self.config.dim_genes]
         )
         self.encoder_x_to_z = ConditionalDenseNN(
             self.config.dim_genes, [128], [self.config.dim_z] * 2
         )
         self.encoder_zx_to_v = ConditionalDenseNN(
-            self.config.dim_genes + self.config.dim_z, [128], [self.config.dim_v, self.config.dim_v]
+            self.config.dim_genes + self.config.dim_z,
+            [128],
+            [self.config.dim_v, self.config.dim_v],
         )
 
         self._epsilon = 1e-5
 
         self.theta = None
-        print("V5")
+
+    @property
+    def device(self):
+        return self.dummy_param.device
 
     def model(self, x, context=None):
         pyro.module("decipher", self)
 
         self.theta = pyro.param(
-            "inverse_dispersion",
-            1.0 * x.new_ones(self.config.dim_genes),
+            "theta",
+            x.new_ones(self.config.dim_genes),
             constraint=constraints.positive,
         )
 
         with pyro.plate("batch", len(x)), poutine.scale(scale=1.0):
             with poutine.scale(scale=self.config.beta):
                 if self.config.prior == "normal":
                     prior = dist.Normal(0, x.new_ones(self.config.dim_v)).to_event(1)
@@ -120,15 +127,15 @@
             # Parametrization of Negative Binomial by the mean and inverse dispersion
             # See https://github.com/pytorch/pytorch/issues/42449
             # noinspection PyTypeChecker
             logit = torch.log(library_size * mu + self._epsilon) - torch.log(
                 self.theta + self._epsilon
             )
             # noinspection PyUnresolvedReferences
-            x_dist = dist.NegativeBinomial(total_count=self.theta, logits=logit)
+            x_dist = dist.NegativeBinomial(total_count=self.theta + self._epsilon, logits=logit)
             pyro.sample("x", x_dist.to_event(1), obs=x)
 
     def guide(self, x, context=None):
         pyro.module("decipher", self)
         with pyro.plate("batch", len(x)), poutine.scale(scale=1.0):
             x = torch.log1p(x)
```

### Comparing `scdecipher-0.1.0/decipher/tools/_decipher/module.py` & `scdecipher-0.1.2/decipher/tools/_decipher/module.py`

 * *Files identical despite different names*

### Comparing `scdecipher-0.1.0/decipher/tools/basis_decomposition.py` & `scdecipher-0.1.2/decipher/tools/basis_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,19 +145,19 @@
     `adata.var['decipher_disruption_combined']` : pd.Series
         The combined disruption scores for each gene.
     `adata.uns['decipher']['disruption_scores']` : pd.DataFrame
         The disruption scores for each gene.
     `adata.uns['decipher']['disruption_scores_samples']` : pd.DataFrame
         The disruption scores for each gene sampled from the posterior.
     """
-    if type(pattern_name_a) == str:
+    if isinstance(pattern_name_a, str):
         pattern_name_a = adata.uns["decipher"]["basis_decomposition"]["pattern_names"].index(
             pattern_name_a
         )
-    if type(pattern_name_b) == str:
+    if isinstance(pattern_name_b, str):
         pattern_name_b = adata.uns["decipher"]["basis_decomposition"]["pattern_names"].index(
             pattern_name_b
         )
     idx_a = pattern_name_a
     idx_b = pattern_name_b
 
     def pairwise_distances(x, y):
```

### Comparing `scdecipher-0.1.0/decipher/tools/decipher.py` & `scdecipher-0.1.2/decipher/tools/decipher.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,50 +2,58 @@
 import os
 
 import numpy as np
 import pyro
 import scanpy as sc
 import torch
 from matplotlib import pyplot as plt
+import pyro.optim
 from pyro import poutine
 from pyro.infer import SVI, Trace_ELBO
-from pyro.optim import MultiStepLR
 from tqdm import tqdm
 
 from decipher.plot.decipher import decipher as plot_decipher_v
 from decipher.tools._decipher import Decipher, DecipherConfig
 from decipher.tools._decipher.data import (
     decipher_load_model,
     decipher_save_model,
     make_data_loader_from_adata,
+    get_dense_X,
 )
 from decipher.tools.utils import EarlyStopping
 from decipher.utils import DECIPHER_GLOBALS, GIFMaker, is_notebook, load_and_show_gif
 
 logger = logging.getLogger(__name__)
 logging.basicConfig(
     format="%(asctime)s | %(levelname)s : %(message)s",
     level=logging.INFO,
 )
 
 
-def predictive_log_likelihood(decipher, dataloader):
-    """Compute the predictive log likelihood of the decipher model."""
-    if type(dataloader) == sc.AnnData:
-        dataloader = make_data_loader_from_adata(dataloader, decipher.config.batch_size)
+def predictive_log_likelihood(decipher, dataloader, n_samples=5):
+    log_weights = []
+    old_beta = decipher.config.beta
+    decipher.config.beta = 1.0
+    try:
+        for i in range(n_samples):
+            total_log_prob = 0
+            for xc in dataloader:
+                xc = [x.to(decipher.device) for x in xc]
+                guide_trace = poutine.trace(decipher.guide).get_trace(*xc)
+                model_trace = poutine.trace(
+                    poutine.replay(decipher.model, trace=guide_trace)
+                ).get_trace(*xc)
+                total_log_prob += model_trace.log_prob_sum() - guide_trace.log_prob_sum()
+            log_weights.append(total_log_prob)
 
-    decipher.eval()
-    log_likelihood = 0
-    for xc in dataloader:
-        guide_trace = poutine.trace(decipher.guide).get_trace(*xc)
-        replayed_model = poutine.replay(decipher.model, trace=guide_trace)
-        blocked_replayed_model = poutine.block(replayed_model, expose=["x"])
-        model_trace = poutine.trace(blocked_replayed_model).get_trace(*xc)
-        log_likelihood += model_trace.log_prob_sum().item()
-    return log_likelihood / len(dataloader.dataset)
+    finally:
+        decipher.config.beta = old_beta
+
+    log_z = torch.logsumexp(torch.tensor(log_weights) - np.log(n_samples), 0)
+    return log_z.item()
 
 
 def _make_train_val_split(adata, val_frac, seed):
     n_val = int(val_frac * adata.shape[0])
     cell_idx = np.arange(adata.shape[0])
     np.random.default_rng(seed).shuffle(cell_idx)
     val_idx = cell_idx[-n_val:]
@@ -59,28 +67,31 @@
 
 
 def decipher_train(
     adata: sc.AnnData,
     decipher_config=DecipherConfig(),
     plot_every_k_epochs=-1,
     plot_kwargs=None,
+    device="cpu",
 ):
     """Train a decipher model.
 
     Parameters
     ----------
     adata: sc.AnnData
         The annotated data matrix.
     decipher_config: DecipherConfig, optional
         Configuration for the decipher model.
     plot_every_k_epochs: int, optional
         If > 0, plot the decipher space every `plot_every_k_epoch` epochs.
         Default: -1 (no plots).
     plot_kwargs: dict, optional
         Additional keyword arguments to pass to `dc.pl.decipher`.
+    device: str, optional
+        The device to use for training. Default: "cpu".
 
     Returns
     -------
     decipher: Decipher
         The trained decipher model.
     val_losses: list of float
         The validation losses at each epoch.
@@ -109,58 +120,89 @@
     adata_val = adata[val_idx, :]
 
     if plot_kwargs is None:
         plot_kwargs = dict()
 
     decipher_config.initialize_from_adata(adata_train)
 
-    dataloader_train = make_data_loader_from_adata(adata_train, decipher_config.batch_size)
+    dataloader_train = make_data_loader_from_adata(
+        adata_train, decipher_config.batch_size, drop_last=True
+    )
     dataloader_val = make_data_loader_from_adata(adata_val, decipher_config.batch_size)
 
     decipher = Decipher(
         config=decipher_config,
     )
+    decipher.to(device)
+
     optimizer = pyro.optim.ClippedAdam(
         {
             "lr": decipher_config.learning_rate,
             "weight_decay": 1e-4,
         }
     )
     elbo = Trace_ELBO()
     svi = SVI(decipher.model, decipher.guide, optimizer, elbo)
     gif_maker = GIFMaker(dpi=120)
 
     # Training loop
     val_losses = []
-    early_stopping = EarlyStopping(patience=5)
+    if (
+        decipher_config.early_stopping_patience is not None
+        and decipher_config.early_stopping_patience > 0
+    ):
+        early_stopping = EarlyStopping(patience=decipher_config.early_stopping_patience)
+    else:
+        early_stopping = EarlyStopping(patience=int(1e30))
+
     pbar = tqdm(range(decipher_config.n_epochs))
+    last_train_elbo = np.nan
+    val_nll = np.nan
     for epoch in pbar:
         train_losses = []
         decipher.train()
         if epoch > 0:
             # freeze the batch norm layers after the first epoch
             # 1) the batch norm layers helps with the initialization
             # 2) but then, they seem to imply a strong normal prior on the latent space
             for module in decipher.modules():
                 if isinstance(module, torch.nn.BatchNorm1d):
                     module.eval()
 
+        n_batches = len(dataloader_train)
+        train_elbo = 0
+        train_elbo_n_obs = 0
         for xc in dataloader_train:
-            loss = svi.step(*xc)
+            try:
+                xc = [x.to(device) for x in xc]
+                loss = svi.step(*xc)
+            except Exception as e:
+                print("ERROR", e)
+                return decipher, val_losses
             train_losses.append(loss)
+            train_elbo += loss
+            train_elbo_n_obs += xc[0].shape[0]
+            pbar.set_description(
+                f"Epoch {epoch} (batch {len(train_losses)}/{n_batches}) | "
+                f"| train elbo: {train_elbo / train_elbo_n_obs:.2f} (last epoch: {last_train_elbo:.2f}) | val ll:"
+                f" {val_nll:.2f}"
+            )
 
-        train_elbo = np.sum(train_losses) / len(dataloader_train.dataset)
         decipher.eval()
-        val_nll = -predictive_log_likelihood(decipher, dataloader_val)
+        val_nll = (
+            -predictive_log_likelihood(decipher, dataloader_val, n_samples=5) / adata_val.shape[0]
+        )
         val_losses.append(val_nll)
         pbar.set_description(
-            f"Epoch {epoch} | train elbo: {train_elbo:.2f} | val ll:" f" {val_nll:.2f}"
+            f"Epoch {epoch} (batch {len(train_losses)}/{n_batches}) | "
+            f"| train elbo: {train_elbo / train_elbo_n_obs:.2f} (last epoch: {last_train_elbo:.2f}) | val ll:"
+            f" {val_nll:.2f}"
         )
+        last_train_elbo = train_elbo / train_elbo_n_obs
         if early_stopping(val_nll):
-            print("Early stopping.")
             break
 
         if plot_every_k_epochs > 0 and (epoch % plot_every_k_epochs == 0):
             _decipher_to_adata(decipher, adata)
             plot_decipher_v(adata, basis="decipher_v", **plot_kwargs)
             gif_maker.add_image(plt.gcf())
             if is_notebook():
@@ -174,24 +216,26 @@
 
     if is_notebook():
         from IPython.core import display
 
         display.clear_output()
         pbar.display()
 
+    if early_stopping.has_stopped():
+        logger.info("Early stopping has been triggered.")
     _decipher_to_adata(decipher, adata)
     decipher_save_model(adata, decipher)
 
     model_run_id = adata.uns["decipher"]["run_id"]
     save_folder = DECIPHER_GLOBALS["save_folder"]
-    full_path = os.path.join(save_folder, model_run_id, "decipher_training.gif")
-    gif_maker.save_gif(full_path)
-
-    if is_notebook():
-        load_and_show_gif(full_path)
+    full_path = os.path.join(save_folder, str(model_run_id), "decipher_training.gif")
+    if gif_maker.images:
+        gif_maker.save_gif(full_path)
+        if is_notebook():
+            load_and_show_gif(full_path)
 
     plot_decipher_v(adata, basis="decipher_v", **plot_kwargs)
 
     return decipher, val_losses
 
 
 def rot(t, u=1):
@@ -315,22 +359,26 @@
     if "decipher_imputed" not in adata.layers:
         decipher_gene_imputation(adata)
     gene_expression_imputed = adata.layers["decipher_imputed"]
     adata.varm["decipher_v_gene_covariance"] = np.cov(
         gene_expression_imputed,
         y=adata.obsm["decipher_v"],
         rowvar=False,
-    )[: adata.X.shape[1], adata.X.shape[1]:]
-    logging.info("Added `.varm['decipher_v_gene_covariance']`: the covariance between Decipher v and each gene.")
+    )[: adata.X.shape[1], adata.X.shape[1] :]
+    logging.info(
+        "Added `.varm['decipher_v_gene_covariance']`: the covariance between Decipher v and each gene."
+    )
     adata.varm["decipher_z_gene_covariance"] = np.cov(
         gene_expression_imputed,
         y=adata.obsm["decipher_z"],
         rowvar=False,
-    )[: adata.X.shape[1], adata.X.shape[1]:]
-    logging.info("Added `.varm['decipher_z_gene_covariance']`: the covariance between Decipher z and each gene.")
+    )[: adata.X.shape[1], adata.X.shape[1] :]
+    logging.info(
+        "Added `.varm['decipher_z_gene_covariance']`: the covariance between Decipher z and each gene."
+    )
 
 
 def _decipher_to_adata(decipher, adata):
     """Compute the decipher v and z spaces from the decipher model. Add them to `adata.obsm`.
 
     Parameters
     ----------
@@ -343,12 +391,12 @@
     -------
     `adata.obsm['decipher_v']`: ndarray
         The decipher v space.
     `adata.obsm['decipher_z']`: ndarray
         The decipher z space.
     """
     decipher.eval()
-    latent_v, latent_z = decipher.compute_v_z_numpy(adata.X.toarray())
+    latent_v, latent_z = decipher.compute_v_z_numpy(get_dense_X(adata))
     adata.obsm["decipher_v"] = latent_v
     adata.obsm["decipher_z"] = latent_z
     logging.info("Added `.obsm['decipher_v']`: the Decipher v space.")
     logging.info("Added `.obsm['decipher_z']`: the Decipher z space.")
```

### Comparing `scdecipher-0.1.0/decipher/tools/trajectory_inference.py` & `scdecipher-0.1.2/decipher/tools/trajectory_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,15 +243,15 @@
     cluster_key="decipher_clusters",
 ):
     data = adata.obs[[subset_column, cluster_key]].copy()
     data.columns = ["subset", "cluster"]
     data["in_subset"] = data["subset"] == subset_value
     # clusters that contains too few cells in the subset are discarded
     # 1) the proportion of cells from the subset in the cluster is too low
-    valid_p = data.groupby("cluster").mean()["in_subset"] > subset_min_percent_per_cluster
+    valid_p = data.groupby("cluster")["in_subset"].mean() > subset_min_percent_per_cluster
     # 2) the number of cells from the subset in the cluster is too low
     valid_n = data.groupby("cluster")["in_subset"].sum() > min_cell_per_cluster
     valid_clusters = valid_p & valid_n
     valid_clusters = valid_clusters[valid_clusters].index
 
     cell_mask = data["cluster"].isin(valid_clusters)  #  & data["in_subset"]
     # TODO: #REPRODUCE# above, the commented part is for reproducibility of the main paper figures
@@ -386,15 +386,18 @@
             t_cluster_ids = nx.shortest_path(tree, start_cluster_id, end_cluster_id)
 
         logging.info(f"Trajectory {t_name} : {t_cluster_ids})")
         t_cluster_locations = np.array(
             [cluster_locations.loc[cluster_id, [0, 1]] for cluster_id in t_cluster_ids]
         ).astype(np.float32)
         trajectory = Trajectory(
-            t_cluster_locations, t_cluster_ids, point_density=point_density, rep_key=rep_key
+            t_cluster_locations,
+            t_cluster_ids,
+            point_density=point_density,
+            rep_key=rep_key,
         )
         adata.uns["decipher"][uns_key][t_name] = trajectory.to_dict()
         logging.info(f"Added trajectory {t_name} to `adata.uns['decipher']['{uns_key}']`.")
 
 
 def decipher_time(adata, n_neighbors=10):
     """Compute the decipher time for each cell, based on the inferred trajectories.
```

### Comparing `scdecipher-0.1.0/decipher/tools/utils.py` & `scdecipher-0.1.2/decipher/tools/utils.py`

 * *Files identical despite different names*

### Comparing `scdecipher-0.1.0/decipher/utils.py` & `scdecipher-0.1.2/decipher/utils.py`

 * *Files identical despite different names*

### Comparing `scdecipher-0.1.0/pyproject.toml` & `scdecipher-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "scdecipher"
-version = "0.1.0"
+version = "0.1.2"
 description = "Decipher is a single-cell analysis package to integrate and compare perturbed samples to healthy samples, to identify the origin of the cell-states perturbations."
-authors = ["Achille Nazaret <achille.nazaret@gmail.com>"]
+authors = ["Achille Nazaret"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "decipher", from="."}]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
@@ -19,7 +19,10 @@
 pyro-ppl = "^1.8.6"
 randomname = "^0.2.1"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 100
```

