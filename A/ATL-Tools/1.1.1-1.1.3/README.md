# Comparing `tmp/atl_tools-1.1.1.tar.gz` & `tmp/atl_tools-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.1.1.tar", last modified: Tue Apr 16 13:51:32 2024, max compression
+gzip compressed data, was "atl_tools-1.1.3.tar", last modified: Thu Apr 18 10:35:35 2024, max compression
```

## Comparing `atl_tools-1.1.1.tar` & `atl_tools-1.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 13:51:32.977479 atl_tools-1.1.1/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 13:51:32.973479 atl_tools-1.1.1/ATL_Tools/
--rw-rw-r--   0 atl       (1002) atl       (1002)    27993 2024-04-16 13:47:51.000000 atl_tools-1.1.1/ATL_Tools/ATL_gdal.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.1/ATL_Tools/ATL_path.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.1/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-16 13:51:32.973479 atl_tools-1.1.1/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     4392 2024-04-16 13:51:32.000000 atl_tools-1.1.1/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-16 13:51:32.000000 atl_tools-1.1.1/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-16 13:51:32.000000 atl_tools-1.1.1/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-16 13:51:32.000000 atl_tools-1.1.1/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     4392 2024-04-16 13:51:32.977479 atl_tools-1.1.1/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)     4093 2024-04-16 13:48:48.000000 atl_tools-1.1.1/README.md
--rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-04-16 13:49:27.000000 atl_tools-1.1.1/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-16 13:51:32.977479 atl_tools-1.1.1/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-18 10:35:35.449017 atl_tools-1.1.3/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-18 10:35:35.445017 atl_tools-1.1.3/ATL_Tools/
+-rw-rw-r--   0 atl       (1002) atl       (1002)    28826 2024-04-18 10:32:41.000000 atl_tools-1.1.3/ATL_Tools/ATL_gdal.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.3/ATL_Tools/ATL_path.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.3/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-18 10:35:35.449017 atl_tools-1.1.3/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     4545 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     4545 2024-04-18 10:35:35.449017 atl_tools-1.1.3/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4247 2024-04-18 10:34:04.000000 atl_tools-1.1.3/README.md
+-rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-04-18 10:33:27.000000 atl_tools-1.1.3/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-18 10:35:35.449017 atl_tools-1.1.3/setup.cfg
```

### Comparing `atl_tools-1.1.1/ATL_Tools/ATL_gdal.py` & `atl_tools-1.1.3/ATL_Tools/ATL_gdal.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,16 @@
     b = np.array([x - trans[0], y - trans[3]])
     
     return np.linalg.solve(a, b)
     
 def Mosaic_all_imgs(img_file_path: str,
                     output_path: str,
                     add_alpha_chan: bool=False,
-                    nan_or_zero: str='zero') -> None:
+                    nan_or_zero: str='zero',
+                    output_band_chan: int=1) -> None:
     
     '''✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
         细节测试:
         mosaic图像：
         ✔ 镶嵌根据矢量裁切后的图像，无数据区域为nan
         ✔ 镶嵌矩形的图像，无数据区域为nan
         mosaic标签：
@@ -277,14 +278,15 @@
     
     Args:
         img_file_path (str)：tif 影像存放路径
         output_path (str): 输出镶嵌后 tif 的路径
         add_alpha_chan (bool): 是否添加alpha通道，将无数据区域显示为空白，默认为False
         Nan_or_Zero (str): 'nan'或'zero'镶嵌后的无效数据nan或0,默认为0
                            'nan'更适合显示，'0更适合训练'
+        output_band_chan (int): 对于多光谱图像，如果只想保存前3个通道的话，指定通道数
         
         例子: Mosaic_all_imgs(img_path_all, output_path, add_alpha_chan=True) # 对于RGB标签，添加alpha通道
               Mosaic_all_imgs(img_path_all, output_path, Nan_or_Zero='zero') # 对于float32 img，mosaic为zero
               Mosaic_all_imgs(img_path_all, output_path, Nan_or_Zero='zero') # 对于float32 img，mosaic为nan #展示用
 
     Returns: 
         镶嵌合成的整体影像
@@ -324,21 +326,26 @@
 
     width_geo_resolution=geotrans[1]
     heigh_geo_resolution=geotrans[5]
     # print(f'width_geo_resolution:{width_geo_resolution}, heigh_geo_resolution:{heigh_geo_resolution}')
 
     columns=math.ceil((max_x-min_x)/width_geo_resolution) 
     rows=math.ceil((max_y-min_y)/(-heigh_geo_resolution))
-    bands = in_ds.RasterCount
+    
+    bands = in_ds.RasterCount  # 读进来的bands
+    if not output_band_chan==None:
+        bands = output_band_chan
+        print("  【ATL-LOG】人为指定输出波段数为:", bands)
     print(f'新合并图像的尺寸: {rows, columns, bands}')
 
     in_band_DataType = in_ds.GetRasterBand(1).DataType
 
     driver=gdal.GetDriverByName('GTiff')
-    out_ds=driver.Create(output_path, columns, rows, bands, in_band_DataType)
+    # out_ds=driver.Create(output_path, columns, rows, bands, in_band_DataType)
+    out_ds=driver.Create(output_path, columns, rows, 3, in_band_DataType)
     out_ds.SetProjection(in_ds.GetProjection())
     geotrans[0] = min_x
     geotrans[3] = max_y
     out_ds.SetGeoTransform(geotrans)
 
 
     #定义仿射逆变换
@@ -387,19 +394,28 @@
     if nan_or_zero=='zero' and add_alpha_chan==False:
         print(f"  【ATL-LOG】空缺部分为'zero', 不添加alpha通道, 支持float32-img、uint8-label")
         pass
     # 最后把所有为0.的地方都变成nan
     # 如果是float32图像的话,nan是可以work的,则会让无数据的地方变成nan,显示的时候就是透明的
     elif nan_or_zero=='nan' and add_alpha_chan==False:
         print(f"  【ATL-LOG】空缺部分为'nan', 不添加alpha通道,支持-float32img")
-        for band_num in range(bands):
-            out_band = out_ds.GetRasterBand(band_num + 1)
-            big_out_band_nan = out_band.ReadAsArray()
-            big_out_band_nan[big_out_band_nan==0.] = np.nan
-            out_band.WriteArray(big_out_band_nan)
+        output_img_ds = gdal.Open(output_path)
+        Transform = output_img_ds.GetGeoTransform()
+        Projection = output_img_ds.GetProjection()
+        
+        img_nan = output_img_ds.ReadAsArray()
+        img_nan = img_nan.transpose(1,2,0)
+        img_nan[img_nan==0.] = np.nan
+
+        save_array_to_tif(img_array = img_nan,
+                          out_path = output_path, # 覆盖图像
+                          Transform = Transform,
+                          Projection = Projection,
+                          Datatype = output_img_ds.GetRasterBand(1).DataType,
+                          Band = bands)
 
     # 如果创建的图像是uint8的话，nan是不行的，只能用0,添加alpha通道
     elif add_alpha_chan==True:
         print(f"  【ATL-LOG】添加alpha通道,支持uint8-rgb-img uint8-RGB-label")
         output_img_ds = gdal.Open(output_path)
         Transform = output_img_ds.GetGeoTransform()
         Projection = output_img_ds.GetProjection()
@@ -417,15 +433,16 @@
 
         alpha_image_array = cv2.merge((output_img, alpha_posi_array))
         # 保存带有Alpha通道的图像
         save_array_to_tif(img_array = alpha_image_array,
                           out_path = output_path, # 覆盖图像
                           Transform = Transform,
                           Projection = Projection,
-                          Datatype = 1)
+                          Datatype = output_img_ds.GetRasterBand(1).DataType,
+                          Band = bands)
 
     else:
         print(f'--> 暂不支持此数据组合的合Mosaic')
         print(f'--> 如数据为 float32, 请使用 nan_or_zero="nan"/"zero", add_alpha_chan=False')
         print(f'--> 如数据为 uint8 RGB, 请使用 nan_or_zero="nan"/"zero", add_alpha_chan=True/False')
```

### Comparing `atl_tools-1.1.1/ATL_Tools/ATL_path.py` & `atl_tools-1.1.3/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.1/ATL_Tools/__init__.py` & `atl_tools-1.1.3/ATL_Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.1/ATL_Tools.egg-info/PKG-INFO` & `atl_tools-1.1.3/ATL_Tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.1
+Version: 1.1.3
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 0. 简介
@@ -83,7 +83,9 @@
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
+- 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
+- 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
```

### Comparing `atl_tools-1.1.1/PKG-INFO` & `atl_tools-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.1
+Version: 1.1.3
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 0. 简介
@@ -83,7 +83,9 @@
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
+- 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
+- 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
```

### Comparing `atl_tools-1.1.1/README.md` & `atl_tools-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,8 +74,10 @@
 - 2023-12-06 v1.0.2 修复README中显示问题。
 - 2023-12-06 v1.0.3 修改项目名称为ATL_Tools。
 - 2024-04-03 v1.0.6 增加ATL_gdal模块，用于处理遥感影像。
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
-- 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
+- 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
+- 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
+- 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
```

