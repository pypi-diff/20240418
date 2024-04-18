# Comparing `tmp/flightplotting-0.2.2.tar.gz` & `tmp/flightplotting-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplotting-0.2.2.tar", last modified: Wed Mar 20 20:41:15 2024, max compression
+gzip compressed data, was "flightplotting-0.2.3.tar", last modified: Thu Apr 18 12:18:21 2024, max compression
```

## Comparing `flightplotting-0.2.2.tar` & `flightplotting-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:41:15.993896 flightplotting-0.2.2/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)    35129 2023-03-28 15:54:20.000000 flightplotting-0.2.2/COPYING
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       34 2023-03-28 15:54:20.000000 flightplotting-0.2.2/MANIFEST.in
--rw-r--r--   0 td6834    (1001) td6834    (1001)      478 2024-03-20 20:41:15.993896 flightplotting-0.2.2/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       88 2023-03-28 15:54:20.000000 flightplotting-0.2.2/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:41:15.989896 flightplotting-0.2.2/flightplotting/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      224 2024-02-14 11:16:04.000000 flightplotting-0.2.2/flightplotting/__init__.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:41:15.993896 flightplotting-0.2.2/flightplotting/data/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)   142015 2023-03-28 15:54:20.000000 flightplotting-0.2.2/flightplotting/data/ColdDraftF3APlane.obj
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        0 2023-03-28 15:54:20.000000 flightplotting-0.2.2/flightplotting/data/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2156 2023-12-19 08:58:58.000000 flightplotting-0.2.2/flightplotting/model.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7645 2024-02-26 08:23:52.000000 flightplotting-0.2.2/flightplotting/plots.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      657 2023-12-19 08:58:58.000000 flightplotting-0.2.2/flightplotting/templates.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1298 2023-05-20 13:06:57.000000 flightplotting-0.2.2/flightplotting/titlerenderer.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7667 2024-02-14 11:15:57.000000 flightplotting-0.2.2/flightplotting/traces.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:41:15.993896 flightplotting-0.2.2/flightplotting.egg-info/
--rw-r--r--   0 td6834    (1001) td6834    (1001)      478 2024-03-20 20:41:15.000000 flightplotting-0.2.2/flightplotting.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      491 2024-03-20 20:41:15.000000 flightplotting-0.2.2/flightplotting.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2024-03-20 20:41:15.000000 flightplotting-0.2.2/flightplotting.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       42 2024-03-20 20:41:15.000000 flightplotting-0.2.2/flightplotting.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       15 2024-03-20 20:41:15.000000 flightplotting-0.2.2/flightplotting.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      443 2024-03-20 20:41:15.993896 flightplotting-0.2.2/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      668 2023-03-28 15:54:20.000000 flightplotting-0.2.2/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2024-03-20 20:41:15.993896 flightplotting-0.2.2/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      484 2023-12-19 08:58:58.000000 flightplotting-0.2.2/tests/test_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-18 12:17:36.000000 flightplotting-0.2.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-18 12:17:36.000000 flightplotting-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 12:18:21.296183 flightplotting-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 12:17:36.000000 flightplotting-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/flightplotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/flightplotting/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   142015 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/data/ColdDraftF3APlane.obj
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/titlerenderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2024-04-18 12:17:36.000000 flightplotting-0.2.3/flightplotting/traces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/flightplotting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-18 12:18:21.000000 flightplotting-0.2.3/flightplotting.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-18 12:18:21.296183 flightplotting-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-18 12:17:36.000000 flightplotting-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 12:18:21.296183 flightplotting-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-18 12:17:36.000000 flightplotting-0.2.3/tests/test_plots.py
```

### Comparing `flightplotting-0.2.2/COPYING` & `flightplotting-0.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.2/flightplotting/data/ColdDraftF3APlane.obj` & `flightplotting-0.2.3/flightplotting/data/ColdDraftF3APlane.obj`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.2/flightplotting/model.py` & `flightplotting-0.2.3/flightplotting/model.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.2/flightplotting/plots.py` & `flightplotting-0.2.3/flightplotting/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,30 +96,49 @@
     
     fig.add_traces(traces)
     
 
     return fig
 
 def plot_regions(st: State, lab_cols: list[str], span=3, colours=None, fig=None):
-    if isinstance(lab_cols, str):
-        lab_cols = [lab_cols]
+    colours = px.colors.qualitative.Plotly if colours is None else colours
+    lab_cols = [lab_cols] if isinstance(lab_cols, str) else lab_cols
+
+    st = st.label(clabs=st.cumulative_labels(*lab_cols))
+    
+    def get_base_label(clab):
+        base = clab
+        try:
+            id = int(clab.split('_')[-1])
+            base = clab[:-len(f'_{id}')]
+        except Exception:
+            pass
+        return base
+    
+    colmap = {}
+
     traces = []
-    if colours is None:
-        colours = px.colors.qualitative.Plotly
-    for i, (k, seg) in enumerate(st.split_labels(lab_cols).items()):
-        colour = colours[i % len(colours)]
-        traces += ribbon(seg, span, colour, k)
+    for i, (k, seg) in enumerate(st.split_labels('clabs').items()):
+        blab = get_base_label(k)
+        if blab not in colmap:
+            colmap[blab] = colours[len(colmap) % len(colours)]
+            leg = True
+        else:
+            leg = False
+
+        traces += ribbon(seg, span, colmap[blab], name=k, showlegend=leg)
 
         traces.append(go.Scatter3d(
             x=seg.pos.x, 
             y=seg.pos.y, 
             z=seg.pos.z,
             mode='lines', 
-            line=dict(width=6, color=colour), 
-            name=k
+            line=dict(width=6, color=colmap[blab]), 
+            name=k,
+            showlegend=False
         ))
     
     if fig is None:
         fig = go.Figure(layout=go.Layout(template="flight3d+judge_view"))
     fig.add_traces(traces)
     return fig
```

### Comparing `flightplotting-0.2.2/flightplotting/templates.py` & `flightplotting-0.2.3/flightplotting/templates.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.2/flightplotting/titlerenderer.py` & `flightplotting-0.2.3/flightplotting/titlerenderer.py`

 * *Files identical despite different names*

### Comparing `flightplotting-0.2.2/flightplotting/traces.py` & `flightplotting-0.2.3/flightplotting/traces.py`

 * *Files 6% similar despite different names*

```diff
@@ -232,24 +232,16 @@
         c = np.empty(2*len(a), dtype=a.dtype)
         c[0::2] = a
         c[1::2] = b
 
     return c
 
 
-def ribbon(sec: State, span: float, color: str, name="none"):
-    """WIP Vectorised version of ribbon, borrowed from kdoaij/FlightPlotting
-
-        refactoring ribbon, objectives:
-            speed it up by avoiding looping over array - done
-            make the colouring more generic - not yet
-        minor mod - 2 triangles per pair of points: - done
-            current pair to next left
-            current right to next pair
-        
+def ribbon(sec: State, span: float, color, **kwargs):
+    """TODO make the colouring more generic
     """
 
     left = sec.body_to_world(Point(0, span/2, 0))
     right = sec.body_to_world(Point(0, -span/2, 0))
 
     points = Point(_npinterzip(left.data, right.data))
 
@@ -263,9 +255,9 @@
     _k = _npinterzip(_ks, _ks) # 2 2 4 4 6 6 
 
 
     return [go.Mesh3d(
         x=points.x, y=points.y, z=points.z, i=_i, j=_j, k=_k,
         intensitymode="cell",
         facecolor=np.full(len(_i), color),
-        name=name,
+        **kwargs
     )]
```

### Comparing `flightplotting-0.2.2/setup.py` & `flightplotting-0.2.3/setup.py`

 * *Files identical despite different names*

