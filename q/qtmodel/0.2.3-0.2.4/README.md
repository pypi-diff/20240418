# Comparing `tmp/qtmodel-0.2.3.tar.gz` & `tmp/qtmodel-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmodel-0.2.3.tar", last modified: Thu Apr 18 06:37:30 2024, max compression
+gzip compressed data, was "qtmodel-0.2.4.tar", last modified: Thu Apr 18 06:56:49 2024, max compression
```

## Comparing `qtmodel-0.2.3.tar` & `qtmodel-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 06:37:30.587307 qtmodel-0.2.3/
--rw-rw-rw-   0        0        0    35532 2024-04-18 06:37:30.587307 qtmodel-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    35115 2024-04-18 06:36:34.000000 qtmodel-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 06:37:30.566698 qtmodel-0.2.3/qtmodel/
--rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.3/qtmodel/__init__.py
--rw-rw-rw-   0        0        0    79987 2024-04-18 06:26:23.000000 qtmodel-0.2.3/qtmodel/qt_mdb.py
--rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.3/qtmodel/qt_odb.py
--rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.3/qtmodel/res_db.py
-drwxrwxrwx   0        0        0        0 2024-04-18 06:37:30.585297 qtmodel-0.2.3/qtmodel.egg-info/
--rw-rw-rw-   0        0        0    35532 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-18 06:37:30.000000 qtmodel-0.2.3/qtmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 06:37:30.587307 qtmodel-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      747 2024-04-18 06:37:05.000000 qtmodel-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:56:49.181876 qtmodel-0.2.4/
+-rw-rw-rw-   0        0        0    37573 2024-04-18 06:56:49.181876 qtmodel-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    37156 2024-04-18 06:49:16.000000 qtmodel-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-18 06:56:49.161505 qtmodel-0.2.4/qtmodel/
+-rw-rw-rw-   0        0        0       93 2024-04-10 06:50:13.000000 qtmodel-0.2.4/qtmodel/__init__.py
+-rw-rw-rw-   0        0        0    80039 2024-04-18 06:49:04.000000 qtmodel-0.2.4/qtmodel/qt_mdb.py
+-rw-rw-rw-   0        0        0     3834 2024-04-10 06:52:58.000000 qtmodel-0.2.4/qtmodel/qt_odb.py
+-rw-rw-rw-   0        0        0     3405 2024-04-17 03:39:04.000000 qtmodel-0.2.4/qtmodel/res_db.py
+drwxrwxrwx   0        0        0        0 2024-04-18 06:56:49.179020 qtmodel-0.2.4/qtmodel.egg-info/
+-rw-rw-rw-   0        0        0    37573 2024-04-18 06:56:48.000000 qtmodel-0.2.4/qtmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-18 06:56:49.000000 qtmodel-0.2.4/qtmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 06:56:48.000000 qtmodel-0.2.4/qtmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-18 06:56:48.000000 qtmodel-0.2.4/qtmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 06:56:49.181876 qtmodel-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      747 2024-04-18 06:56:45.000000 qtmodel-0.2.4/setup.py
```

### Comparing `qtmodel-0.2.3/PKG-INFO` & `qtmodel-0.2.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,114 @@
-Metadata-Version: 2.1
-Name: qtmodel
-Version: 0.2.3
-Summary: python modeling for qt
-Home-page: https://github.com/Inface0443/pyqt
-Author: dqy-zhj
-Author-email: 1105417715@qq.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 ##  初始化模型
 ### initial
 初始化模型
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.initial()
 ```  
 ##  节点单元操作
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
-```Python  
+```Python
 # 示例代码
-mdb.add_structure_group("新建结构组1")
+from qtmodel import mdb
+mdb.add_structure_group(name="新建结构组1")
 mdb.add_structure_group(name="新建结构组2",index=2)
 ```  
 ### remove_structure_group
 可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
 > 参数:  
 > name:结构组名称  
 > index:结构组编号  
-```Python  
+```Python
 # 示例代码
-mdb.remove_structure_group(name=“新建结构组1”)
+from qtmodel import mdb
+mdb.remove_structure_group(name="新建结构组1")
 mdb.remove_structure_group(index = 2)
 ```  
 ### add_structure_to_group
 为结构组添加节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
 ### remove_structure_in_group
 为结构组删除节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
 ### add_node
 根据坐标信息和节点编号添加节点，默认自动识别编号
 > 参数:  
 > x: 节点坐标x  
 > y: 节点坐标y  
 > z: 节点坐标z  
 > index: 节点编号，默认自动识别编号 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node(1,2,3)
 mdb.add_node(x= 1,y = 2,z = 4,index = 2)
 ```  
 ### add_nodes
 添加多个节点，可以选择指定节点编号
 > 参数:  
 > node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodes([[1,2,3],[4,5,6]])
 mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
 ```  
 ### remove_node
 删除指定节点,不输入参数时默认删除所有节点
 > 参数:  
 > index:节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_node()
 mdb.remove_node(index=1)
 ```  
 ### add_element
 根据单元编号和单元类型添加单元
 > 参数:  
 > index:单元编号  
 > ele_type:单元类型 1-梁 2-索 3-杆 4-板  
 > node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]  
 > beta_angle:贝塔角  
 > mat_id:材料编号  
 > sec_id:截面编号  
-```Python  
+```Python
 # 示例代码
-mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1.sec_id=1)
+from qtmodel import mdb
+mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
 ```  
 ### remove_element
 删除指定编号的单元
 > 参数:  
 > index: 单元编号,默认时删除所有单元  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_element()
 mdb.remove_element(index=1)
 ```  
 ##  材料操作
 ### add_material
 添加材料
 > 参数:  
@@ -120,46 +116,50 @@
 > name:材料名称  
 > material_type: 材料类型  
 > standard:规范名称  
 > database:数据库  
 > construct_factor:构造系数  
 > modified:是否修改默认材料参数,默认不修改 (可选参数)  
 > data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)  
-```Python  
+```Python
 # 示例代码
-mdb.add_material(index=1,name=“混凝土材料1”,material_type="混凝土",standard="公路18规范",database="C50")
-mdb.add_material(index=1,name=“自定义材料1”,material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+from qtmodel import mdb
+mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
+mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
 ```  
 ### add_time_material
 添加收缩徐变材料
 > 参数:  
 > index: 指定收缩徐变编号,默认则自动识别 (可选参数)  
 > name: 收缩徐变名  
 > code_index: 收缩徐变规范索引  
 > time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
 ```  
 ### update_material_creep
 将收缩徐变参数连接到材料
 > 参数:  
 > index: 材料编号  
 > creep_id: 收缩徐变编号  
 > f_cuk: 材料标准抗压强度,仅自定义材料是需要输入  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_material_creep(index=1,creep_id=1,f_cuk=5e7)
 ```  
 ### remove_material
 删除指定材料
 > 参数:  
 > index:指定材料编号，默认则删除所有材料  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_material()
 mdb.remove_material(index=1)
 ```  
 ##  截面和板厚操作
 ### add_parameter_section
 添加截面信息
 > 参数:  
@@ -177,17 +177,18 @@
 > box_height: 混凝土箱梁梁高 (仅混凝土箱梁截面需要)  
 > mat_combine: 组合截面材料信息 [弹性模量比s/c、密度比s/c、钢材泊松比、混凝土泊松比、热膨胀系数比s/c] (仅组合材料需要)  
 > bias_type:偏心类型 默认中心  
 > center_type:中心类型 默认质心  
 > shear_consider:考虑剪切 bool 默认考虑剪切变形  
 > bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要)  
 > bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
-mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心)
+from qtmodel import mdb
+mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
 mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
 ```  
 ### add_steel_section
 添加钢梁截面,包括参数型钢梁截面和自定义带肋钢梁截面
 > 参数:  
@@ -201,50 +202,54 @@
 > rib_place:肋板位置 list[tuple[布置位置,具体位置,参考点位置,list[tuple[间隔,肋板名，加劲肋位置,加劲肋名]]]]  
 > 布置位置 0-上...  具体位置 0-桥面1.。。 参考点位置 0-左  加劲肋位置 0-上/左 1-下/右 2-两侧 (详细信息参考UI界面顺序)  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要,相对形心)  
 > bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_steel_section(name="钢梁截面1",section_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
 mdb.add_steel_section(name="钢梁截面2",section_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
 rib_place2 = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
-bias_type=“中上”)
+bias_type="中上")
 ```  
 ### add_user_section
 添加自定义截面,目前仅支持特性截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > sec_type:截面类型  
 > property_info:截面特性列表  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_user_section(name="自定义特性截面",property_info=[i for i in range(25)])
 ```  
 ### add_tapper_section
 添加变截面,需先建立单一截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > begin_id:截面始端编号  
 > end_id:截面末端编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tapper_section(name="变截面1",begin_id=1,end_id=2)
 ```  
 ### remove_section
 删除截面信息
 > 参数:  
 > index: 截面编号,参数为默认时删除全部截面  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_section()
 mdb.remove_section(1)
 ```  
 ### add_thickness
 添加板厚
 > 参数:  
 > index: 板厚id  
@@ -253,160 +258,174 @@
 > thick_type: 板厚类型 0-普通板 1-加劲肋板  
 > bias_info:  默认不偏心,偏心时输入列表[type,value] type:0-厚度比 1-数值  
 > rib_pos: 肋板位置 0-下部 1-上部  
 > dist_v: 纵向截面肋板间距  
 > dist_l: 横向截面肋板间距  
 > rib_v: 纵向肋板信息  
 > rib_l: 横向肋板信息  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_thickness(name="厚度1", t=0.2,thick_type=0,bias_info=[0,0.8])
 mdb.add_thickness(name="厚度2", t=0.2,thick_type=1,rib_pos=0,dis_v=0.1,rib_v=[1,1,0.02,0.02])
 ```  
 ### remove_thickness
 删除板厚
 > 参数:  
 > index:板厚编号,默认时删除所有板厚信息  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_thickness()
 mdb.remove_thickness(index=1)
 ```  
 ### add_tapper_section_group
 添加变截面组
 > 参数:  
 > ids:变截面组编号  
 > name: 变截面组名  
 > factor_w: 宽度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > factor_h: 高度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > ref_w: 宽度方向参考点 0-i 1-j  
 > ref_h: 高度方向参考点 0-i 1-j  
 > dis_w: 宽度方向距离  
 > dis_h: 高度方向距离  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tapper_section_group(ids=[1,2,3,4],name="变截面组1")
 ```  
 ### update_section_bias
 更新截面偏心
 > 参数:  
 > index:截面编号  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_point:自定义偏心点(仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_section_bias(index=1,bias_type="中上",center_type="几何中心")
 mdb.update_section_bias(index=1,bias_type="自定义",bias_point=[0.1,0.2])
 ```  
 ##  边界操作
 ### add_boundary_group
 新建边界组
 > 参数:  
 > name:边界组名  
 > index:边界组编号，默认自动识别当前编号 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_boundary_group(name="边界组1")
 ```  
 ### remove_boundary_group
 按照名称删除边界组
 > 参数:  
 > name: 边界组名称，默认删除所有边界组 (非必须参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_boundary_group()
 mdb.remove_boundary_group(name="边界组1")
 ```  
 ### remove_all_boundary
 根据边界组名称、边界的类型和编号删除边界信息,默认时删除所有边界信息
 > 参数:  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_all_boundary()
 ```  
 ### remove_boundary
 根据节点号删除边界一般支撑、弹性支承，根据单元号删除梁端约束、根据主节点号删除主从约束、根据从节点号删除约束方程
 > 参数:  
 > remove_id:节点号 or 单元号 or主节点号  or 从节点号  
 > bd_type:边界类型  1-一般支承 2-弹性支承 3-主从约束 4-弹性连接 5-约束方程 6-梁端约束  
 > group:边界所处边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_boundary(remove_id = 1, bd_type = 1,group="边界组1")
 ```  
 ### add_general_support
 添加一般支承
 > 参数:  
 > node_id:节点编号  
 > boundary_info:边界信息  [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名,默认为默认边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_general_support(node_id=1, boundary_info=[True,True,True,False,False,False])
 ```  
 ### add_elastic_support
 添加弹性支承
 > 参数:  
 > node_id:节点编号  
 > support_type:支承类型 1-线性  2-受拉  3-受压  
 > boundary_info:边界信息 受拉和受压时列表长度为1  线性时列表长度为6  
 > group_name:边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_elastic_support(node_d=1,support_type=1,boundary_info=[1e6,0,1e6,0,0,0])
 ```  
 ### add_master_slave_link
 添加主从约束
 > 参数:  
 > master_id:主节点号  
 > slave_id:从节点号  
 > boundary_info:边界信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_master_slave_link(master_id=1,slave_id=2,boundary_info=[True,True,True,False,False,False])
 ```  
 ### add_elastic_link
 添加弹性连接
 > 参数:  
 > link_type:节点类型   1-一般弹性连接 2-刚性连接 3-受拉弹性连接 4-受压弹性连接  
 > start_id:起始节点号  
 > end_id:终节点号  
 > beta_angle:贝塔角  
 > boundary_info:边界信息  
 > group_name:边界组名  
 > dis_ratio:距i端距离比 (仅一般弹性连接需要)  
 > kx:受拉或受压刚度  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_elastic_link(link_type=1,start_id=1,end_id=2,boundary_info=[1e6,1e6,1e6,0,0,0])
 mdb.add_elastic_link(link_type=2,start_id=1,end_id=2)
 mdb.add_elastic_link(link_type=3,start_id=1,end_id=2,kx=1e6)
 ```  
 ### add_beam_constraint
 添加梁端约束
 > 参数:  
 > beam_id:梁号  
 > info_i:i端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > info_j:j端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_constraint(beam_id=2,info_i=[True,True,True,False,False,False],info_j=[True,True,True,False,False,False])
 ```  
 ### add_node_axis
 添加节点坐标
 > 参数:  
 > input_type:输入方式 1-角度 2-三点  3-向量  
 > node_id:节点号  
 > coord_info:局部坐标信息 -List<float>(角)  -List<List<float>>(三点 or 向量)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_axis(input_type=1,node_id=1,coord_info=[45,45,45])
 mdb.add_node_axis(input_type=2,node_id=1,coord_info=[[0,0,1],[0,1,0],[1,0,0]])
 mdb.add_node_axis(input_type=3,node_id=1,coord_info=[[0,0,1],[0,1,0]])
 ```  
 ##  移动荷载
 ### add_standard_vehicle
 添加标准车辆
@@ -421,128 +440,140 @@
 > 6-城市轨道交通桥梁规范(GB/T51234-2017)  
 > load_type: 荷载类型  
 > 支持类型: "公路I级","公路II级","城A车道","城B车道","地铁A型车","地铁B型车","地铁C型车","汽10"  
 > "汽15","汽20","汽超20","特载","挂80","挂100","挂120","公路疲劳荷载1","公路疲劳荷载2","公路疲劳荷载3",  
 > "汽36轻", "汽38重","高速铁路","城际铁路","客货共线铁路","重载铁路","中活载","长大货物车检算荷载"  
 > load_length: 默认为0即不限制荷载长度  (铁路桥涵规范 Q/CR 9300-2017 所需参数)  
 > n:车厢数: 默认6节车厢 (城市轨道交通桥梁规范 GB/T51234-2017 所需参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_standard_vehicle("高速铁路",standard_code=1,load_type="高速铁路")
 ```  
 ### add_node_tandem
 添加节点纵列
 > 参数:  
 > name:节点纵列名  
 > start_id:起始节点号  
 > node_ids:节点列表  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_tandem("节点纵列1",1,[i+1 for i in range(12)])
 ```  
 ### add_influence_plane
 添加影响面
 > 参数:  
 > name:影响面名称  
 > tandem_names:节点纵列名称组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_influence_plane("影响面1",["节点纵列1","节点纵列2"])
 ```  
 ### add_lane_line
 添加车道线
 > 参数:  
 > name:车道线名称  
 > influence_name:影响面名称  
 > tandem_name:节点纵列名  
 > offset:偏移  
 > lane_width:车道宽度  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_lane_line("车道1","影响面1","节点纵列1",offset=0,lane_width=3.1)
 ```  
 ### add_live_load_case
 添加移动荷载工况
 > 参数:  
 > name:荷载工况名  
 > influence_plane:影响线名  
 > span:跨度  
 > car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > train_detail: 火车相关系数 (横向折减列表float[8],纵向折减系数,强度冲击,疲劳冲击)  
 > metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]  
-```Python  
+```Python
 # 示例代码
-mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[(“车辆名称”,1.0,["车道1","车道2"])...])
+from qtmodel import mdb
+mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
 ```  
 ### remove_vehicle
 删除车辆信息
 > 参数:  
 > index:车辆荷载编号  
 > name:车辆名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_vehicle(index=1)
 mdb.remove_vehicle(name="车辆名称")
 ```  
 ### remove_node_tandem
 按照 节点纵列编号/节点纵列名 删除节点纵列
 > 参数:  
 > index:节点纵列编号  
 > name:节点纵列名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_node_tandem(index=1)
 mdb.remove_node_tandem(name="节点纵列1")
 ```  
 ### remove_influence_plane
 按照 影响面编号/影响面名称 删除影响面
 > 参数:  
 > index:影响面编号  
 > name:影响面名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_influence_plane(index=1)
 mdb.remove_influence_plane(name="影响面1")
 ```  
 ### remove_lane_line
 按照 车道线编号/车道线名称 删除车道线
 > 参数:  
 > name:车道线名称  
 > index:车道线编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_lane_line(index=1)
 mdb.remove_lane_line(name="车道线1")
 ```  
 ### remove_live_load_case
 删除移动荷载工况
 > 参数:  
 > name:移动荷载工况名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_live_load_case(name="活载工况1")
 ```  
 ##  钢束操作
 ### add_tendon_group
 按照名称添加钢束组，添加时可指定钢束组id
 > 参数:  
 > name: 钢束组名称  
 > index: 钢束组编号(非必须参数)，默认自动识别  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_group(name="钢束组1")
 ```  
 ### remove_tendon_group
 按照钢束组名称或钢束组编号删除钢束组，两参数均为默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称,默认自动识别 (可选参数)  
 > index:钢束组编号,默认自动识别 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon_group(name="钢束组1")
 mdb.remove_tendon_group(index=1)
 ```  
 ### add_tendon_property
 添加钢束特性
 > 参数:  
 > name:钢束特性名  
@@ -550,16 +581,17 @@
 > tendon_type: 0-PRE 1-POST  
 > material_id: 钢材材料编号  
 > duct_type: 1-金属波纹管  2-塑料波纹管  3-铁皮管  4-钢管  5-抽芯成型  
 > steel_type: 1-钢绞线  2-螺纹钢筋  
 > steel_detail: 钢绞线[钢束面积,孔道直径,摩阻系数,偏差系数]  螺纹钢筋[钢筋直径,钢束面积,孔道直径,摩阻系数,偏差系数,张拉方式(1-一次张拉\2-超张拉)]  
 > loos_detail: 松弛信息[规范(1-公规 2-铁规),张拉(1-一次张拉 2-超张拉),松弛(1-一般松弛 2-低松弛)] (仅钢绞线需要,默认为[1,1,1])  
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=[1,1,1])
 ```  
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
@@ -570,366 +602,402 @@
 > position_type: 定位方式 1-直线  2-轨迹线  
 > control_points: 控制点信息[(x1,y1,z1,r1),(x2,y2,z2,r2)....]  
 > point_insert: 定位方式为直线时为插入点坐标[x,y,z], 轨迹线时为 [插入端(1-I 2-J),插入方向(1-ij 2-ji),插入单元id]  
 > tendon_direction:直线钢束X方向向量 x轴-[1,0,0] y轴-[0,1,0]  默认为[1,0,0] (轨迹线不用赋值)  
 > rotation_angle:绕钢束旋转角度  
 > track_group:轨迹线结构组名  (直线时不用赋值)  
 > projection:直线钢束投影，默认为true  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=1,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(0,0,0))
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=2,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(1,1,1),track_group="轨迹线结构组1")
 ```  
 ### remove_tendon
 按照名称或编号删除钢束,默认时删除所有钢束
 > 参数:  
 > name:钢束名称  
 > index:钢束编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon(name="钢束1")
 mdb.remove_tendon(index=1)
 mdb.remove_tendon()
 ```  
 ### remove_tendon_property
 按照名称或编号删除钢束组,默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称  
 > index:钢束组编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon_property(name="钢束特性1")
 mdb.remove_tendon_property(index=1)
 mdb.remove_tendon_property()
 ```  
 ### add_nodal_mass
 添加节点质量
 > 参数:  
 > node_id:节点编号  
 > mass_info:[m,rmX,rmY,rmZ]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodal_mass(node_id=1,mass_info=(100,0,0,0))
 ```  
 ### remove_nodal_mass
 删除节点质量
 > 参数:  
 > node_id:节点号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_nodal_mass(node_id=1)
 ```  
 ### add_pre_stress
 添加预应力
 > 参数:  
 > case_name:荷载工况名  
 > tendon_name:钢束名  
 > pre_type:预应力类型 0-始端 1-末端 2-两端  
 > force:预应力  
 > group_name:边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_pre_stress(case_name="荷载工况名",tendon_name="钢束1",force=1390000)
 ```  
 ### remove_pre_stress
 删除预应力
 > 参数:  
 > case_name:荷载工况  
 > tendon_name:钢束组  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_pre_stress(case_name="工况1",tendon_name="钢束1",group_name="默认荷载组")
 ```  
 ##  荷载操作
 ### add_load_group
 根据荷载组名称添加荷载组
 > 参数:  
 > name: 荷载组名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_group(name="荷载组1")
 ```  
 ### remove_load_group
 根据荷载组名称或荷载组id删除荷载组,参数为默认时删除所有荷载组
 > 参数:  
 > name: 荷载组名称  
 > index: 荷载组编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_load_group(name="荷载组1")
 mdb.remove_load_group(index="1")
 ```  
 ### add_nodal_force
 添加节点荷载
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodal_force(case_name="荷载工况1",node_id=1,load_info=(1,1,1,1,1,1),group_name="默认结构组")
 ```  
 ### remove_nodal_force
 删除节点荷载
 > 参数:  
 > case_name:荷载工况名  
 > node_id:节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_nodal_force(case_name="荷载工况1",node_id=1)
 ```  
 ### add_node_displacement
 添加节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 > load_info:[Dx,Dy,Dz,Rx,Ry,Rz]  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_displacement(case_name="荷载工况1",node_id=1,load_info=(1,0,0,0,0,0),group_name="默认荷载组")
 ```  
 ### remove_nodal_displacement
 删除节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
-```Python  
+```Python
 # 示例代码
-mdn.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
+from qtmodel import mdb
+mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
 ```  
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩  
 > coord_system:坐标系 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
 > uniform_load:均布荷载值  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型 1-集中力   2-集中弯矩  3-分布力   4-分布弯矩  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
-mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1，group_name="默认荷载组")
+from qtmodel import mdb
+mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
 ```  
 ### add_initial_tension
 添加初始拉力
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > tension:初始拉力  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_initial_tension(element_id=1,case_name="工况1",tension=100,tension_type=1)
 ```  
 ### add_cable_length_load
 添加索长张拉
 > 参数:  
 > element_id:单元类型  
 > case_name:荷载工况名  
 > length:长度  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
 ```  
 ### add_plate_element_load
 添加版单元荷载
 > 参数:  
 > element_id:单元id  
 > case_name:荷载工况名  
 > load_type:荷载类型   1-集中力  2-集中弯矩  3-分布力  4-分布弯矩  
 > load_place:荷载位置  0-面IJKL 1-边IJ  2-边JK  3-边KL  4-边LI  (仅分布荷载需要)  
 > coord_system:坐标系  (默认3) 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z  
 > group_name:荷载组名  
 > load_list:荷载列表  
 > xy_list:荷载位置信息 [IJ方向距离x,IL方向距离y]  (仅集中荷载需要,x,y代表荷载距离板单元I端的绝对值)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=[0.2,0.5])
 ```  
 ### add_deviation_parameter
 添加制造误差
 > 参数:  
 > name:名称  
 > element_type:单元类型  1-梁单元  2-板单元  
 > parameters:参数列表  
 > 梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]  
 > 板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]  
-```Python  
+```Python
 # 示例代码
-mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameterInfo=parameters)
+from qtmodel import mdb
+mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameters=[1,0,0,0,0,0,0])
+mdb.add_deviation_parameter(name="板端制造误差",elementType=1,parameters=[1,0,0,0,0])
 ```  
 ### add_deviation_load
 添加制造误差荷载
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > parameters:参数名列表 梁杆单元时-[制造误差参数名称]   板单元时-[I端误差名,J端误差名,K端误差名,L端误差名]  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
-mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=[“梁端误差”])
-mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=[“板端误差1”,"板端误差2","板端误差3","板端误差4"])
+from qtmodel import mdb
+mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
+mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
 ```  
 ### add_element_temperature
 添加单元温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:最终温度  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_element_temperature(element_id=1,case_name="自重",temperature=1,group_name="默认荷载组")
 ```  
 ### add_gradient_temperature
 添加梯度温度
-```Python  
+```Python
 # 示例代码
-mdb.add_gradient_temperature(elementId=1,caseName=“荷载工况1”,groupName=“荷载组名1,temperature=10)
-mdb.add_gradient_temperature(elementId=2,caseName=“荷载工况2”,groupName=”荷载组名2“,temperature=10,element_type=2)
+from qtmodel import mdb
+mdb.add_gradient_temperature(elementId=1,caseName="荷载工况1",groupName="荷载组名1",temperature=10)
+mdb.add_gradient_temperature(elementId=2,caseName="荷载工况2",groupName="荷载组名2",temperature=10,element_type=2)
 ```  
 ### add_beam_section_temperature
 添加梁截面温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > paving_thick:铺设厚度(m)  
 > temperature_type:温度类型  1-升温(默认) 2-降温  
 > paving_type:铺设类型     1-沥青混凝土(默认)  2-水泥混凝土  
 > group_name:荷载组名  
 > modify:是否修改规范温度  
 > temp_list:温度列表[T1,T2]  (仅修改时需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_section_temperature(element_id=1,case_name="工况1",paving_thick=0.1)
 ```  
 ### add_index_temperature
 添加指数温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:温差  
 > index:指数  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_index_temperature(element_id=1,case_name="工况1",temperature=20,index=2)
 ```  
 ### add_top_plate_temperature
 添加顶板温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载  
 > temperature:最终温度  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_top_plate_temperature(element_id=1,case_name="工况1",temperature=40,group_name="默认荷载组")
 ```  
 ##  沉降操作
 ### add_sink_group
 添加沉降组
 > 参数:  
 > name: 沉降组名  
 > sink: 沉降值  
 > node_ids: 节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_sink_group(name="沉降1",sink=0.1,node_ids=[1,2,3])
 ```  
 ### remove_sink_group
 按照名称删除沉降组
 > 参数:  
 > name:沉降组名,默认删除所有沉降组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_sink_group()
 mdb.remove_sink_group(name="沉降1")
 ```  
 ### add_sink_case
 添加沉降工况
 > 参数:  
 > name:荷载工况名  
 > sink_groups:沉降组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_sink_case(name="沉降工况1",sink_groups=["沉降1","沉降2"])
 ```  
 ### remove_sink_case
 按照名称删除沉降工况,不输入名称时默认删除所有沉降工况
 > 参数:  
 > name:沉降工况名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_sink_case()
 mdb.remove_sink_case(name="沉降1")
 ```  
 ### add_concurrent_reaction
 添加并发反力组
 > 参数:  
 > names: 结构组名称集合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_concurrent_reaction(["默认结构组"])
 ```  
 ### remove_concurrent_reaction
 删除所有并发反力组
 > 参数:  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_concurrent_reaction()
 ```  
 ### add_concurrent_force
 创建并发内力组
 > 参数:  
 > names: 结构组名称集合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_concurrent_force(["默认结构组"])
 ```  
 ### remove_concurrent_force
 删除所有并发内力组
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_concurrent_force()
 ```  
 ### add_load_case
 添加荷载工况
 > 参数:  
 > name:沉降名  
 > case_type:荷载工况类型  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_case(name="工况1",case_type=1)
 ```  
 ### remove_load_case
 删除荷载工况,参数均为默认时删除全部荷载工况
 > 参数:  
 > index:荷载编号  
 > name:荷载名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_case(index=1)
 mdb.add_load_case(name="工况1")
 mdb.add_load_case()
 ```  
 ### test_print
 测试运行
 ##  施工阶段和荷载组合
@@ -947,17 +1015,18 @@
 > delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]  
 > active_loads:激活荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > delete_loads:钝化荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
 > index:施工阶段编号，默认自动添加  
-```Python  
+```Python
 # 示例代码
-mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+from qtmodel import mdb
+mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
 ### update_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
@@ -969,54 +1038,57 @@
 > 位置:  0-变形前 1-变形后  
 > delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]  
 > active_loads:激活荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > delete_loads:钝化荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
-```Python  
+```Python
 # 示例代码
-mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+from qtmodel import mdb
+mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
 ### update_weight_stage
 添加施工阶段信息
 > 参数:  
 > stage_name:施工阶段信息  
 > structure_group_name:结构组名  
 > weight_stage_id: 计自重阶段号: 0-不计自重,1-本阶段 n-第n阶段  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_weight_stage(stage_name="施工阶段1",structure_group_name="默认结构组",weight_stage_id=1)
 ```  
 ### remove_construction_stage
 按照施工阶段名删除施工阶段,默认删除所有施工阶段
 > 参数:  
 > name:所删除施工阶段名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_construction_stage(name="施工阶段1")
 ```  
 ### add_load_combine
 添加荷载组合
 > 参数:  
 > name:荷载组合名  
 > combine_type:荷载组合类型 1-叠加  2-判别  3-包络  
 > describe:描述  
 > combine_info:荷载组合信息 [(荷载工况类型,工况名,系数)...]  
 > 荷载工况类型: "ST"-静力荷载工况  "CS"-施工阶段荷载工况  "CB"-荷载组合  
 > "MV"-移动荷载工况  "SM"-沉降荷载工况  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_combine(name="荷载组合1",combine_type=1,describe="无",combine_info=[("CS","合计值",1),("CS","恒载",1)])
 ```  
 ### remove_load_combine
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
 ```  
 
-
-
```

### Comparing `qtmodel-0.2.3/README.md` & `qtmodel-0.2.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,128 @@
+Metadata-Version: 2.1
+Name: qtmodel
+Version: 0.2.4
+Summary: python modeling for qt
+Home-page: https://github.com/Inface0443/pyqt
+Author: dqy-zhj
+Author-email: 1105417715@qq.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+
 ##  初始化模型
 ### initial
 初始化模型
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.initial()
 ```  
 ##  节点单元操作
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
-```Python  
+```Python
 # 示例代码
-mdb.add_structure_group("新建结构组1")
+from qtmodel import mdb
+mdb.add_structure_group(name="新建结构组1")
 mdb.add_structure_group(name="新建结构组2",index=2)
 ```  
 ### remove_structure_group
 可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
 > 参数:  
 > name:结构组名称  
 > index:结构组编号  
-```Python  
+```Python
 # 示例代码
-mdb.remove_structure_group(name=“新建结构组1”)
+from qtmodel import mdb
+mdb.remove_structure_group(name="新建结构组1")
 mdb.remove_structure_group(index = 2)
 ```  
 ### add_structure_to_group
 为结构组添加节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
 ### remove_structure_in_group
 为结构组删除节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
 ### add_node
 根据坐标信息和节点编号添加节点，默认自动识别编号
 > 参数:  
 > x: 节点坐标x  
 > y: 节点坐标y  
 > z: 节点坐标z  
 > index: 节点编号，默认自动识别编号 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node(1,2,3)
 mdb.add_node(x= 1,y = 2,z = 4,index = 2)
 ```  
 ### add_nodes
 添加多个节点，可以选择指定节点编号
 > 参数:  
 > node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodes([[1,2,3],[4,5,6]])
 mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
 ```  
 ### remove_node
 删除指定节点,不输入参数时默认删除所有节点
 > 参数:  
 > index:节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_node()
 mdb.remove_node(index=1)
 ```  
 ### add_element
 根据单元编号和单元类型添加单元
 > 参数:  
 > index:单元编号  
 > ele_type:单元类型 1-梁 2-索 3-杆 4-板  
 > node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]  
 > beta_angle:贝塔角  
 > mat_id:材料编号  
 > sec_id:截面编号  
-```Python  
+```Python
 # 示例代码
-mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1.sec_id=1)
+from qtmodel import mdb
+mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
 ```  
 ### remove_element
 删除指定编号的单元
 > 参数:  
 > index: 单元编号,默认时删除所有单元  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_element()
 mdb.remove_element(index=1)
 ```  
 ##  材料操作
 ### add_material
 添加材料
 > 参数:  
@@ -106,46 +130,50 @@
 > name:材料名称  
 > material_type: 材料类型  
 > standard:规范名称  
 > database:数据库  
 > construct_factor:构造系数  
 > modified:是否修改默认材料参数,默认不修改 (可选参数)  
 > data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)  
-```Python  
+```Python
 # 示例代码
-mdb.add_material(index=1,name=“混凝土材料1”,material_type="混凝土",standard="公路18规范",database="C50")
-mdb.add_material(index=1,name=“自定义材料1”,material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+from qtmodel import mdb
+mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
+mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
 ```  
 ### add_time_material
 添加收缩徐变材料
 > 参数:  
 > index: 指定收缩徐变编号,默认则自动识别 (可选参数)  
 > name: 收缩徐变名  
 > code_index: 收缩徐变规范索引  
 > time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
 ```  
 ### update_material_creep
 将收缩徐变参数连接到材料
 > 参数:  
 > index: 材料编号  
 > creep_id: 收缩徐变编号  
 > f_cuk: 材料标准抗压强度,仅自定义材料是需要输入  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_material_creep(index=1,creep_id=1,f_cuk=5e7)
 ```  
 ### remove_material
 删除指定材料
 > 参数:  
 > index:指定材料编号，默认则删除所有材料  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_material()
 mdb.remove_material(index=1)
 ```  
 ##  截面和板厚操作
 ### add_parameter_section
 添加截面信息
 > 参数:  
@@ -163,17 +191,18 @@
 > box_height: 混凝土箱梁梁高 (仅混凝土箱梁截面需要)  
 > mat_combine: 组合截面材料信息 [弹性模量比s/c、密度比s/c、钢材泊松比、混凝土泊松比、热膨胀系数比s/c] (仅组合材料需要)  
 > bias_type:偏心类型 默认中心  
 > center_type:中心类型 默认质心  
 > shear_consider:考虑剪切 bool 默认考虑剪切变形  
 > bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要)  
 > bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
-mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心)
+from qtmodel import mdb
+mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
 mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
 ```  
 ### add_steel_section
 添加钢梁截面,包括参数型钢梁截面和自定义带肋钢梁截面
 > 参数:  
@@ -187,50 +216,54 @@
 > rib_place:肋板位置 list[tuple[布置位置,具体位置,参考点位置,list[tuple[间隔,肋板名，加劲肋位置,加劲肋名]]]]  
 > 布置位置 0-上...  具体位置 0-桥面1.。。 参考点位置 0-左  加劲肋位置 0-上/左 1-下/右 2-两侧 (详细信息参考UI界面顺序)  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要,相对形心)  
 > bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_steel_section(name="钢梁截面1",section_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
 mdb.add_steel_section(name="钢梁截面2",section_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
 rib_place2 = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
-bias_type=“中上”)
+bias_type="中上")
 ```  
 ### add_user_section
 添加自定义截面,目前仅支持特性截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > sec_type:截面类型  
 > property_info:截面特性列表  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_user_section(name="自定义特性截面",property_info=[i for i in range(25)])
 ```  
 ### add_tapper_section
 添加变截面,需先建立单一截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > begin_id:截面始端编号  
 > end_id:截面末端编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tapper_section(name="变截面1",begin_id=1,end_id=2)
 ```  
 ### remove_section
 删除截面信息
 > 参数:  
 > index: 截面编号,参数为默认时删除全部截面  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_section()
 mdb.remove_section(1)
 ```  
 ### add_thickness
 添加板厚
 > 参数:  
 > index: 板厚id  
@@ -239,160 +272,174 @@
 > thick_type: 板厚类型 0-普通板 1-加劲肋板  
 > bias_info:  默认不偏心,偏心时输入列表[type,value] type:0-厚度比 1-数值  
 > rib_pos: 肋板位置 0-下部 1-上部  
 > dist_v: 纵向截面肋板间距  
 > dist_l: 横向截面肋板间距  
 > rib_v: 纵向肋板信息  
 > rib_l: 横向肋板信息  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_thickness(name="厚度1", t=0.2,thick_type=0,bias_info=[0,0.8])
 mdb.add_thickness(name="厚度2", t=0.2,thick_type=1,rib_pos=0,dis_v=0.1,rib_v=[1,1,0.02,0.02])
 ```  
 ### remove_thickness
 删除板厚
 > 参数:  
 > index:板厚编号,默认时删除所有板厚信息  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_thickness()
 mdb.remove_thickness(index=1)
 ```  
 ### add_tapper_section_group
 添加变截面组
 > 参数:  
 > ids:变截面组编号  
 > name: 变截面组名  
 > factor_w: 宽度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > factor_h: 高度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > ref_w: 宽度方向参考点 0-i 1-j  
 > ref_h: 高度方向参考点 0-i 1-j  
 > dis_w: 宽度方向距离  
 > dis_h: 高度方向距离  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tapper_section_group(ids=[1,2,3,4],name="变截面组1")
 ```  
 ### update_section_bias
 更新截面偏心
 > 参数:  
 > index:截面编号  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_point:自定义偏心点(仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_section_bias(index=1,bias_type="中上",center_type="几何中心")
 mdb.update_section_bias(index=1,bias_type="自定义",bias_point=[0.1,0.2])
 ```  
 ##  边界操作
 ### add_boundary_group
 新建边界组
 > 参数:  
 > name:边界组名  
 > index:边界组编号，默认自动识别当前编号 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_boundary_group(name="边界组1")
 ```  
 ### remove_boundary_group
 按照名称删除边界组
 > 参数:  
 > name: 边界组名称，默认删除所有边界组 (非必须参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_boundary_group()
 mdb.remove_boundary_group(name="边界组1")
 ```  
 ### remove_all_boundary
 根据边界组名称、边界的类型和编号删除边界信息,默认时删除所有边界信息
 > 参数:  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_all_boundary()
 ```  
 ### remove_boundary
 根据节点号删除边界一般支撑、弹性支承，根据单元号删除梁端约束、根据主节点号删除主从约束、根据从节点号删除约束方程
 > 参数:  
 > remove_id:节点号 or 单元号 or主节点号  or 从节点号  
 > bd_type:边界类型  1-一般支承 2-弹性支承 3-主从约束 4-弹性连接 5-约束方程 6-梁端约束  
 > group:边界所处边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_boundary(remove_id = 1, bd_type = 1,group="边界组1")
 ```  
 ### add_general_support
 添加一般支承
 > 参数:  
 > node_id:节点编号  
 > boundary_info:边界信息  [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名,默认为默认边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_general_support(node_id=1, boundary_info=[True,True,True,False,False,False])
 ```  
 ### add_elastic_support
 添加弹性支承
 > 参数:  
 > node_id:节点编号  
 > support_type:支承类型 1-线性  2-受拉  3-受压  
 > boundary_info:边界信息 受拉和受压时列表长度为1  线性时列表长度为6  
 > group_name:边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_elastic_support(node_d=1,support_type=1,boundary_info=[1e6,0,1e6,0,0,0])
 ```  
 ### add_master_slave_link
 添加主从约束
 > 参数:  
 > master_id:主节点号  
 > slave_id:从节点号  
 > boundary_info:边界信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_master_slave_link(master_id=1,slave_id=2,boundary_info=[True,True,True,False,False,False])
 ```  
 ### add_elastic_link
 添加弹性连接
 > 参数:  
 > link_type:节点类型   1-一般弹性连接 2-刚性连接 3-受拉弹性连接 4-受压弹性连接  
 > start_id:起始节点号  
 > end_id:终节点号  
 > beta_angle:贝塔角  
 > boundary_info:边界信息  
 > group_name:边界组名  
 > dis_ratio:距i端距离比 (仅一般弹性连接需要)  
 > kx:受拉或受压刚度  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_elastic_link(link_type=1,start_id=1,end_id=2,boundary_info=[1e6,1e6,1e6,0,0,0])
 mdb.add_elastic_link(link_type=2,start_id=1,end_id=2)
 mdb.add_elastic_link(link_type=3,start_id=1,end_id=2,kx=1e6)
 ```  
 ### add_beam_constraint
 添加梁端约束
 > 参数:  
 > beam_id:梁号  
 > info_i:i端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > info_j:j端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_constraint(beam_id=2,info_i=[True,True,True,False,False,False],info_j=[True,True,True,False,False,False])
 ```  
 ### add_node_axis
 添加节点坐标
 > 参数:  
 > input_type:输入方式 1-角度 2-三点  3-向量  
 > node_id:节点号  
 > coord_info:局部坐标信息 -List<float>(角)  -List<List<float>>(三点 or 向量)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_axis(input_type=1,node_id=1,coord_info=[45,45,45])
 mdb.add_node_axis(input_type=2,node_id=1,coord_info=[[0,0,1],[0,1,0],[1,0,0]])
 mdb.add_node_axis(input_type=3,node_id=1,coord_info=[[0,0,1],[0,1,0]])
 ```  
 ##  移动荷载
 ### add_standard_vehicle
 添加标准车辆
@@ -407,128 +454,140 @@
 > 6-城市轨道交通桥梁规范(GB/T51234-2017)  
 > load_type: 荷载类型  
 > 支持类型: "公路I级","公路II级","城A车道","城B车道","地铁A型车","地铁B型车","地铁C型车","汽10"  
 > "汽15","汽20","汽超20","特载","挂80","挂100","挂120","公路疲劳荷载1","公路疲劳荷载2","公路疲劳荷载3",  
 > "汽36轻", "汽38重","高速铁路","城际铁路","客货共线铁路","重载铁路","中活载","长大货物车检算荷载"  
 > load_length: 默认为0即不限制荷载长度  (铁路桥涵规范 Q/CR 9300-2017 所需参数)  
 > n:车厢数: 默认6节车厢 (城市轨道交通桥梁规范 GB/T51234-2017 所需参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_standard_vehicle("高速铁路",standard_code=1,load_type="高速铁路")
 ```  
 ### add_node_tandem
 添加节点纵列
 > 参数:  
 > name:节点纵列名  
 > start_id:起始节点号  
 > node_ids:节点列表  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_tandem("节点纵列1",1,[i+1 for i in range(12)])
 ```  
 ### add_influence_plane
 添加影响面
 > 参数:  
 > name:影响面名称  
 > tandem_names:节点纵列名称组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_influence_plane("影响面1",["节点纵列1","节点纵列2"])
 ```  
 ### add_lane_line
 添加车道线
 > 参数:  
 > name:车道线名称  
 > influence_name:影响面名称  
 > tandem_name:节点纵列名  
 > offset:偏移  
 > lane_width:车道宽度  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_lane_line("车道1","影响面1","节点纵列1",offset=0,lane_width=3.1)
 ```  
 ### add_live_load_case
 添加移动荷载工况
 > 参数:  
 > name:荷载工况名  
 > influence_plane:影响线名  
 > span:跨度  
 > car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > train_detail: 火车相关系数 (横向折减列表float[8],纵向折减系数,强度冲击,疲劳冲击)  
 > metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]  
-```Python  
+```Python
 # 示例代码
-mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[(“车辆名称”,1.0,["车道1","车道2"])...])
+from qtmodel import mdb
+mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
 ```  
 ### remove_vehicle
 删除车辆信息
 > 参数:  
 > index:车辆荷载编号  
 > name:车辆名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_vehicle(index=1)
 mdb.remove_vehicle(name="车辆名称")
 ```  
 ### remove_node_tandem
 按照 节点纵列编号/节点纵列名 删除节点纵列
 > 参数:  
 > index:节点纵列编号  
 > name:节点纵列名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_node_tandem(index=1)
 mdb.remove_node_tandem(name="节点纵列1")
 ```  
 ### remove_influence_plane
 按照 影响面编号/影响面名称 删除影响面
 > 参数:  
 > index:影响面编号  
 > name:影响面名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_influence_plane(index=1)
 mdb.remove_influence_plane(name="影响面1")
 ```  
 ### remove_lane_line
 按照 车道线编号/车道线名称 删除车道线
 > 参数:  
 > name:车道线名称  
 > index:车道线编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_lane_line(index=1)
 mdb.remove_lane_line(name="车道线1")
 ```  
 ### remove_live_load_case
 删除移动荷载工况
 > 参数:  
 > name:移动荷载工况名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_live_load_case(name="活载工况1")
 ```  
 ##  钢束操作
 ### add_tendon_group
 按照名称添加钢束组，添加时可指定钢束组id
 > 参数:  
 > name: 钢束组名称  
 > index: 钢束组编号(非必须参数)，默认自动识别  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_group(name="钢束组1")
 ```  
 ### remove_tendon_group
 按照钢束组名称或钢束组编号删除钢束组，两参数均为默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称,默认自动识别 (可选参数)  
 > index:钢束组编号,默认自动识别 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon_group(name="钢束组1")
 mdb.remove_tendon_group(index=1)
 ```  
 ### add_tendon_property
 添加钢束特性
 > 参数:  
 > name:钢束特性名  
@@ -536,16 +595,17 @@
 > tendon_type: 0-PRE 1-POST  
 > material_id: 钢材材料编号  
 > duct_type: 1-金属波纹管  2-塑料波纹管  3-铁皮管  4-钢管  5-抽芯成型  
 > steel_type: 1-钢绞线  2-螺纹钢筋  
 > steel_detail: 钢绞线[钢束面积,孔道直径,摩阻系数,偏差系数]  螺纹钢筋[钢筋直径,钢束面积,孔道直径,摩阻系数,偏差系数,张拉方式(1-一次张拉\2-超张拉)]  
 > loos_detail: 松弛信息[规范(1-公规 2-铁规),张拉(1-一次张拉 2-超张拉),松弛(1-一般松弛 2-低松弛)] (仅钢绞线需要,默认为[1,1,1])  
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=[1,1,1])
 ```  
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
@@ -556,366 +616,402 @@
 > position_type: 定位方式 1-直线  2-轨迹线  
 > control_points: 控制点信息[(x1,y1,z1,r1),(x2,y2,z2,r2)....]  
 > point_insert: 定位方式为直线时为插入点坐标[x,y,z], 轨迹线时为 [插入端(1-I 2-J),插入方向(1-ij 2-ji),插入单元id]  
 > tendon_direction:直线钢束X方向向量 x轴-[1,0,0] y轴-[0,1,0]  默认为[1,0,0] (轨迹线不用赋值)  
 > rotation_angle:绕钢束旋转角度  
 > track_group:轨迹线结构组名  (直线时不用赋值)  
 > projection:直线钢束投影，默认为true  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=1,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(0,0,0))
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=2,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(1,1,1),track_group="轨迹线结构组1")
 ```  
 ### remove_tendon
 按照名称或编号删除钢束,默认时删除所有钢束
 > 参数:  
 > name:钢束名称  
 > index:钢束编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon(name="钢束1")
 mdb.remove_tendon(index=1)
 mdb.remove_tendon()
 ```  
 ### remove_tendon_property
 按照名称或编号删除钢束组,默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称  
 > index:钢束组编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon_property(name="钢束特性1")
 mdb.remove_tendon_property(index=1)
 mdb.remove_tendon_property()
 ```  
 ### add_nodal_mass
 添加节点质量
 > 参数:  
 > node_id:节点编号  
 > mass_info:[m,rmX,rmY,rmZ]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodal_mass(node_id=1,mass_info=(100,0,0,0))
 ```  
 ### remove_nodal_mass
 删除节点质量
 > 参数:  
 > node_id:节点号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_nodal_mass(node_id=1)
 ```  
 ### add_pre_stress
 添加预应力
 > 参数:  
 > case_name:荷载工况名  
 > tendon_name:钢束名  
 > pre_type:预应力类型 0-始端 1-末端 2-两端  
 > force:预应力  
 > group_name:边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_pre_stress(case_name="荷载工况名",tendon_name="钢束1",force=1390000)
 ```  
 ### remove_pre_stress
 删除预应力
 > 参数:  
 > case_name:荷载工况  
 > tendon_name:钢束组  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_pre_stress(case_name="工况1",tendon_name="钢束1",group_name="默认荷载组")
 ```  
 ##  荷载操作
 ### add_load_group
 根据荷载组名称添加荷载组
 > 参数:  
 > name: 荷载组名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_group(name="荷载组1")
 ```  
 ### remove_load_group
 根据荷载组名称或荷载组id删除荷载组,参数为默认时删除所有荷载组
 > 参数:  
 > name: 荷载组名称  
 > index: 荷载组编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_load_group(name="荷载组1")
 mdb.remove_load_group(index="1")
 ```  
 ### add_nodal_force
 添加节点荷载
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodal_force(case_name="荷载工况1",node_id=1,load_info=(1,1,1,1,1,1),group_name="默认结构组")
 ```  
 ### remove_nodal_force
 删除节点荷载
 > 参数:  
 > case_name:荷载工况名  
 > node_id:节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_nodal_force(case_name="荷载工况1",node_id=1)
 ```  
 ### add_node_displacement
 添加节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 > load_info:[Dx,Dy,Dz,Rx,Ry,Rz]  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_displacement(case_name="荷载工况1",node_id=1,load_info=(1,0,0,0,0,0),group_name="默认荷载组")
 ```  
 ### remove_nodal_displacement
 删除节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
-```Python  
+```Python
 # 示例代码
-mdn.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
+from qtmodel import mdb
+mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
 ```  
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩  
 > coord_system:坐标系 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
 > uniform_load:均布荷载值  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型 1-集中力   2-集中弯矩  3-分布力   4-分布弯矩  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
-mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1，group_name="默认荷载组")
+from qtmodel import mdb
+mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
 ```  
 ### add_initial_tension
 添加初始拉力
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > tension:初始拉力  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_initial_tension(element_id=1,case_name="工况1",tension=100,tension_type=1)
 ```  
 ### add_cable_length_load
 添加索长张拉
 > 参数:  
 > element_id:单元类型  
 > case_name:荷载工况名  
 > length:长度  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
 ```  
 ### add_plate_element_load
 添加版单元荷载
 > 参数:  
 > element_id:单元id  
 > case_name:荷载工况名  
 > load_type:荷载类型   1-集中力  2-集中弯矩  3-分布力  4-分布弯矩  
 > load_place:荷载位置  0-面IJKL 1-边IJ  2-边JK  3-边KL  4-边LI  (仅分布荷载需要)  
 > coord_system:坐标系  (默认3) 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z  
 > group_name:荷载组名  
 > load_list:荷载列表  
 > xy_list:荷载位置信息 [IJ方向距离x,IL方向距离y]  (仅集中荷载需要,x,y代表荷载距离板单元I端的绝对值)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=[0.2,0.5])
 ```  
 ### add_deviation_parameter
 添加制造误差
 > 参数:  
 > name:名称  
 > element_type:单元类型  1-梁单元  2-板单元  
 > parameters:参数列表  
 > 梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]  
 > 板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]  
-```Python  
+```Python
 # 示例代码
-mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameterInfo=parameters)
+from qtmodel import mdb
+mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameters=[1,0,0,0,0,0,0])
+mdb.add_deviation_parameter(name="板端制造误差",elementType=1,parameters=[1,0,0,0,0])
 ```  
 ### add_deviation_load
 添加制造误差荷载
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > parameters:参数名列表 梁杆单元时-[制造误差参数名称]   板单元时-[I端误差名,J端误差名,K端误差名,L端误差名]  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
-mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=[“梁端误差”])
-mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=[“板端误差1”,"板端误差2","板端误差3","板端误差4"])
+from qtmodel import mdb
+mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
+mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
 ```  
 ### add_element_temperature
 添加单元温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:最终温度  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_element_temperature(element_id=1,case_name="自重",temperature=1,group_name="默认荷载组")
 ```  
 ### add_gradient_temperature
 添加梯度温度
-```Python  
+```Python
 # 示例代码
-mdb.add_gradient_temperature(elementId=1,caseName=“荷载工况1”,groupName=“荷载组名1,temperature=10)
-mdb.add_gradient_temperature(elementId=2,caseName=“荷载工况2”,groupName=”荷载组名2“,temperature=10,element_type=2)
+from qtmodel import mdb
+mdb.add_gradient_temperature(elementId=1,caseName="荷载工况1",groupName="荷载组名1",temperature=10)
+mdb.add_gradient_temperature(elementId=2,caseName="荷载工况2",groupName="荷载组名2",temperature=10,element_type=2)
 ```  
 ### add_beam_section_temperature
 添加梁截面温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > paving_thick:铺设厚度(m)  
 > temperature_type:温度类型  1-升温(默认) 2-降温  
 > paving_type:铺设类型     1-沥青混凝土(默认)  2-水泥混凝土  
 > group_name:荷载组名  
 > modify:是否修改规范温度  
 > temp_list:温度列表[T1,T2]  (仅修改时需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_section_temperature(element_id=1,case_name="工况1",paving_thick=0.1)
 ```  
 ### add_index_temperature
 添加指数温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:温差  
 > index:指数  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_index_temperature(element_id=1,case_name="工况1",temperature=20,index=2)
 ```  
 ### add_top_plate_temperature
 添加顶板温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载  
 > temperature:最终温度  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_top_plate_temperature(element_id=1,case_name="工况1",temperature=40,group_name="默认荷载组")
 ```  
 ##  沉降操作
 ### add_sink_group
 添加沉降组
 > 参数:  
 > name: 沉降组名  
 > sink: 沉降值  
 > node_ids: 节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_sink_group(name="沉降1",sink=0.1,node_ids=[1,2,3])
 ```  
 ### remove_sink_group
 按照名称删除沉降组
 > 参数:  
 > name:沉降组名,默认删除所有沉降组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_sink_group()
 mdb.remove_sink_group(name="沉降1")
 ```  
 ### add_sink_case
 添加沉降工况
 > 参数:  
 > name:荷载工况名  
 > sink_groups:沉降组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_sink_case(name="沉降工况1",sink_groups=["沉降1","沉降2"])
 ```  
 ### remove_sink_case
 按照名称删除沉降工况,不输入名称时默认删除所有沉降工况
 > 参数:  
 > name:沉降工况名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_sink_case()
 mdb.remove_sink_case(name="沉降1")
 ```  
 ### add_concurrent_reaction
 添加并发反力组
 > 参数:  
 > names: 结构组名称集合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_concurrent_reaction(["默认结构组"])
 ```  
 ### remove_concurrent_reaction
 删除所有并发反力组
 > 参数:  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_concurrent_reaction()
 ```  
 ### add_concurrent_force
 创建并发内力组
 > 参数:  
 > names: 结构组名称集合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_concurrent_force(["默认结构组"])
 ```  
 ### remove_concurrent_force
 删除所有并发内力组
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_concurrent_force()
 ```  
 ### add_load_case
 添加荷载工况
 > 参数:  
 > name:沉降名  
 > case_type:荷载工况类型  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_case(name="工况1",case_type=1)
 ```  
 ### remove_load_case
 删除荷载工况,参数均为默认时删除全部荷载工况
 > 参数:  
 > index:荷载编号  
 > name:荷载名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_case(index=1)
 mdb.add_load_case(name="工况1")
 mdb.add_load_case()
 ```  
 ### test_print
 测试运行
 ##  施工阶段和荷载组合
@@ -933,17 +1029,18 @@
 > delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]  
 > active_loads:激活荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > delete_loads:钝化荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
 > index:施工阶段编号，默认自动添加  
-```Python  
+```Python
 # 示例代码
-mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+from qtmodel import mdb
+mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
 ### update_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
@@ -955,52 +1052,59 @@
 > 位置:  0-变形前 1-变形后  
 > delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]  
 > active_loads:激活荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > delete_loads:钝化荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
-```Python  
+```Python
 # 示例代码
-mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+from qtmodel import mdb
+mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
 ### update_weight_stage
 添加施工阶段信息
 > 参数:  
 > stage_name:施工阶段信息  
 > structure_group_name:结构组名  
 > weight_stage_id: 计自重阶段号: 0-不计自重,1-本阶段 n-第n阶段  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_weight_stage(stage_name="施工阶段1",structure_group_name="默认结构组",weight_stage_id=1)
 ```  
 ### remove_construction_stage
 按照施工阶段名删除施工阶段,默认删除所有施工阶段
 > 参数:  
 > name:所删除施工阶段名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_construction_stage(name="施工阶段1")
 ```  
 ### add_load_combine
 添加荷载组合
 > 参数:  
 > name:荷载组合名  
 > combine_type:荷载组合类型 1-叠加  2-判别  3-包络  
 > describe:描述  
 > combine_info:荷载组合信息 [(荷载工况类型,工况名,系数)...]  
 > 荷载工况类型: "ST"-静力荷载工况  "CS"-施工阶段荷载工况  "CB"-荷载组合  
 > "MV"-移动荷载工况  "SM"-沉降荷载工况  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_combine(name="荷载组合1",combine_type=1,describe="无",combine_info=[("CS","合计值",1),("CS","恒载",1)])
 ```  
 ### remove_load_combine
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
 ```  
 
+
+
```

### Comparing `qtmodel-0.2.3/qtmodel/qt_mdb.py` & `qtmodel-0.2.4/qtmodel/qt_mdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,41 +25,41 @@
     def add_structure_group(name: str = "", index: int = -1):
         """
         添加结构组
         Args:
             name: 结构组名
             index: 结构组编号(非必须参数)，默认自动识别当前编号
         example:
-                mdb.add_structure_group("新建结构组1")
+                mdb.add_structure_group(name="新建结构组1")
                 mdb.add_structure_group(name="新建结构组2",index=2)
         Returns: 无
         """
         qt_model.AddStructureGroup(name=name, id=index)
 
     @staticmethod
     def remove_structure_group(name: str = "", index: int = -1):
         """
         可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
         Args:
             name:结构组名称
             index:结构组编号
         example:
-                mdb.remove_structure_group(name=“新建结构组1”)
+                mdb.remove_structure_group(name="新建结构组1")
                 mdb.remove_structure_group(index = 2)
         Returns: 无
         """
         if index != -1:
             qt_model.RemoveStructureGroup(id=index)
         elif name != "":
             qt_model.RemoveStructureGroup(name=name)
         else:
             qt_model.RemoveAllStructureGroup()
 
     @staticmethod
-    def add_structure_to_group(name: int = "", node_ids: list[int] = None, element_ids: list[int] = None):
+    def add_structure_to_group(name: str = "", node_ids: list[int] = None, element_ids: list[int] = None):
         """
         为结构组添加节点和/或单元
         Args:
              name: 结构组名
              node_ids: 节点编号列表(可选参数)
              element_ids: 单元编号列表(可选参数)
         example:
@@ -148,15 +148,15 @@
             index:单元编号
             ele_type:单元类型 1-梁 2-索 3-杆 4-板
             node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]
             beta_angle:贝塔角
             mat_id:材料编号
             sec_id:截面编号
         example:
-            mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1.sec_id=1)
+            mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
         Returns: 无
         """
         if node_ids is None and ele_type != 4:
             raise Exception("操作错误,请输入此单元所需节点列表,[i,j]")
         if node_ids is None and ele_type == 4:
             raise Exception("操作错误,请输入此板单元所需节点列表,[i,j,k,l]")
         if ele_type == 1:
@@ -200,16 +200,16 @@
             material_type: 材料类型
             standard:规范名称
             database:数据库
             construct_factor:构造系数
             modified:是否修改默认材料参数,默认不修改 (可选参数)
             data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)
         example:
-            mdb.add_material(index=1,name=“混凝土材料1”,material_type="混凝土",standard="公路18规范",database="C50")
-            mdb.add_material(index=1,name=“自定义材料1”,material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+            mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
+            mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
         Returns: 无
         """
         list_material = ["混凝土", "钢材", "预应力", "钢丝", "钢筋", "自定义"]
         if material_type not in list_material:
             raise Exception(f"操作错误,material_type不在指定列表:{list_material}中")
         if modified and len(data_info) != 4:
             raise Exception("操作错误,modify_info数据无效!")
@@ -325,15 +325,15 @@
              mat_combine: 组合截面材料信息 [弹性模量比s/c、密度比s/c、钢材泊松比、混凝土泊松比、热膨胀系数比s/c] (仅组合材料需要)
              bias_type:偏心类型 默认中心
              center_type:中心类型 默认质心
              shear_consider:考虑剪切 bool 默认考虑剪切变形
              bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要)
              bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)
         example:
-            mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心)
+            mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
             mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
                 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
                 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
         Returns: 无
         """
         sec_type_list = ["矩形", "圆形", "圆管", "箱型", "实腹八边形",
                          "空腹八边形", "内八角形", "实腹圆端型", "T形", "倒T形",
@@ -388,15 +388,15 @@
              bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要,相对形心)
              bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)
         example:
             mdb.add_steel_section(name="钢梁截面1",section_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
             mdb.add_steel_section(name="钢梁截面2",section_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
                 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
                 rib_place2 = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
-                bias_type=“中上”)
+                bias_type="中上")
         Returns: 无
         """
 
         if sec_info is None:
             raise Exception("操作错误,请输入此截面的截面信息，参数列表可参考截面定义窗口")
         section_type = "工字钢梁" if sec_type == 1 else "箱型钢梁"
         rib_names = list(rib_info.keys())
@@ -807,15 +807,15 @@
              influence_plane:影响线名
              span:跨度
              car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)
              train_detail: 火车相关系数 (横向折减列表float[8],纵向折减系数,强度冲击,疲劳冲击)
              metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)
              sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]
         example:
-            mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[(“车辆名称”,1.0,["车道1","车道2"])...])
+            mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
         Returns: 无
         """
         if sub_case is None:
             raise Exception("操作错误，子工况信息列表不能为空")
         qt_model.AddLiveLoadCase(name=name, influencePlane=influence_plane, span=span, subCase=sub_case)
 
     @staticmethod
@@ -1188,15 +1188,15 @@
     def remove_nodal_displacement(node_id: int = -1, case_name: str = ""):
         """
         删除节点位移
         Args:
             node_id:节点编号
             case_name:荷载工况名
         example:
-            mdn.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
+            mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
         Returns: 无
         """
         qt_model.RemoveNodalDisplacement(caseName=case_name, nodeId=-node_id)
 
     @staticmethod
     def add_beam_load(beam_id: int = 1, case_name: str = "", load_type: int = 1, coord_system: int = 3, list_x: list[float] = None,
                       list_load: list[float] = None, uniform_load: float = 0, group_name="默认荷载组"):
@@ -1226,15 +1226,15 @@
         删除梁单元荷载
         Args:
             element_id:单元号
             case_name:荷载工况名
             load_type:荷载类型 1-集中力   2-集中弯矩  3-分布力   4-分布弯矩
             group_name:边界组名
         example:
-            mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1，group_name="默认荷载组")
+            mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
         Returns: 无
         """
         qt_model.RemoveBeamLoad(caseName=case_name, elementId=element_id, loadType=load_type, groupName=group_name)
 
     @staticmethod
     def add_initial_tension(element_id: int = 1, case_name: str = "", group_name: str = "默认荷载组", tension: float = 0, tension_type: int = 1):
         """
@@ -1301,15 +1301,16 @@
         Args:
             name:名称
             element_type:单元类型  1-梁单元  2-板单元
             parameters:参数列表
                 梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]
                 板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]
         example:
-            mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameterInfo=parameters)
+            mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameters=[1,0,0,0,0,0,0])
+            mdb.add_deviation_parameter(name="板端制造误差",elementType=1,parameters=[1,0,0,0,0])
         Returns: 无
         """
         if parameters is None:
             raise Exception("操作错误，制造误差信息不能为空")
         if len(parameters) != 5 or len(parameters) != 7:
             raise Exception("操作错误，误差列表有误")
         qt_model.AddDeviationParameter(name=name, elementType=element_type, parameterInfo=parameters)
@@ -1320,16 +1321,16 @@
         添加制造误差荷载
         Args:
             element_id:单元编号
             case_name:荷载工况名
             parameters:参数名列表 梁杆单元时-[制造误差参数名称]   板单元时-[I端误差名,J端误差名,K端误差名,L端误差名]
             group_name:荷载组名
         example:
-            mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=[“梁端误差”])
-            mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=[“板端误差1”,"板端误差2","板端误差3","板端误差4"])
+            mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
+            mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
         Returns: 无
         """
         if parameters is None:
             raise Exception("操作错误，制造误差名称信息不能为空")
         qt_model.AddDeviationLoad(elementId=element_id, caseName=case_name, parameterName=parameters, groupName=group_name)
 
     @staticmethod
@@ -1355,16 +1356,16 @@
              element_id:单元编号
              case_name:荷载工况名
              temperature:温差
              section_oriental:截面方向 1-截面Y向(默认)  2-截面Z向  (仅梁单元需要)
              element_type:单元类型 1-梁单元(默认)  2-板单元
              group_name:荷载组名
         example:
-            mdb.add_gradient_temperature(elementId=1,caseName=“荷载工况1”,groupName=“荷载组名1,temperature=10)
-            mdb.add_gradient_temperature(elementId=2,caseName=“荷载工况2”,groupName=”荷载组名2“,temperature=10,element_type=2)
+            mdb.add_gradient_temperature(elementId=1,caseName="荷载工况1",groupName="荷载组名1",temperature=10)
+            mdb.add_gradient_temperature(elementId=2,caseName="荷载工况2",groupName="荷载组名2",temperature=10,element_type=2)
         Returns: 无
         """
         qt_model.AddGradientTemperature(elementId=element_id, caseName=case_name, temperature=temperature,
                                         sectionOriental=section_oriental, elementType=element_type, groupNmae=group_name)
 
     @staticmethod
     def add_beam_section_temperature(element_id: int = 1, case_name: str = "", paving_thick: float = 0, temperature_type: int = 1,
@@ -1605,15 +1606,15 @@
            active_loads:激活荷载组信息 [(荷载组1,时间),...]
                                时间: 0-开始 1-结束
            delete_loads:钝化荷载组信息 [(荷载组1,时间),...]
                                时间: 0-开始 1-结束
            temp_loads:临时荷载信息 [荷载组1，荷载组2,..]
            index:施工阶段编号，默认自动添加
         example:
-           mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+           mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
                 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
         Returns: 无
         """
         qt_model.AddConstructionStage(name=name, duration=duration, activeStructures=active_structures, inActiveStructures=delete_structures
                                       , activeBoundaries=active_boundaries, inActiveBoundaries=delete_boundaries, activeLoads=active_loads,
                                       inActiveLoads=delete_loads, tempLoads=temp_loads, id=index)
 
@@ -1640,15 +1641,15 @@
            delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]
            active_loads:激活荷载组信息 [(荷载组1,时间),...]
                                时间: 0-开始 1-结束
            delete_loads:钝化荷载组信息 [(荷载组1,时间),...]
                                时间: 0-开始 1-结束
            temp_loads:临时荷载信息 [荷载组1，荷载组2,..]
         example:
-           mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+           mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
                active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
         Returns: 无
         """
         qt_model.UpdateConstructionStage(name=name, duration=duration, activeStructures=active_structures, inActiveStructures=delete_structures
                                          , activeBoundaries=active_boundaries, inActiveBoundaries=delete_boundaries, activeLoads=active_loads,
                                          inActiveLoads=delete_loads, tempLoads=temp_loads)
```

### Comparing `qtmodel-0.2.3/qtmodel/qt_odb.py` & `qtmodel-0.2.4/qtmodel/qt_odb.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.3/qtmodel/res_db.py` & `qtmodel-0.2.4/qtmodel/res_db.py`

 * *Files identical despite different names*

### Comparing `qtmodel-0.2.3/qtmodel.egg-info/PKG-INFO` & `qtmodel-0.2.4/qtmodel.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,128 @@
 Metadata-Version: 2.1
 Name: qtmodel
-Version: 0.2.3
+Version: 0.2.4
 Summary: python modeling for qt
 Home-page: https://github.com/Inface0443/pyqt
 Author: dqy-zhj
 Author-email: 1105417715@qq.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 ##  初始化模型
 ### initial
 初始化模型
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.initial()
 ```  
 ##  节点单元操作
 ### add_structure_group
 添加结构组
 > 参数:  
 > name: 结构组名  
 > index: 结构组编号(非必须参数)，默认自动识别当前编号  
-```Python  
+```Python
 # 示例代码
-mdb.add_structure_group("新建结构组1")
+from qtmodel import mdb
+mdb.add_structure_group(name="新建结构组1")
 mdb.add_structure_group(name="新建结构组2",index=2)
 ```  
 ### remove_structure_group
 可根据结构与组名或结构组编号删除结构组，当组名和组编号均为默认则删除所有结构组
 > 参数:  
 > name:结构组名称  
 > index:结构组编号  
-```Python  
+```Python
 # 示例代码
-mdb.remove_structure_group(name=“新建结构组1”)
+from qtmodel import mdb
+mdb.remove_structure_group(name="新建结构组1")
 mdb.remove_structure_group(index = 2)
 ```  
 ### add_structure_to_group
 为结构组添加节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
 ### remove_structure_in_group
 为结构组删除节点和/或单元
 > 参数:  
 > name: 结构组名  
 > node_ids: 节点编号列表(可选参数)  
 > element_ids: 单元编号列表(可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_structure_to_group(name="现有结构组1",node_ids=[1,2,3,4],element_ids=[1,2])
 ```  
 ### add_node
 根据坐标信息和节点编号添加节点，默认自动识别编号
 > 参数:  
 > x: 节点坐标x  
 > y: 节点坐标y  
 > z: 节点坐标z  
 > index: 节点编号，默认自动识别编号 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node(1,2,3)
 mdb.add_node(x= 1,y = 2,z = 4,index = 2)
 ```  
 ### add_nodes
 添加多个节点，可以选择指定节点编号
 > 参数:  
 > node_list:节点坐标信息 [[x1,y1,z1],...]或 [[id1,x1,y1,z1]...]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodes([[1,2,3],[4,5,6]])
 mdb.add_nodes([[1,1,2,3],[2,4,5,6]])
 ```  
 ### remove_node
 删除指定节点,不输入参数时默认删除所有节点
 > 参数:  
 > index:节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_node()
 mdb.remove_node(index=1)
 ```  
 ### add_element
 根据单元编号和单元类型添加单元
 > 参数:  
 > index:单元编号  
 > ele_type:单元类型 1-梁 2-索 3-杆 4-板  
 > node_ids:单元对应的节点列表 [i,j] 或 [i,j,k,l]  
 > beta_angle:贝塔角  
 > mat_id:材料编号  
 > sec_id:截面编号  
-```Python  
+```Python
 # 示例代码
-mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1.sec_id=1)
+from qtmodel import mdb
+mdb.add_element(index=1,ele_type=1,node_ids=[1,2],beta_angle=1,mat_id=1,sec_id=1)
 ```  
 ### remove_element
 删除指定编号的单元
 > 参数:  
 > index: 单元编号,默认时删除所有单元  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_element()
 mdb.remove_element(index=1)
 ```  
 ##  材料操作
 ### add_material
 添加材料
 > 参数:  
@@ -120,46 +130,50 @@
 > name:材料名称  
 > material_type: 材料类型  
 > standard:规范名称  
 > database:数据库  
 > construct_factor:构造系数  
 > modified:是否修改默认材料参数,默认不修改 (可选参数)  
 > data_info:材料参数列表[弹性模量,容重,泊松比,热膨胀系数] (可选参数)  
-```Python  
+```Python
 # 示例代码
-mdb.add_material(index=1,name=“混凝土材料1”,material_type="混凝土",standard="公路18规范",database="C50")
-mdb.add_material(index=1,name=“自定义材料1”,material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
+from qtmodel import mdb
+mdb.add_material(index=1,name="混凝土材料1",material_type="混凝土",standard="公路18规范",database="C50")
+mdb.add_material(index=1,name="自定义材料1",material_type="自定义",data_info=[3.5e10,2.5e4,0.2,1.5e-5])
 ```  
 ### add_time_material
 添加收缩徐变材料
 > 参数:  
 > index: 指定收缩徐变编号,默认则自动识别 (可选参数)  
 > name: 收缩徐变名  
 > code_index: 收缩徐变规范索引  
 > time_parameter: 对应规范的收缩徐变参数列表,默认不改变规范中信息 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_time_material(index=1,name="收缩徐变材料1",code_index=1)
 ```  
 ### update_material_creep
 将收缩徐变参数连接到材料
 > 参数:  
 > index: 材料编号  
 > creep_id: 收缩徐变编号  
 > f_cuk: 材料标准抗压强度,仅自定义材料是需要输入  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_material_creep(index=1,creep_id=1,f_cuk=5e7)
 ```  
 ### remove_material
 删除指定材料
 > 参数:  
 > index:指定材料编号，默认则删除所有材料  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_material()
 mdb.remove_material(index=1)
 ```  
 ##  截面和板厚操作
 ### add_parameter_section
 添加截面信息
 > 参数:  
@@ -177,17 +191,18 @@
 > box_height: 混凝土箱梁梁高 (仅混凝土箱梁截面需要)  
 > mat_combine: 组合截面材料信息 [弹性模量比s/c、密度比s/c、钢材泊松比、混凝土泊松比、热膨胀系数比s/c] (仅组合材料需要)  
 > bias_type:偏心类型 默认中心  
 > center_type:中心类型 默认质心  
 > shear_consider:考虑剪切 bool 默认考虑剪切变形  
 > bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要)  
 > bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
-mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心)
+from qtmodel import mdb
+mdb.add_parameter_section(name="截面1",sec_type="矩形",sec_info=[2,4],bias_type="中心")
 mdb.add_parameter_section(name="截面2",sec_type="混凝土箱梁",box_height=2,box_number=3,
 sec_info=[0.02,0,12,3,1,2,1,5,6,0.2,0.4,0.1,0.13,0.28,0.3,0.5,0.5,0.5,0.2],
 charm_info=["1*0.2,0.1*0.2","0.5*0.15,0.3*0.2","0.4*0.2","0.5*0.2"])
 ```  
 ### add_steel_section
 添加钢梁截面,包括参数型钢梁截面和自定义带肋钢梁截面
 > 参数:  
@@ -201,50 +216,54 @@
 > rib_place:肋板位置 list[tuple[布置位置,具体位置,参考点位置,list[tuple[间隔,肋板名，加劲肋位置,加劲肋名]]]]  
 > 布置位置 0-上...  具体位置 0-桥面1.。。 参考点位置 0-左  加劲肋位置 0-上/左 1-下/右 2-两侧 (详细信息参考UI界面顺序)  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_x:自定义偏心点x坐标 (仅自定义类型偏心需要,相对形心)  
 > bias_y:自定义偏心点y坐标 (仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_steel_section(name="钢梁截面1",section_type=1,sec_info=[0,0,0.5,0.5,0.5,0.5,0.7,0.02,0.02,0.02])
 mdb.add_steel_section(name="钢梁截面2",section_type=2,sec_info=[0,0.15,0.25,0.5,0.25,0.15,0.4,0.15,0.7,0.02,0.02,0.02,0.02],
 rib_info = {"板肋1": [0.1,0.02],"T形肋1":[0.1,0.02,0.02,0.02]},
 rib_place2 = [(0, 0, 0, [(0.1, "板肋1", 2, "默认名称1"), (0.2, "板肋1", 2, "默认名称2")]), (0, 0, 1, [(0.1, "T形肋1", 0, "默认名称3")])],
-bias_type=“中上”)
+bias_type="中上")
 ```  
 ### add_user_section
 添加自定义截面,目前仅支持特性截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > sec_type:截面类型  
 > property_info:截面特性列表  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_user_section(name="自定义特性截面",property_info=[i for i in range(25)])
 ```  
 ### add_tapper_section
 添加变截面,需先建立单一截面
 > 参数:  
 > index:截面编号  
 > name:截面名称  
 > begin_id:截面始端编号  
 > end_id:截面末端编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tapper_section(name="变截面1",begin_id=1,end_id=2)
 ```  
 ### remove_section
 删除截面信息
 > 参数:  
 > index: 截面编号,参数为默认时删除全部截面  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_section()
 mdb.remove_section(1)
 ```  
 ### add_thickness
 添加板厚
 > 参数:  
 > index: 板厚id  
@@ -253,160 +272,174 @@
 > thick_type: 板厚类型 0-普通板 1-加劲肋板  
 > bias_info:  默认不偏心,偏心时输入列表[type,value] type:0-厚度比 1-数值  
 > rib_pos: 肋板位置 0-下部 1-上部  
 > dist_v: 纵向截面肋板间距  
 > dist_l: 横向截面肋板间距  
 > rib_v: 纵向肋板信息  
 > rib_l: 横向肋板信息  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_thickness(name="厚度1", t=0.2,thick_type=0,bias_info=[0,0.8])
 mdb.add_thickness(name="厚度2", t=0.2,thick_type=1,rib_pos=0,dis_v=0.1,rib_v=[1,1,0.02,0.02])
 ```  
 ### remove_thickness
 删除板厚
 > 参数:  
 > index:板厚编号,默认时删除所有板厚信息  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_thickness()
 mdb.remove_thickness(index=1)
 ```  
 ### add_tapper_section_group
 添加变截面组
 > 参数:  
 > ids:变截面组编号  
 > name: 变截面组名  
 > factor_w: 宽度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > factor_h: 高度方向变化阶数 线性(1.0) 非线性(!=1.0)  
 > ref_w: 宽度方向参考点 0-i 1-j  
 > ref_h: 高度方向参考点 0-i 1-j  
 > dis_w: 宽度方向距离  
 > dis_h: 高度方向距离  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tapper_section_group(ids=[1,2,3,4],name="变截面组1")
 ```  
 ### update_section_bias
 更新截面偏心
 > 参数:  
 > index:截面编号  
 > bias_type:偏心类型  
 > center_type:中心类型  
 > shear_consider:考虑剪切  
 > bias_point:自定义偏心点(仅自定义类型偏心需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_section_bias(index=1,bias_type="中上",center_type="几何中心")
 mdb.update_section_bias(index=1,bias_type="自定义",bias_point=[0.1,0.2])
 ```  
 ##  边界操作
 ### add_boundary_group
 新建边界组
 > 参数:  
 > name:边界组名  
 > index:边界组编号，默认自动识别当前编号 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_boundary_group(name="边界组1")
 ```  
 ### remove_boundary_group
 按照名称删除边界组
 > 参数:  
 > name: 边界组名称，默认删除所有边界组 (非必须参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_boundary_group()
 mdb.remove_boundary_group(name="边界组1")
 ```  
 ### remove_all_boundary
 根据边界组名称、边界的类型和编号删除边界信息,默认时删除所有边界信息
 > 参数:  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_all_boundary()
 ```  
 ### remove_boundary
 根据节点号删除边界一般支撑、弹性支承，根据单元号删除梁端约束、根据主节点号删除主从约束、根据从节点号删除约束方程
 > 参数:  
 > remove_id:节点号 or 单元号 or主节点号  or 从节点号  
 > bd_type:边界类型  1-一般支承 2-弹性支承 3-主从约束 4-弹性连接 5-约束方程 6-梁端约束  
 > group:边界所处边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_boundary(remove_id = 1, bd_type = 1,group="边界组1")
 ```  
 ### add_general_support
 添加一般支承
 > 参数:  
 > node_id:节点编号  
 > boundary_info:边界信息  [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名,默认为默认边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_general_support(node_id=1, boundary_info=[True,True,True,False,False,False])
 ```  
 ### add_elastic_support
 添加弹性支承
 > 参数:  
 > node_id:节点编号  
 > support_type:支承类型 1-线性  2-受拉  3-受压  
 > boundary_info:边界信息 受拉和受压时列表长度为1  线性时列表长度为6  
 > group_name:边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_elastic_support(node_d=1,support_type=1,boundary_info=[1e6,0,1e6,0,0,0])
 ```  
 ### add_master_slave_link
 添加主从约束
 > 参数:  
 > master_id:主节点号  
 > slave_id:从节点号  
 > boundary_info:边界信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_master_slave_link(master_id=1,slave_id=2,boundary_info=[True,True,True,False,False,False])
 ```  
 ### add_elastic_link
 添加弹性连接
 > 参数:  
 > link_type:节点类型   1-一般弹性连接 2-刚性连接 3-受拉弹性连接 4-受压弹性连接  
 > start_id:起始节点号  
 > end_id:终节点号  
 > beta_angle:贝塔角  
 > boundary_info:边界信息  
 > group_name:边界组名  
 > dis_ratio:距i端距离比 (仅一般弹性连接需要)  
 > kx:受拉或受压刚度  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_elastic_link(link_type=1,start_id=1,end_id=2,boundary_info=[1e6,1e6,1e6,0,0,0])
 mdb.add_elastic_link(link_type=2,start_id=1,end_id=2)
 mdb.add_elastic_link(link_type=3,start_id=1,end_id=2,kx=1e6)
 ```  
 ### add_beam_constraint
 添加梁端约束
 > 参数:  
 > beam_id:梁号  
 > info_i:i端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > info_j:j端约束信息 [X,Y,Z,Rx,Ry,Rz] ture-固定 false-自由  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_constraint(beam_id=2,info_i=[True,True,True,False,False,False],info_j=[True,True,True,False,False,False])
 ```  
 ### add_node_axis
 添加节点坐标
 > 参数:  
 > input_type:输入方式 1-角度 2-三点  3-向量  
 > node_id:节点号  
 > coord_info:局部坐标信息 -List<float>(角)  -List<List<float>>(三点 or 向量)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_axis(input_type=1,node_id=1,coord_info=[45,45,45])
 mdb.add_node_axis(input_type=2,node_id=1,coord_info=[[0,0,1],[0,1,0],[1,0,0]])
 mdb.add_node_axis(input_type=3,node_id=1,coord_info=[[0,0,1],[0,1,0]])
 ```  
 ##  移动荷载
 ### add_standard_vehicle
 添加标准车辆
@@ -421,128 +454,140 @@
 > 6-城市轨道交通桥梁规范(GB/T51234-2017)  
 > load_type: 荷载类型  
 > 支持类型: "公路I级","公路II级","城A车道","城B车道","地铁A型车","地铁B型车","地铁C型车","汽10"  
 > "汽15","汽20","汽超20","特载","挂80","挂100","挂120","公路疲劳荷载1","公路疲劳荷载2","公路疲劳荷载3",  
 > "汽36轻", "汽38重","高速铁路","城际铁路","客货共线铁路","重载铁路","中活载","长大货物车检算荷载"  
 > load_length: 默认为0即不限制荷载长度  (铁路桥涵规范 Q/CR 9300-2017 所需参数)  
 > n:车厢数: 默认6节车厢 (城市轨道交通桥梁规范 GB/T51234-2017 所需参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_standard_vehicle("高速铁路",standard_code=1,load_type="高速铁路")
 ```  
 ### add_node_tandem
 添加节点纵列
 > 参数:  
 > name:节点纵列名  
 > start_id:起始节点号  
 > node_ids:节点列表  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_tandem("节点纵列1",1,[i+1 for i in range(12)])
 ```  
 ### add_influence_plane
 添加影响面
 > 参数:  
 > name:影响面名称  
 > tandem_names:节点纵列名称组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_influence_plane("影响面1",["节点纵列1","节点纵列2"])
 ```  
 ### add_lane_line
 添加车道线
 > 参数:  
 > name:车道线名称  
 > influence_name:影响面名称  
 > tandem_name:节点纵列名  
 > offset:偏移  
 > lane_width:车道宽度  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_lane_line("车道1","影响面1","节点纵列1",offset=0,lane_width=3.1)
 ```  
 ### add_live_load_case
 添加移动荷载工况
 > 参数:  
 > name:荷载工况名  
 > influence_plane:影响线名  
 > span:跨度  
 > car_detail: 汽车相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > train_detail: 火车相关系数 (横向折减列表float[8],纵向折减系数,强度冲击,疲劳冲击)  
 > metro_detail: 轻轨相关系数 (横向折减列表float[8],纵向折减系数,冲击强度)  
 > sub_case:子工况信息 [(车辆名称,系数,["车道1","车道2"])...]  
-```Python  
+```Python
 # 示例代码
-mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[(“车辆名称”,1.0,["车道1","车道2"])...])
+from qtmodel import mdb
+mdb.add_live_load_case("活载工况1","影响面1",100,sub_case=[("车辆名称",1.0,["车道1","车道2"]),])
 ```  
 ### remove_vehicle
 删除车辆信息
 > 参数:  
 > index:车辆荷载编号  
 > name:车辆名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_vehicle(index=1)
 mdb.remove_vehicle(name="车辆名称")
 ```  
 ### remove_node_tandem
 按照 节点纵列编号/节点纵列名 删除节点纵列
 > 参数:  
 > index:节点纵列编号  
 > name:节点纵列名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_node_tandem(index=1)
 mdb.remove_node_tandem(name="节点纵列1")
 ```  
 ### remove_influence_plane
 按照 影响面编号/影响面名称 删除影响面
 > 参数:  
 > index:影响面编号  
 > name:影响面名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_influence_plane(index=1)
 mdb.remove_influence_plane(name="影响面1")
 ```  
 ### remove_lane_line
 按照 车道线编号/车道线名称 删除车道线
 > 参数:  
 > name:车道线名称  
 > index:车道线编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_lane_line(index=1)
 mdb.remove_lane_line(name="车道线1")
 ```  
 ### remove_live_load_case
 删除移动荷载工况
 > 参数:  
 > name:移动荷载工况名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_live_load_case(name="活载工况1")
 ```  
 ##  钢束操作
 ### add_tendon_group
 按照名称添加钢束组，添加时可指定钢束组id
 > 参数:  
 > name: 钢束组名称  
 > index: 钢束组编号(非必须参数)，默认自动识别  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_group(name="钢束组1")
 ```  
 ### remove_tendon_group
 按照钢束组名称或钢束组编号删除钢束组，两参数均为默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称,默认自动识别 (可选参数)  
 > index:钢束组编号,默认自动识别 (可选参数)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon_group(name="钢束组1")
 mdb.remove_tendon_group(index=1)
 ```  
 ### add_tendon_property
 添加钢束特性
 > 参数:  
 > name:钢束特性名  
@@ -550,16 +595,17 @@
 > tendon_type: 0-PRE 1-POST  
 > material_id: 钢材材料编号  
 > duct_type: 1-金属波纹管  2-塑料波纹管  3-铁皮管  4-钢管  5-抽芯成型  
 > steel_type: 1-钢绞线  2-螺纹钢筋  
 > steel_detail: 钢绞线[钢束面积,孔道直径,摩阻系数,偏差系数]  螺纹钢筋[钢筋直径,钢束面积,孔道直径,摩阻系数,偏差系数,张拉方式(1-一次张拉\2-超张拉)]  
 > loos_detail: 松弛信息[规范(1-公规 2-铁规),张拉(1-一次张拉 2-超张拉),松弛(1-一般松弛 2-低松弛)] (仅钢绞线需要,默认为[1,1,1])  
 > slip_info: 滑移信息[始端距离,末端距离] 默认为[0.006, 0.006]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_property(name="钢束1",tendon_type="先张",material_id=1,duct_type=1,steel_type=1,
 steel_detail=[0.00014,0.10,0.25,0.0015],loos_detail=[1,1,1])
 ```  
 ### add_tendon_3d
 添加三维钢束
 > 参数:  
 > name:钢束名称  
@@ -570,366 +616,402 @@
 > position_type: 定位方式 1-直线  2-轨迹线  
 > control_points: 控制点信息[(x1,y1,z1,r1),(x2,y2,z2,r2)....]  
 > point_insert: 定位方式为直线时为插入点坐标[x,y,z], 轨迹线时为 [插入端(1-I 2-J),插入方向(1-ij 2-ji),插入单元id]  
 > tendon_direction:直线钢束X方向向量 x轴-[1,0,0] y轴-[0,1,0]  默认为[1,0,0] (轨迹线不用赋值)  
 > rotation_angle:绕钢束旋转角度  
 > track_group:轨迹线结构组名  (直线时不用赋值)  
 > projection:直线钢束投影，默认为true  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=1,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(0,0,0))
 mdb.add_tendon_3d("BB1",property_name="22-15",num=2,position_type=2,
 control_points=[(0,0,-1,0),(10,0,-1,0)],point_insert=(1,1,1),track_group="轨迹线结构组1")
 ```  
 ### remove_tendon
 按照名称或编号删除钢束,默认时删除所有钢束
 > 参数:  
 > name:钢束名称  
 > index:钢束编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon(name="钢束1")
 mdb.remove_tendon(index=1)
 mdb.remove_tendon()
 ```  
 ### remove_tendon_property
 按照名称或编号删除钢束组,默认时删除所有钢束组
 > 参数:  
 > name:钢束组名称  
 > index:钢束组编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_tendon_property(name="钢束特性1")
 mdb.remove_tendon_property(index=1)
 mdb.remove_tendon_property()
 ```  
 ### add_nodal_mass
 添加节点质量
 > 参数:  
 > node_id:节点编号  
 > mass_info:[m,rmX,rmY,rmZ]  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodal_mass(node_id=1,mass_info=(100,0,0,0))
 ```  
 ### remove_nodal_mass
 删除节点质量
 > 参数:  
 > node_id:节点号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_nodal_mass(node_id=1)
 ```  
 ### add_pre_stress
 添加预应力
 > 参数:  
 > case_name:荷载工况名  
 > tendon_name:钢束名  
 > pre_type:预应力类型 0-始端 1-末端 2-两端  
 > force:预应力  
 > group_name:边界组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_pre_stress(case_name="荷载工况名",tendon_name="钢束1",force=1390000)
 ```  
 ### remove_pre_stress
 删除预应力
 > 参数:  
 > case_name:荷载工况  
 > tendon_name:钢束组  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_pre_stress(case_name="工况1",tendon_name="钢束1",group_name="默认荷载组")
 ```  
 ##  荷载操作
 ### add_load_group
 根据荷载组名称添加荷载组
 > 参数:  
 > name: 荷载组名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_group(name="荷载组1")
 ```  
 ### remove_load_group
 根据荷载组名称或荷载组id删除荷载组,参数为默认时删除所有荷载组
 > 参数:  
 > name: 荷载组名称  
 > index: 荷载组编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_load_group(name="荷载组1")
 mdb.remove_load_group(index="1")
 ```  
 ### add_nodal_force
 添加节点荷载
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_nodal_force(case_name="荷载工况1",node_id=1,load_info=(1,1,1,1,1,1),group_name="默认结构组")
 ```  
 ### remove_nodal_force
 删除节点荷载
 > 参数:  
 > case_name:荷载工况名  
 > node_id:节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_nodal_force(case_name="荷载工况1",node_id=1)
 ```  
 ### add_node_displacement
 添加节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
 > load_info:[Dx,Dy,Dz,Rx,Ry,Rz]  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_node_displacement(case_name="荷载工况1",node_id=1,load_info=(1,0,0,0,0,0),group_name="默认荷载组")
 ```  
 ### remove_nodal_displacement
 删除节点位移
 > 参数:  
 > node_id:节点编号  
 > case_name:荷载工况名  
-```Python  
+```Python
 # 示例代码
-mdn.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
+from qtmodel import mdb
+mdb.remove_nodal_displacement(case_name="荷载工况1",node_id=1)
 ```  
 ### add_beam_load
 添加梁单元荷载
 > 参数:  
 > beam_id:单元编号  
 > case_name:荷载工况名  
 > load_type:荷载类型 1-集中荷载 2-集中弯矩 3-均布荷载 4-均布弯矩 5-梯形荷载 6-梯形弯矩  
 > coord_system:坐标系 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z  
 > list_x:荷载位置信息 ,荷载距离单元I端的相对距离  
 > list_load:荷载数值信息  
 > uniform_load:均布荷载值  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=1,list_x=[0.1,0.5,0.8],list_load=[100,100,100])
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=3,list_x=[0,1],uniform_load=100)
 mdb.add_beam_load(case_name="荷载工况1",beam_id=1,load_type=5,list_x=[0.4,0.8],list_load=[100,200])
 ```  
 ### remove_beam_load
 删除梁单元荷载
 > 参数:  
 > element_id:单元号  
 > case_name:荷载工况名  
 > load_type:荷载类型 1-集中力   2-集中弯矩  3-分布力   4-分布弯矩  
 > group_name:边界组名  
-```Python  
+```Python
 # 示例代码
-mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1，group_name="默认荷载组")
+from qtmodel import mdb
+mdb.remove_beam_load(case_name="工况1",element_id=1,load_type=1,group_name="默认荷载组")
 ```  
 ### add_initial_tension
 添加初始拉力
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > tension:初始拉力  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_initial_tension(element_id=1,case_name="工况1",tension=100,tension_type=1)
 ```  
 ### add_cable_length_load
 添加索长张拉
 > 参数:  
 > element_id:单元类型  
 > case_name:荷载工况名  
 > length:长度  
 > tension_type:张拉类型  1-全量   2-增量  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_cable_length_load(element_id=1,case_name="工况1",length=1,tension_type=1)
 ```  
 ### add_plate_element_load
 添加版单元荷载
 > 参数:  
 > element_id:单元id  
 > case_name:荷载工况名  
 > load_type:荷载类型   1-集中力  2-集中弯矩  3-分布力  4-分布弯矩  
 > load_place:荷载位置  0-面IJKL 1-边IJ  2-边JK  3-边KL  4-边LI  (仅分布荷载需要)  
 > coord_system:坐标系  (默认3) 1-整体坐标X  2-整体坐标Y 3-整体坐标Z  4-局部坐标X  5-局部坐标Y  6-局部坐标Z  
 > group_name:荷载组名  
 > load_list:荷载列表  
 > xy_list:荷载位置信息 [IJ方向距离x,IL方向距离y]  (仅集中荷载需要,x,y代表荷载距离板单元I端的绝对值)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_plate_element_load(element_id=1,case_name="工况1",load_type=1,group_name="默认荷载组",load_list=[1000],xy_list=[0.2,0.5])
 ```  
 ### add_deviation_parameter
 添加制造误差
 > 参数:  
 > name:名称  
 > element_type:单元类型  1-梁单元  2-板单元  
 > parameters:参数列表  
 > 梁杆单元:[轴向,I端X向转角,I端Y向转角,I端Z向转角,J端X向转角,J端Y向转角,J端Z向转角]  
 > 板单元:[X向位移,Y向位移,Z向位移,X向转角,Y向转角]  
-```Python  
+```Python
 # 示例代码
-mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameterInfo=parameters)
+from qtmodel import mdb
+mdb.add_deviation_parameter(name="梁端制造误差",elementType=1,parameters=[1,0,0,0,0,0,0])
+mdb.add_deviation_parameter(name="板端制造误差",elementType=1,parameters=[1,0,0,0,0])
 ```  
 ### add_deviation_load
 添加制造误差荷载
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > parameters:参数名列表 梁杆单元时-[制造误差参数名称]   板单元时-[I端误差名,J端误差名,K端误差名,L端误差名]  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
-mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=[“梁端误差”])
-mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=[“板端误差1”,"板端误差2","板端误差3","板端误差4"])
+from qtmodel import mdb
+mdb.add_deviation_load(element_id=1,case_name="工况1",parameters=["梁端误差"])
+mdb.add_deviation_load(element_id=2,case_name="工况1",parameters=["板端误差1","板端误差2","板端误差3","板端误差4"])
 ```  
 ### add_element_temperature
 添加单元温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:最终温度  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_element_temperature(element_id=1,case_name="自重",temperature=1,group_name="默认荷载组")
 ```  
 ### add_gradient_temperature
 添加梯度温度
-```Python  
+```Python
 # 示例代码
-mdb.add_gradient_temperature(elementId=1,caseName=“荷载工况1”,groupName=“荷载组名1,temperature=10)
-mdb.add_gradient_temperature(elementId=2,caseName=“荷载工况2”,groupName=”荷载组名2“,temperature=10,element_type=2)
+from qtmodel import mdb
+mdb.add_gradient_temperature(elementId=1,caseName="荷载工况1",groupName="荷载组名1",temperature=10)
+mdb.add_gradient_temperature(elementId=2,caseName="荷载工况2",groupName="荷载组名2",temperature=10,element_type=2)
 ```  
 ### add_beam_section_temperature
 添加梁截面温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > paving_thick:铺设厚度(m)  
 > temperature_type:温度类型  1-升温(默认) 2-降温  
 > paving_type:铺设类型     1-沥青混凝土(默认)  2-水泥混凝土  
 > group_name:荷载组名  
 > modify:是否修改规范温度  
 > temp_list:温度列表[T1,T2]  (仅修改时需要)  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_beam_section_temperature(element_id=1,case_name="工况1",paving_thick=0.1)
 ```  
 ### add_index_temperature
 添加指数温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载工况名  
 > temperature:温差  
 > index:指数  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_index_temperature(element_id=1,case_name="工况1",temperature=20,index=2)
 ```  
 ### add_top_plate_temperature
 添加顶板温度
 > 参数:  
 > element_id:单元编号  
 > case_name:荷载  
 > temperature:最终温度  
 > group_name:荷载组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_top_plate_temperature(element_id=1,case_name="工况1",temperature=40,group_name="默认荷载组")
 ```  
 ##  沉降操作
 ### add_sink_group
 添加沉降组
 > 参数:  
 > name: 沉降组名  
 > sink: 沉降值  
 > node_ids: 节点编号  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_sink_group(name="沉降1",sink=0.1,node_ids=[1,2,3])
 ```  
 ### remove_sink_group
 按照名称删除沉降组
 > 参数:  
 > name:沉降组名,默认删除所有沉降组  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_sink_group()
 mdb.remove_sink_group(name="沉降1")
 ```  
 ### add_sink_case
 添加沉降工况
 > 参数:  
 > name:荷载工况名  
 > sink_groups:沉降组名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_sink_case(name="沉降工况1",sink_groups=["沉降1","沉降2"])
 ```  
 ### remove_sink_case
 按照名称删除沉降工况,不输入名称时默认删除所有沉降工况
 > 参数:  
 > name:沉降工况名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_sink_case()
 mdb.remove_sink_case(name="沉降1")
 ```  
 ### add_concurrent_reaction
 添加并发反力组
 > 参数:  
 > names: 结构组名称集合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_concurrent_reaction(["默认结构组"])
 ```  
 ### remove_concurrent_reaction
 删除所有并发反力组
 > 参数:  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_concurrent_reaction()
 ```  
 ### add_concurrent_force
 创建并发内力组
 > 参数:  
 > names: 结构组名称集合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_concurrent_force(["默认结构组"])
 ```  
 ### remove_concurrent_force
 删除所有并发内力组
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_concurrent_force()
 ```  
 ### add_load_case
 添加荷载工况
 > 参数:  
 > name:沉降名  
 > case_type:荷载工况类型  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_case(name="工况1",case_type=1)
 ```  
 ### remove_load_case
 删除荷载工况,参数均为默认时删除全部荷载工况
 > 参数:  
 > index:荷载编号  
 > name:荷载名  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_case(index=1)
 mdb.add_load_case(name="工况1")
 mdb.add_load_case()
 ```  
 ### test_print
 测试运行
 ##  施工阶段和荷载组合
@@ -947,17 +1029,18 @@
 > delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]  
 > active_loads:激活荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > delete_loads:钝化荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
 > index:施工阶段编号，默认自动添加  
-```Python  
+```Python
 # 示例代码
-mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+from qtmodel import mdb
+mdb.add_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
 ### update_construction_stage
 添加施工阶段信息
 > 参数:  
 > name:施工阶段信息  
 > duration:时长  
@@ -969,54 +1052,59 @@
 > 位置:  0-变形前 1-变形后  
 > delete_boundaries:钝化边界组信息 [边界组1，结构组2,...]  
 > active_loads:激活荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > delete_loads:钝化荷载组信息 [(荷载组1,时间),...]  
 > 时间: 0-开始 1-结束  
 > temp_loads:临时荷载信息 [荷载组1，荷载组2,..]  
-```Python  
+```Python
 # 示例代码
-mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[(“结构组1”,5,1,1),(“结构组2”,5,1,1)],
+from qtmodel import mdb
+mdb.update_construction_stage(name="施工阶段1",duration=5,active_structures=[("结构组1",5,1,1),("结构组2",5,1,1)],
 active_boundaries=[("默认边界组",1)],active_loads=[("默认荷载组1",0)])
 ```  
 ### update_weight_stage
 添加施工阶段信息
 > 参数:  
 > stage_name:施工阶段信息  
 > structure_group_name:结构组名  
 > weight_stage_id: 计自重阶段号: 0-不计自重,1-本阶段 n-第n阶段  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.update_weight_stage(stage_name="施工阶段1",structure_group_name="默认结构组",weight_stage_id=1)
 ```  
 ### remove_construction_stage
 按照施工阶段名删除施工阶段,默认删除所有施工阶段
 > 参数:  
 > name:所删除施工阶段名称  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_construction_stage(name="施工阶段1")
 ```  
 ### add_load_combine
 添加荷载组合
 > 参数:  
 > name:荷载组合名  
 > combine_type:荷载组合类型 1-叠加  2-判别  3-包络  
 > describe:描述  
 > combine_info:荷载组合信息 [(荷载工况类型,工况名,系数)...]  
 > 荷载工况类型: "ST"-静力荷载工况  "CS"-施工阶段荷载工况  "CB"-荷载组合  
 > "MV"-移动荷载工况  "SM"-沉降荷载工况  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.add_load_combine(name="荷载组合1",combine_type=1,describe="无",combine_info=[("CS","合计值",1),("CS","恒载",1)])
 ```  
 ### remove_load_combine
 删除荷载组合
 > 参数:  
 > name:指定删除荷载组合名，默认时则删除所有荷载组合  
-```Python  
+```Python
 # 示例代码
+from qtmodel import mdb
 mdb.remove_load_combine(name="荷载组合1")
 ```
```

### Comparing `qtmodel-0.2.3/setup.py` & `qtmodel-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # 读取文件内容
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="qtmodel",
-    version="0.2.3",
+    version="0.2.4",
     author="dqy-zhj",
     author_email="1105417715@qq.com",
     description="python modeling for qt",
     long_description=long_description,  # 使用读取的 README.md 文件内容
     long_description_content_type="text/markdown",  # 指明内容格式为markdown
     url="https://github.com/Inface0443/pyqt",
     packages=find_packages(),
```

