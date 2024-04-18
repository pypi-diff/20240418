# Comparing `tmp/tetos-0.0.1.tar.gz` & `tmp/tetos-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tetos-0.0.1.tar", last modified: Wed Apr 17 10:06:52 2024, max compression
+gzip compressed data, was "tetos-0.0.2.tar", last modified: Wed Apr 17 12:52:44 2024, max compression
```

## Comparing `tetos-0.0.1.tar` & `tetos-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      551 2024-04-17 10:06:49.180806 tetos-0.0.1/LICENSE
--rw-r--r--   0        0        0     1582 2024-04-17 10:06:49.180806 tetos-0.0.1/README.md
--rw-r--r--   0        0        0     1336 2024-04-17 10:06:52.464830 tetos-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/__init__.py
--rw-r--r--   0        0        0      806 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/__main__.py
--rw-r--r--   0        0        0     3469 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/azure.py
--rw-r--r--   0        0        0     1924 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/base.py
--rw-r--r--   0        0        0     9868 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/consts.py
--rw-r--r--   0        0        0     2116 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/edge.py
--rw-r--r--   0        0        0     2826 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/openai.py
--rw-r--r--   0        0        0     8566 2024-04-17 10:06:49.180806 tetos-0.0.1/src/tetos/volc.py
--rw-r--r--   0        0        0     1624 2024-04-17 10:06:49.180806 tetos-0.0.1/tests/test_speakers.py
--rw-r--r--   0        0        0     2593 1970-01-01 00:00:00.000000 tetos-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      551 2024-04-17 12:52:34.963584 tetos-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1999 2024-04-17 12:52:34.963584 tetos-0.0.2/README.md
+-rw-r--r--   0        0        0     1377 2024-04-17 12:52:44.531483 tetos-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/__init__.py
+-rw-r--r--   0        0        0      855 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/__main__.py
+-rw-r--r--   0        0        0     3382 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/azure.py
+-rw-r--r--   0        0        0     2394 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/base.py
+-rw-r--r--   0        0        0     9868 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/consts.py
+-rw-r--r--   0        0        0     2016 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/edge.py
+-rw-r--r--   0        0        0     4291 2024-04-17 12:52:34.963584 tetos-0.0.2/src/tetos/google.py
+-rw-r--r--   0        0        0     2726 2024-04-17 12:52:34.967584 tetos-0.0.2/src/tetos/openai.py
+-rw-r--r--   0        0        0     8720 2024-04-17 12:52:34.967584 tetos-0.0.2/src/tetos/volc.py
+-rw-r--r--   0        0        0     1624 2024-04-17 12:52:34.967584 tetos-0.0.2/tests/test_speakers.py
+-rw-r--r--   0        0        0     3059 1970-01-01 00:00:00.000000 tetos-0.0.2/PKG-INFO
```

### Comparing `tetos-0.0.1/LICENSE` & `tetos-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tetos-0.0.1/README.md` & `tetos-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 - [Azure TTS](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/text-to-speech)
 
   Required parameters(Please refer to the documentation to get the secrets):
 
   - `speech_key`: Azure Speech service key
   - `service_region`: Azure Speech service region
 
+- [Google TTS](https://cloud.google.com/text-to-speech?hl=zh-CN)
+
+  Requirements:
+
+  - [Enable the Text-to-Speech API in the Google Cloud Console](https://console.developers.google.com/apis/api/texttospeech.googleapis.com/overview?project=586547753837)
+  - Environment variables `GOOGLE_APPLICATION_CREDENTIALS` pointing to the service account key file
+
 - [Volcengine TTS(火山引擎)](https://console.volcengine.com/sami)
 
   Required parameters:
 
   - `access_key`: Volcengine access key ID. ([Get it here](https://console.volcengine.com/iam/keymanage/))
   - `secret_key`: Volcengine access secret key. ([Get it here](https://console.volcengine.com/iam/keymanage/))
   - `app_key`: Volcengine app key
@@ -46,22 +53,26 @@
 
 ## API Usage
 
 Use Azure TTS as an example:
 
 ```python
 from tetos.azure import AzureSpeaker
-import asyncio
-
-async def main():
-    speaker = AzureSpeaker(speech_key='...', service_region='...')
-    await speaker.synthesize('Hello, world!', 'output.mp3')
 
-if __name__ == '__main__':
-    asyncio.run(main())
+speaker = AzureSpeaker(speech_key='...', speech_region='...')
+speaker.say('Hello, world!', 'output.mp3')
 ```
 
 The initialization parameters may be different for other providers.
 
+## Behind a proxy
+
+TeTos respects the proxy environment variables `HTTP_PROXY`, `HTTPS_PROXY`, `ALL_PROXY` and `NO_PROXY`.
+
+## TODO
+
+- [x] Google TTS
+- [ ] SSML support
+
 ## License
 
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
```

### Comparing `tetos-0.0.1/pyproject.toml` & `tetos-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 dependencies = [
     "edge-tts>=6.1.10",
     "openai>=1.20.0",
     "mutagen>=1.47.0",
     "azure-cognitiveservices-speech>=1.37.0",
     "anyio>=4.3.0",
     "click>=8.1.7",
+    "google-cloud-texttospeech>=2.16.3",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
 keywords = [
     "tts",
     "text-to-speech",
@@ -30,15 +31,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.0.1"
+version = "0.0.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 Repository = "https://github.com/frostming/tetos"
```

### Comparing `tetos-0.0.1/src/tetos/__main__.py` & `tetos-0.0.2/src/tetos/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 import click
 
 from .azure import AzureSpeaker
 from .edge import EdgeSpeaker
+from .google import GoogleSpeaker
 from .openai import OpenAISpeaker
 from .volc import VolcSpeaker
 
 
 def setup_logger(debug: bool = False):
     logger = logging.getLogger("tetos")
     handler = logging.StreamHandler()
@@ -18,13 +19,13 @@
 
 @click.group(context_settings={"show_default": True})
 @click.option("--verbose", "-v", is_flag=True, help="Enable verbose logging.")
 def tts(verbose: bool) -> None:
     setup_logger(verbose)
 
 
-for speaker in (OpenAISpeaker, EdgeSpeaker, AzureSpeaker, VolcSpeaker):
+for speaker in (OpenAISpeaker, EdgeSpeaker, AzureSpeaker, VolcSpeaker, GoogleSpeaker):
     tts.add_command(speaker.get_command())
 
 
 if __name__ == "__main__":
     tts()
```

### Comparing `tetos-0.0.1/src/tetos/azure.py` & `tetos-0.0.2/src/tetos/azure.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,11 +86,10 @@
         )
         @click.option("--voice", default="en-US-AriaNeural", help="The voice to use.")
         @common_options(cls)
         def azure(
             speech_key: str, speech_region: str, voice: str, text: str, output: str
         ) -> None:
             speaker = cls(speech_key, speech_region, voice=voice)
-            anyio.run(speaker.synthesize, text, Path(output))
-            click.echo(f"Speech generated successfully at {output}")
+            speaker.say(text, Path(output))
 
         return azure
```

### Comparing `tetos-0.0.1/src/tetos/consts.py` & `tetos-0.0.2/src/tetos/consts.py`

 * *Files identical despite different names*

### Comparing `tetos-0.0.1/src/tetos/edge.py` & `tetos-0.0.2/src/tetos/edge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dataclasses import dataclass
 from pathlib import Path
 
-import anyio
 import click
 
 from .base import Speaker, SynthesizeError, common_options
 from .consts import AZURE_SUPPORTED_VOICES
 
 
 @dataclass
@@ -53,11 +52,10 @@
         @click.option("--pitch", default="+0Hz", help="The pitch of speech.")
         @click.option("--volume", default="+0%", help="The volume of speech.")
         @common_options(cls)
         def edge(
             voice: str, rate: str, pitch: str, volume: str, text: str, output: str
         ) -> None:
             speaker = cls(voice=voice, rate=rate, pitch=pitch, volume=volume)
-            anyio.run(speaker.synthesize, text, Path(output))
-            click.echo(f"Speech generated successfully at {output}")
+            speaker.say(text, Path(output))
 
         return edge
```

### Comparing `tetos-0.0.1/src/tetos/openai.py` & `tetos-0.0.2/src/tetos/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 from typing import cast
 
-import anyio
 import click
 import mutagen.mp3
 
 from .base import Speaker, common_options
 
 
 class OpenAISpeaker(Speaker):
@@ -84,11 +83,10 @@
             speaker = cls(
                 model=model,
                 voice=voice,
                 speed=speed,
                 api_key=api_key,
                 api_base=api_base,
             )
-            anyio.run(speaker.synthesize, text, Path(output))
-            click.echo(f"Speech generated successfully at {output}")
+            speaker.say(text, Path(output))
 
         return openai
```

### Comparing `tetos-0.0.1/src/tetos/volc.py` & `tetos-0.0.2/src/tetos/volc.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,25 +171,32 @@
             "token": await self._ensure_token(),
             "namespace": "TTS",
             "payload": tts_payload,
         }
 
         resp = await self.client.post(self.SAMI_API_URL, json=req)
         if resp.is_error:
-            logger.error("Failed to get tts: %s", resp.text)
-            raise SynthesizeError("Failed to get tts from volcengine")
+            raise self._get_error(resp)
         data = resp.json()
         if data["status_code"] == 20000000 and len(data["data"]) > 0:
             file = anyio.Path(out_file)
             async with await file.open("wb") as f:
                 await f.write(base64.b64decode(data["data"]))
             payload = json.loads(data["payload"])
             return cast(float, payload["duration"])
         raise SynthesizeError("Failed to get tts from volcengine")
 
+    def _get_error(self, resp: Response) -> SynthesizeError:
+        logger.error("Failed to get tts from volcengine: %s", resp.text)
+        try:
+            data = resp.json()
+            return SynthesizeError(data["status_text"])
+        except Exception:
+            return SynthesizeError("Failed to get tts from volcengine")
+
     @classmethod
     def list_voices(cls) -> list[str]:
         return VOLC_SUPPORTED_VOICES
 
     @classmethod
     def get_command(cls) -> click.Command:
         @click.command()
@@ -239,11 +246,10 @@
                 secret_key,
                 app_key,
                 voice=voice,
                 sample_rate=sample_rate,
                 speech_rate=speech_rate,
                 pitch_rate=pitch_rate,
             )
-            anyio.run(speaker.synthesize, text, Path(output))
-            click.echo(f"Speech generated successfully at {output}")
+            speaker.say(text, Path(output))
 
         return volc
```

### Comparing `tetos-0.0.1/tests/test_speakers.py` & `tetos-0.0.2/tests/test_speakers.py`

 * *Files identical despite different names*

### Comparing `tetos-0.0.1/PKG-INFO` & `tetos-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tetos
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unified interface for multiple Text-to-Speech (TTS) providers
 Keywords: tts,text-to-speech,speech,audio,ai,nlp
 Author-Email: Frost Ming <me@frostming.com>
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,15 @@
 Requires-Python: >=3.8
 Requires-Dist: edge-tts>=6.1.10
 Requires-Dist: openai>=1.20.0
 Requires-Dist: mutagen>=1.47.0
 Requires-Dist: azure-cognitiveservices-speech>=1.37.0
 Requires-Dist: anyio>=4.3.0
 Requires-Dist: click>=8.1.7
+Requires-Dist: google-cloud-texttospeech>=2.16.3
 Description-Content-Type: text/markdown
 
 # TeToS
 
 A unified interface for multiple Text-to-Speech (TTS) providers.
 
 
@@ -41,14 +42,21 @@
 - [Azure TTS](https://docs.microsoft.com/en-us/azure/cognitive-services/speech-service/text-to-speech)
 
   Required parameters(Please refer to the documentation to get the secrets):
 
   - `speech_key`: Azure Speech service key
   - `service_region`: Azure Speech service region
 
+- [Google TTS](https://cloud.google.com/text-to-speech?hl=zh-CN)
+
+  Requirements:
+
+  - [Enable the Text-to-Speech API in the Google Cloud Console](https://console.developers.google.com/apis/api/texttospeech.googleapis.com/overview?project=586547753837)
+  - Environment variables `GOOGLE_APPLICATION_CREDENTIALS` pointing to the service account key file
+
 - [Volcengine TTS(火山引擎)](https://console.volcengine.com/sami)
 
   Required parameters:
 
   - `access_key`: Volcengine access key ID. ([Get it here](https://console.volcengine.com/iam/keymanage/))
   - `secret_key`: Volcengine access secret key. ([Get it here](https://console.volcengine.com/iam/keymanage/))
   - `app_key`: Volcengine app key
@@ -72,22 +80,26 @@
 
 ## API Usage
 
 Use Azure TTS as an example:
 
 ```python
 from tetos.azure import AzureSpeaker
-import asyncio
-
-async def main():
-    speaker = AzureSpeaker(speech_key='...', service_region='...')
-    await speaker.synthesize('Hello, world!', 'output.mp3')
 
-if __name__ == '__main__':
-    asyncio.run(main())
+speaker = AzureSpeaker(speech_key='...', speech_region='...')
+speaker.say('Hello, world!', 'output.mp3')
 ```
 
 The initialization parameters may be different for other providers.
 
+## Behind a proxy
+
+TeTos respects the proxy environment variables `HTTP_PROXY`, `HTTPS_PROXY`, `ALL_PROXY` and `NO_PROXY`.
+
+## TODO
+
+- [x] Google TTS
+- [ ] SSML support
+
 ## License
 
 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
```

