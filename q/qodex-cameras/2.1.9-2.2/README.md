# Comparing `tmp/qodex_cameras-2.1.9-py3-none-any.whl.zip` & `tmp/qodex_cameras-2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 39843 bytes, number of entries: 18
+Zip file size: 39807 bytes, number of entries: 18
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 06:46 qodex_cameras/__init__.py
 -rw-rw-rw-  2.0 fat      166 b- defN 23-May-02 11:08 qodex_cameras/functions.py
--rw-rw-rw-  2.0 fat     3092 b- defN 24-Apr-08 10:46 qodex_cameras/main.py
+-rw-rw-rw-  2.0 fat     3016 b- defN 24-Apr-18 06:03 qodex_cameras/main.py
 -rw-rw-rw-  2.0 fat     3274 b- defN 24-Apr-08 11:49 qodex_cameras/mixins.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-12 08:58 qodex_cameras/settings.py
 -rw-rw-rw-  2.0 fat     2007 b- defN 24-Apr-01 15:03 qodex_cameras/video_saver.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 04:44 qodex_cameras/other/__init__.py
 -rw-rw-rw-  2.0 fat     6078 b- defN 23-May-02 04:46 qodex_cameras/other/pyhik_mode.py
 -rw-rw-rw-  2.0 fat     7365 b- defN 23-May-12 06:25 qodex_cameras/photos/Test.png
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 05:38 qodex_cameras/photos/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-02 12:07 qodex_cameras/tests/__init__.py
 -rw-rw-rw-  2.0 fat     1372 b- defN 24-Feb-21 14:19 qodex_cameras/tests/main_tests.py
 -rw-rw-rw-  2.0 fat    26529 b- defN 23-May-12 08:58 qodex_cameras/tests/test.png
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-08 11:50 qodex_cameras-2.1.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      304 b- defN 24-Apr-08 11:50 qodex_cameras-2.1.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 11:50 qodex_cameras-2.1.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-08 11:50 qodex_cameras-2.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1508 b- defN 24-Apr-08 11:50 qodex_cameras-2.1.9.dist-info/RECORD
-18 files, 53276 bytes uncompressed, 37345 bytes compressed:  29.9%
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-18 06:04 qodex_cameras-2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 24-Apr-18 06:04 qodex_cameras-2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 06:04 qodex_cameras-2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-18 06:04 qodex_cameras-2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1498 b- defN 24-Apr-18 06:04 qodex_cameras-2.2.dist-info/RECORD
+18 files, 53188 bytes uncompressed, 37329 bytes compressed:  29.8%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: qodex_cameras/tests/main_tests.py
 Comment: 
 
 Filename: qodex_cameras/tests/test.png
 Comment: 
 
-Filename: qodex_cameras-2.1.9.dist-info/LICENSE
+Filename: qodex_cameras-2.2.dist-info/LICENSE
 Comment: 
 
-Filename: qodex_cameras-2.1.9.dist-info/METADATA
+Filename: qodex_cameras-2.2.dist-info/METADATA
 Comment: 
 
-Filename: qodex_cameras-2.1.9.dist-info/WHEEL
+Filename: qodex_cameras-2.2.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_cameras-2.1.9.dist-info/top_level.txt
+Filename: qodex_cameras-2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_cameras-2.1.9.dist-info/RECORD
+Filename: qodex_cameras-2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qodex_cameras/main.py

```diff
@@ -32,29 +32,27 @@
 
     def get_photo_rest(self):
         return self.get_http_photo()
 
     def start_record(self, rtsp_stream_link=None, output="output.avi"):
         self.output = output
         pic_res = self.make_pic()
-        if not pic_res["error"]:
-            self.start_record_thumb = pic_res
+        self.start_record_thumb = pic_res
         rtsp_stream_link = f"rtsp://{self.cam_login}:{self.cam_pass}@{self.ip}:{self.rtsp_port}/Streaming/Channels/101"
         super(HikCamera, self).start_record(
             rtsp_stream_link=rtsp_stream_link, output=output)
 
     def stop_record(self):
         threading.Thread(target=self.make_stop_record_thumb).start()
         super(HikCamera, self).stop_record()
         return self.output
 
     def make_stop_record_thumb(self):
         pic_res = self.make_pic()
-        if not pic_res["error"]:
-            self.start_record_thumb = pic_res
+        self.start_record_thumb = pic_res
 
 class HikCameraCarNumberRecognition(HikCamera,
                                     recognition.MailNumberRecognitionRus):
     def __init__(self, ip, port, login, password, mail_token,
                  pics_folder=None, rtsp_port=554, test_mode=False,
                  auth_method="Basic", save_pics=False, photo_type_name=None):
         super().__init__(ip, port, login, password,
```

## Comparing `qodex_cameras-2.1.9.dist-info/LICENSE` & `qodex_cameras-2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qodex_cameras-2.1.9.dist-info/RECORD` & `qodex_cameras-2.2.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 qodex_cameras/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/functions.py,sha256=elNHnnx3zelcKnAOLK3E6ETMpV3PZPXfWclPRYSqiZA,166
-qodex_cameras/main.py,sha256=mH6cJTTieW6TJ2kATkve60Hm46V8athW8bTeZ2KUXwo,3092
+qodex_cameras/main.py,sha256=ICTtly-zbIb95rxMW-eWWAlYiecwDyfhsOwSeqnD5i8,3016
 qodex_cameras/mixins.py,sha256=FLH7Q8lHxENLbCy9G7gCXrBUnh--jGvN89ah7nM0YXY,3274
 qodex_cameras/settings.py,sha256=xupNck2qOhJLj0WQjB47Z6dm179vhVF1FJ-dDcgX4c0,384
 qodex_cameras/video_saver.py,sha256=ebzsVuUQuKxO_Jv8Z7yFZdYx8XEI3ZkfyAo7b-Gutpg,2007
 qodex_cameras/other/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/other/pyhik_mode.py,sha256=FyG_QWVdcTi5dnSwv3Iq-L0H4PYW6wKBeVJpkYRt58Q,6078
 qodex_cameras/photos/Test.png,sha256=v54Of9PyXTQ-X6_ji_105kC2ISyuxG6UxJDBzcdV4ac,7365
 qodex_cameras/photos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_cameras/tests/main_tests.py,sha256=2i8_idlYsYF6jL10A36VtsOPbH-HofShSKPyBkdVAPo,1372
 qodex_cameras/tests/test.png,sha256=EZ4YZtPhTRLJBM2ZMr-ZyXqVMKgYlmW-25syShwy_8s,26529
-qodex_cameras-2.1.9.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-qodex_cameras-2.1.9.dist-info/METADATA,sha256=JnaTbyUky-xZJlvYEJTydxJ4HVu6Uk4IMF3rpQ8H7Cg,304
-qodex_cameras-2.1.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-qodex_cameras-2.1.9.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
-qodex_cameras-2.1.9.dist-info/RECORD,,
+qodex_cameras-2.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+qodex_cameras-2.2.dist-info/METADATA,sha256=2fV1UGkEMlBlLyovWJeOR3v8xnyaL4SQ91J-M0HvAcI,302
+qodex_cameras-2.2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+qodex_cameras-2.2.dist-info/top_level.txt,sha256=TUs_F_ccN29bu8q7TOb4gyqz9ZJY8Jb93IueSTAuBHA,14
+qodex_cameras-2.2.dist-info/RECORD,,
```

