# Comparing `tmp/virusrecom-1.1.4.tar.gz` & `tmp/virusrecom-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\virusrecom-1.1.4.tar", last modified: Wed Mar 13 07:55:17 2024, max compression
+gzip compressed data, was "dist\virusrecom-1.1.5.tar", last modified: Thu Apr 18 13:23:40 2024, max compression
```

## Comparing `virusrecom-1.1.4.tar` & `virusrecom-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 07:55:17.000000 virusrecom-1.1.4/
--rw-rw-rw-   0        0        0    26526 2023-03-06 15:44:50.000000 virusrecom-1.1.4/LICENSE
--rw-rw-rw-   0        0        0    18436 2024-03-13 07:55:17.000000 virusrecom-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    16997 2024-01-24 14:09:37.000000 virusrecom-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-03-13 07:55:17.000000 virusrecom-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-03-13 07:33:44.000000 virusrecom-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom/
--rw-rw-rw-   0        0        0      340 2023-08-09 12:54:33.000000 virusrecom-1.1.4/virusrecom/__init__.py
--rw-rw-rw-   0        0        0    15464 2024-01-08 14:00:12.000000 virusrecom-1.1.4/virusrecom/corecp.py
--rw-rw-rw-   0        0        0    17814 2024-03-13 07:34:15.000000 virusrecom-1.1.4/virusrecom/main.py
--rw-rw-rw-   0        0        0    21972 2024-03-13 07:35:35.000000 virusrecom-1.1.4/virusrecom/my_func.py
--rw-rw-rw-   0        0        0     2450 2023-03-06 15:44:50.000000 virusrecom-1.1.4/virusrecom/plt_corlor_list.py
--rw-rw-rw-   0        0        0     1956 2023-03-06 15:44:50.000000 virusrecom-1.1.4/virusrecom/sequence_align.py
-drwxrwxrwx   0        0        0        0 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/
--rw-rw-rw-   0        0        0    18436 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       89 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-13 07:55:17.000000 virusrecom-1.1.4/virusrecom.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 13:23:40.000000 virusrecom-1.1.5/
+-rw-rw-rw-   0        0        0    26526 2023-03-06 15:44:50.000000 virusrecom-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0    18436 2024-04-18 13:23:40.000000 virusrecom-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16997 2024-01-24 14:09:37.000000 virusrecom-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-18 13:23:40.000000 virusrecom-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-04-18 09:18:11.000000 virusrecom-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:23:40.000000 virusrecom-1.1.5/virusrecom/
+-rw-rw-rw-   0        0        0      340 2023-08-09 12:54:33.000000 virusrecom-1.1.5/virusrecom/__init__.py
+-rw-rw-rw-   0        0        0    15464 2024-01-08 14:00:12.000000 virusrecom-1.1.5/virusrecom/corecp.py
+-rw-rw-rw-   0        0        0    17814 2024-04-18 09:18:39.000000 virusrecom-1.1.5/virusrecom/main.py
+-rw-rw-rw-   0        0        0    21939 2024-04-18 09:19:48.000000 virusrecom-1.1.5/virusrecom/my_func.py
+-rw-rw-rw-   0        0        0     2424 2024-04-18 13:21:37.000000 virusrecom-1.1.5/virusrecom/plt_corlor_list.py
+-rw-rw-rw-   0        0        0     1956 2023-03-06 15:44:50.000000 virusrecom-1.1.5/virusrecom/sequence_align.py
+drwxrwxrwx   0        0        0        0 2024-04-18 13:23:40.000000 virusrecom-1.1.5/virusrecom.egg-info/
+-rw-rw-rw-   0        0        0    18436 2024-04-18 13:23:39.000000 virusrecom-1.1.5/virusrecom.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-04-18 13:23:39.000000 virusrecom-1.1.5/virusrecom.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 13:23:39.000000 virusrecom-1.1.5/virusrecom.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-18 13:23:39.000000 virusrecom-1.1.5/virusrecom.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       89 2024-04-18 13:23:39.000000 virusrecom-1.1.5/virusrecom.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-18 13:23:39.000000 virusrecom-1.1.5/virusrecom.egg-info/top_level.txt
```

### Comparing `virusrecom-1.1.4/LICENSE` & `virusrecom-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `virusrecom-1.1.4/PKG-INFO` & `virusrecom-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virusrecom
-Version: 1.1.4
+Version: 1.1.5
 Summary: An information-theory-based method for recombination detection of viral lineages.
 Home-page: https://github.com/ZhijianZhou01/virusrecom
 Author: Zhi-Jian Zhou
 Author-email: zjzhou@hnu.edu.cn
 Keywords: recombination,virus,evolution,information entropy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `virusrecom-1.1.4/README.md` & `virusrecom-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `virusrecom-1.1.4/setup.py` & `virusrecom-1.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r",encoding="utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="virusrecom",
-  version="1.1.4",
+  version="1.1.5",
   author="Zhi-Jian Zhou",
   author_email="zjzhou@hnu.edu.cn",
   description="An information-theory-based method for recombination detection of viral lineages.",
   keywords="recombination, virus, evolution, information entropy",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ZhijianZhou01/virusrecom",
```

### Comparing `virusrecom-1.1.4/virusrecom/corecp.py` & `virusrecom-1.1.5/virusrecom/corecp.py`

 * *Files identical despite different names*

### Comparing `virusrecom-1.1.4/virusrecom/main.py` & `virusrecom-1.1.5/virusrecom/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     print("\n" + "-------------------------------------------------")
 
     print("  Name: Virus Recombination (VirusRecom)")
 
     print(
         "  Description: Detecting recombination of viral lineages (or subtypes) using information theory.")
 
-    print("  Version: 1.1.4 (2024-03-13)")
+    print("  Version: 1.1.5 (2024-04-18)")
 
     print("  Author: Zhi-Jian Zhou")
 
     print("  Citation: Brief Bioinform. 2023 Jan 19;24(1)")
 
     print("-------------------------------------------------" + "\n")
```

### Comparing `virusrecom-1.1.4/virusrecom/my_func.py` & `virusrecom-1.1.5/virusrecom/my_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,15 +552,15 @@
 
 
 
 def wic_plot(lineage_name,site_list,input_data,query_lineage_name,output_path):
 
     lineage_count = len(lineage_name)
 
-    fig_high = int(max(site_list) * 3 / 10000) * 2
+    fig_high = int(lineage_count * 2)
 
     fig, ax = plt.subplots(len(lineage_name), 1,
                            figsize=(
                            lineage_count, fig_high))
 
     fig.suptitle("Query seq: " + query_lineage_name, family="Arial")
     fig.tight_layout()
@@ -745,15 +745,15 @@
 
     # print(breakpoint_data)
 
     breakpoint_data.to_excel(
         excel_writer=break_p_data,
         index=False)
 
-    fig_high2 = int(max(central_pos_list) * 3 / 10000) * 2
+    fig_high2 = int(lineage_count * 2)
 
     figs, axs = plt.subplots(lineage_count, 1, figsize=(lineage_count,
                                                         fig_high2))
 
     figs.suptitle("Query seq: " + query_seq_prefix, family="Arial")
     figs.tight_layout()
```

### Comparing `virusrecom-1.1.4/virusrecom/plt_corlor_list.py` & `virusrecom-1.1.5/virusrecom/plt_corlor_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,19 +15,17 @@
 "#b3de69",
 "#fccde5",
 "#d9d9d9",
 "#e5d8bd",
 "#ccebc5",
 "#694d9f",
 "#80b1d3",
-"#bebada", # AY.45
-"#8dd3c7", # BA.2
-"#fb8072", # BA.1
-
-
+"#bebada",
+"#8dd3c7",
+"#fb8072",
 "olivedrab",
 "darkorange",
 "darkcyan",
 "darkblue",
 "dodgerblue",
 "lightgreen",
 "orangered",
```

### Comparing `virusrecom-1.1.4/virusrecom/sequence_align.py` & `virusrecom-1.1.5/virusrecom/sequence_align.py`

 * *Files identical despite different names*

### Comparing `virusrecom-1.1.4/virusrecom.egg-info/PKG-INFO` & `virusrecom-1.1.5/virusrecom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: virusrecom
-Version: 1.1.4
+Version: 1.1.5
 Summary: An information-theory-based method for recombination detection of viral lineages.
 Home-page: https://github.com/ZhijianZhou01/virusrecom
 Author: Zhi-Jian Zhou
 Author-email: zjzhou@hnu.edu.cn
 Keywords: recombination,virus,evolution,information entropy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

