# Comparing `tmp/livekit-0.9.1.tar.gz` & `tmp/livekit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit-0.9.1.tar", last modified: Wed Feb 14 22:23:28 2024, max compression
+gzip compressed data, was "livekit-0.9.2.tar", last modified: Wed Mar 27 17:01:01 2024, max compression
```

## Comparing `livekit-0.9.1.tar` & `livekit-0.9.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.705911 livekit-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-14 22:23:28.705911 livekit-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-02-14 22:23:15.000000 livekit-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.697911 livekit-0.9.1/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.701911 livekit-0.9.1/livekit/rtc/
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_ffi_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.705911 livekit-0.9.1/livekit/rtc/_proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/audio_frame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/audio_frame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/e2ee_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/e2ee_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/ffi_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28780 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/ffi_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/handle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/participant_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/participant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/room_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    57765 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/room_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23553 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/stats_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    72100 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/track_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/track_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/video_frame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_proto/video_frame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/audio_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/audio_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/audio_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/e2ee.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/participant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.705911 livekit-0.9.1/livekit/rtc/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/room.py
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/track_publication.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/video_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/video_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-02-14 22:23:15.000000 livekit-0.9.1/livekit/rtc/video_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.705911 livekit-0.9.1/livekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-14 22:23:28.000000 livekit-0.9.1/livekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-14 22:23:28.000000 livekit-0.9.1/livekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 22:23:28.000000 livekit-0.9.1/livekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-14 22:23:28.000000 livekit-0.9.1/livekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-14 22:23:28.000000 livekit-0.9.1/livekit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-02-14 22:23:15.000000 livekit-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 22:23:28.705911 livekit-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-14 22:23:15.000000 livekit-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:23:28.705911 livekit-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-14 22:23:15.000000 livekit-0.9.1/tests/test_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.737252 livekit-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 17:01:01.737252 livekit-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-27 17:00:51.000000 livekit-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.729252 livekit-0.9.2/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.733252 livekit-0.9.2/livekit/rtc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_ffi_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.733252 livekit-0.9.2/livekit/rtc/_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/audio_frame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19052 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/audio_frame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/e2ee_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/e2ee_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/ffi_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28780 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/ffi_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/handle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/participant_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/participant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/room_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57765 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/room_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23553 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/stats_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72100 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/track_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/track_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/video_frame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21530 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_proto/video_frame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/audio_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/audio_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/audio_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/e2ee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.733252 livekit-0.9.2/livekit/rtc/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16966 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/track_publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/video_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/video_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-03-27 17:00:51.000000 livekit-0.9.2/livekit/rtc/video_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.733252 livekit-0.9.2/livekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 17:01:01.000000 livekit-0.9.2/livekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-27 17:01:01.000000 livekit-0.9.2/livekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:01:01.000000 livekit-0.9.2/livekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-27 17:01:01.000000 livekit-0.9.2/livekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-27 17:01:01.000000 livekit-0.9.2/livekit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-27 17:00:51.000000 livekit-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 17:01:01.737252 livekit-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-27 17:00:51.000000 livekit-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:01:01.733252 livekit-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-27 17:00:51.000000 livekit-0.9.2/tests/test_chat.py
```

### Comparing `livekit-0.9.1/PKG-INFO` & `livekit-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python Real-time SDK for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit-0.9.1/livekit/rtc/__init__.py` & `livekit-0.9.2/livekit/rtc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,66 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""LiveKit RTC SDK
-"""
+"""LiveKit RTC SDK"""
 
+from ._proto import stats_pb2 as stats
+from ._proto.e2ee_pb2 import EncryptionState, EncryptionType
 from ._proto.room_pb2 import (
     ConnectionQuality,
     ConnectionState,
-    DataPacketKind,
-    TrackPublishOptions,
-    IceTransportType,
     ContinualGatheringPolicy,
+    DataPacketKind,
     IceServer,
+    IceTransportType,
+    TrackPublishOptions,
 )
-from ._proto.e2ee_pb2 import EncryptionType, EncryptionState
 from ._proto.track_pb2 import StreamState, TrackKind, TrackSource
 from ._proto.video_frame_pb2 import VideoBufferType, VideoRotation
-from ._proto import stats_pb2 as stats
 from .audio_frame import AudioFrame
 from .audio_source import AudioSource
-from .audio_stream import AudioStream, AudioFrameEvent
+from .audio_stream import AudioFrameEvent, AudioStream
+from .chat import ChatManager, ChatMessage
+from .e2ee import (
+    E2EEManager,
+    E2EEOptions,
+    FrameCryptor,
+    KeyProvider,
+    KeyProviderOptions,
+)
 from .participant import LocalParticipant, Participant, RemoteParticipant
-from .room import ConnectError, Room, RoomOptions, RtcConfiguration, DataPacket
+from .room import ConnectError, DataPacket, Room, RoomOptions, RtcConfiguration
 from .track import (
+    AudioTrack,
     LocalAudioTrack,
+    LocalTrack,
     LocalVideoTrack,
     RemoteAudioTrack,
+    RemoteTrack,
     RemoteVideoTrack,
     Track,
-    LocalTrack,
-    RemoteTrack,
-    AudioTrack,
     VideoTrack,
 )
-from .e2ee import (
-    E2EEManager,
-    E2EEOptions,
-    KeyProviderOptions,
-    KeyProvider,
-    FrameCryptor,
-)
 from .track_publication import (
     LocalTrackPublication,
     RemoteTrackPublication,
     TrackPublication,
 )
+from .version import __version__
 from .video_frame import (
     VideoFrame,
 )
 from .video_source import VideoSource
-from .video_stream import VideoStream, VideoFrameEvent
-from .chat import ChatManager, ChatMessage
-
-from .version import __version__
+from .video_stream import VideoFrameEvent, VideoStream
 
 __all__ = [
     "ConnectionQuality",
     "ConnectionState",
     "DataPacketKind",
     "TrackPublishOptions",
     "IceTransportType",
```

### Comparing `livekit-0.9.1/livekit/rtc/_event_emitter.py` & `livekit-0.9.2/livekit/rtc/_event_emitter.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_ffi_client.py` & `livekit-0.9.2/livekit/rtc/_ffi_client.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/audio_frame_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/audio_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/audio_frame_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/audio_frame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/e2ee_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/e2ee_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/e2ee_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/e2ee_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/ffi_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/ffi_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/ffi_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/ffi_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/handle_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/handle_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/handle_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/participant_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/participant_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/participant_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/participant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/room_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/room_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/room_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/room_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/stats_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/stats_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/stats_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/track_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/track_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/track_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/track_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/video_frame_pb2.py` & `livekit-0.9.2/livekit/rtc/_proto/video_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_proto/video_frame_pb2.pyi` & `livekit-0.9.2/livekit/rtc/_proto/video_frame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/_utils.py` & `livekit-0.9.2/livekit/rtc/_utils.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/audio_frame.py` & `livekit-0.9.2/livekit/rtc/audio_frame.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/audio_source.py` & `livekit-0.9.2/livekit/rtc/audio_source.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/audio_stream.py` & `livekit-0.9.2/livekit/rtc/audio_stream.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/chat.py` & `livekit-0.9.2/livekit/rtc/chat.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/e2ee.py` & `livekit-0.9.2/livekit/rtc/e2ee.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/participant.py` & `livekit-0.9.2/livekit/rtc/participant.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/room.py` & `livekit-0.9.2/livekit/rtc/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
 import ctypes
 import logging
 from dataclasses import dataclass, field
-from typing import Dict, Optional, Literal
-from ._ffi_client import FfiHandle, FfiClient
+from typing import Dict, Literal, Optional
+
+from ._event_emitter import EventEmitter
+from ._ffi_client import FfiClient, FfiHandle
 from ._proto import ffi_pb2 as proto_ffi
 from ._proto import participant_pb2 as proto_participant
 from ._proto import room_pb2 as proto_room
 from ._proto.room_pb2 import ConnectionState
 from ._proto.track_pb2 import TrackKind
 from ._utils import BroadcastQueue
-from ._event_emitter import EventEmitter
 from .e2ee import E2EEManager, E2EEOptions
 from .participant import LocalParticipant, Participant, RemoteParticipant
 from .track import RemoteAudioTrack, RemoteVideoTrack
 from .track_publication import RemoteTrackPublication
 
 EventTypes = Literal[
     "participant_connected",
@@ -76,17 +77,17 @@
     rtc_config: Optional[RtcConfiguration] = None
 
 
 @dataclass
 class DataPacket:
     data: bytes
     kind: proto_room.DataPacketKind.ValueType
-    participant: Optional[
-        RemoteParticipant
-    ] = None  # None when the data has been sent by a server SDK
+    participant: Optional[RemoteParticipant] = (
+        None  # None when the data has been sent by a server SDK
+    )
     topic: Optional[str] = None
 
 
 class ConnectError(Exception):
     def __init__(self, message: str):
         self.message = message
```

### Comparing `livekit-0.9.1/livekit/rtc/track.py` & `livekit-0.9.2/livekit/rtc/track.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/track_publication.py` & `livekit-0.9.2/livekit/rtc/track_publication.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/video_frame.py` & `livekit-0.9.2/livekit/rtc/video_frame.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/video_source.py` & `livekit-0.9.2/livekit/rtc/video_source.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit/rtc/video_stream.py` & `livekit-0.9.2/livekit/rtc/video_stream.py`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/livekit.egg-info/PKG-INFO` & `livekit-0.9.2/livekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python Real-time SDK for LiveKit
 Home-page: https://github.com/livekit/python-sdks
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/python-sdks/
 Keywords: webrtc,realtime,audio,video,livekit
```

### Comparing `livekit-0.9.1/livekit.egg-info/SOURCES.txt` & `livekit-0.9.2/livekit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 livekit/rtc/_utils.py
 livekit/rtc/audio_frame.py
 livekit/rtc/audio_source.py
 livekit/rtc/audio_stream.py
 livekit/rtc/chat.py
 livekit/rtc/e2ee.py
 livekit/rtc/participant.py
+livekit/rtc/py.typed
 livekit/rtc/room.py
 livekit/rtc/track.py
 livekit/rtc/track_publication.py
 livekit/rtc/version.py
 livekit/rtc/video_frame.py
 livekit/rtc/video_source.py
 livekit/rtc/video_stream.py
```

### Comparing `livekit-0.9.1/pyproject.toml` & `livekit-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `livekit-0.9.1/setup.py` & `livekit-0.9.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import pathlib
-import setuptools
-import setuptools.command.build_py
-from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
-from wheel.bdist_wheel import get_platform
+from typing import Any, Dict
+
+import setuptools  # type: ignore
+import setuptools.command.build_py  # type: ignore
+from wheel.bdist_wheel import bdist_wheel as _bdist_wheel  # type: ignore
+from wheel.bdist_wheel import get_platform  # type: ignore
 
 here = pathlib.Path(__file__).parent.resolve()
-about = {}
+about: Dict[Any, Any] = {}
 with open(os.path.join(here, "livekit", "rtc", "version.py"), "r") as f:
     exec(f.read(), about)
 
 
 class bdist_wheel(_bdist_wheel):
     def finalize_options(self):
         self.plat_name = get_platform(None)  # force a platform tag
```

### Comparing `livekit-0.9.1/tests/test_chat.py` & `livekit-0.9.2/tests/test_chat.py`

 * *Files identical despite different names*

