# Comparing `tmp/aistudio_sdk-0.2.2-py3-none-any.whl.zip` & `tmp/aistudio_sdk-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 27592 bytes, number of entries: 23
+Zip file size: 27542 bytes, number of entries: 23
 -rw-r--r--  2.0 unx      534 b- defN 24-Mar-26 11:53 aistudio_sdk/__init__.py
 -rw-r--r--  2.0 unx     4896 b- defN 24-Apr-09 06:54 aistudio_sdk/cmdline.py
 -rw-r--r--  2.0 unx     1389 b- defN 24-Apr-16 12:50 aistudio_sdk/config.py
--rw-r--r--  2.0 unx    25051 b- defN 24-Apr-16 12:40 aistudio_sdk/hub.py
+-rw-r--r--  2.0 unx    25057 b- defN 24-Apr-18 07:28 aistudio_sdk/hub.py
 -rw-r--r--  2.0 unx     1898 b- defN 24-Mar-27 05:51 aistudio_sdk/log.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 08:07 aistudio_sdk/constant/__init__.py
 -rw-r--r--  2.0 unx      626 b- defN 24-Mar-27 05:41 aistudio_sdk/constant/const.py
 -rw-r--r--  2.0 unx     2388 b- defN 24-Apr-16 12:39 aistudio_sdk/constant/err_code.py
--rw-r--r--  2.0 unx      387 b- defN 24-Apr-16 12:51 aistudio_sdk/constant/version.py
+-rw-r--r--  2.0 unx      387 b- defN 24-Apr-18 07:28 aistudio_sdk/constant/version.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 08:07 aistudio_sdk/requests/__init__.py
 -rw-r--r--  2.0 unx    16394 b- defN 24-Apr-16 12:36 aistudio_sdk/requests/hub.py
 -rw-r--r--  2.0 unx     5201 b- defN 24-Apr-08 09:04 aistudio_sdk/requests/pipeline.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Mar-02 07:06 aistudio_sdk/sdk/__init__.py
 -rw-r--r--  2.0 unx    12521 b- defN 24-Mar-28 07:00 aistudio_sdk/sdk/pipeline.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 08:07 aistudio_sdk/tests/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-02 08:07 aistudio_sdk/utils/__init__.py
 -rw-r--r--  2.0 unx     5653 b- defN 24-Mar-05 07:19 aistudio_sdk/utils/bos_sdk.py
 -rw-r--r--  2.0 unx     4785 b- defN 24-Mar-05 13:56 aistudio_sdk/utils/util.py
--rw-r--r--  2.0 unx     1130 b- defN 24-Apr-16 12:51 aistudio_sdk-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 12:51 aistudio_sdk-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-16 12:51 aistudio_sdk-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Apr-16 12:51 aistudio_sdk-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1929 b- defN 24-Apr-16 12:51 aistudio_sdk-0.2.2.dist-info/RECORD
-23 files, 84942 bytes uncompressed, 24436 bytes compressed:  71.2%
+-rw-r--r--  2.0 unx     1047 b- defN 24-Apr-18 07:32 aistudio_sdk-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 07:32 aistudio_sdk-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-18 07:32 aistudio_sdk-0.2.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-18 07:32 aistudio_sdk-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1929 b- defN 24-Apr-18 07:32 aistudio_sdk-0.2.3.dist-info/RECORD
+23 files, 84865 bytes uncompressed, 24386 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: aistudio_sdk/utils/bos_sdk.py
 Comment: 
 
 Filename: aistudio_sdk/utils/util.py
 Comment: 
 
-Filename: aistudio_sdk-0.2.2.dist-info/METADATA
+Filename: aistudio_sdk-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: aistudio_sdk-0.2.2.dist-info/WHEEL
+Filename: aistudio_sdk-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: aistudio_sdk-0.2.2.dist-info/entry_points.txt
+Filename: aistudio_sdk-0.2.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: aistudio_sdk-0.2.2.dist-info/top_level.txt
+Filename: aistudio_sdk-0.2.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aistudio_sdk-0.2.2.dist-info/RECORD
+Filename: aistudio_sdk-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aistudio_sdk/hub.py

```diff
@@ -308,15 +308,15 @@
 
         is_http_valid = True if upload_href and file_size < config.LFS_FILE_SIZE_LIMIT_PUT else False
 
         def _uploading_using_sts():
             """
             使用sts上传文件
             """
-            from aistudio_sdk.bos_sdk import sts_client, upload_file, upload_super_file
+            from aistudio_sdk.utils.bos_sdk import sts_client, upload_file, upload_super_file
             try:
                 client = sts_client(sts_token.get("bos_host"), sts_token.get("access_key_id"),
                            sts_token.get("secret_access_key"), sts_token.get("session_token"))
                 res = upload_super_file(client,
                                         bucket=sts_token.get("bucket_name"), file=file_path, key=sts_token.get("key"))
                 return res
             except Exception as e:
```

## aistudio_sdk/constant/version.py

```diff
@@ -7,8 +7,8 @@
 ################################################################################
 """
 本文件注明版本号
 
 Authors: xiangyiqing(xiangyiqing@baidu.com)
 Date:    2023/07/24
 """
-VERSION = "0.2.2"
+VERSION = "0.2.3"
```

## Comparing `aistudio_sdk-0.2.2.dist-info/METADATA` & `aistudio_sdk-0.2.3.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistudio-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python client library for the AIStudio API
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: bce-python-sdk
 Requires-Dist: prettytable
@@ -16,17 +16,15 @@
 实现封装AIStudio模型库API的PythonSDK，支持AIStudio开发者进行模型库的操作开发需求
 
 快速开始
 ---
 如何构建、安装、运行
 
 ```bash
-python setup.py bdist_wheel
-pip uninstall -y aistudio-sdk
-pip install output/dist/aistudio_sdk-0.1.7-py3-none-any.whl
+pip install aistudio-sdk --upgrade
 ```
 
 测试
 ---
 如何执行自动化测试
 
 如何贡献
```

## Comparing `aistudio_sdk-0.2.2.dist-info/RECORD` & `aistudio_sdk-0.2.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 aistudio_sdk/__init__.py,sha256=4oyJtPCAfg6YBNzeJ0d-MS10vaQfkO9O86z3nbH5Y8k,534
 aistudio_sdk/cmdline.py,sha256=KAbCUBCv9AKvHTindIzUtr39z7zDm9IP6tzBGdp-5Ng,4896
 aistudio_sdk/config.py,sha256=pv42pDoGYQEc14IhEMnzaD3eZ9eDxVlyHnyYHhH67Yw,1389
-aistudio_sdk/hub.py,sha256=f0y5tPIt1lvY3zccoI0xMx9eMLmlq4rsmfv5I2S_C_8,25051
+aistudio_sdk/hub.py,sha256=TBeGp5RJEGjxlxmMflPt8HwGr94uz2dG56VzdGnbv68,25057
 aistudio_sdk/log.py,sha256=eylK9nw-orLahseNTkI5_X0ZneUxiAweYPZDReOZxkY,1898
 aistudio_sdk/constant/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aistudio_sdk/constant/const.py,sha256=jn2cpKRoNTuZQ5Uau76p6P1A6Gdty1W9lsxgDc7kt8k,626
 aistudio_sdk/constant/err_code.py,sha256=ZFybkcHn2AeNAJp05xMv1SDAl7IW6_9XYCI8wyFCwy4,2388
-aistudio_sdk/constant/version.py,sha256=B6t64Ww0uUcOfae1Ng0ofeo2qc6A-6kzs96HCBnOzQ4,387
+aistudio_sdk/constant/version.py,sha256=hxpuvVTasiO1V9LT4qynwzwCYN4xNVWCH0YmwNtu9ks,387
 aistudio_sdk/requests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aistudio_sdk/requests/hub.py,sha256=1tH6Yj7RbkLYkoPLxR_wSvr4crb8hks3AXNJ3wigVR0,16394
 aistudio_sdk/requests/pipeline.py,sha256=_NHbuTea7D4aDV5tsdQof-meFAAurjCFO2_ckLBPrH0,5201
 aistudio_sdk/sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aistudio_sdk/sdk/pipeline.py,sha256=TanllZPc-xyuFuYLDQfpXC7ZdqkVoa0Gx5nphJ_eu18,12521
 aistudio_sdk/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aistudio_sdk/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aistudio_sdk/utils/bos_sdk.py,sha256=RnORp8P6MYbmjorfBYFM0BfgIr5tgp5epV60rduT73g,5653
 aistudio_sdk/utils/util.py,sha256=Sm3pAjykh3nT86RzMIaGxjcPh__2TTYdyAfC0aKN47M,4785
-aistudio_sdk-0.2.2.dist-info/METADATA,sha256=fi1MlTuibB86CYAL-P7jBhUf8T6aDCtr5YjnIUkH6k0,1130
-aistudio_sdk-0.2.2.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
-aistudio_sdk-0.2.2.dist-info/entry_points.txt,sha256=2S1UPsawP86d_GKOtesmj2dfoQl0yD7tgJqvPjbPMzY,55
-aistudio_sdk-0.2.2.dist-info/top_level.txt,sha256=-gcmvd8vRpFAPY7aqcgeoSPvF1A0NBW2_zNEcqmme74,13
-aistudio_sdk-0.2.2.dist-info/RECORD,,
+aistudio_sdk-0.2.3.dist-info/METADATA,sha256=O-kBU_9rggnDw9vlLJBg4B_5HcfndOr0YMOKU4THxGY,1047
+aistudio_sdk-0.2.3.dist-info/WHEEL,sha256=U88EhGIw8Sj2_phqajeu_EAi3RAo8-C6zV3REsWbWbs,92
+aistudio_sdk-0.2.3.dist-info/entry_points.txt,sha256=2S1UPsawP86d_GKOtesmj2dfoQl0yD7tgJqvPjbPMzY,55
+aistudio_sdk-0.2.3.dist-info/top_level.txt,sha256=-gcmvd8vRpFAPY7aqcgeoSPvF1A0NBW2_zNEcqmme74,13
+aistudio_sdk-0.2.3.dist-info/RECORD,,
```

