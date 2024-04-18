# Comparing `tmp/ocp_tessellate-2.2.2.tar.gz` & `tmp/ocp_tessellate-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-2.2.2.tar", last modified: Sat Mar 23 16:43:54 2024, max compression
+gzip compressed data, was "ocp_tessellate-2.3.0.tar", last modified: Wed Apr 17 18:21:06 2024, max compression
```

## Comparing `ocp_tessellate-2.2.2.tar` & `ocp_tessellate-2.3.0.tar`

### file list

```diff
@@ -1,25 +1,41 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:43:54.025211 ocp_tessellate-2.2.2/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2024-03-23 16:43:54.025268 ocp_tessellate-2.2.2/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-2.2.2/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:43:54.024394 ocp_tessellate-2.2.2/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2980 2023-11-24 07:13:16.000000 ocp_tessellate-2.2.2/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2024-03-23 16:43:44.000000 ocp_tessellate-2.2.2/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    15543 2024-03-23 14:19:47.000000 ocp_tessellate-2.2.2/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    32764 2024-03-17 10:14:02.000000 ocp_tessellate-2.2.2/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10683 2024-03-17 10:14:02.000000 ocp_tessellate-2.2.2/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-06-19 18:39:04.000000 ocp_tessellate-2.2.2/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3048 2023-11-24 07:13:16.000000 ocp_tessellate-2.2.2/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    25136 2024-03-14 07:11:29.000000 ocp_tessellate-2.2.2/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-06-19 19:00:22.000000 ocp_tessellate-2.2.2/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    15833 2024-01-17 07:33:06.000000 ocp_tessellate-2.2.2/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1065 2023-11-24 07:13:16.000000 ocp_tessellate-2.2.2/ocp_tessellate/trace.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-27 16:19:21.000000 ocp_tessellate-2.2.2/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-03-23 16:43:54.025093 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2024-03-23 16:43:53.000000 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      585 2024-03-23 16:43:54.000000 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-03-23 16:43:53.000000 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-03-23 16:43:53.000000 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      112 2024-03-23 16:43:53.000000 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2024-03-23 16:43:53.000000 ocp_tessellate-2.2.2/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2024-03-23 16:43:54.025507 ocp_tessellate-2.2.2/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1627 2024-03-23 16:43:44.000000 ocp_tessellate-2.2.2/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:21:06.869821 ocp_tessellate-2.3.0/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-17 18:21:06.869753 ocp_tessellate-2.3.0/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-2.3.0/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:21:06.866662 ocp_tessellate-2.3.0/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2942 2024-04-14 10:24:20.000000 ocp_tessellate-2.3.0/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2024-04-14 16:37:56.000000 ocp_tessellate-2.3.0/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    15868 2024-04-14 16:23:53.000000 ocp_tessellate-2.3.0/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    35114 2024-04-17 06:20:41.000000 ocp_tessellate-2.3.0/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10683 2024-03-17 10:14:02.000000 ocp_tessellate-2.3.0/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-06-19 18:39:04.000000 ocp_tessellate-2.3.0/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3048 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.0/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    25136 2024-03-14 07:11:29.000000 ocp_tessellate-2.3.0/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-06-19 19:00:22.000000 ocp_tessellate-2.3.0/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    18140 2024-04-16 19:28:47.000000 ocp_tessellate-2.3.0/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1065 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.0/ocp_tessellate/trace.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6177 2024-04-14 10:38:44.000000 ocp_tessellate-2.3.0/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:21:06.869325 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1109 2024-04-17 18:21:06.000000 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      975 2024-04-17 18:21:06.000000 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-17 18:21:06.000000 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2024-04-17 18:21:06.000000 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      112 2024-04-17 18:21:06.000000 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2024-04-17 18:21:06.000000 ocp_tessellate-2.3.0/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2024-04-17 18:21:06.870057 ocp_tessellate-2.3.0/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1627 2024-04-14 16:37:56.000000 ocp_tessellate-2.3.0/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2024-04-17 18:21:06.869130 ocp_tessellate-2.3.0/tests/
+-rw-r--r--   0 bernhard   (501) staff       (20)     1419 2024-03-21 20:20:19.000000 ocp_tessellate-2.3.0/tests/test_cache.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1100 2024-01-17 07:33:06.000000 ocp_tessellate-2.3.0/tests/test_cadquery_sketch.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      895 2023-06-17 10:13:33.000000 ocp_tessellate-2.3.0/tests/test_color.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1200 2023-06-19 17:26:20.000000 ocp_tessellate-2.3.0/tests/test_coordsystem.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     2027 2023-11-28 20:16:07.000000 ocp_tessellate-2.3.0/tests/test_instances.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      516 2023-06-19 19:05:58.000000 ocp_tessellate-2.3.0/tests/test_parallel.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      870 2023-11-24 07:13:16.000000 ocp_tessellate-2.3.0/tests/test_partgroup.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      637 2023-06-19 17:37:19.000000 ocp_tessellate-2.3.0/tests/test_stl.py
+-rw-r--r--   0 bernhard   (501) staff       (20)      811 2024-03-21 20:15:15.000000 ocp_tessellate-2.3.0/tests/tests_build123d assembly.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8564 2024-01-17 07:33:06.000000 ocp_tessellate-2.3.0/tests/tests_build123d hinge.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3328 2023-11-28 20:16:07.000000 ocp_tessellate-2.3.0/tests/tests_build123d.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1879 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.0/tests/tests_cadquery.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3022 2023-06-19 17:42:50.000000 ocp_tessellate-2.3.0/tests/tests_cadquery_boxes.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3697 2023-07-21 16:20:28.000000 ocp_tessellate-2.3.0/tests/tests_cadquery_door.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     8496 2023-11-21 06:59:53.000000 ocp_tessellate-2.3.0/tests/tests_cadquery_hexapod.py
```

### Comparing `ocp_tessellate-2.2.2/PKG-INFO` & `ocp_tessellate-2.3.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 2.2.2
+Version: 2.3.0
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -12,10 +12,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
+Requires-Dist: webcolors~=1.12
+Requires-Dist: numpy
+Requires-Dist: numpy-quaternion
+Requires-Dist: cachetools~=5.2.0
+Requires-Dist: imagesize
 Provides-Extra: dev
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pyYaml; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/__init__.py` & `ocp_tessellate-2.3.0/ocp_tessellate/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 from ._version import __version_info__ as ot_version_info
 from .cad_objects import (
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_PartGroup,
     OCP_Vertices,
-    get_instances,
-    set_instances,
 )
 from .convert import web_color
 from .defaults import (
     create_args,
     get_default,
     get_defaults,
     reset_defaults,
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/_version.py` & `ocp_tessellate-2.3.0/ocp_tessellate/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "2.2.2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "2.3.0"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/cad_objects.py` & `ocp_tessellate-2.3.0/ocp_tessellate/cad_objects.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,53 +44,43 @@
 from .defaults import get_default
 import imagesize
 
 UNSELECTED = 0
 SELECTED = 1
 EMPTY = 3
 
-PROTOCOL_VERSION = 2
+PROTOCOL_VERSION = 3
 
 #
 # Simple Part and PartGroup classes
 #
 
 
 class Instance:
     def __init__(self, shape):
         self.shape = shape
         self.mesh = None
         self.quality = None
 
 
-INSTANCES = []
-
-
-def get_instances():
-    return [instance.mesh for instance in INSTANCES]
-
-
-def set_instances(instances):
-    global INSTANCES
-    INSTANCES = [Instance(instance) for instance in instances]
-
-
 class CADObject(object):
     def __init__(self):
         self.color = Color(get_default("default_color"))
 
     def to_state(self):
         raise NotImplementedError("not implemented yet")
 
     def to_assembly(self):
         raise NotImplementedError("not implemented yet")
 
     def collect_shapes(
         self,
         path,
+        instances,
+        meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
         parallel,
         progress,
@@ -130,30 +120,37 @@
 
     def to_assembly(self):
         return OCP_PartGroup([self])
 
     def collect_shapes(
         self,
         path,
+        instances,
+        meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
         parallel=False,
         progress=None,
         timeit=False,
     ):
         self.id = f"{path}/{self.name}"
 
         if isinstance(self.shape, dict):
             ind = self.shape["ref"]
-            shape = [INSTANCES[ind].shape]
-            mesh = INSTANCES[ind].mesh
-            quality = INSTANCES[ind].quality
+            if isinstance(instances[ind], Instance):
+                mesh = instances[ind].mesh
+            else:
+                shape = instances[ind][1]
+                if not isinstance(shape, (list, tuple)):
+                    shape = [shape]
+                meshed_instances[ind] = Instance(shape)
+                mesh = None
         else:
             ind = None
             shape = self.shape
             mesh = None
 
         if mesh is None:
             with Timer(timeit, self.name, "compute quality:", 2) as t:
@@ -183,25 +180,25 @@
             combined_loc = get_location(loc, False)
             if self.loc is not None:
                 combined_loc = combined_loc * self.loc
             t, q = loc_to_tq(combined_loc)
 
             if parallel and is_apply_result(mesh):
                 # store the instance mesh
-                if ind is not None and INSTANCES[ind].mesh is None:
-                    INSTANCES[ind].mesh = mesh
-                    INSTANCES[ind].quality = quality
+                if ind is not None and meshed_instances[ind].mesh is None:
+                    meshed_instances[ind].mesh = mesh
+                    meshed_instances[ind].quality = quality
                 mesh = {"ref": ind, "t": t, "q": q}
                 bb = {}
             else:
                 bb = np_bbox(mesh["vertices"], t, q)
                 # store the instance mesh
-                if ind is not None and INSTANCES[ind].mesh is None:
-                    INSTANCES[ind].mesh = mesh
-                    INSTANCES[ind].quality = quality
+                if ind is not None and meshed_instances[ind].mesh is None:
+                    meshed_instances[ind].mesh = mesh
+                    meshed_instances[ind].quality = quality
 
                 if isinstance(self.shape, dict):
                     mesh = self.shape  # return the instance id
 
         if isinstance(self.color, tuple):
             color = [c.web_color for c in self.color]  # pylint: disable=not-an-iterable
             alpha = 1.0
@@ -280,14 +277,16 @@
 
     def to_assembly(self):
         return OCP_PartGroup([self])
 
     def collect_shapes(
         self,
         path,
+        instances,
+        meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
         parallel=False,
         progress=None,
@@ -341,14 +340,16 @@
 
     def to_assembly(self):
         return OCP_PartGroup([self])
 
     def collect_shapes(
         self,
         path,
+        instances,
+        meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
         parallel=False,
         progress=None,
@@ -398,14 +399,16 @@
 
     def add_list(self, cad_objs):
         self.objects += cad_objs
 
     def collect_shapes(
         self,
         path,
+        instances,
+        meshed_instances,
         loc,
         deviation,
         angular_tolerance,
         edge_accuracy,
         render_edges,
         parallel=False,
         progress=None,
@@ -429,14 +432,16 @@
         }
 
         map = {"parts": [], "id": self.id}
 
         for obj in self.objects:
             mapping, mesh = obj.collect_shapes(
                 self.id,
+                instances,
+                meshed_instances,
                 combined_loc,
                 deviation,
                 angular_tolerance,
                 edge_accuracy,
                 render_edges,
                 parallel,
                 progress,
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/convert.py` & `ocp_tessellate-2.3.0/ocp_tessellate/convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,27 +11,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from collections.abc import Iterable
-
+import enum
 import json
 
+import numpy as np
+
 from .cad_objects import (
     CoordSystem,
     CoordAxis,
+    CADObject,
     OCP_Edges,
     OCP_Faces,
     OCP_Part,
     OCP_PartGroup,
     OCP_Vertices,
-    get_instances,
-    set_instances,
 )
 from .defaults import get_default, preset
 from .mp_tessellator import get_mp_result, is_apply_result
 from .ocp_utils import (
     BoundingBox,
     copy_shape,
     downcast,
@@ -109,32 +110,35 @@
 
 
 def web_color(name):
     wc = Color(name)
     return ocp_color(*wc.percentage)
 
 
-def tessellate_group(group, kwargs=None, progress=None, timeit=False):
+def tessellate_group(group, instances, kwargs=None, progress=None, timeit=False):
     if kwargs is None:
         kwargs = {}
 
-    map, shapes = group.collect_shapes(
+    meshed_instances = [None] * len(instances)
+    mapping, shapes = group.collect_shapes(
         "",
+        instances,
+        meshed_instances,
         None,
         deviation=preset("deviation", kwargs.get("deviation")),
         angular_tolerance=preset("angular_tolerance", kwargs.get("angular_tolerance")),
         edge_accuracy=preset("edge_accuracy", kwargs.get("edge_accuracy")),
         render_edges=preset("render_edges", kwargs.get("render_edges")),
         parallel=kwargs.get("parallel"),
         progress=progress,
         timeit=timeit,
     )
     states = group.to_state()
 
-    return get_instances(), shapes, states, map
+    return [instance.mesh for instance in meshed_instances], shapes, states, mapping
 
 
 def combined_bb(shapes):
     def c_bb(shapes, bb):
         for shape in shapes["parts"]:
             if shape.get("parts") is None:
                 if bb is None:
@@ -515,16 +519,38 @@
     for obj_name, obj_color, obj_alpha, cad_obj in zip(names, colors, alphas, cad_objs):
         #
         # Retrieve the provided color or get default color
         # OCP_Faces, OCP_edges and OCP_Vertices bring their own color info
         # TODO default color for shapes is used
         #
 
-        # filter color objects that can come from vscode_ocp_cad_viewer
-        if is_ocp_color(cad_obj):
+        # Silently skip enums and known types
+        if (
+            isinstance(cad_obj, enum.Enum)
+            or is_ocp_color(cad_obj)
+            or isinstance(cad_obj, (int, float, bool, str, np.number, np.ndarray))
+        ):
+            continue
+
+        if not (
+            is_wrapped(cad_obj)
+            or isinstance(cad_obj, (CADObject, Iterable, dict))
+            or is_cadquery(cad_obj)
+            or is_cadquery_assembly(cad_obj)
+            or is_cadquery_sketch(cad_obj)
+            or is_build123d(cad_obj)
+            or is_compound(cad_obj)
+            or is_topods_shape(cad_obj)
+            or is_toploc_location(cad_obj)
+        ):
+            print(
+                "Skipping object"
+                + ("" if obj_name is None else f" '{obj_name}'")
+                + f" of type {type(cad_obj)}"
+            )
             continue
 
         if not isinstance(cad_obj, (OCP_Faces, OCP_Edges, OCP_Vertices)):
             if hasattr(cad_obj, "color") and cad_obj.color is not None:
                 *color, alpha = get_rgba(cad_obj.color, obj_alpha, Color(default_color))
             else:
                 color, alpha = obj_color, obj_alpha
@@ -550,14 +576,18 @@
             len(cad_obj.objects) == 0
             or (len(cad_obj.objects) == 1 and is_vector(cad_obj.objects[0]))
         ):  # Workplane:
             cad_obj = cad_obj.plane.location
             if obj_name is None:
                 obj_name = "workplane"
 
+        # ensure builder objects participate in finding instances
+        if is_build123d(cad_obj) and hasattr(cad_obj, "_obj"):
+            cad_obj = cad_obj._obj
+
         if is_cadquery_assembly(cad_obj):
             _debug("to_assembly: cadquery assembly", obj_name)
 
             add_to_ass = False
             if is_assembly:
                 ass = pg
                 ass.name = cad_obj.name
@@ -687,41 +717,69 @@
         elif (
             isinstance(cad_obj, Iterable)
             and not hasattr(cad_obj, "wrapped")
             and not hasattr(cad_obj, "first")
             and not hasattr(cad_obj, "last")
         ):
             _debug(
-                "to_assembly: iterables other then Compounds and ShapeLists", obj_name
+                "to_assembly: iterables other than Compounds and ShapeLists", obj_name
+            )
+
+            pg2 = OCP_PartGroup(
+                [],
+                name=(
+                    ("Dict" if isinstance(cad_obj, dict) else "List")
+                    if obj_name is None
+                    else obj_name
+                ),
             )
+            if isinstance(cad_obj, dict):
+                named_child = cad_obj.items()
+            else:
+                named_child = zip([None] * len(list(cad_obj)), cad_obj)
+
+            for name, child in named_child:
+                if hasattr(child, "name") and child.name is not None:
+                    name = child.name
+                elif (
+                    hasattr(child, "label")
+                    and child.label is not None
+                    and child.label != ""
+                ):
+                    name = child.label
+                elif not isinstance(cad_obj, dict):
+                    name = obj_name
 
-            pg2 = OCP_PartGroup([], name="List" if obj_name is None else obj_name)
-            for child in cad_obj:
                 part, instances = _to_assembly(
                     child,
                     default_color=default_color,
-                    names=None,
+                    names=[name],
                     colors=[obj_color],
                     alphas=[obj_alpha],
                     render_mates=render_mates,
                     render_joints=render_joints,
                     helper_scale=helper_scale,
                     instances=instances,
                     progress=progress,
                     is_assembly=is_assembly,
                 )
                 if isinstance(part, OCP_PartGroup) and len(part.objects) == 1:
                     pg2.add(part.objects[0])
                 else:
-                    pg2.add(part)
+                    if len(part.objects) > 0:
+                        pg2.add(part)
 
-            names = make_unique([obj.name for obj in pg2.objects])
-            for name, obj in zip(names, pg2.objects):
-                obj.name = name
-            pg.add(pg2)
+            if len(pg2.objects) > 0:
+                if len(pg2.objects) == 1:
+                    pg.add(pg2.objects[0])
+                else:
+                    names = make_unique([obj.name for obj in pg2.objects])
+                    for name, obj in zip(names, pg2.objects):
+                        obj.name = name
+                    pg.add(pg2)
 
         elif hasattr(cad_obj, "wrapped") and (
             is_toploc_location(cad_obj.wrapped) or is_gp_plane(cad_obj.wrapped)
         ):
             if is_gp_plane(cad_obj.wrapped) and hasattr(cad_obj, "location"):
                 cad_obj = cad_obj.location
 
@@ -864,14 +922,26 @@
                         loc=identity_location(),  # mates inherit the parent location, so actually add a no-op
                     )
 
                     # add mates partgroup
                     if pg2.objects:
                         pg.add(pg2)
 
+        elif is_topods_solid(cad_obj):
+            _debug("    to_assembly: TopoDS_Solid", obj_name)
+            part = get_instance(
+                cad_obj,
+                id(cad_obj),
+                obj_name,
+                rgba,
+                instances,
+                progress,
+            )
+            pg.add(part)
+
         else:
             _debug("to_assembly: generic case", obj_name)
             #
             # Render non iterable objects
             #
 
             # cad_obj.wrapped and cad_obj.obj.wrapped behave the same way
@@ -984,16 +1054,15 @@
     if len(pg.objects) == 1 and isinstance(pg.objects[0], OCP_PartGroup):
         if pg.objects[0].loc is None:
             pg.objects[0].loc = pg.loc
         elif pg.loc is not None:
             pg.objects[0].loc = pg.loc * pg.objects[0].loc
         pg = pg.objects[0]
 
-    set_instances([instance[1] for instance in instances])
-    return pg
+    return pg, instances
 
 
 def export_three_cad_viewer_json(*objs, filename=None):
     def decode(instances, shapes):
         def walk(obj):
             typ = None
             for attr in obj.keys():
@@ -1008,16 +1077,16 @@
                     if typ == "shapes":
                         if obj["shape"].get("ref") is not None:
                             ind = obj["shape"]["ref"]
                             obj["shape"] = instances[ind]
 
         walk(shapes)
 
-    part_group = to_assembly(*objs)
-    instances, shapes, states, map = tessellate_group(part_group)
+    part_group, instances = to_assembly(*objs)
+    instances, shapes, states, map = tessellate_group(part_group, instances)
     decode(instances, shapes)
 
     j = numpy_to_json([shapes, states])
     if filename is None:
         return j
     else:
         with open(filename, "w") as fd:
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/defaults.py` & `ocp_tessellate-2.3.0/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/mp_tess.py` & `ocp_tessellate-2.3.0/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-2.3.0/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-2.3.0/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/stepreader.py` & `ocp_tessellate-2.3.0/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/tessellator.py` & `ocp_tessellate-2.3.0/ocp_tessellate/tessellator.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,14 +48,35 @@
     get_face_type,
     get_edge_type,
     is_line,
     length,
 )
 from .trace import Trace
 
+try:
+    from ocp_addons.tessellator import tessellate as tessellate_c
+
+    def enable_native_tessellator():
+        os.environ["NATIVE_TESSELLATOR"] = "1"
+
+    def disable_native_tessellator():
+        os.environ["NATIVE_TESSELLATOR"] = "0"
+
+    def is_native_tessellator_enabled():
+        return os.environ.get("NATIVE_TESSELLATOR") == "1"
+
+    if os.environ.get("NATIVE_TESSELLATOR") is None:
+        enable_native_tessellator()
+
+    NATIVE = True
+
+except ImportError:
+
+    NATIVE = False
+
 MAX_HASH_KEY = 2147483647
 LOG_FILE = "ocp_tessellate.log"
 
 #
 # Caching helpers
 #
 
@@ -140,17 +161,19 @@
     }
 
 
 class Tessellator:
     def __init__(self, shape_id):
         self.shape_id = shape_id
         self.triangles = []
+        self.triangles_per_face = []
         self.vertices = []  # triangle vertices
         self.normals = []
         self.edges = []
+        self.segments_per_edge = []
 
         self.obj_vertices = []  # object vertices
         self.face_types = []
         self.edge_types = []
 
         self.shape = None
 
@@ -173,23 +196,23 @@
     ):
         self.shape = shape
 
         count = self.number_solids(shape)
         with Timer(
             debug,
             "",
-            f"mesh incrementally {'(parallel)' if count > 1 else ''}",
+            f"mesh incrementally",
             3,
             debug,
         ):
             # Remove previous mesh data
-            BRepTools.Clean_s(shape)
-            BRepMesh_IncrementalMesh(
-                shape, quality, False, angular_tolerance, count > 1
-            )
+            # https://dev.opencascade.org/node/81262#comment-21130
+            # BRepTools.Clean_s(shape)
+            # print(quality, False, angular_tolerance, True)
+            BRepMesh_IncrementalMesh(shape, quality, False, angular_tolerance, True)
 
         trace = Trace(LOG_FILE)
 
         if compute_faces:
             with Timer(debug, "", "get nodes, triangles and normals", 3):
                 self.tessellate(trace)
 
@@ -223,19 +246,15 @@
                 i1, i2 = 1, 2
 
             internal = face.Orientation() == TopAbs_Orientation.TopAbs_INTERNAL
 
             self.face_types.append(get_face_type(face).value)
 
             poly = BRep_Tool.Triangulation_s(face, loc_buf)
-            if poly is None:
-                self.vertices.extend([])
-                self.triangles.append([])
-                self.normals.extend([])
-            else:
+            if poly is not None:
                 Trsf = loc_buf.Transformation()
 
                 # add vertices
                 flat = []
                 for i in range(1, poly.NbNodes() + 1):
                     flat.extend(poly.Node(i).Transformed(Trsf).Coord())
                 self.vertices.extend(flat)
@@ -243,15 +262,16 @@
                 # add triangles
                 flat = []
                 for i in range(1, poly.NbTriangles() + 1):
                     coord = poly.Triangle(i).Get()
                     flat.extend(
                         (coord[0] + offset, coord[i1] + offset, coord[i2] + offset)
                     )
-                self.triangles.append(flat)
+                self.triangles.extend(flat)
+                self.triangles_per_face.append(poly.NbTriangles())
 
                 # add normals
                 if poly.HasUVNodes():
                     prop = BRepGProp_Face(face)
                     flat = []
                     for i in range(1, poly.NbNodes() + 1):
                         u, v = poly.UVNode(i).Coord()
@@ -313,45 +333,104 @@
                 index = indices.Value
 
             transf = loc.Transformation()
             v1 = None
             for j in nrange:
                 v2 = triangle.Node(index(j)).Transformed(transf).Coord()
                 if v1 is not None:
-                    edges.append((v1, v2))
+                    edges.extend((v1, v2))
                 v1 = v2
-            self.edges.append(edges)
+            self.edges.extend(edges)
+            self.segments_per_edge.append(len(edges) // 2)
 
         if len(self.edges) == 0:
             self._compute_missing_edges()
 
     def get_vertices(self):
         return np.asarray(self.vertices, dtype=np.float32)
 
     def get_triangles(self):
-        return [np.asarray(t, dtype=np.int32) for t in self.triangles]
+        return np.asarray(self.triangles, dtype=np.int32)
+
+    def get_triangles_per_face(self):
+        return np.asarray(self.triangles_per_face, dtype=np.int32)
 
     def get_face_types(self):
         return np.asarray(self.face_types, dtype=np.int32)
 
     def get_edge_types(self):
         return np.asarray(self.edge_types, dtype=np.int32)
 
     def get_normals(self):
         if len(self.normals) == 0:
             self._compute_missing_normals()
         return np.asarray(self.normals, dtype=np.float32)
 
     def get_edges(self):
-        return [np.asarray(edge, dtype=np.float32) for edge in self.edges]
+        return np.asarray(self.edges, dtype=np.float32)
+
+    def get_segments_per_edge(self):
+        return np.asarray(self.segments_per_edge, dtype=np.int32)
 
     def get_obj_vertices(self):
         return np.asarray(self.obj_vertices, dtype=np.float32)
 
 
+class NativeTessellator:
+    def __init__(self, shape_id):
+        self.shape_id = shape_id
+        self.mesh = None
+
+    def compute(
+        self,
+        shape,
+        quality,
+        angular_tolerance,
+        compute_faces=True,
+        compute_edges=True,
+        debug=False,
+    ):
+        self.mesh = tessellate_c(
+            # shape, quality, angular_tolerance, parallel=True, debug=debug, timeit=debug
+            shape,
+            quality,
+            angular_tolerance,
+            True,
+            0,
+            debug,
+        )
+
+    def get_vertices(self):
+        return self.mesh.vertices
+
+    def get_triangles(self):
+        return self.mesh.triangles
+
+    def get_triangles_per_face(self):
+        return self.mesh.triangles_per_face
+
+    def get_face_types(self):
+        return self.mesh.face_types
+
+    def get_edge_types(self):
+        return self.mesh.edge_types
+
+    def get_normals(self):
+        return self.mesh.normals
+
+    def get_edges(self):
+        return self.mesh.segments
+
+    def get_segments_per_edge(self):
+        return self.mesh.segments_per_edge
+
+    def get_obj_vertices(self):
+        return self.mesh.obj_vertices
+
+
 def compute_quality(bb, deviation=0.1):
     # Since tessellation caching depends on quality, try to come up with stable a quality value
     quality = round_sig(
         (round_sig(bb.xsize, 3) + round_sig(bb.ysize, 3) + round_sig(bb.zsize, 3))
         / 300
         * deviation,
         3,
@@ -370,33 +449,43 @@
     angular_tolerance: float,
     compute_faces=True,
     compute_edges=True,
     debug=False,
     progress=None,
     shape_id="",
 ):
-    if progress is not None:
-        progress.update("+")
 
     compound = (
         make_compound(shapes) if len(shapes) > 1 else shapes[0]
     )  # pylint: disable=protected-access
-    tess = Tessellator(shape_id)
+
+    if NATIVE and is_native_tessellator_enabled():
+        if progress is not None:
+            progress.update("*")
+        tess = NativeTessellator(shape_id)
+    else:
+        if progress is not None:
+            progress.update("+")
+        tess = Tessellator(shape_id)
+
     tess.compute(
         compound, quality, angular_tolerance, compute_faces, compute_edges, debug
     )
     return {
         "vertices": tess.get_vertices(),
         "triangles": tess.get_triangles(),
         "normals": tess.get_normals(),
         "edges": tess.get_edges(),
         # added for version 2
         "obj_vertices": tess.get_obj_vertices(),
         "face_types": tess.get_face_types(),
         "edge_types": tess.get_edge_types(),
+        # added for version 3 (optional)
+        "triangles_per_face": tess.get_triangles_per_face(),
+        "segments_per_edge": tess.get_segments_per_edge(),
     }
 
 
 def discretize_edge(edge, deflection=0.1, num=None):
     curve_adaptator = BRepAdaptor_Curve(edge)
 
     if num is not None and num > 1:
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/trace.py` & `ocp_tessellate-2.3.0/ocp_tessellate/trace.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate/utils.py` & `ocp_tessellate-2.3.0/ocp_tessellate/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import json
 import math
 import numpy as np
 import time
 import warnings
 from webcolors import name_to_rgb, hex_to_rgb, rgb_to_hex
 
@@ -89,28 +90,26 @@
     return [[edge_list[i], edge_list[i + 1]] for i in range(len(edge_list) - 1)]
 
 
 def flatten(nested_list):
     return [y for x in nested_list for y in x]
 
 
-def numpy_to_buffer_json(value, indent=None):
+def numpy_to_buffer_json(value):
     def walk(obj):
         if isinstance(obj, np.ndarray):
-            if str(obj.dtype) in ("int32", "int64", "uint64"):
-                return obj.tolist()
-
             if not obj.flags["C_CONTIGUOUS"]:
                 obj = np.ascontiguousarray(obj)
 
             obj = obj.ravel()
             return {
                 "shape": obj.shape,
                 "dtype": str(obj.dtype),
-                "buffer": memoryview(obj).hex(),
+                "buffer": base64.b64encode(memoryview(obj)).decode(),
+                "codec": "b64",
             }
         elif isinstance(obj, (tuple, list)):
             return [walk(el) for el in obj]
         elif isinstance(obj, dict):
             rv = {}
             for k, v in obj.items():
                 rv[k] = walk(v)
```

### Comparing `ocp_tessellate-2.2.2/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-2.3.0/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocp-tessellate
-Version: 2.2.2
+Name: ocp_tessellate
+Version: 2.3.0
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
@@ -12,10 +12,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
+Requires-Dist: webcolors~=1.12
+Requires-Dist: numpy
+Requires-Dist: numpy-quaternion
+Requires-Dist: cachetools~=5.2.0
+Requires-Dist: imagesize
 Provides-Extra: dev
+Requires-Dist: pylint; extra == "dev"
+Requires-Dist: pyYaml; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 
 Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs
```

### Comparing `ocp_tessellate-2.2.2/setup.cfg` & `ocp_tessellate-2.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.2.2
+current_version = 2.3.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-2.2.2/setup.py` & `ocp_tessellate-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "2.2.2",
+    "version": "2.3.0",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

