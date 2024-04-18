# Comparing `tmp/livekit-protocol-0.4.0.tar.gz` & `tmp/livekit_protocol-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-protocol-0.4.0.tar", last modified: Thu Apr  4 00:52:23 2024, max compression
+gzip compressed data, was "livekit_protocol-0.5.0.tar", last modified: Thu Apr 18 18:12:17 2024, max compression
```

## Comparing `livekit-protocol-0.4.0.tar` & `livekit_protocol-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.287329 livekit-protocol-0.4.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/livekit/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/agent.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/analytics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/egress.py
--rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/egress.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/ingress.py
--rw-r--r--   0 runner    (1001) docker     (127)    13224 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/ingress.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18390 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    31005 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/room.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/livekit/protocol/webhook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/livekit_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 00:52:23.000000 livekit-protocol-0.4.0/livekit_protocol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:52:23.291329 livekit-protocol-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-04 00:52:04.000000 livekit-protocol-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:16.994712 livekit_protocol-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-18 18:12:16.994712 livekit_protocol-0.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:16.990712 livekit_protocol-0.5.0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:16.994712 livekit_protocol-0.5.0/livekit/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/agent.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8874 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14676 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/analytics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/egress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/egress.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/ingress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13336 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/ingress.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19338 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32695 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/room.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/sip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/sip.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/livekit/protocol/webhook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:12:16.994712 livekit_protocol-0.5.0/livekit_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-18 18:12:16.000000 livekit_protocol-0.5.0/livekit_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-18 18:12:16.000000 livekit_protocol-0.5.0/livekit_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:12:16.000000 livekit_protocol-0.5.0/livekit_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-18 18:12:16.000000 livekit_protocol-0.5.0/livekit_protocol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-18 18:12:16.000000 livekit_protocol-0.5.0/livekit_protocol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:12:16.994712 livekit_protocol-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-18 18:12:04.000000 livekit_protocol-0.5.0/setup.py
```

### Comparing `livekit-protocol-0.4.0/PKG-INFO` & `livekit_protocol-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-protocol
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python protocol stubs for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit-protocol-0.4.0/livekit/protocol/agent.py` & `livekit_protocol-0.5.0/livekit/protocol/agent.py`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/agent.pyi` & `livekit_protocol-0.5.0/livekit/protocol/agent.pyi`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/analytics.py` & `livekit_protocol-0.5.0/livekit/protocol/analytics.py`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/analytics.pyi` & `livekit_protocol-0.5.0/livekit/protocol/analytics.pyi`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/egress.py` & `livekit_protocol-0.5.0/livekit/protocol/egress.py`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/egress.pyi` & `livekit_protocol-0.5.0/livekit/protocol/egress.pyi`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/ingress.py` & `livekit_protocol-0.5.0/livekit/protocol/ingress.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,52 +11,52 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import models as _models_
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15livekit_ingress.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\xbb\x02\n\x14\x43reateIngressRequest\x12)\n\ninput_type\x18\x01 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x0b\n\x03url\x18\t \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\n \x01(\t\x12\x1a\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\"\xcd\x01\n\x13IngressAudioOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressAudioEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressAudioEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\xcd\x01\n\x13IngressVideoOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressVideoEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressVideoEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\x7f\n\x1bIngressAudioEncodingOptions\x12(\n\x0b\x61udio_codec\x18\x01 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x0f\n\x07\x62itrate\x18\x02 \x01(\r\x12\x13\n\x0b\x64isable_dtx\x18\x03 \x01(\x08\x12\x10\n\x08\x63hannels\x18\x04 \x01(\r\"\x80\x01\n\x1bIngressVideoEncodingOptions\x12(\n\x0bvideo_codec\x18\x01 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x12\n\nframe_rate\x18\x02 \x01(\x01\x12#\n\x06layers\x18\x03 \x03(\x0b\x32\x13.livekit.VideoLayer\"\x92\x03\n\x0bIngressInfo\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nstream_key\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12)\n\ninput_type\x18\x05 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x1a\n\x12\x62ypass_transcoding\x18\r \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\x12\x11\n\troom_name\x18\x08 \x01(\t\x12\x1c\n\x14participant_identity\x18\t \x01(\t\x12\x18\n\x10participant_name\x18\n \x01(\t\x12\x1c\n\x14participant_metadata\x18\x0e \x01(\t\x12\x10\n\x08reusable\x18\x0b \x01(\x08\x12$\n\x05state\x18\x0c \x01(\x0b\x32\x15.livekit.IngressState\"\x8a\x03\n\x0cIngressState\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.livekit.IngressState.Status\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\'\n\x05video\x18\x03 \x01(\x0b\x32\x18.livekit.InputVideoState\x12\'\n\x05\x61udio\x18\x04 \x01(\x0b\x32\x18.livekit.InputAudioState\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x12\n\nstarted_at\x18\x07 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x08 \x01(\x03\x12\x13\n\x0bresource_id\x18\t \x01(\t\x12\"\n\x06tracks\x18\x06 \x03(\x0b\x32\x12.livekit.TrackInfo\"{\n\x06Status\x12\x15\n\x11\x45NDPOINT_INACTIVE\x10\x00\x12\x16\n\x12\x45NDPOINT_BUFFERING\x10\x01\x12\x17\n\x13\x45NDPOINT_PUBLISHING\x10\x02\x12\x12\n\x0e\x45NDPOINT_ERROR\x10\x03\x12\x15\n\x11\x45NDPOINT_COMPLETE\x10\x04\"o\n\x0fInputVideoState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x11\n\tframerate\x18\x05 \x01(\x01\"d\n\x0fInputAudioState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\x10\n\x08\x63hannels\x18\x03 \x01(\r\x12\x13\n\x0bsample_rate\x18\x04 \x01(\r\"\xb3\x02\n\x14UpdateIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\t \x01(\t\x12\x1f\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08H\x00\x88\x01\x01\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptionsB\x15\n\x13_bypass_transcoding\";\n\x12ListIngressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x12\n\ningress_id\x18\x02 \x01(\t\":\n\x13ListIngressResponse\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.livekit.IngressInfo\"*\n\x14\x44\x65leteIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t*=\n\x0cIngressInput\x12\x0e\n\nRTMP_INPUT\x10\x00\x12\x0e\n\nWHIP_INPUT\x10\x01\x12\r\n\tURL_INPUT\x10\x02*I\n\x1aIngressAudioEncodingPreset\x12\x16\n\x12OPUS_STEREO_96KBPS\x10\x00\x12\x13\n\x0fOPUS_MONO_64KBS\x10\x01*\x84\x03\n\x1aIngressVideoEncodingPreset\x12\x1c\n\x18H264_720P_30FPS_3_LAYERS\x10\x00\x12\x1d\n\x19H264_1080P_30FPS_3_LAYERS\x10\x01\x12\x1c\n\x18H264_540P_25FPS_2_LAYERS\x10\x02\x12\x1b\n\x17H264_720P_30FPS_1_LAYER\x10\x03\x12\x1c\n\x18H264_1080P_30FPS_1_LAYER\x10\x04\x12(\n$H264_720P_30FPS_3_LAYERS_HIGH_MOTION\x10\x05\x12)\n%H264_1080P_30FPS_3_LAYERS_HIGH_MOTION\x10\x06\x12(\n$H264_540P_25FPS_2_LAYERS_HIGH_MOTION\x10\x07\x12\'\n#H264_720P_30FPS_1_LAYER_HIGH_MOTION\x10\x08\x12(\n$H264_1080P_30FPS_1_LAYER_HIGH_MOTION\x10\t2\xa5\x02\n\x07Ingress\x12\x44\n\rCreateIngress\x12\x1d.livekit.CreateIngressRequest\x1a\x14.livekit.IngressInfo\x12\x44\n\rUpdateIngress\x12\x1d.livekit.UpdateIngressRequest\x1a\x14.livekit.IngressInfo\x12H\n\x0bListIngress\x12\x1b.livekit.ListIngressRequest\x1a\x1c.livekit.ListIngressResponse\x12\x44\n\rDeleteIngress\x12\x1d.livekit.DeleteIngressRequest\x1a\x14.livekit.IngressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15livekit_ingress.proto\x12\x07livekit\x1a\x14livekit_models.proto\"\xbb\x02\n\x14\x43reateIngressRequest\x12)\n\ninput_type\x18\x01 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x0b\n\x03url\x18\t \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\n \x01(\t\x12\x1a\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\"\xcd\x01\n\x13IngressAudioOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressAudioEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressAudioEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\xcd\x01\n\x13IngressVideoOptions\x12\x0c\n\x04name\x18\x01 \x01(\t\x12$\n\x06source\x18\x02 \x01(\x0e\x32\x14.livekit.TrackSource\x12\x35\n\x06preset\x18\x03 \x01(\x0e\x32#.livekit.IngressVideoEncodingPresetH\x00\x12\x37\n\x07options\x18\x04 \x01(\x0b\x32$.livekit.IngressVideoEncodingOptionsH\x00\x42\x12\n\x10\x65ncoding_options\"\x7f\n\x1bIngressAudioEncodingOptions\x12(\n\x0b\x61udio_codec\x18\x01 \x01(\x0e\x32\x13.livekit.AudioCodec\x12\x0f\n\x07\x62itrate\x18\x02 \x01(\r\x12\x13\n\x0b\x64isable_dtx\x18\x03 \x01(\x08\x12\x10\n\x08\x63hannels\x18\x04 \x01(\r\"\x80\x01\n\x1bIngressVideoEncodingOptions\x12(\n\x0bvideo_codec\x18\x01 \x01(\x0e\x32\x13.livekit.VideoCodec\x12\x12\n\nframe_rate\x18\x02 \x01(\x01\x12#\n\x06layers\x18\x03 \x03(\x0b\x32\x13.livekit.VideoLayer\"\x92\x03\n\x0bIngressInfo\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nstream_key\x18\x03 \x01(\t\x12\x0b\n\x03url\x18\x04 \x01(\t\x12)\n\ninput_type\x18\x05 \x01(\x0e\x32\x15.livekit.IngressInput\x12\x1a\n\x12\x62ypass_transcoding\x18\r \x01(\x08\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptions\x12\x11\n\troom_name\x18\x08 \x01(\t\x12\x1c\n\x14participant_identity\x18\t \x01(\t\x12\x18\n\x10participant_name\x18\n \x01(\t\x12\x1c\n\x14participant_metadata\x18\x0e \x01(\t\x12\x10\n\x08reusable\x18\x0b \x01(\x08\x12$\n\x05state\x18\x0c \x01(\x0b\x32\x15.livekit.IngressState\"\x9e\x03\n\x0cIngressState\x12,\n\x06status\x18\x01 \x01(\x0e\x32\x1c.livekit.IngressState.Status\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\'\n\x05video\x18\x03 \x01(\x0b\x32\x18.livekit.InputVideoState\x12\'\n\x05\x61udio\x18\x04 \x01(\x0b\x32\x18.livekit.InputAudioState\x12\x0f\n\x07room_id\x18\x05 \x01(\t\x12\x12\n\nstarted_at\x18\x07 \x01(\x03\x12\x10\n\x08\x65nded_at\x18\x08 \x01(\x03\x12\x12\n\nupdated_at\x18\n \x01(\x03\x12\x13\n\x0bresource_id\x18\t \x01(\t\x12\"\n\x06tracks\x18\x06 \x03(\x0b\x32\x12.livekit.TrackInfo\"{\n\x06Status\x12\x15\n\x11\x45NDPOINT_INACTIVE\x10\x00\x12\x16\n\x12\x45NDPOINT_BUFFERING\x10\x01\x12\x17\n\x13\x45NDPOINT_PUBLISHING\x10\x02\x12\x12\n\x0e\x45NDPOINT_ERROR\x10\x03\x12\x15\n\x11\x45NDPOINT_COMPLETE\x10\x04\"o\n\x0fInputVideoState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\r\n\x05width\x18\x03 \x01(\r\x12\x0e\n\x06height\x18\x04 \x01(\r\x12\x11\n\tframerate\x18\x05 \x01(\x01\"d\n\x0fInputAudioState\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x17\n\x0f\x61verage_bitrate\x18\x02 \x01(\r\x12\x10\n\x08\x63hannels\x18\x03 \x01(\r\x12\x13\n\x0bsample_rate\x18\x04 \x01(\r\"\xb3\x02\n\x14UpdateIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\troom_name\x18\x03 \x01(\t\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x18\n\x10participant_name\x18\x05 \x01(\t\x12\x1c\n\x14participant_metadata\x18\t \x01(\t\x12\x1f\n\x12\x62ypass_transcoding\x18\x08 \x01(\x08H\x00\x88\x01\x01\x12+\n\x05\x61udio\x18\x06 \x01(\x0b\x32\x1c.livekit.IngressAudioOptions\x12+\n\x05video\x18\x07 \x01(\x0b\x32\x1c.livekit.IngressVideoOptionsB\x15\n\x13_bypass_transcoding\";\n\x12ListIngressRequest\x12\x11\n\troom_name\x18\x01 \x01(\t\x12\x12\n\ningress_id\x18\x02 \x01(\t\":\n\x13ListIngressResponse\x12#\n\x05items\x18\x01 \x03(\x0b\x32\x14.livekit.IngressInfo\"*\n\x14\x44\x65leteIngressRequest\x12\x12\n\ningress_id\x18\x01 \x01(\t*=\n\x0cIngressInput\x12\x0e\n\nRTMP_INPUT\x10\x00\x12\x0e\n\nWHIP_INPUT\x10\x01\x12\r\n\tURL_INPUT\x10\x02*I\n\x1aIngressAudioEncodingPreset\x12\x16\n\x12OPUS_STEREO_96KBPS\x10\x00\x12\x13\n\x0fOPUS_MONO_64KBS\x10\x01*\x84\x03\n\x1aIngressVideoEncodingPreset\x12\x1c\n\x18H264_720P_30FPS_3_LAYERS\x10\x00\x12\x1d\n\x19H264_1080P_30FPS_3_LAYERS\x10\x01\x12\x1c\n\x18H264_540P_25FPS_2_LAYERS\x10\x02\x12\x1b\n\x17H264_720P_30FPS_1_LAYER\x10\x03\x12\x1c\n\x18H264_1080P_30FPS_1_LAYER\x10\x04\x12(\n$H264_720P_30FPS_3_LAYERS_HIGH_MOTION\x10\x05\x12)\n%H264_1080P_30FPS_3_LAYERS_HIGH_MOTION\x10\x06\x12(\n$H264_540P_25FPS_2_LAYERS_HIGH_MOTION\x10\x07\x12\'\n#H264_720P_30FPS_1_LAYER_HIGH_MOTION\x10\x08\x12(\n$H264_1080P_30FPS_1_LAYER_HIGH_MOTION\x10\t2\xa5\x02\n\x07Ingress\x12\x44\n\rCreateIngress\x12\x1d.livekit.CreateIngressRequest\x1a\x14.livekit.IngressInfo\x12\x44\n\rUpdateIngress\x12\x1d.livekit.UpdateIngressRequest\x1a\x14.livekit.IngressInfo\x12H\n\x0bListIngress\x12\x1b.livekit.ListIngressRequest\x1a\x1c.livekit.ListIngressResponse\x12\x44\n\rDeleteIngress\x12\x1d.livekit.DeleteIngressRequest\x1a\x14.livekit.IngressInfoBFZ#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ingress', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
-  _globals['_INGRESSINPUT']._serialized_start=2542
-  _globals['_INGRESSINPUT']._serialized_end=2603
-  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_start=2605
-  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_end=2678
-  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_start=2681
-  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_end=3069
+  _globals['_INGRESSINPUT']._serialized_start=2562
+  _globals['_INGRESSINPUT']._serialized_end=2623
+  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_start=2625
+  _globals['_INGRESSAUDIOENCODINGPRESET']._serialized_end=2698
+  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_start=2701
+  _globals['_INGRESSVIDEOENCODINGPRESET']._serialized_end=3089
   _globals['_CREATEINGRESSREQUEST']._serialized_start=57
   _globals['_CREATEINGRESSREQUEST']._serialized_end=372
   _globals['_INGRESSAUDIOOPTIONS']._serialized_start=375
   _globals['_INGRESSAUDIOOPTIONS']._serialized_end=580
   _globals['_INGRESSVIDEOOPTIONS']._serialized_start=583
   _globals['_INGRESSVIDEOOPTIONS']._serialized_end=788
   _globals['_INGRESSAUDIOENCODINGOPTIONS']._serialized_start=790
   _globals['_INGRESSAUDIOENCODINGOPTIONS']._serialized_end=917
   _globals['_INGRESSVIDEOENCODINGOPTIONS']._serialized_start=920
   _globals['_INGRESSVIDEOENCODINGOPTIONS']._serialized_end=1048
   _globals['_INGRESSINFO']._serialized_start=1051
   _globals['_INGRESSINFO']._serialized_end=1453
   _globals['_INGRESSSTATE']._serialized_start=1456
-  _globals['_INGRESSSTATE']._serialized_end=1850
-  _globals['_INGRESSSTATE_STATUS']._serialized_start=1727
-  _globals['_INGRESSSTATE_STATUS']._serialized_end=1850
-  _globals['_INPUTVIDEOSTATE']._serialized_start=1852
-  _globals['_INPUTVIDEOSTATE']._serialized_end=1963
-  _globals['_INPUTAUDIOSTATE']._serialized_start=1965
-  _globals['_INPUTAUDIOSTATE']._serialized_end=2065
-  _globals['_UPDATEINGRESSREQUEST']._serialized_start=2068
-  _globals['_UPDATEINGRESSREQUEST']._serialized_end=2375
-  _globals['_LISTINGRESSREQUEST']._serialized_start=2377
-  _globals['_LISTINGRESSREQUEST']._serialized_end=2436
-  _globals['_LISTINGRESSRESPONSE']._serialized_start=2438
-  _globals['_LISTINGRESSRESPONSE']._serialized_end=2496
-  _globals['_DELETEINGRESSREQUEST']._serialized_start=2498
-  _globals['_DELETEINGRESSREQUEST']._serialized_end=2540
-  _globals['_INGRESS']._serialized_start=3072
-  _globals['_INGRESS']._serialized_end=3365
+  _globals['_INGRESSSTATE']._serialized_end=1870
+  _globals['_INGRESSSTATE_STATUS']._serialized_start=1747
+  _globals['_INGRESSSTATE_STATUS']._serialized_end=1870
+  _globals['_INPUTVIDEOSTATE']._serialized_start=1872
+  _globals['_INPUTVIDEOSTATE']._serialized_end=1983
+  _globals['_INPUTAUDIOSTATE']._serialized_start=1985
+  _globals['_INPUTAUDIOSTATE']._serialized_end=2085
+  _globals['_UPDATEINGRESSREQUEST']._serialized_start=2088
+  _globals['_UPDATEINGRESSREQUEST']._serialized_end=2395
+  _globals['_LISTINGRESSREQUEST']._serialized_start=2397
+  _globals['_LISTINGRESSREQUEST']._serialized_end=2456
+  _globals['_LISTINGRESSRESPONSE']._serialized_start=2458
+  _globals['_LISTINGRESSRESPONSE']._serialized_end=2516
+  _globals['_DELETEINGRESSREQUEST']._serialized_start=2518
+  _globals['_DELETEINGRESSREQUEST']._serialized_end=2560
+  _globals['_INGRESS']._serialized_start=3092
+  _globals['_INGRESS']._serialized_end=3385
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.4.0/livekit/protocol/ingress.pyi` & `livekit_protocol-0.5.0/livekit/protocol/ingress.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     participant_name: str
     participant_metadata: str
     reusable: bool
     state: IngressState
     def __init__(self, ingress_id: _Optional[str] = ..., name: _Optional[str] = ..., stream_key: _Optional[str] = ..., url: _Optional[str] = ..., input_type: _Optional[_Union[IngressInput, str]] = ..., bypass_transcoding: bool = ..., audio: _Optional[_Union[IngressAudioOptions, _Mapping]] = ..., video: _Optional[_Union[IngressVideoOptions, _Mapping]] = ..., room_name: _Optional[str] = ..., participant_identity: _Optional[str] = ..., participant_name: _Optional[str] = ..., participant_metadata: _Optional[str] = ..., reusable: bool = ..., state: _Optional[_Union[IngressState, _Mapping]] = ...) -> None: ...
 
 class IngressState(_message.Message):
-    __slots__ = ("status", "error", "video", "audio", "room_id", "started_at", "ended_at", "resource_id", "tracks")
+    __slots__ = ("status", "error", "video", "audio", "room_id", "started_at", "ended_at", "updated_at", "resource_id", "tracks")
     class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         ENDPOINT_INACTIVE: _ClassVar[IngressState.Status]
         ENDPOINT_BUFFERING: _ClassVar[IngressState.Status]
         ENDPOINT_PUBLISHING: _ClassVar[IngressState.Status]
         ENDPOINT_ERROR: _ClassVar[IngressState.Status]
         ENDPOINT_COMPLETE: _ClassVar[IngressState.Status]
@@ -165,26 +165,28 @@
     STATUS_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     VIDEO_FIELD_NUMBER: _ClassVar[int]
     AUDIO_FIELD_NUMBER: _ClassVar[int]
     ROOM_ID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
+    UPDATED_AT_FIELD_NUMBER: _ClassVar[int]
     RESOURCE_ID_FIELD_NUMBER: _ClassVar[int]
     TRACKS_FIELD_NUMBER: _ClassVar[int]
     status: IngressState.Status
     error: str
     video: InputVideoState
     audio: InputAudioState
     room_id: str
     started_at: int
     ended_at: int
+    updated_at: int
     resource_id: str
     tracks: _containers.RepeatedCompositeFieldContainer[_models.TrackInfo]
-    def __init__(self, status: _Optional[_Union[IngressState.Status, str]] = ..., error: _Optional[str] = ..., video: _Optional[_Union[InputVideoState, _Mapping]] = ..., audio: _Optional[_Union[InputAudioState, _Mapping]] = ..., room_id: _Optional[str] = ..., started_at: _Optional[int] = ..., ended_at: _Optional[int] = ..., resource_id: _Optional[str] = ..., tracks: _Optional[_Iterable[_Union[_models.TrackInfo, _Mapping]]] = ...) -> None: ...
+    def __init__(self, status: _Optional[_Union[IngressState.Status, str]] = ..., error: _Optional[str] = ..., video: _Optional[_Union[InputVideoState, _Mapping]] = ..., audio: _Optional[_Union[InputAudioState, _Mapping]] = ..., room_id: _Optional[str] = ..., started_at: _Optional[int] = ..., ended_at: _Optional[int] = ..., updated_at: _Optional[int] = ..., resource_id: _Optional[str] = ..., tracks: _Optional[_Iterable[_Union[_models.TrackInfo, _Mapping]]] = ...) -> None: ...
 
 class InputVideoState(_message.Message):
     __slots__ = ("mime_type", "average_bitrate", "width", "height", "framerate")
     MIME_TYPE_FIELD_NUMBER: _ClassVar[int]
     AVERAGE_BITRATE_FIELD_NUMBER: _ClassVar[int]
     WIDTH_FIELD_NUMBER: _ClassVar[int]
     HEIGHT_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `livekit-protocol-0.4.0/livekit/protocol/models.py` & `livekit_protocol-0.5.0/livekit/protocol/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14livekit_models.proto\x12\x07livekit\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc9\x02\n\x04Room\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rempty_timeout\x18\x03 \x01(\r\x12\x19\n\x11\x64\x65parture_timeout\x18\x0e \x01(\r\x12\x18\n\x10max_participants\x18\x04 \x01(\r\x12\x15\n\rcreation_time\x18\x05 \x01(\x03\x12\x15\n\rturn_password\x18\x06 \x01(\t\x12&\n\x0e\x65nabled_codecs\x18\x07 \x03(\x0b\x32\x0e.livekit.Codec\x12\x10\n\x08metadata\x18\x08 \x01(\t\x12\x18\n\x10num_participants\x18\t \x01(\r\x12\x16\n\x0enum_publishers\x18\x0b \x01(\r\x12\x18\n\x10\x61\x63tive_recording\x18\n \x01(\x08\x12&\n\x07version\x18\r \x01(\x0b\x32\x15.livekit.TimedVersion\"(\n\x05\x43odec\x12\x0c\n\x04mime\x18\x01 \x01(\t\x12\x11\n\tfmtp_line\x18\x02 \x01(\t\"9\n\x0cPlayoutDelay\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\r\x12\x0b\n\x03max\x18\x03 \x01(\r\"\xde\x01\n\x15ParticipantPermission\x12\x15\n\rcan_subscribe\x18\x01 \x01(\x08\x12\x13\n\x0b\x63\x61n_publish\x18\x02 \x01(\x08\x12\x18\n\x10\x63\x61n_publish_data\x18\x03 \x01(\x08\x12\x31\n\x13\x63\x61n_publish_sources\x18\t \x03(\x0e\x32\x14.livekit.TrackSource\x12\x0e\n\x06hidden\x18\x07 \x01(\x08\x12\x10\n\x08recorder\x18\x08 \x01(\x08\x12\x1b\n\x13\x63\x61n_update_metadata\x18\n \x01(\x08\x12\r\n\x05\x61gent\x18\x0b \x01(\x08\"\xd1\x03\n\x0fParticipantInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12-\n\x05state\x18\x03 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12\"\n\x06tracks\x18\x04 \x03(\x0b\x32\x12.livekit.TrackInfo\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12\x11\n\tjoined_at\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\t \x01(\t\x12\x0f\n\x07version\x18\n \x01(\r\x12\x32\n\npermission\x18\x0b \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\x14\n\x0cis_publisher\x18\r \x01(\x08\x12+\n\x04kind\x18\x0e \x01(\x0e\x32\x1d.livekit.ParticipantInfo.Kind\">\n\x05State\x12\x0b\n\x07JOINING\x10\x00\x12\n\n\x06JOINED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x10\n\x0c\x44ISCONNECTED\x10\x03\"A\n\x04Kind\x12\x0c\n\x08STANDARD\x10\x00\x12\x0b\n\x07INGRESS\x10\x01\x12\n\n\x06\x45GRESS\x10\x02\x12\x07\n\x03SIP\x10\x03\x12\t\n\x05\x41GENT\x10\x04\"3\n\nEncryption\"%\n\x04Type\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GCM\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\"f\n\x12SimulcastCodecInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\t\x12\x0b\n\x03\x63id\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer\"\xc1\x03\n\tTrackInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.livekit.TrackType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x11\n\tsimulcast\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x08 \x01(\x08\x12$\n\x06source\x18\t \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\n \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x11\n\tmime_type\x18\x0b \x01(\t\x12\x0b\n\x03mid\x18\x0c \x01(\t\x12+\n\x06\x63odecs\x18\r \x03(\x0b\x32\x1b.livekit.SimulcastCodecInfo\x12\x0e\n\x06stereo\x18\x0e \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\x0f \x01(\x08\x12,\n\nencryption\x18\x10 \x01(\x0e\x32\x18.livekit.Encryption.Type\x12\x0e\n\x06stream\x18\x11 \x01(\t\x12&\n\x07version\x18\x12 \x01(\x0b\x32\x15.livekit.TimedVersion\"r\n\nVideoLayer\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x0c\n\x04ssrc\x18\x05 \x01(\r\"\xa0\x02\n\nDataPacket\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x18.livekit.DataPacket.KindB\x02\x18\x01\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x1e\n\x16\x64\x65stination_identities\x18\x05 \x03(\t\x12#\n\x04user\x18\x02 \x01(\x0b\x32\x13.livekit.UserPacketH\x00\x12\x33\n\x07speaker\x18\x03 \x01(\x0b\x32\x1c.livekit.ActiveSpeakerUpdateB\x02\x18\x01H\x00\x12$\n\x08sip_dtmf\x18\x06 \x01(\x0b\x32\x10.livekit.SipDTMFH\x00\"\x1f\n\x04Kind\x12\x0c\n\x08RELIABLE\x10\x00\x12\t\n\x05LOSSY\x10\x01\x42\x07\n\x05value\"=\n\x13\x41\x63tiveSpeakerUpdate\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo\"9\n\x0bSpeakerInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\"\xbc\x01\n\nUserPacket\x12\x1b\n\x0fparticipant_sid\x18\x01 \x01(\tB\x02\x18\x01\x12 \n\x14participant_identity\x18\x05 \x01(\tB\x02\x18\x01\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x1c\n\x10\x64\x65stination_sids\x18\x03 \x03(\tB\x02\x18\x01\x12\"\n\x16\x64\x65stination_identities\x18\x06 \x03(\tB\x02\x18\x01\x12\x12\n\x05topic\x18\x04 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_topic\"&\n\x07SipDTMF\x12\x0c\n\x04\x63ode\x18\x03 \x01(\r\x12\r\n\x05\x64igit\x18\x04 \x01(\t\"@\n\x11ParticipantTracks\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\ntrack_sids\x18\x02 \x03(\t\"\xce\x01\n\nServerInfo\x12,\n\x07\x65\x64ition\x18\x01 \x01(\x0e\x32\x1b.livekit.ServerInfo.Edition\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\x0e\n\x06region\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x12\n\ndebug_info\x18\x06 \x01(\t\x12\x16\n\x0e\x61gent_protocol\x18\x07 \x01(\x05\"\"\n\x07\x45\x64ition\x12\x0c\n\x08Standard\x10\x00\x12\t\n\x05\x43loud\x10\x01\"\xdd\x02\n\nClientInfo\x12$\n\x03sdk\x18\x01 \x01(\x0e\x32\x17.livekit.ClientInfo.SDK\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\n\n\x02os\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\x06 \x01(\t\x12\x0f\n\x07\x62rowser\x18\x07 \x01(\t\x12\x17\n\x0f\x62rowser_version\x18\x08 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\t \x01(\t\x12\x0f\n\x07network\x18\n \x01(\t\"\x83\x01\n\x03SDK\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02JS\x10\x01\x12\t\n\x05SWIFT\x10\x02\x12\x0b\n\x07\x41NDROID\x10\x03\x12\x0b\n\x07\x46LUTTER\x10\x04\x12\x06\n\x02GO\x10\x05\x12\t\n\x05UNITY\x10\x06\x12\x10\n\x0cREACT_NATIVE\x10\x07\x12\x08\n\x04RUST\x10\x08\x12\n\n\x06PYTHON\x10\t\x12\x07\n\x03\x43PP\x10\n\"\x8c\x02\n\x13\x43lientConfiguration\x12*\n\x05video\x18\x01 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12+\n\x06screen\x18\x02 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12\x37\n\x11resume_connection\x18\x03 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\x12\x30\n\x0f\x64isabled_codecs\x18\x04 \x01(\x0b\x32\x17.livekit.DisabledCodecs\x12\x31\n\x0b\x66orce_relay\x18\x05 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"L\n\x12VideoConfiguration\x12\x36\n\x10hardware_encoder\x18\x01 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"Q\n\x0e\x44isabledCodecs\x12\x1e\n\x06\x63odecs\x18\x01 \x03(\x0b\x32\x0e.livekit.Codec\x12\x1f\n\x07publish\x18\x02 \x03(\x0b\x32\x0e.livekit.Codec\"\x80\x02\n\x08RTPDrift\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x17\n\x0fstart_timestamp\x18\x04 \x01(\x04\x12\x15\n\rend_timestamp\x18\x05 \x01(\x04\x12\x17\n\x0frtp_clock_ticks\x18\x06 \x01(\x04\x12\x15\n\rdrift_samples\x18\x07 \x01(\x03\x12\x10\n\x08\x64rift_ms\x18\x08 \x01(\x01\x12\x12\n\nclock_rate\x18\t \x01(\x01\"\xa0\n\n\x08RTPStats\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x0f\n\x07packets\x18\x04 \x01(\r\x12\x13\n\x0bpacket_rate\x18\x05 \x01(\x01\x12\r\n\x05\x62ytes\x18\x06 \x01(\x04\x12\x14\n\x0cheader_bytes\x18\' \x01(\x04\x12\x0f\n\x07\x62itrate\x18\x07 \x01(\x01\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x18\n\x10packet_loss_rate\x18\t \x01(\x01\x12\x1e\n\x16packet_loss_percentage\x18\n \x01(\x02\x12\x19\n\x11packets_duplicate\x18\x0b \x01(\r\x12\x1d\n\x15packet_duplicate_rate\x18\x0c \x01(\x01\x12\x17\n\x0f\x62ytes_duplicate\x18\r \x01(\x04\x12\x1e\n\x16header_bytes_duplicate\x18( \x01(\x04\x12\x19\n\x11\x62itrate_duplicate\x18\x0e \x01(\x01\x12\x17\n\x0fpackets_padding\x18\x0f \x01(\r\x12\x1b\n\x13packet_padding_rate\x18\x10 \x01(\x01\x12\x15\n\rbytes_padding\x18\x11 \x01(\x04\x12\x1c\n\x14header_bytes_padding\x18) \x01(\x04\x12\x17\n\x0f\x62itrate_padding\x18\x12 \x01(\x01\x12\x1c\n\x14packets_out_of_order\x18\x13 \x01(\r\x12\x0e\n\x06\x66rames\x18\x14 \x01(\r\x12\x12\n\nframe_rate\x18\x15 \x01(\x01\x12\x16\n\x0ejitter_current\x18\x16 \x01(\x01\x12\x12\n\njitter_max\x18\x17 \x01(\x01\x12:\n\rgap_histogram\x18\x18 \x03(\x0b\x32#.livekit.RTPStats.GapHistogramEntry\x12\r\n\x05nacks\x18\x19 \x01(\r\x12\x11\n\tnack_acks\x18% \x01(\r\x12\x13\n\x0bnack_misses\x18\x1a \x01(\r\x12\x15\n\rnack_repeated\x18& \x01(\r\x12\x0c\n\x04plis\x18\x1b \x01(\r\x12,\n\x08last_pli\x18\x1c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x66irs\x18\x1d \x01(\r\x12,\n\x08last_fir\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brtt_current\x18\x1f \x01(\r\x12\x0f\n\x07rtt_max\x18  \x01(\r\x12\x12\n\nkey_frames\x18! \x01(\r\x12\x32\n\x0elast_key_frame\x18\" \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flayer_lock_plis\x18# \x01(\r\x12\x37\n\x13last_layer_lock_pli\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x0cpacket_drift\x18, \x01(\x0b\x32\x11.livekit.RTPDrift\x12\'\n\x0creport_drift\x18- \x01(\x0b\x32\x11.livekit.RTPDrift\x12/\n\x14rebased_report_drift\x18. \x01(\x0b\x32\x11.livekit.RTPDrift\x1a\x33\n\x11GapHistogramEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"1\n\x0cTimedVersion\x12\x12\n\nunix_micro\x18\x01 \x01(\x03\x12\r\n\x05ticks\x18\x02 \x01(\x05*/\n\nAudioCodec\x12\x0e\n\nDEFAULT_AC\x10\x00\x12\x08\n\x04OPUS\x10\x01\x12\x07\n\x03\x41\x41\x43\x10\x02*V\n\nVideoCodec\x12\x0e\n\nDEFAULT_VC\x10\x00\x12\x11\n\rH264_BASELINE\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH264_HIGH\x10\x03\x12\x07\n\x03VP8\x10\x04*)\n\nImageCodec\x12\x0e\n\nIC_DEFAULT\x10\x00\x12\x0b\n\x07IC_JPEG\x10\x01*+\n\tTrackType\x12\t\n\x05\x41UDIO\x10\x00\x12\t\n\x05VIDEO\x10\x01\x12\x08\n\x04\x44\x41TA\x10\x02*`\n\x0bTrackSource\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43\x41MERA\x10\x01\x12\x0e\n\nMICROPHONE\x10\x02\x12\x10\n\x0cSCREEN_SHARE\x10\x03\x12\x16\n\x12SCREEN_SHARE_AUDIO\x10\x04*6\n\x0cVideoQuality\x12\x07\n\x03LOW\x10\x00\x12\n\n\x06MEDIUM\x10\x01\x12\x08\n\x04HIGH\x10\x02\x12\x07\n\x03OFF\x10\x03*@\n\x11\x43onnectionQuality\x12\x08\n\x04POOR\x10\x00\x12\x08\n\x04GOOD\x10\x01\x12\r\n\tEXCELLENT\x10\x02\x12\x08\n\x04LOST\x10\x03*;\n\x13\x43lientConfigSetting\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02*\xdb\x01\n\x10\x44isconnectReason\x12\x12\n\x0eUNKNOWN_REASON\x10\x00\x12\x14\n\x10\x43LIENT_INITIATED\x10\x01\x12\x16\n\x12\x44UPLICATE_IDENTITY\x10\x02\x12\x13\n\x0fSERVER_SHUTDOWN\x10\x03\x12\x17\n\x13PARTICIPANT_REMOVED\x10\x04\x12\x10\n\x0cROOM_DELETED\x10\x05\x12\x12\n\x0eSTATE_MISMATCH\x10\x06\x12\x10\n\x0cJOIN_FAILURE\x10\x07\x12\r\n\tMIGRATION\x10\x08\x12\x10\n\x0cSIGNAL_CLOSE\x10\t*\x89\x01\n\x0fReconnectReason\x12\x0e\n\nRR_UNKNOWN\x10\x00\x12\x1a\n\x16RR_SIGNAL_DISCONNECTED\x10\x01\x12\x17\n\x13RR_PUBLISHER_FAILED\x10\x02\x12\x18\n\x14RR_SUBSCRIBER_FAILED\x10\x03\x12\x17\n\x13RR_SWITCH_CANDIDATE\x10\x04*T\n\x11SubscriptionError\x12\x0e\n\nSE_UNKNOWN\x10\x00\x12\x18\n\x14SE_CODEC_UNSUPPORTED\x10\x01\x12\x15\n\x11SE_TRACK_NOTFOUND\x10\x02*\xa3\x01\n\x11\x41udioTrackFeature\x12\r\n\tTF_STEREO\x10\x00\x12\r\n\tTF_NO_DTX\x10\x01\x12\x18\n\x14TF_AUTO_GAIN_CONTROL\x10\x02\x12\x18\n\x14TF_ECHO_CANCELLATION\x10\x03\x12\x18\n\x14TF_NOISE_SUPPRESSION\x10\x04\x12\"\n\x1eTF_ENHANCED_NOISE_CANCELLATION\x10\x05\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14livekit_models.proto\x12\x07livekit\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc9\x02\n\x04Room\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rempty_timeout\x18\x03 \x01(\r\x12\x19\n\x11\x64\x65parture_timeout\x18\x0e \x01(\r\x12\x18\n\x10max_participants\x18\x04 \x01(\r\x12\x15\n\rcreation_time\x18\x05 \x01(\x03\x12\x15\n\rturn_password\x18\x06 \x01(\t\x12&\n\x0e\x65nabled_codecs\x18\x07 \x03(\x0b\x32\x0e.livekit.Codec\x12\x10\n\x08metadata\x18\x08 \x01(\t\x12\x18\n\x10num_participants\x18\t \x01(\r\x12\x16\n\x0enum_publishers\x18\x0b \x01(\r\x12\x18\n\x10\x61\x63tive_recording\x18\n \x01(\x08\x12&\n\x07version\x18\r \x01(\x0b\x32\x15.livekit.TimedVersion\"(\n\x05\x43odec\x12\x0c\n\x04mime\x18\x01 \x01(\t\x12\x11\n\tfmtp_line\x18\x02 \x01(\t\"9\n\x0cPlayoutDelay\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0b\n\x03min\x18\x02 \x01(\r\x12\x0b\n\x03max\x18\x03 \x01(\r\"\xde\x01\n\x15ParticipantPermission\x12\x15\n\rcan_subscribe\x18\x01 \x01(\x08\x12\x13\n\x0b\x63\x61n_publish\x18\x02 \x01(\x08\x12\x18\n\x10\x63\x61n_publish_data\x18\x03 \x01(\x08\x12\x31\n\x13\x63\x61n_publish_sources\x18\t \x03(\x0e\x32\x14.livekit.TrackSource\x12\x0e\n\x06hidden\x18\x07 \x01(\x08\x12\x10\n\x08recorder\x18\x08 \x01(\x08\x12\x1b\n\x13\x63\x61n_update_metadata\x18\n \x01(\x08\x12\r\n\x05\x61gent\x18\x0b \x01(\x08\"\xd1\x03\n\x0fParticipantInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\x10\n\x08identity\x18\x02 \x01(\t\x12-\n\x05state\x18\x03 \x01(\x0e\x32\x1e.livekit.ParticipantInfo.State\x12\"\n\x06tracks\x18\x04 \x03(\x0b\x32\x12.livekit.TrackInfo\x12\x10\n\x08metadata\x18\x05 \x01(\t\x12\x11\n\tjoined_at\x18\x06 \x01(\x03\x12\x0c\n\x04name\x18\t \x01(\t\x12\x0f\n\x07version\x18\n \x01(\r\x12\x32\n\npermission\x18\x0b \x01(\x0b\x32\x1e.livekit.ParticipantPermission\x12\x0e\n\x06region\x18\x0c \x01(\t\x12\x14\n\x0cis_publisher\x18\r \x01(\x08\x12+\n\x04kind\x18\x0e \x01(\x0e\x32\x1d.livekit.ParticipantInfo.Kind\">\n\x05State\x12\x0b\n\x07JOINING\x10\x00\x12\n\n\x06JOINED\x10\x01\x12\n\n\x06\x41\x43TIVE\x10\x02\x12\x10\n\x0c\x44ISCONNECTED\x10\x03\"A\n\x04Kind\x12\x0c\n\x08STANDARD\x10\x00\x12\x0b\n\x07INGRESS\x10\x01\x12\n\n\x06\x45GRESS\x10\x02\x12\x07\n\x03SIP\x10\x03\x12\t\n\x05\x41GENT\x10\x04\"3\n\nEncryption\"%\n\x04Type\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03GCM\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\"f\n\x12SimulcastCodecInfo\x12\x11\n\tmime_type\x18\x01 \x01(\t\x12\x0b\n\x03mid\x18\x02 \x01(\t\x12\x0b\n\x03\x63id\x18\x03 \x01(\t\x12#\n\x06layers\x18\x04 \x03(\x0b\x32\x13.livekit.VideoLayer\"\xc1\x03\n\tTrackInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12 \n\x04type\x18\x02 \x01(\x0e\x32\x12.livekit.TrackType\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\r\n\x05muted\x18\x04 \x01(\x08\x12\r\n\x05width\x18\x05 \x01(\r\x12\x0e\n\x06height\x18\x06 \x01(\r\x12\x11\n\tsimulcast\x18\x07 \x01(\x08\x12\x13\n\x0b\x64isable_dtx\x18\x08 \x01(\x08\x12$\n\x06source\x18\t \x01(\x0e\x32\x14.livekit.TrackSource\x12#\n\x06layers\x18\n \x03(\x0b\x32\x13.livekit.VideoLayer\x12\x11\n\tmime_type\x18\x0b \x01(\t\x12\x0b\n\x03mid\x18\x0c \x01(\t\x12+\n\x06\x63odecs\x18\r \x03(\x0b\x32\x1b.livekit.SimulcastCodecInfo\x12\x0e\n\x06stereo\x18\x0e \x01(\x08\x12\x13\n\x0b\x64isable_red\x18\x0f \x01(\x08\x12,\n\nencryption\x18\x10 \x01(\x0e\x32\x18.livekit.Encryption.Type\x12\x0e\n\x06stream\x18\x11 \x01(\t\x12&\n\x07version\x18\x12 \x01(\x0b\x32\x15.livekit.TimedVersion\"r\n\nVideoLayer\x12&\n\x07quality\x18\x01 \x01(\x0e\x32\x15.livekit.VideoQuality\x12\r\n\x05width\x18\x02 \x01(\r\x12\x0e\n\x06height\x18\x03 \x01(\r\x12\x0f\n\x07\x62itrate\x18\x04 \x01(\r\x12\x0c\n\x04ssrc\x18\x05 \x01(\r\"\xd1\x02\n\nDataPacket\x12*\n\x04kind\x18\x01 \x01(\x0e\x32\x18.livekit.DataPacket.KindB\x02\x18\x01\x12\x1c\n\x14participant_identity\x18\x04 \x01(\t\x12\x1e\n\x16\x64\x65stination_identities\x18\x05 \x03(\t\x12#\n\x04user\x18\x02 \x01(\x0b\x32\x13.livekit.UserPacketH\x00\x12\x33\n\x07speaker\x18\x03 \x01(\x0b\x32\x1c.livekit.ActiveSpeakerUpdateB\x02\x18\x01H\x00\x12$\n\x08sip_dtmf\x18\x06 \x01(\x0b\x32\x10.livekit.SipDTMFH\x00\x12/\n\rtranscription\x18\x07 \x01(\x0b\x32\x16.livekit.TranscriptionH\x00\"\x1f\n\x04Kind\x12\x0c\n\x08RELIABLE\x10\x00\x12\t\n\x05LOSSY\x10\x01\x42\x07\n\x05value\"=\n\x13\x41\x63tiveSpeakerUpdate\x12&\n\x08speakers\x18\x01 \x03(\x0b\x32\x14.livekit.SpeakerInfo\"9\n\x0bSpeakerInfo\x12\x0b\n\x03sid\x18\x01 \x01(\t\x12\r\n\x05level\x18\x02 \x01(\x02\x12\x0e\n\x06\x61\x63tive\x18\x03 \x01(\x08\"\xa0\x02\n\nUserPacket\x12\x1b\n\x0fparticipant_sid\x18\x01 \x01(\tB\x02\x18\x01\x12 \n\x14participant_identity\x18\x05 \x01(\tB\x02\x18\x01\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x1c\n\x10\x64\x65stination_sids\x18\x03 \x03(\tB\x02\x18\x01\x12\"\n\x16\x64\x65stination_identities\x18\x06 \x03(\tB\x02\x18\x01\x12\x12\n\x05topic\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x0f\n\x02id\x18\x08 \x01(\tH\x01\x88\x01\x01\x12\x17\n\nstart_time\x18\t \x01(\x04H\x02\x88\x01\x01\x12\x15\n\x08\x65nd_time\x18\n \x01(\x04H\x03\x88\x01\x01\x42\x08\n\x06_topicB\x05\n\x03_idB\r\n\x0b_start_timeB\x0b\n\t_end_time\"&\n\x07SipDTMF\x12\x0c\n\x04\x63ode\x18\x03 \x01(\r\x12\r\n\x05\x64igit\x18\x04 \x01(\t\"\x82\x01\n\rTranscription\x12\x1c\n\x14participant_identity\x18\x02 \x01(\t\x12\x10\n\x08track_id\x18\x03 \x01(\t\x12/\n\x08segments\x18\x04 \x03(\x0b\x32\x1d.livekit.TranscriptionSegment\x12\x10\n\x08language\x18\x05 \x01(\t\"e\n\x14TranscriptionSegment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x12\n\nstart_time\x18\x03 \x01(\x04\x12\x10\n\x08\x65nd_time\x18\x04 \x01(\x04\x12\r\n\x05\x66inal\x18\x05 \x01(\x08\"@\n\x11ParticipantTracks\x12\x17\n\x0fparticipant_sid\x18\x01 \x01(\t\x12\x12\n\ntrack_sids\x18\x02 \x03(\t\"\xce\x01\n\nServerInfo\x12,\n\x07\x65\x64ition\x18\x01 \x01(\x0e\x32\x1b.livekit.ServerInfo.Edition\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\x0e\n\x06region\x18\x04 \x01(\t\x12\x0f\n\x07node_id\x18\x05 \x01(\t\x12\x12\n\ndebug_info\x18\x06 \x01(\t\x12\x16\n\x0e\x61gent_protocol\x18\x07 \x01(\x05\"\"\n\x07\x45\x64ition\x12\x0c\n\x08Standard\x10\x00\x12\t\n\x05\x43loud\x10\x01\"\xdd\x02\n\nClientInfo\x12$\n\x03sdk\x18\x01 \x01(\x0e\x32\x17.livekit.ClientInfo.SDK\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\x05\x12\n\n\x02os\x18\x04 \x01(\t\x12\x12\n\nos_version\x18\x05 \x01(\t\x12\x14\n\x0c\x64\x65vice_model\x18\x06 \x01(\t\x12\x0f\n\x07\x62rowser\x18\x07 \x01(\t\x12\x17\n\x0f\x62rowser_version\x18\x08 \x01(\t\x12\x0f\n\x07\x61\x64\x64ress\x18\t \x01(\t\x12\x0f\n\x07network\x18\n \x01(\t\"\x83\x01\n\x03SDK\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x06\n\x02JS\x10\x01\x12\t\n\x05SWIFT\x10\x02\x12\x0b\n\x07\x41NDROID\x10\x03\x12\x0b\n\x07\x46LUTTER\x10\x04\x12\x06\n\x02GO\x10\x05\x12\t\n\x05UNITY\x10\x06\x12\x10\n\x0cREACT_NATIVE\x10\x07\x12\x08\n\x04RUST\x10\x08\x12\n\n\x06PYTHON\x10\t\x12\x07\n\x03\x43PP\x10\n\"\x8c\x02\n\x13\x43lientConfiguration\x12*\n\x05video\x18\x01 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12+\n\x06screen\x18\x02 \x01(\x0b\x32\x1b.livekit.VideoConfiguration\x12\x37\n\x11resume_connection\x18\x03 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\x12\x30\n\x0f\x64isabled_codecs\x18\x04 \x01(\x0b\x32\x17.livekit.DisabledCodecs\x12\x31\n\x0b\x66orce_relay\x18\x05 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"L\n\x12VideoConfiguration\x12\x36\n\x10hardware_encoder\x18\x01 \x01(\x0e\x32\x1c.livekit.ClientConfigSetting\"Q\n\x0e\x44isabledCodecs\x12\x1e\n\x06\x63odecs\x18\x01 \x03(\x0b\x32\x0e.livekit.Codec\x12\x1f\n\x07publish\x18\x02 \x03(\x0b\x32\x0e.livekit.Codec\"\x80\x02\n\x08RTPDrift\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x17\n\x0fstart_timestamp\x18\x04 \x01(\x04\x12\x15\n\rend_timestamp\x18\x05 \x01(\x04\x12\x17\n\x0frtp_clock_ticks\x18\x06 \x01(\x04\x12\x15\n\rdrift_samples\x18\x07 \x01(\x03\x12\x10\n\x08\x64rift_ms\x18\x08 \x01(\x01\x12\x12\n\nclock_rate\x18\t \x01(\x01\"\xa0\n\n\x08RTPStats\x12.\n\nstart_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x10\n\x08\x64uration\x18\x03 \x01(\x01\x12\x0f\n\x07packets\x18\x04 \x01(\r\x12\x13\n\x0bpacket_rate\x18\x05 \x01(\x01\x12\r\n\x05\x62ytes\x18\x06 \x01(\x04\x12\x14\n\x0cheader_bytes\x18\' \x01(\x04\x12\x0f\n\x07\x62itrate\x18\x07 \x01(\x01\x12\x14\n\x0cpackets_lost\x18\x08 \x01(\r\x12\x18\n\x10packet_loss_rate\x18\t \x01(\x01\x12\x1e\n\x16packet_loss_percentage\x18\n \x01(\x02\x12\x19\n\x11packets_duplicate\x18\x0b \x01(\r\x12\x1d\n\x15packet_duplicate_rate\x18\x0c \x01(\x01\x12\x17\n\x0f\x62ytes_duplicate\x18\r \x01(\x04\x12\x1e\n\x16header_bytes_duplicate\x18( \x01(\x04\x12\x19\n\x11\x62itrate_duplicate\x18\x0e \x01(\x01\x12\x17\n\x0fpackets_padding\x18\x0f \x01(\r\x12\x1b\n\x13packet_padding_rate\x18\x10 \x01(\x01\x12\x15\n\rbytes_padding\x18\x11 \x01(\x04\x12\x1c\n\x14header_bytes_padding\x18) \x01(\x04\x12\x17\n\x0f\x62itrate_padding\x18\x12 \x01(\x01\x12\x1c\n\x14packets_out_of_order\x18\x13 \x01(\r\x12\x0e\n\x06\x66rames\x18\x14 \x01(\r\x12\x12\n\nframe_rate\x18\x15 \x01(\x01\x12\x16\n\x0ejitter_current\x18\x16 \x01(\x01\x12\x12\n\njitter_max\x18\x17 \x01(\x01\x12:\n\rgap_histogram\x18\x18 \x03(\x0b\x32#.livekit.RTPStats.GapHistogramEntry\x12\r\n\x05nacks\x18\x19 \x01(\r\x12\x11\n\tnack_acks\x18% \x01(\r\x12\x13\n\x0bnack_misses\x18\x1a \x01(\r\x12\x15\n\rnack_repeated\x18& \x01(\r\x12\x0c\n\x04plis\x18\x1b \x01(\r\x12,\n\x08last_pli\x18\x1c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04\x66irs\x18\x1d \x01(\r\x12,\n\x08last_fir\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0brtt_current\x18\x1f \x01(\r\x12\x0f\n\x07rtt_max\x18  \x01(\r\x12\x12\n\nkey_frames\x18! \x01(\r\x12\x32\n\x0elast_key_frame\x18\" \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flayer_lock_plis\x18# \x01(\r\x12\x37\n\x13last_layer_lock_pli\x18$ \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\x0cpacket_drift\x18, \x01(\x0b\x32\x11.livekit.RTPDrift\x12\'\n\x0creport_drift\x18- \x01(\x0b\x32\x11.livekit.RTPDrift\x12/\n\x14rebased_report_drift\x18. \x01(\x0b\x32\x11.livekit.RTPDrift\x1a\x33\n\x11GapHistogramEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"1\n\x0cTimedVersion\x12\x12\n\nunix_micro\x18\x01 \x01(\x03\x12\r\n\x05ticks\x18\x02 \x01(\x05*/\n\nAudioCodec\x12\x0e\n\nDEFAULT_AC\x10\x00\x12\x08\n\x04OPUS\x10\x01\x12\x07\n\x03\x41\x41\x43\x10\x02*V\n\nVideoCodec\x12\x0e\n\nDEFAULT_VC\x10\x00\x12\x11\n\rH264_BASELINE\x10\x01\x12\r\n\tH264_MAIN\x10\x02\x12\r\n\tH264_HIGH\x10\x03\x12\x07\n\x03VP8\x10\x04*)\n\nImageCodec\x12\x0e\n\nIC_DEFAULT\x10\x00\x12\x0b\n\x07IC_JPEG\x10\x01*+\n\tTrackType\x12\t\n\x05\x41UDIO\x10\x00\x12\t\n\x05VIDEO\x10\x01\x12\x08\n\x04\x44\x41TA\x10\x02*`\n\x0bTrackSource\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06\x43\x41MERA\x10\x01\x12\x0e\n\nMICROPHONE\x10\x02\x12\x10\n\x0cSCREEN_SHARE\x10\x03\x12\x16\n\x12SCREEN_SHARE_AUDIO\x10\x04*6\n\x0cVideoQuality\x12\x07\n\x03LOW\x10\x00\x12\n\n\x06MEDIUM\x10\x01\x12\x08\n\x04HIGH\x10\x02\x12\x07\n\x03OFF\x10\x03*@\n\x11\x43onnectionQuality\x12\x08\n\x04POOR\x10\x00\x12\x08\n\x04GOOD\x10\x01\x12\r\n\tEXCELLENT\x10\x02\x12\x08\n\x04LOST\x10\x03*;\n\x13\x43lientConfigSetting\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x44ISABLED\x10\x01\x12\x0b\n\x07\x45NABLED\x10\x02*\xdb\x01\n\x10\x44isconnectReason\x12\x12\n\x0eUNKNOWN_REASON\x10\x00\x12\x14\n\x10\x43LIENT_INITIATED\x10\x01\x12\x16\n\x12\x44UPLICATE_IDENTITY\x10\x02\x12\x13\n\x0fSERVER_SHUTDOWN\x10\x03\x12\x17\n\x13PARTICIPANT_REMOVED\x10\x04\x12\x10\n\x0cROOM_DELETED\x10\x05\x12\x12\n\x0eSTATE_MISMATCH\x10\x06\x12\x10\n\x0cJOIN_FAILURE\x10\x07\x12\r\n\tMIGRATION\x10\x08\x12\x10\n\x0cSIGNAL_CLOSE\x10\t*\x89\x01\n\x0fReconnectReason\x12\x0e\n\nRR_UNKNOWN\x10\x00\x12\x1a\n\x16RR_SIGNAL_DISCONNECTED\x10\x01\x12\x17\n\x13RR_PUBLISHER_FAILED\x10\x02\x12\x18\n\x14RR_SUBSCRIBER_FAILED\x10\x03\x12\x17\n\x13RR_SWITCH_CANDIDATE\x10\x04*T\n\x11SubscriptionError\x12\x0e\n\nSE_UNKNOWN\x10\x00\x12\x18\n\x14SE_CODEC_UNSUPPORTED\x10\x01\x12\x15\n\x11SE_TRACK_NOTFOUND\x10\x02*\xa3\x01\n\x11\x41udioTrackFeature\x12\r\n\tTF_STEREO\x10\x00\x12\r\n\tTF_NO_DTX\x10\x01\x12\x18\n\x14TF_AUTO_GAIN_CONTROL\x10\x02\x12\x18\n\x14TF_ECHO_CANCELLATION\x10\x03\x12\x18\n\x14TF_NOISE_SUPPRESSION\x10\x04\x12\"\n\x1eTF_ENHANCED_NOISE_CANCELLATION\x10\x05\x42\x46Z#github.com/livekit/protocol/livekit\xaa\x02\rLiveKit.Proto\xea\x02\x0eLiveKit::Protob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'models', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z#github.com/livekit/protocol/livekit\252\002\rLiveKit.Proto\352\002\016LiveKit::Proto'
@@ -33,38 +33,38 @@
   _globals['_USERPACKET'].fields_by_name['participant_identity']._serialized_options = b'\030\001'
   _globals['_USERPACKET'].fields_by_name['destination_sids']._options = None
   _globals['_USERPACKET'].fields_by_name['destination_sids']._serialized_options = b'\030\001'
   _globals['_USERPACKET'].fields_by_name['destination_identities']._options = None
   _globals['_USERPACKET'].fields_by_name['destination_identities']._serialized_options = b'\030\001'
   _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._options = None
   _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_options = b'8\001'
-  _globals['_AUDIOCODEC']._serialized_start=5245
-  _globals['_AUDIOCODEC']._serialized_end=5292
-  _globals['_VIDEOCODEC']._serialized_start=5294
-  _globals['_VIDEOCODEC']._serialized_end=5380
-  _globals['_IMAGECODEC']._serialized_start=5382
-  _globals['_IMAGECODEC']._serialized_end=5423
-  _globals['_TRACKTYPE']._serialized_start=5425
-  _globals['_TRACKTYPE']._serialized_end=5468
-  _globals['_TRACKSOURCE']._serialized_start=5470
-  _globals['_TRACKSOURCE']._serialized_end=5566
-  _globals['_VIDEOQUALITY']._serialized_start=5568
-  _globals['_VIDEOQUALITY']._serialized_end=5622
-  _globals['_CONNECTIONQUALITY']._serialized_start=5624
-  _globals['_CONNECTIONQUALITY']._serialized_end=5688
-  _globals['_CLIENTCONFIGSETTING']._serialized_start=5690
-  _globals['_CLIENTCONFIGSETTING']._serialized_end=5749
-  _globals['_DISCONNECTREASON']._serialized_start=5752
-  _globals['_DISCONNECTREASON']._serialized_end=5971
-  _globals['_RECONNECTREASON']._serialized_start=5974
-  _globals['_RECONNECTREASON']._serialized_end=6111
-  _globals['_SUBSCRIPTIONERROR']._serialized_start=6113
-  _globals['_SUBSCRIPTIONERROR']._serialized_end=6197
-  _globals['_AUDIOTRACKFEATURE']._serialized_start=6200
-  _globals['_AUDIOTRACKFEATURE']._serialized_end=6363
+  _globals['_AUDIOCODEC']._serialized_start=5630
+  _globals['_AUDIOCODEC']._serialized_end=5677
+  _globals['_VIDEOCODEC']._serialized_start=5679
+  _globals['_VIDEOCODEC']._serialized_end=5765
+  _globals['_IMAGECODEC']._serialized_start=5767
+  _globals['_IMAGECODEC']._serialized_end=5808
+  _globals['_TRACKTYPE']._serialized_start=5810
+  _globals['_TRACKTYPE']._serialized_end=5853
+  _globals['_TRACKSOURCE']._serialized_start=5855
+  _globals['_TRACKSOURCE']._serialized_end=5951
+  _globals['_VIDEOQUALITY']._serialized_start=5953
+  _globals['_VIDEOQUALITY']._serialized_end=6007
+  _globals['_CONNECTIONQUALITY']._serialized_start=6009
+  _globals['_CONNECTIONQUALITY']._serialized_end=6073
+  _globals['_CLIENTCONFIGSETTING']._serialized_start=6075
+  _globals['_CLIENTCONFIGSETTING']._serialized_end=6134
+  _globals['_DISCONNECTREASON']._serialized_start=6137
+  _globals['_DISCONNECTREASON']._serialized_end=6356
+  _globals['_RECONNECTREASON']._serialized_start=6359
+  _globals['_RECONNECTREASON']._serialized_end=6496
+  _globals['_SUBSCRIPTIONERROR']._serialized_start=6498
+  _globals['_SUBSCRIPTIONERROR']._serialized_end=6582
+  _globals['_AUDIOTRACKFEATURE']._serialized_start=6585
+  _globals['_AUDIOTRACKFEATURE']._serialized_end=6748
   _globals['_ROOM']._serialized_start=67
   _globals['_ROOM']._serialized_end=396
   _globals['_CODEC']._serialized_start=398
   _globals['_CODEC']._serialized_end=438
   _globals['_PLAYOUTDELAY']._serialized_start=440
   _globals['_PLAYOUTDELAY']._serialized_end=497
   _globals['_PARTICIPANTPERMISSION']._serialized_start=500
@@ -82,43 +82,47 @@
   _globals['_SIMULCASTCODECINFO']._serialized_start=1245
   _globals['_SIMULCASTCODECINFO']._serialized_end=1347
   _globals['_TRACKINFO']._serialized_start=1350
   _globals['_TRACKINFO']._serialized_end=1799
   _globals['_VIDEOLAYER']._serialized_start=1801
   _globals['_VIDEOLAYER']._serialized_end=1915
   _globals['_DATAPACKET']._serialized_start=1918
-  _globals['_DATAPACKET']._serialized_end=2206
-  _globals['_DATAPACKET_KIND']._serialized_start=2166
-  _globals['_DATAPACKET_KIND']._serialized_end=2197
-  _globals['_ACTIVESPEAKERUPDATE']._serialized_start=2208
-  _globals['_ACTIVESPEAKERUPDATE']._serialized_end=2269
-  _globals['_SPEAKERINFO']._serialized_start=2271
-  _globals['_SPEAKERINFO']._serialized_end=2328
-  _globals['_USERPACKET']._serialized_start=2331
-  _globals['_USERPACKET']._serialized_end=2519
-  _globals['_SIPDTMF']._serialized_start=2521
-  _globals['_SIPDTMF']._serialized_end=2559
-  _globals['_PARTICIPANTTRACKS']._serialized_start=2561
-  _globals['_PARTICIPANTTRACKS']._serialized_end=2625
-  _globals['_SERVERINFO']._serialized_start=2628
-  _globals['_SERVERINFO']._serialized_end=2834
-  _globals['_SERVERINFO_EDITION']._serialized_start=2800
-  _globals['_SERVERINFO_EDITION']._serialized_end=2834
-  _globals['_CLIENTINFO']._serialized_start=2837
-  _globals['_CLIENTINFO']._serialized_end=3186
-  _globals['_CLIENTINFO_SDK']._serialized_start=3055
-  _globals['_CLIENTINFO_SDK']._serialized_end=3186
-  _globals['_CLIENTCONFIGURATION']._serialized_start=3189
-  _globals['_CLIENTCONFIGURATION']._serialized_end=3457
-  _globals['_VIDEOCONFIGURATION']._serialized_start=3459
-  _globals['_VIDEOCONFIGURATION']._serialized_end=3535
-  _globals['_DISABLEDCODECS']._serialized_start=3537
-  _globals['_DISABLEDCODECS']._serialized_end=3618
-  _globals['_RTPDRIFT']._serialized_start=3621
-  _globals['_RTPDRIFT']._serialized_end=3877
-  _globals['_RTPSTATS']._serialized_start=3880
-  _globals['_RTPSTATS']._serialized_end=5192
-  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_start=5141
-  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_end=5192
-  _globals['_TIMEDVERSION']._serialized_start=5194
-  _globals['_TIMEDVERSION']._serialized_end=5243
+  _globals['_DATAPACKET']._serialized_end=2255
+  _globals['_DATAPACKET_KIND']._serialized_start=2215
+  _globals['_DATAPACKET_KIND']._serialized_end=2246
+  _globals['_ACTIVESPEAKERUPDATE']._serialized_start=2257
+  _globals['_ACTIVESPEAKERUPDATE']._serialized_end=2318
+  _globals['_SPEAKERINFO']._serialized_start=2320
+  _globals['_SPEAKERINFO']._serialized_end=2377
+  _globals['_USERPACKET']._serialized_start=2380
+  _globals['_USERPACKET']._serialized_end=2668
+  _globals['_SIPDTMF']._serialized_start=2670
+  _globals['_SIPDTMF']._serialized_end=2708
+  _globals['_TRANSCRIPTION']._serialized_start=2711
+  _globals['_TRANSCRIPTION']._serialized_end=2841
+  _globals['_TRANSCRIPTIONSEGMENT']._serialized_start=2843
+  _globals['_TRANSCRIPTIONSEGMENT']._serialized_end=2944
+  _globals['_PARTICIPANTTRACKS']._serialized_start=2946
+  _globals['_PARTICIPANTTRACKS']._serialized_end=3010
+  _globals['_SERVERINFO']._serialized_start=3013
+  _globals['_SERVERINFO']._serialized_end=3219
+  _globals['_SERVERINFO_EDITION']._serialized_start=3185
+  _globals['_SERVERINFO_EDITION']._serialized_end=3219
+  _globals['_CLIENTINFO']._serialized_start=3222
+  _globals['_CLIENTINFO']._serialized_end=3571
+  _globals['_CLIENTINFO_SDK']._serialized_start=3440
+  _globals['_CLIENTINFO_SDK']._serialized_end=3571
+  _globals['_CLIENTCONFIGURATION']._serialized_start=3574
+  _globals['_CLIENTCONFIGURATION']._serialized_end=3842
+  _globals['_VIDEOCONFIGURATION']._serialized_start=3844
+  _globals['_VIDEOCONFIGURATION']._serialized_end=3920
+  _globals['_DISABLEDCODECS']._serialized_start=3922
+  _globals['_DISABLEDCODECS']._serialized_end=4003
+  _globals['_RTPDRIFT']._serialized_start=4006
+  _globals['_RTPDRIFT']._serialized_end=4262
+  _globals['_RTPSTATS']._serialized_start=4265
+  _globals['_RTPSTATS']._serialized_end=5577
+  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_start=5526
+  _globals['_RTPSTATS_GAPHISTOGRAMENTRY']._serialized_end=5577
+  _globals['_TIMEDVERSION']._serialized_start=5579
+  _globals['_TIMEDVERSION']._serialized_end=5628
 # @@protoc_insertion_point(module_scope)
```

### Comparing `livekit-protocol-0.4.0/livekit/protocol/models.pyi` & `livekit_protocol-0.5.0/livekit/protocol/models.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -342,34 +342,36 @@
     width: int
     height: int
     bitrate: int
     ssrc: int
     def __init__(self, quality: _Optional[_Union[VideoQuality, str]] = ..., width: _Optional[int] = ..., height: _Optional[int] = ..., bitrate: _Optional[int] = ..., ssrc: _Optional[int] = ...) -> None: ...
 
 class DataPacket(_message.Message):
-    __slots__ = ("kind", "participant_identity", "destination_identities", "user", "speaker", "sip_dtmf")
+    __slots__ = ("kind", "participant_identity", "destination_identities", "user", "speaker", "sip_dtmf", "transcription")
     class Kind(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         RELIABLE: _ClassVar[DataPacket.Kind]
         LOSSY: _ClassVar[DataPacket.Kind]
     RELIABLE: DataPacket.Kind
     LOSSY: DataPacket.Kind
     KIND_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
     DESTINATION_IDENTITIES_FIELD_NUMBER: _ClassVar[int]
     USER_FIELD_NUMBER: _ClassVar[int]
     SPEAKER_FIELD_NUMBER: _ClassVar[int]
     SIP_DTMF_FIELD_NUMBER: _ClassVar[int]
+    TRANSCRIPTION_FIELD_NUMBER: _ClassVar[int]
     kind: DataPacket.Kind
     participant_identity: str
     destination_identities: _containers.RepeatedScalarFieldContainer[str]
     user: UserPacket
     speaker: ActiveSpeakerUpdate
     sip_dtmf: SipDTMF
-    def __init__(self, kind: _Optional[_Union[DataPacket.Kind, str]] = ..., participant_identity: _Optional[str] = ..., destination_identities: _Optional[_Iterable[str]] = ..., user: _Optional[_Union[UserPacket, _Mapping]] = ..., speaker: _Optional[_Union[ActiveSpeakerUpdate, _Mapping]] = ..., sip_dtmf: _Optional[_Union[SipDTMF, _Mapping]] = ...) -> None: ...
+    transcription: Transcription
+    def __init__(self, kind: _Optional[_Union[DataPacket.Kind, str]] = ..., participant_identity: _Optional[str] = ..., destination_identities: _Optional[_Iterable[str]] = ..., user: _Optional[_Union[UserPacket, _Mapping]] = ..., speaker: _Optional[_Union[ActiveSpeakerUpdate, _Mapping]] = ..., sip_dtmf: _Optional[_Union[SipDTMF, _Mapping]] = ..., transcription: _Optional[_Union[Transcription, _Mapping]] = ...) -> None: ...
 
 class ActiveSpeakerUpdate(_message.Message):
     __slots__ = ("speakers",)
     SPEAKERS_FIELD_NUMBER: _ClassVar[int]
     speakers: _containers.RepeatedCompositeFieldContainer[SpeakerInfo]
     def __init__(self, speakers: _Optional[_Iterable[_Union[SpeakerInfo, _Mapping]]] = ...) -> None: ...
 
@@ -380,37 +382,69 @@
     ACTIVE_FIELD_NUMBER: _ClassVar[int]
     sid: str
     level: float
     active: bool
     def __init__(self, sid: _Optional[str] = ..., level: _Optional[float] = ..., active: bool = ...) -> None: ...
 
 class UserPacket(_message.Message):
-    __slots__ = ("participant_sid", "participant_identity", "payload", "destination_sids", "destination_identities", "topic")
+    __slots__ = ("participant_sid", "participant_identity", "payload", "destination_sids", "destination_identities", "topic", "id", "start_time", "end_time")
     PARTICIPANT_SID_FIELD_NUMBER: _ClassVar[int]
     PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
     PAYLOAD_FIELD_NUMBER: _ClassVar[int]
     DESTINATION_SIDS_FIELD_NUMBER: _ClassVar[int]
     DESTINATION_IDENTITIES_FIELD_NUMBER: _ClassVar[int]
     TOPIC_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    START_TIME_FIELD_NUMBER: _ClassVar[int]
+    END_TIME_FIELD_NUMBER: _ClassVar[int]
     participant_sid: str
     participant_identity: str
     payload: bytes
     destination_sids: _containers.RepeatedScalarFieldContainer[str]
     destination_identities: _containers.RepeatedScalarFieldContainer[str]
     topic: str
-    def __init__(self, participant_sid: _Optional[str] = ..., participant_identity: _Optional[str] = ..., payload: _Optional[bytes] = ..., destination_sids: _Optional[_Iterable[str]] = ..., destination_identities: _Optional[_Iterable[str]] = ..., topic: _Optional[str] = ...) -> None: ...
+    id: str
+    start_time: int
+    end_time: int
+    def __init__(self, participant_sid: _Optional[str] = ..., participant_identity: _Optional[str] = ..., payload: _Optional[bytes] = ..., destination_sids: _Optional[_Iterable[str]] = ..., destination_identities: _Optional[_Iterable[str]] = ..., topic: _Optional[str] = ..., id: _Optional[str] = ..., start_time: _Optional[int] = ..., end_time: _Optional[int] = ...) -> None: ...
 
 class SipDTMF(_message.Message):
     __slots__ = ("code", "digit")
     CODE_FIELD_NUMBER: _ClassVar[int]
     DIGIT_FIELD_NUMBER: _ClassVar[int]
     code: int
     digit: str
     def __init__(self, code: _Optional[int] = ..., digit: _Optional[str] = ...) -> None: ...
 
+class Transcription(_message.Message):
+    __slots__ = ("participant_identity", "track_id", "segments", "language")
+    PARTICIPANT_IDENTITY_FIELD_NUMBER: _ClassVar[int]
+    TRACK_ID_FIELD_NUMBER: _ClassVar[int]
+    SEGMENTS_FIELD_NUMBER: _ClassVar[int]
+    LANGUAGE_FIELD_NUMBER: _ClassVar[int]
+    participant_identity: str
+    track_id: str
+    segments: _containers.RepeatedCompositeFieldContainer[TranscriptionSegment]
+    language: str
+    def __init__(self, participant_identity: _Optional[str] = ..., track_id: _Optional[str] = ..., segments: _Optional[_Iterable[_Union[TranscriptionSegment, _Mapping]]] = ..., language: _Optional[str] = ...) -> None: ...
+
+class TranscriptionSegment(_message.Message):
+    __slots__ = ("id", "text", "start_time", "end_time", "final")
+    ID_FIELD_NUMBER: _ClassVar[int]
+    TEXT_FIELD_NUMBER: _ClassVar[int]
+    START_TIME_FIELD_NUMBER: _ClassVar[int]
+    END_TIME_FIELD_NUMBER: _ClassVar[int]
+    FINAL_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    text: str
+    start_time: int
+    end_time: int
+    final: bool
+    def __init__(self, id: _Optional[str] = ..., text: _Optional[str] = ..., start_time: _Optional[int] = ..., end_time: _Optional[int] = ..., final: bool = ...) -> None: ...
+
 class ParticipantTracks(_message.Message):
     __slots__ = ("participant_sid", "track_sids")
     PARTICIPANT_SID_FIELD_NUMBER: _ClassVar[int]
     TRACK_SIDS_FIELD_NUMBER: _ClassVar[int]
     participant_sid: str
     track_sids: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, participant_sid: _Optional[str] = ..., track_sids: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `livekit-protocol-0.4.0/livekit/protocol/room.py` & `livekit_protocol-0.5.0/livekit/protocol/room.py`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/room.pyi` & `livekit_protocol-0.5.0/livekit/protocol/room.pyi`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/webhook.py` & `livekit_protocol-0.5.0/livekit/protocol/webhook.py`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit/protocol/webhook.pyi` & `livekit_protocol-0.5.0/livekit/protocol/webhook.pyi`

 * *Files identical despite different names*

### Comparing `livekit-protocol-0.4.0/livekit_protocol.egg-info/PKG-INFO` & `livekit_protocol-0.5.0/livekit_protocol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-protocol
-Version: 0.4.0
+Version: 0.5.0
 Summary: Python protocol stubs for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit-protocol-0.4.0/livekit_protocol.egg-info/SOURCES.txt` & `livekit_protocol-0.5.0/livekit_protocol.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 livekit/protocol/ingress.py
 livekit/protocol/ingress.pyi
 livekit/protocol/models.py
 livekit/protocol/models.pyi
 livekit/protocol/py.typed
 livekit/protocol/room.py
 livekit/protocol/room.pyi
+livekit/protocol/sip.py
+livekit/protocol/sip.pyi
 livekit/protocol/version.py
 livekit/protocol/webhook.py
 livekit/protocol/webhook.pyi
 livekit_protocol.egg-info/PKG-INFO
 livekit_protocol.egg-info/SOURCES.txt
 livekit_protocol.egg-info/dependency_links.txt
 livekit_protocol.egg-info/requires.txt
```

### Comparing `livekit-protocol-0.4.0/setup.py` & `livekit_protocol-0.5.0/setup.py`

 * *Files identical despite different names*

