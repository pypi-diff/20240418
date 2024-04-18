# Comparing `tmp/brickagx-0.6.1-cp39-cp39-win_amd64.whl.zip` & `tmp/brickagx-0.6.2-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8634237 bytes, number of entries: 35
+Zip file size: 8631650 bytes, number of entries: 35
 -rw-r--r--  2.0 fat     1458 b- defN 80-Jan-01 00:00 rebrick/__init__.py
--rw-r--r--  2.0 fat  5349376 b- defN 80-Jan-01 00:00 rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd
+-rw-r--r--  2.0 fat  5330944 b- defN 80-Jan-01 00:00 rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  1504768 b- defN 80-Jan-01 00:00 rebrick/_CorePythonSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  2526208 b- defN 80-Jan-01 00:00 rebrick/_DriveTrainSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  1246208 b- defN 80-Jan-01 00:00 rebrick/_MathSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  2137600 b- defN 80-Jan-01 00:00 rebrick/_Physics1DSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat 11220992 b- defN 80-Jan-01 00:00 rebrick/_Physics3DSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  7019008 b- defN 80-Jan-01 00:00 rebrick/_PhysicsSwig.cp39-win_amd64.pyd
 -rw-r--r--  2.0 fat  5448704 b- defN 80-Jan-01 00:00 rebrick/_RoboticsSwig.cp39-win_amd64.pyd
@@ -26,12 +26,12 @@
 -rw-r--r--  2.0 fat  2295209 b- defN 80-Jan-01 00:00 rebrick/Physics3D.py
 -rw-r--r--  2.0 fat   938547 b- defN 80-Jan-01 00:00 rebrick/Robotics.py
 -rw-r--r--  2.0 fat    46727 b- defN 80-Jan-01 00:00 rebrick/Simulation.py
 -rw-r--r--  2.0 fat    41484 b- defN 80-Jan-01 00:00 rebrick/Terrain.py
 -rw-r--r--  2.0 fat    23897 b- defN 80-Jan-01 00:00 rebrick/Urdf.py
 -rw-r--r--  2.0 fat   451249 b- defN 80-Jan-01 00:00 rebrick/Vehicles.py
 -rw-r--r--  2.0 fat   146491 b- defN 80-Jan-01 00:00 rebrick/Visuals.py
--rw-r--r--  2.0 fat      159 b- defN 80-Jan-01 00:00 brickagx-0.6.1.dist-info/entry_points.txt
--rw-r--r--  2.0 fat     7834 b- defN 80-Jan-01 00:00 brickagx-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 fat       96 b- defN 80-Jan-01 00:00 brickagx-0.6.1.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2989 b- defN 16-Jan-01 00:00 brickagx-0.6.1.dist-info/RECORD
-35 files, 48936852 bytes uncompressed, 8629573 bytes compressed:  82.4%
+?rw-r--r--  2.0 fat      159 b- defN 16-Jan-01 00:00 brickagx-0.6.2.dist-info/entry_points.txt
+?rw-r--r--  2.0 fat       96 b- defN 16-Jan-01 00:00 brickagx-0.6.2.dist-info/WHEEL
+?rw-r--r--  2.0 fat     7732 b- defN 16-Jan-01 00:00 brickagx-0.6.2.dist-info/METADATA
+?rw-r--r--  2.0 fat     2989 b- defN 16-Jan-01 00:00 brickagx-0.6.2.dist-info/RECORD
+35 files, 48918318 bytes uncompressed, 8626986 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -87,20 +87,20 @@
 
 Filename: rebrick/Vehicles.py
 Comment: 
 
 Filename: rebrick/Visuals.py
 Comment: 
 
-Filename: brickagx-0.6.1.dist-info/entry_points.txt
+Filename: brickagx-0.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: brickagx-0.6.1.dist-info/METADATA
+Filename: brickagx-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: brickagx-0.6.1.dist-info/WHEEL
+Filename: brickagx-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: brickagx-0.6.1.dist-info/RECORD
+Filename: brickagx-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rebrick/__init__.py

```diff
@@ -1,10 +1,10 @@
 import os
 __AGXVERSION__ = "2.37.3.2"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 try:
     import agx
     if agx.__version__ != __AGXVERSION__:
         print(f"This version of brickagx is compiled for AGX {__AGXVERSION__} only and may crash with your {agx.__version__} version, upgrade brickagx or AGX to make sure the versions are suited for eachother")
 except:
     print("Failed finding AGX Dynamics, have you run setup_env?")
     exit(255)
```

## Comparing `brickagx-0.6.1.dist-info/METADATA` & `brickagx-0.6.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
-Name: BrickAgx
-Version: 0.6.1
+Name: brickagx
+Version: 0.6.2
 Summary: Brick.AGX python interface development
 Home-page: https://pub.algoryx.dev/brick/
 License: Apache 2.0
 Author: Algoryx
 Author-email: algoryx@algoryx.com
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: agx (==2.37.3.2)
-Requires-Dist: brickbundles (>=0.6.1,<0.7.0)
+Requires-Dist: brickbundles (>=0.6.2,<0.7.0)
 Requires-Dist: pclick (>=0.3.1,<0.4.0)
 Description-Content-Type: text/markdown
 
 # BRICK AGX
 
 The brickagx package implements all Brick bundles such as Physics, Robotics, DriveTrain and Simulation using [AGX Dynamics Real-time multi-body simulation](https://www.algoryx.se/agx-dynamics/).
 The package contains python bindings and native libraries needed to load and run .brick files.
```

## Comparing `brickagx-0.6.1.dist-info/RECORD` & `brickagx-0.6.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-rebrick/__init__.py,sha256=aXSH4EyGGe4ZMIHILdINhqrLnYr5SLCCH1iIv_h--yQ,1458
-rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd,sha256=jTRaNGyxNKAPNmVHNRkFcGsz50WmkbZ8TFY0M12h-Wk,5349376
-rebrick/_CorePythonSwig.cp39-win_amd64.pyd,sha256=AITHS6jE96Ei018AIAab9e95R6thELGkwHRp7gAn1BE,1504768
-rebrick/_DriveTrainSwig.cp39-win_amd64.pyd,sha256=Sbm2qWB0Sk2KNJ1gIUAMRHWLTtI-q9ehowMiB28dtu0,2526208
-rebrick/_MathSwig.cp39-win_amd64.pyd,sha256=x8ScAhPsHwhJeQuO6oP8VRu97nsZDKPmOWdScJqwrAo,1246208
-rebrick/_Physics1DSwig.cp39-win_amd64.pyd,sha256=BP4p4fZ1zGG5kLBfCvbEM8k-Vr-8om7qrMpp3yJ_wc4,2137600
-rebrick/_Physics3DSwig.cp39-win_amd64.pyd,sha256=xDxwHc3bTWfK7BiILzlANgvhiLoYj-Jx1FX1s0_TFNU,11220992
-rebrick/_PhysicsSwig.cp39-win_amd64.pyd,sha256=xNrgibQEMDYO0JlA-Gh_uJqkvOjAlk8gHXdsh6LvC1o,7019008
-rebrick/_RoboticsSwig.cp39-win_amd64.pyd,sha256=P0aQK_1jT7qzBygzqBWJOQZxBt5bM5bC8Gjjb-xZdDg,5448704
-rebrick/_SimulationSwig.cp39-win_amd64.pyd,sha256=w7d3WXP9DSjN1udcnOHpfTJQuZGmjH6sxqCZD-y8BX4,704512
-rebrick/_TerrainSwig.cp39-win_amd64.pyd,sha256=ysnPhckMPzrwwvW2OCvui4opNY2tzA4zs06VF6Aqdgo,728576
-rebrick/_UrdfSwig.cp39-win_amd64.pyd,sha256=Z4ia_9hAp6T0angh_1RBfhWIMJRYu_WaQoNoPpSRTH4,631296
-rebrick/_VehiclesSwig.cp39-win_amd64.pyd,sha256=GaaoO5p1fUkniZkeNYTVquEQPWZFqFWatzI_RlSFvRo,2862080
-rebrick/_VisualsSwig.cp39-win_amd64.pyd,sha256=WlxgVxF_uE7z3pzgnVVzvjD3zGgdchg_YGwmf4SoThw,997376
+rebrick/__init__.py,sha256=MhLOOz_dzYTxJio932lGppjSveBktTXwOZI4Xlc6-tc,1458
+rebrick/_BrickAgxPyApi.cp39-win_amd64.pyd,sha256=C0dypor_dm5MnU_mNFNCAkLSZy3UAqQKmT0EaaTJSVs,5330944
+rebrick/_CorePythonSwig.cp39-win_amd64.pyd,sha256=ujZDUkEbo1pQmhBy9eAnSX85PB3IR9aAFq9XsUIDhDM,1504768
+rebrick/_DriveTrainSwig.cp39-win_amd64.pyd,sha256=l081I68if_YKe6YPR1zOaKY4i3Hr1yJ9Dj503nlbidU,2526208
+rebrick/_MathSwig.cp39-win_amd64.pyd,sha256=bWmFBdmWpOAH5JQhodCbq1UHa2BSxo3q4OsiBGTP9V8,1246208
+rebrick/_Physics1DSwig.cp39-win_amd64.pyd,sha256=3sUCSJytQ8zRZFzeRpKYbEJNd3rhsR4JjOMUKvIBkFE,2137600
+rebrick/_Physics3DSwig.cp39-win_amd64.pyd,sha256=ITBNJI3A_rK8tQu8_sugmRzWgKMJmvT2iHN2COZeaHo,11220992
+rebrick/_PhysicsSwig.cp39-win_amd64.pyd,sha256=fDGZZk4itKiNBnHQLKxkJSDRJ9k-qvdo66x3LSAfsZY,7019008
+rebrick/_RoboticsSwig.cp39-win_amd64.pyd,sha256=kbzNRPpxnUDUJhp9212t8g1j1DGuiTaaby-8dhmF5YI,5448704
+rebrick/_SimulationSwig.cp39-win_amd64.pyd,sha256=3CXlhI4T064T6aUOtkmo3gSAo2bWpMLqM943HNbACqA,704512
+rebrick/_TerrainSwig.cp39-win_amd64.pyd,sha256=XnTSCQt3eNRwOvzvL4uIdc74Xuxxig0UuATdWKUydno,728576
+rebrick/_UrdfSwig.cp39-win_amd64.pyd,sha256=nhuXo3cWvw3em863ogoD0hOR8w4uR7oeKRaPpXETLZE,631296
+rebrick/_VehiclesSwig.cp39-win_amd64.pyd,sha256=4ZoBo4xHgl9WvwRtMf7_9QM8becMnz_vRk5OTJLoe-0,2862080
+rebrick/_VisualsSwig.cp39-win_amd64.pyd,sha256=_J9vpcDPco0wmhtqBAGAr65mti7iNvcvwHCtyDFE268,997376
 rebrick/agxtobrick.py,sha256=ww7fV5G2M5gABgE8jdaUdDqxKT9VhBAnRSzUOGFRLM4,2212
 rebrick/anytobrick.py,sha256=mZ8zVvHTRjgg-dMriwsSAunH6rfc3FYKvKdW2CvA8f4,2264
 rebrick/api.py,sha256=bGYD0yIQVIfrmQmMukRT2MpQyNcIr6VQPOPEBGGh2Zc,39756
 rebrick/brickvalidate.py,sha256=mDRvBgYbQGiuh_YW4mxcCMg4nuAuo8Wb1lOwuvdf_wo,2013
 rebrick/brickview.py,sha256=PV-9zQnyUe_1CYOLe_bpX_xUtDlX9vlk3lRBlvNbSSU,5270
 rebrick/Core.py,sha256=HG5JzjuU75zRkbQoxnjDLpVHP6-QJplcP-UHZ4ybrn4,133079
 rebrick/DriveTrain.py,sha256=WTnbCvIVDErntjw-GqO4og2CsIm7jBu99hzB8bMKhgc,414656
@@ -25,11 +25,11 @@
 rebrick/Physics3D.py,sha256=FVduDB1lg3a7fepgRDO6lpaZXHGyhYGHXCZUpa0ZD-w,2295209
 rebrick/Robotics.py,sha256=94JwLNEF0sqjy2FWp-6Qui_O3dAMPuIwbBHVyVJn9nY,938547
 rebrick/Simulation.py,sha256=W613zVuHLbrwPeXjEttuOkyNShpD87qLnFL_Ufb2gE4,46727
 rebrick/Terrain.py,sha256=dO2rCRzw3F69T0-zF4zfbe4VE9yToiyeIkitwy7UIkY,41484
 rebrick/Urdf.py,sha256=Ze5Cq7gYUOclnhJoYP_h1owN4hJLONLWZmDXJ_k_o2g,23897
 rebrick/Vehicles.py,sha256=WTDFgjBU90y5wtj9oR4Obujnb4H1fc0kup9pYNJ6_XM,451249
 rebrick/Visuals.py,sha256=bDAB3cMVA4otGy1XZRreOW_u6g5LwAFxVhT1rDiVeqQ,146491
-brickagx-0.6.1.dist-info/entry_points.txt,sha256=8dPzLXD5RkYUaPkiAcnDTgJ0LO8XkcKz5bP51VVPIjs,159
-brickagx-0.6.1.dist-info/METADATA,sha256=Vcanr56ivqYljFop94F_RC4yrnQQGo490f8KO7Doy5I,7834
-brickagx-0.6.1.dist-info/WHEEL,sha256=T7hzPzFWHJiWCVylm2UCj5payilA7ulisMC0IiBEe3o,96
-brickagx-0.6.1.dist-info/RECORD,,
+brickagx-0.6.2.dist-info/entry_points.txt,sha256=8dPzLXD5RkYUaPkiAcnDTgJ0LO8XkcKz5bP51VVPIjs,159
+brickagx-0.6.2.dist-info/WHEEL,sha256=kYdP1dg9l3e6xn0Rrij_x3k9CDJtdYnYq9HLT1afyLE,96
+brickagx-0.6.2.dist-info/METADATA,sha256=9Dd5v9Gk3gNabkDuOZRk3m43vFdCkgxLh4sis4qTRlg,7732
+brickagx-0.6.2.dist-info/RECORD,,
```

