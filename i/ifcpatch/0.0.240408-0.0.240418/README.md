# Comparing `tmp/ifcpatch-0.0.240408.tar.gz` & `tmp/ifcpatch-0.0.240418.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifcpatch-0.0.240408.tar", last modified: Mon Apr  8 00:32:17 2024, max compression
+gzip compressed data, was "ifcpatch-0.0.240418.tar", last modified: Thu Apr 18 00:56:55 2024, max compression
```

## Comparing `ifcpatch-0.0.240408.tar` & `ifcpatch-0.0.240418.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:32:17.734398 ifcpatch-0.0.240408/
--rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-08 00:32:11.000000 ifcpatch-0.0.240408/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-08 00:32:11.000000 ifcpatch-0.0.240408/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 00:32:17.734398 ifcpatch-0.0.240408/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:32:17.734398 ifcpatch-0.0.240408/ifcpatch/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-08 00:32:11.000000 ifcpatch-0.0.240408/ifcpatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-08 00:32:11.000000 ifcpatch-0.0.240408/ifcpatch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:32:17.734398 ifcpatch-0.0.240408/ifcpatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 00:32:17.000000 ifcpatch-0.0.240408/ifcpatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-08 00:32:17.000000 ifcpatch-0.0.240408/ifcpatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:32:17.000000 ifcpatch-0.0.240408/ifcpatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-08 00:32:17.000000 ifcpatch-0.0.240408/ifcpatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 00:32:17.000000 ifcpatch-0.0.240408/ifcpatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-08 00:32:15.000000 ifcpatch-0.0.240408/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:32:17.734398 ifcpatch-0.0.240408/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:32:17.734398 ifcpatch-0.0.240408/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-08 00:32:11.000000 ifcpatch-0.0.240408/test/test_ExtractElements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-08 00:32:11.000000 ifcpatch-0.0.240408/test/test_RegenerateGlobalIds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/
+-rw-r--r--   0 runner    (1001) docker     (127)    32473 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/ifcpatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/ifcpatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/ifcpatch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/ifcpatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 00:56:55.000000 ifcpatch-0.0.240418/ifcpatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-18 00:56:53.000000 ifcpatch-0.0.240418/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 00:56:55.727825 ifcpatch-0.0.240418/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/test/test_ExtractElements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/test/test_MergeDuplicateTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-18 00:56:51.000000 ifcpatch-0.0.240418/test/test_RegenerateGlobalIds.py
```

### Comparing `ifcpatch-0.0.240408/COPYING` & `ifcpatch-0.0.240418/COPYING`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240408/COPYING.LESSER` & `ifcpatch-0.0.240418/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240408/ifcpatch/__init__.py` & `ifcpatch-0.0.240418/ifcpatch/__init__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240408/ifcpatch/__main__.py` & `ifcpatch-0.0.240418/ifcpatch/__main__.py`

 * *Files identical despite different names*

### Comparing `ifcpatch-0.0.240408/pyproject.toml` & `ifcpatch-0.0.240418/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifcpatch"
-version = "0.0.240408"
+version = "0.0.240418"
 authors = [
   { name="Dion Moult", email="dion@thinkmoult.com" },
 ]
 description = "IFC patching utility"
 readme = "README.md"
-keywords = ["IFC", "IDS", "BIM"]
+keywords = ["IFC", "BIM"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
 ]
-dependencies = [
-    "ifcopenshell",
-]
+dependencies = ["ifcopenshell", "toposort", "numpy"]
 
 [project.urls]
 Homepage = "http://ifcopenshell.org"
 Documentation = "https://docs.ifcopenshell.org"
 Issues = "https://github.com/IfcOpenShell/IfcOpenShell/issues"
 
 [tool.setuptools.packages.find]
```

### Comparing `ifcpatch-0.0.240408/test/test_ExtractElements.py` & `ifcpatch-0.0.240418/test/test_ExtractElements.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,61 +18,63 @@
 
 import os
 import pytest
 import ifcpatch
 import ifcopenshell
 import ifcopenshell.api
 import ifcopenshell.util.element
+import test.bootstrap
 
 
-class TestExtractElements:
+class TestExtractElements(test.bootstrap.IFC4):
     def test_basic(self):
-        ifc_file = ifcopenshell.file()
-        project = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcProject")
-        wall = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcWall")
-        output = ifcpatch.execute({"file": ifc_file, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
+        project = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcProject")
+        wall = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcWall")
+        output = ifcpatch.execute({"file": self.file, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
 
         assert output.by_type("IfcProject")[0].GlobalId == project.GlobalId
         assert output.by_type("IfcWall")[0].GlobalId == wall.GlobalId
 
     def test_keep_spatial_structure(self):
-        ifc_file = ifcopenshell.file()
-        project = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcProject")
+        project = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcProject")
 
-        site = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcSite")
-        building = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcBuilding")
-        storey = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcBuildingStorey")
-        wall = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcWall")
-        ifcopenshell.api.run("aggregate.assign_object", ifc_file, product=building, relating_object=site)
-        ifcopenshell.api.run("aggregate.assign_object", ifc_file, product=storey, relating_object=building)
-        ifcopenshell.api.run("spatial.assign_container", ifc_file, products=[wall], relating_structure=storey)
+        site = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcSite")
+        building = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcBuilding")
+        storey = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcBuildingStorey")
+        wall = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcWall")
+        ifcopenshell.api.run("aggregate.assign_object", self.file, products=[building], relating_object=site)
+        ifcopenshell.api.run("aggregate.assign_object", self.file, products=[storey], relating_object=building)
+        ifcopenshell.api.run("spatial.assign_container", self.file, products=[wall], relating_structure=storey)
 
-        output = ifcpatch.execute({"file": ifc_file, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
+        output = ifcpatch.execute({"file": self.file, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
 
         wall_new = output.by_type("IfcWall")[0]
         assert (storey_new := ifcopenshell.util.element.get_container(wall_new)).GlobalId == storey.GlobalId
         assert (building_new := ifcopenshell.util.element.get_aggregate(storey_new)).GlobalId == building.GlobalId
         assert (site_new := ifcopenshell.util.element.get_aggregate(building_new)).GlobalId == site.GlobalId
 
     def test_keep_aggregate_in_spatial_structure(self):
-        ifc_file = ifcopenshell.file()
-        project = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcProject")
+        project = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcProject")
 
-        element = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcElementAssembly")
-        container = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcBuildingStorey")
-        subelement = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcWall")
-        ifcopenshell.api.run("spatial.assign_container", ifc_file, products=[element], relating_structure=container)
-        ifcopenshell.api.run("aggregate.assign_object", ifc_file, product=subelement, relating_object=element)
+        element = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcElementAssembly")
+        container = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcBuildingStorey")
+        subelement = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcWall")
+        ifcopenshell.api.run("spatial.assign_container", self.file, products=[element], relating_structure=container)
+        ifcopenshell.api.run("aggregate.assign_object", self.file, products=[subelement], relating_object=element)
 
-        output = ifcpatch.execute({"file": ifc_file, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
+        output = ifcpatch.execute({"file": self.file, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
 
         wall_new = output.by_type("IfcWall")[0]
         assembly = output.by_type("IfcElementAssembly")[0]
 
         assert ifcopenshell.util.element.get_aggregate(wall_new).GlobalId == element.GlobalId
         assert ifcopenshell.util.element.get_container(assembly).GlobalId == container.GlobalId
 
     def test_getting_the_psets_of_a_product_as_a_dictionary(self):
         ifc = ifcopenshell.open(os.path.join(os.getcwd(), "test", "files", "basic.ifc"))
         output = ifcpatch.execute({"file": ifc, "recipe": "ExtractElements", "arguments": ["IfcWall"]})
         assert output.by_type("IfcWall")
         assert not output.by_type("IfcSlab")
+
+
+class TestExtractElementsIFC2X3(test.bootstrap.IFC2X3, TestExtractElements):
+    pass
```

### Comparing `ifcpatch-0.0.240408/test/test_RegenerateGlobalIds.py` & `ifcpatch-0.0.240418/test/test_RegenerateGlobalIds.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,31 +18,34 @@
 
 import os
 import pytest
 import ifcpatch
 import ifcopenshell
 import ifcopenshell.api
 import ifcopenshell.util.element
+import test.bootstrap
 
 
-class TestRegenerateGlobalIds:
+class TestRegenerateGlobalIds(test.bootstrap.IFC4):
     def test_run(self):
-        ifc_file = ifcopenshell.file()
-        project = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcProject")
-        wall = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcWall")
+        project = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcProject")
+        wall = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcWall")
         used_guids = {project.GlobalId, wall.GlobalId}
-        ifcpatch.execute({"file": ifc_file, "recipe": "RegenerateGlobalIds", "arguments": [False]})
+        ifcpatch.execute({"file": self.file, "recipe": "RegenerateGlobalIds", "arguments": [False]})
         new_guids = {project.GlobalId, wall.GlobalId}
         assert not new_guids.intersection(used_guids)
 
     def test_regenerate_guids_for_duplicates(self):
-        ifc_file = ifcopenshell.file()
-        project = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcProject")
-        wall1 = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcWall")
-        wall2 = ifcopenshell.api.run("root.create_entity", ifc_file, ifc_class="IfcWall")
+        project = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcProject")
+        wall1 = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcWall")
+        wall2 = ifcopenshell.api.run("root.create_entity", self.file, ifc_class="IfcWall")
         wall1.GlobalId = wall2.GlobalId
         used_guids = {project, wall1.GlobalId, wall2.GlobalId}
 
-        ifcpatch.execute({"file": ifc_file, "recipe": "RegenerateGlobalIds", "arguments": [True]})
+        ifcpatch.execute({"file": self.file, "recipe": "RegenerateGlobalIds", "arguments": [True]})
         new_guids = {project, wall1.GlobalId, wall2.GlobalId}
         assert len(new_guids) == 3
         assert len(new_guids.intersection(used_guids)) == 2
+
+
+class TestRegenerateGlobalIdsIFC2X3(test.bootstrap.IFC2X3, TestRegenerateGlobalIds):
+    pass
```

