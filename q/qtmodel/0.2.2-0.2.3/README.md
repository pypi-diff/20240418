# Comparing `tmp/qtmodel-0.2.2.tar.gz` & `tmp/qtmodel-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.2.2.tar", last modified: Thu Apr 18 03:50:18 2024, max compression
+gzip compressed data, was "qtmodel-0.2.3.tar", last modified: Thu Apr 18 06:37:30 2024, max compression
```

## Comparing `qtmodel-0.2.2.tar` & `qtmodel-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 03:50:18.391693 qtmodel-0.2.2/
--rw-rw-rw-   0        0        0    19837 2024-04-18 03:50:18.390659 qtmodel-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    19420 2024-04-10 06:53:56.000000 qtmodel-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 03:50:18.382655 qtmodel-0.2.2/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.2/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    79661 2024-04-18 03:48:40.000000 qtmodel-0.2.2/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.2/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.2/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:50:18.388662 qtmodel-0.2.2/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    19837 2024-04-18 03:50:17.000000 qtmodel-0.2.2/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-18 03:50:18.000000 qtmodel-0.2.2/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:50:17.000000 qtmodel-0.2.2/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 03:50:18.000000 qtmodel-0.2.2/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 03:50:18.391693 qtmodel-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-18 03:50:04.000000 qtmodel-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:37:30.587307 qtmodel-0.2.3/
+-rw-rw-rw-   0        0        0    35532 2024-04-18 06:37:30.587307 qtmodel-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    35115 2024-04-18 06:36:34.000000 qtmodel-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 06:37:30.566698 qtmodel-0.2.3/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.3/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    79987 2024-04-18 06:26:23.000000 qtmodel-0.2.3/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.3/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.3/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:37:30.585297 qtmodel-0.2.3/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    35532 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:37:30.587307 qtmodel-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-18 06:37:05.000000 qtmodel-0.2.3/setup.py
```

### Comparing `qtmodel-0.2.2/qtmodel/qt_mdb.py` & `qtmodel-0.2.3/qtmodel/qt_mdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1061,15 +1061,16 @@
 
     @staticmethod
     def remove_nodal_mass(node_id: int = -1):
         """
         删除节点质量
         Args:
              node_id:节点号
-        mdb.remove_nodal_mass(node_id=1)
+        example:
+            mdb.remove_nodal_mass(node_id=1)
         Returns: 无
         """
         qt_model.RemoveNodalMass(nodeId=node_id)
 
     @staticmethod
     def add_pre_stress(case_name: str = "", tendon_name: str = "", pre_type: int = 2, force: float = 1395000, group_name: str = "默认荷载组"):
         """
@@ -1263,27 +1264,29 @@
         example:
             mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
         Returns: 无
         """
         qt_model.AddCableLenghtLoad(elementId=element_id, caseName=case_name, groupName=group_name, length=length, tensionType=tension_type)
 
     @staticmethod
-    def add_plate_element_load(element_id: int = 1, case_name: str = "", load_type: int = 1, load_place: int = 1, coord_system: int = 1,
+    def add_plate_element_load(element_id: int = 1, case_name: str = "", load_type: int = 1, load_place: int = 1, coord_system: int = 3,
                                group_name: str = "默认荷载组", load_list: list[float] = None, xy_list: tuple[float, float] = None):
         """
         添加版单元荷载
         Args:
              element_id:单元id
              case_name:荷载工况名
              load_type:荷载类型   1-集中力  2-集中弯矩  3-分布力  4-分布弯矩
-             load_place:荷载位置  0-面IJKL 1-边IJ  2-边JK  3-边KL  4-边LI
-             coord_system:坐标系
+             load_place:荷载位置  0-面IJKL 1-边IJ  2-边JK  3-边KL  4-边LI  (仅分布荷载需要)
+             coord_system:坐标系  (默认3) 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z
              group_name:荷载组名
              load_list:荷载列表
              xy_list:荷载位置信息 [IJ方向距离x,IL方向距离y]  (仅集中荷载需要,x,y代表荷载距离板单元I端的绝对值)
+        example:
+            mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=[0.2,0.5])
         Returns: 无
         """
         if load_type == 1 or load_type == 2:
             qt_model.AddPlateElementLoad(elementId=element_id, caseName=case_name, loadType=load_type,
                                          coordSystem=coord_system, groupName=group_name, loads=load_list[0])
         elif load_type == 3 or load_type == 4:
             if load_place == 0:
```

### Comparing `qtmodel-0.2.2/qtmodel/qt_odb.py` & `qtmodel-0.2.3/qtmodel/qt_odb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.2/qtmodel/res_db.py` & `qtmodel-0.2.3/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.2/setup.py` & `qtmodel-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.2.2",
+    version="0.2.3",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

