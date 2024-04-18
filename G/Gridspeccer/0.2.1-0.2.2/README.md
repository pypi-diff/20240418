# Comparing `tmp/Gridspeccer-0.2.1.tar.gz` & `tmp/gridspeccer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Gridspeccer-0.2.1.tar", last modified: Thu Feb  2 15:01:53 2023, max compression
+gzip compressed data, was "gridspeccer-0.2.2.tar", last modified: Thu Apr 18 14:29:07 2024, max compression
```

## Comparing `Gridspeccer-0.2.1.tar` & `gridspeccer-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:01:53.290505 Gridspeccer-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/AUTHORS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:01:53.290505 Gridspeccer-0.2.1/Gridspeccer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 15:01:53.000000 Gridspeccer-0.2.1/Gridspeccer.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-02 15:01:53.290505 Gridspeccer-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:01:53.290505 Gridspeccer-0.2.1/gridspeccer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/gridspeccer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28032 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/gridspeccer/aux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/gridspeccer/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/gridspeccer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 15:01:53.290505 Gridspeccer-0.2.1/gridspeccer/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/gridspeccer/defaults/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/gridspeccer/defaults/tex_matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 15:01:53.290505 Gridspeccer-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-02 15:01:39.000000 Gridspeccer-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:29:07.024164 gridspeccer-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/AUTHORS.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:29:07.024164 gridspeccer-0.2.2/Gridspeccer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 14:29:07.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-18 14:29:07.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:29:07.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 14:29:07.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-18 14:29:07.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 14:29:07.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 14:29:06.000000 gridspeccer-0.2.2/Gridspeccer.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-18 14:29:07.024164 gridspeccer-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:29:07.024164 gridspeccer-0.2.2/gridspeccer/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/gridspeccer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28032 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/gridspeccer/aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/gridspeccer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/gridspeccer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 14:29:07.024164 gridspeccer-0.2.2/gridspeccer/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/gridspeccer/defaults/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/gridspeccer/defaults/tex_matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 14:29:07.024164 gridspeccer-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-18 14:28:58.000000 gridspeccer-0.2.2/setup.py
```

### Comparing `Gridspeccer-0.2.1/LICENSE` & `gridspeccer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Gridspeccer-0.2.1/README.md` & `gridspeccer-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Gridspeccer-0.2.1/gridspeccer/aux.py` & `gridspeccer-0.2.2/gridspeccer/aux.py`

 * *Files identical despite different names*

### Comparing `Gridspeccer-0.2.1/gridspeccer/cli.py` & `gridspeccer-0.2.2/gridspeccer/cli.py`

 * *Files identical despite different names*

### Comparing `Gridspeccer-0.2.1/gridspeccer/core.py` & `gridspeccer-0.2.2/gridspeccer/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     xpos_default=0.04,
     ypos_default=0.90,
     zpos_default=0.00,
     label_xpos=None,
     label_ypos=None,
     label_zpos=None,
     label_color=None,
+    label_size=None,
     fontdict=None,
     latexformat="\\textbf{{{}}}",
     listoflabels=string.ascii_lowercase,
 ):
     """plot labels
 
     Parameters
@@ -195,38 +196,40 @@
         List of labels to be used for labelling. by default lowercase letters,
         but can be any list to accomodate uppercase or b1, b2 like labels.
     """
     label_xpos = label_xpos if label_xpos is not None else {}
     label_ypos = label_ypos if label_ypos is not None else {}
     label_zpos = label_zpos if label_zpos is not None else {}
     label_color = label_color if label_color is not None else {}
+    label_size = label_size if label_size is not None else {}
 
     for label_idx, char in zip(labels_to_plot,
                                listoflabels):
         log.info("Subplot %s receives label %s", label_idx, char)
         plot_caption(
             axes[label_idx],
             latexformat.format(char),
             xpos=label_xpos.get(label_idx, xpos_default),
             ypos=label_ypos.get(label_idx, ypos_default),
             zpos=label_zpos.get(label_idx, zpos_default),
             color=label_color.get(label_idx, "k"),
+            size=label_size.get(label_idx, 16) if isinstance(label_size, dict) else label_size,
             fontdict=fontdict,
         )
 
 
-def plot_caption(axis, caption, xpos=0.04, ypos=0.88, zpos=0.0, color="k", fontdict=None):
+def plot_caption(axis, caption, xpos=0.04, ypos=0.88, zpos=0.0, color="k", size=16, fontdict=None):
     "plot caption"
     # find out how our caption will look in reality
     caption_args = {
         "ha": "left",
         "va": "bottom",
         # "weight": "bold",
         "style": "normal",
-        "size": 16,
+        "size": size,
         "color": color,
         "zorder": 1000,
     }
     # r = get_renderer(axis.figure)
     # bb = t.get_window_extent(renderer=r)
 
     # if fontdict is None:
```

### Comparing `Gridspeccer-0.2.1/gridspeccer/defaults/matplotlibrc` & `gridspeccer-0.2.2/gridspeccer/defaults/matplotlibrc`

 * *Files identical despite different names*

### Comparing `Gridspeccer-0.2.1/gridspeccer/defaults/tex_matplotlibrc` & `gridspeccer-0.2.2/gridspeccer/defaults/tex_matplotlibrc`

 * *Files identical despite different names*

### Comparing `Gridspeccer-0.2.1/setup.py` & `gridspeccer-0.2.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 """making plotting of multipanel plots easier with dedicated gridspec use"""
 
 from setuptools import setup, find_packages
 
-VERSION = "0.2.1"
+VERSION = "0.2.2"
 
 setup(
     name="Gridspeccer",
     version=VERSION,
     description="Helper scripts to organize multi-figure plots.",
     author="Oliver Breitwieser",
     author_email="oliver.breitwieser@kip.uni-heidelberg.de",
```

