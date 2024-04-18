# Comparing `tmp/hume-0.4.2.tar.gz` & `tmp/hume-0.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.4.2.tar", max compression
+gzip compressed data, was "hume-0.5.0rc1.tar", max compression
```

## Comparing `hume-0.4.2.tar` & `hume-0.5.0rc1.tar`

### file list

```diff
@@ -1,37 +1,53 @@
--rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.4.2/LICENSE
--rw-r--r--   0        0        0     2414 2023-12-04 20:35:41.602295 hume-0.4.2/README.md
--rw-r--r--   0        0        0      567 2023-06-29 18:23:24.723354 hume-0.4.2/hume/__init__.py
--rw-r--r--   0        0        0      500 2023-06-29 18:23:24.723574 hume-0.4.2/hume/_batch/__init__.py
--rw-r--r--   0        0        0     4336 2023-11-09 21:12:31.406291 hume-0.4.2/hume/_batch/batch_job.py
--rw-r--r--   0        0        0     6007 2023-11-09 21:00:59.607768 hume-0.4.2/hume/_batch/batch_job_details.py
--rw-r--r--   0        0        0      630 2023-11-09 21:01:00.346348 hume-0.4.2/hume/_batch/batch_job_state.py
--rw-r--r--   0        0        0      993 2023-11-09 21:01:01.114331 hume-0.4.2/hume/_batch/batch_job_status.py
--rw-r--r--   0        0        0    10868 2023-11-09 21:01:02.745157 hume-0.4.2/hume/_batch/hume_batch_client.py
--rw-r--r--   0        0        0      939 2023-11-09 21:01:03.627916 hume-0.4.2/hume/_batch/transcription_config.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.4.2/hume/_common/__init__.py
--rw-r--r--   0        0        0      145 2024-03-05 16:15:59.860210 hume-0.4.2/hume/_common/api_type.py
--rw-r--r--   0        0        0     1459 2023-11-09 21:00:54.653998 hume-0.4.2/hume/_common/client_base.py
--rw-r--r--   0        0        0     1803 2023-11-09 21:12:31.406497 hume-0.4.2/hume/_common/config_base.py
--rw-r--r--   0        0        0     2319 2023-11-09 21:12:31.406677 hume-0.4.2/hume/_common/config_utils.py
--rw-r--r--   0        0        0     3544 2023-11-09 21:12:31.406859 hume-0.4.2/hume/_common/retry_utils.py
--rw-r--r--   0        0        0       19 2024-03-05 15:28:25.149122 hume-0.4.2/hume/_common/socket/__init__.py
--rw-r--r--   0        0        0      191 2023-06-29 18:23:24.725504 hume-0.4.2/hume/_stream/__init__.py
--rw-r--r--   0        0        0     4437 2023-11-09 21:12:31.407053 hume-0.4.2/hume/_stream/hume_stream_client.py
--rw-r--r--   0        0        0     9778 2023-11-09 21:12:31.407378 hume-0.4.2/hume/_stream/stream_socket.py
--rw-r--r--   0        0        0      191 2024-03-05 15:28:05.626416 hume-0.4.2/hume/_voice/__init__.py
--rw-r--r--   0        0        0     4576 2024-03-05 16:16:41.541596 hume-0.4.2/hume/_voice/hume_voice_client.py
--rw-r--r--   0        0        0     9736 2024-03-05 16:20:47.940091 hume-0.4.2/hume/_voice/voice_socket.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.4.2/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.4.2/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       96 2023-06-29 18:23:24.726302 hume-0.4.2/hume/models/__init__.py
--rw-r--r--   0        0        0      587 2023-06-29 18:23:24.726358 hume-0.4.2/hume/models/config/__init__.py
--rw-r--r--   0        0        0      497 2023-11-09 20:57:38.956825 hume-0.4.2/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2573 2023-11-09 20:57:39.824281 hume-0.4.2/hume/models/config/face_config.py
--rw-r--r--   0        0        0      509 2023-11-09 20:57:40.714740 hume-0.4.2/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2235 2023-11-09 20:57:41.603323 hume-0.4.2/hume/models/config/language_config.py
--rw-r--r--   0        0        0      631 2023-11-09 21:12:31.407759 hume-0.4.2/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1000 2023-11-09 21:00:35.504654 hume-0.4.2/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1785 2023-11-09 21:00:36.417937 hume-0.4.2/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      804 2023-11-09 21:00:37.205021 hume-0.4.2/hume/models/model_type.py
--rw-r--r--   0        0        0     2655 2024-02-26 23:15:20.925848 hume-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 hume-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.0rc1/LICENSE
+-rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.0rc1/README.md
+-rw-r--r--   0        0        0      824 2024-04-18 07:05:31.675321 hume-0.5.0rc1/hume/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.0rc1/hume/_common/__init__.py
+-rw-r--r--   0        0        0     4853 2024-04-09 05:23:34.092782 hume-0.5.0rc1/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.0rc1/hume/_common/config_base.py
+-rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.0rc1/hume/_common/protocol.py
+-rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.0rc1/hume/_common/utilities/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.0rc1/hume/_common/utilities/config_utilities.py
+-rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.0rc1/hume/_common/utilities/model_utilities.py
+-rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.0rc1/hume/_common/utilities/paging_utilities.py
+-rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.0rc1/hume/_common/utilities/retry_utilities.py
+-rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.0rc1/hume/_common/utilities/typing_utilities.py
+-rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.0rc1/hume/_measurement/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.0rc1/hume/_measurement/batch/__init__.py
+-rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.0rc1/hume/_measurement/batch/batch_job.py
+-rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.0rc1/hume/_measurement/batch/batch_job_details.py
+-rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.0rc1/hume/_measurement/batch/batch_job_state.py
+-rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.0rc1/hume/_measurement/batch/batch_job_status.py
+-rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.0rc1/hume/_measurement/batch/hume_batch_client.py
+-rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.0rc1/hume/_measurement/batch/transcription_config.py
+-rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.0rc1/hume/_measurement/stream/__init__.py
+-rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.0rc1/hume/_measurement/stream/hume_stream_client.py
+-rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.0rc1/hume/_measurement/stream/stream_socket.py
+-rw-r--r--   0        0        0      435 2024-04-18 07:05:31.675469 hume-0.5.0rc1/hume/_voice/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-18 10:40:32.709085 hume-0.5.0rc1/hume/_voice/hume_voice_client.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.675674 hume-0.5.0rc1/hume/_voice/microphone/__init__.py
+-rw-r--r--   0        0        0     1371 2024-04-18 10:40:32.750347 hume-0.5.0rc1/hume/_voice/microphone/asyncio_utilities.py
+-rw-r--r--   0        0        0      728 2024-04-18 10:40:32.750572 hume-0.5.0rc1/hume/_voice/microphone/audio_utilities.py
+-rw-r--r--   0        0        0     3348 2024-04-18 10:40:33.206749 hume-0.5.0rc1/hume/_voice/microphone/microphone.py
+-rw-r--r--   0        0        0     5943 2024-04-18 10:40:33.207136 hume-0.5.0rc1/hume/_voice/microphone/microphone_interface.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676175 hume-0.5.0rc1/hume/_voice/mixins/__init__.py
+-rw-r--r--   0        0        0     2166 2024-04-18 10:40:33.207487 hume-0.5.0rc1/hume/_voice/mixins/chat_mixin.py
+-rw-r--r--   0        0        0     2841 2024-04-18 10:40:32.751582 hume-0.5.0rc1/hume/_voice/mixins/chats_mixin.py
+-rw-r--r--   0        0        0     4744 2024-04-18 10:40:32.751861 hume-0.5.0rc1/hume/_voice/mixins/configs_mixin.py
+-rw-r--r--   0        0        0       19 2024-04-18 07:05:31.676663 hume-0.5.0rc1/hume/_voice/models/__init__.py
+-rw-r--r--   0        0        0     2608 2024-04-18 10:40:32.752076 hume-0.5.0rc1/hume/_voice/models/chats_models.py
+-rw-r--r--   0        0        0     1723 2024-04-18 10:40:32.752282 hume-0.5.0rc1/hume/_voice/models/configs_models.py
+-rw-r--r--   0        0        0     2407 2024-04-18 10:40:33.239201 hume-0.5.0rc1/hume/_voice/voice_socket.py
+-rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.0rc1/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.0rc1/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.0rc1/hume/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.0rc1/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.0rc1/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.0rc1/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.0rc1/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.0rc1/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.0rc1/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.0rc1/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.0rc1/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.0rc1/hume/models/model_type.py
+-rw-r--r--   0        0        0     2781 2024-04-18 10:43:17.215157 hume-0.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 hume-0.5.0rc1/PKG-INFO
```

### Comparing `hume-0.4.2/LICENSE` & `hume-0.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.4.2/README.md` & `hume-0.5.0rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     <a href="https://github.com/HumeAI/hume-python-sdk/actions/workflows/ci.yml"><img src="https://github.com/HumeAI/hume-python-sdk/actions/workflows/ci.yaml/badge.svg" alt="CI"></a>
   </div>
   <br>
 </div>
 
 To get started, create an account at [beta.hume.ai](https://beta.hume.ai).
 
-> **Note**
-> Our current version is not yet considered a stable release. As we are still in the development phase, we have chosen to continue releasing under the 0 major release until we are ready to launch version 1.0.0. Our APIs might undergo breaking changes that are necessary for us to improve our tooling and ensure a more stable and reliable release in the future. We encourage you to keep up with our [API changelog](https://dev.hume.ai/changelog) and mailing list to stay up to date with the latest changes.
+> **Note:**
+> Our APIs might undergo breaking changes that are necessary for us to improve our tooling and ensure a more reliable release in the future. Early versions of this SDK may have partial support or support may be fully discontinued. We encourage you to [join our Discord](https://link.hume.ai/discord) to to stay up to date with the latest changes.
 
 ## Documentation & Examples
 
 For complete documentation check out the [Python SDK docs site](https://humeai.github.io/hume-python-sdk/) or [try some recipes](https://dev.hume.ai/recipes) from our platform documentation.
 
 Example notebooks can be found in the [examples folder](./examples/README.md).
```

#### html2text {}

```diff
@@ -1,23 +1,21 @@
     [https://storage.googleapis.com/hume-public-logos/hume/hume-banner.png]
                        ************ HHuummee AAII PPyytthhoonn SSDDKK ************
            IInntteeggrraattee HHuummee AAPPIIss ddiirreeccttllyy iinnttoo yyoouurr PPyytthhoonn aapppplliiccaattiioonn
 
                           _[_D_o_c_s_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_P_I_]_[_C_I_]
 
 To get started, create an account at [beta.hume.ai](https://beta.hume.ai). >
-**Note** > Our current version is not yet considered a stable release. As we
-are still in the development phase, we have chosen to continue releasing under
-the 0 major release until we are ready to launch version 1.0.0. Our APIs might
-undergo breaking changes that are necessary for us to improve our tooling and
-ensure a more stable and reliable release in the future. We encourage you to
-keep up with our [API changelog](https://dev.hume.ai/changelog) and mailing
-list to stay up to date with the latest changes. ## Documentation & Examples
-For complete documentation check out the [Python SDK docs site](https://
-humeai.github.io/hume-python-sdk/) or [try some recipes](https://dev.hume.ai/
+**Note:** > Our APIs might undergo breaking changes that are necessary for us
+to improve our tooling and ensure a more reliable release in the future. Early
+versions of this SDK may have partial support or support may be fully
+discontinued. We encourage you to [join our Discord](https://link.hume.ai/
+discord) to to stay up to date with the latest changes. ## Documentation &
+Examples For complete documentation check out the [Python SDK docs site](https:
+//humeai.github.io/hume-python-sdk/) or [try some recipes](https://dev.hume.ai/
 recipes) from our platform documentation. Example notebooks can be found in the
 [examples folder](./examples/README.md). ## Other Resources - [Hume AI
 Homepage](https://hume.ai) - [Platform Documentation](https://help.hume.ai/
 basics/about-hume-ai) ## Citations Hume's expressive communication platform has
 been built on top of published scientific research. If you use this SDK in your
 work please see [our docs](https://dev.hume.ai/docs/published) for the best way
 to cite Hume's publications. ## Support If you have questions, require
```

### Comparing `hume-0.4.2/hume/__init__.py` & `hume-0.5.0rc1/hume/_measurement/batch/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """Module init."""
-from importlib.metadata import version
 
-from hume._batch import BatchJob, BatchJobDetails, BatchJobState, BatchJobStatus, HumeBatchClient, TranscriptionConfig
-from hume._stream import HumeStreamClient, StreamSocket
-from hume.error.hume_client_exception import HumeClientException
-
-__version__ = version("hume")
+from hume._measurement.batch.batch_job import BatchJob
+from hume._measurement.batch.batch_job_details import BatchJobDetails
+from hume._measurement.batch.batch_job_state import BatchJobState
+from hume._measurement.batch.batch_job_status import BatchJobStatus
+from hume._measurement.batch.hume_batch_client import HumeBatchClient
+from hume._measurement.batch.transcription_config import TranscriptionConfig
 
 __all__ = [
-    "__version__",
     "BatchJob",
     "BatchJobDetails",
     "BatchJobState",
     "BatchJobStatus",
     "HumeBatchClient",
-    "HumeClientException",
-    "HumeStreamClient",
-    "StreamSocket",
     "TranscriptionConfig",
 ]
```

### Comparing `hume-0.4.2/hume/_batch/batch_job.py` & `hume-0.5.0rc1/hume/_measurement/batch/batch_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Batch job."""
+
 import json
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Union
 
-from hume._batch.batch_job_details import BatchJobDetails
-from hume._batch.batch_job_status import BatchJobStatus
-from hume._common.retry_utils import RetryIterError, retry
+from hume._common.utilities.retry_utilities import RetryIterError, retry
+from hume._measurement.batch.batch_job_details import BatchJobDetails
+from hume._measurement.batch.batch_job_status import BatchJobStatus
 from hume.error.hume_client_exception import HumeClientException
 
 if TYPE_CHECKING:
-    from hume._batch.hume_batch_client import HumeBatchClient
+    from hume._measurement.batch.hume_batch_client import HumeBatchClient
 
 
 class BatchJob:
     """Batch job."""
 
     TIMEOUT_MESSAGE = (
         "Connection to API has been terminated after {}s, but your job will continue to run. "
```

### Comparing `hume-0.4.2/hume/_batch/batch_job_details.py` & `hume-0.5.0rc1/hume/_measurement/batch/batch_job_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Batch job details."""
+
 import json
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
-from hume._batch.batch_job_state import BatchJobState
-from hume._batch.batch_job_status import BatchJobStatus
-from hume._common.config_utils import config_from_model_type
+from hume._common.utilities.config_utilities import config_from_model_type
+from hume._measurement.batch.batch_job_state import BatchJobState
+from hume._measurement.batch.batch_job_status import BatchJobStatus
 from hume.error.hume_client_exception import HumeClientException
 from hume.models import ModelType
 from hume.models.config.model_config_base import ModelConfigBase
 
 
 class BatchJobDetails:
     """Batch job details."""
```

### Comparing `hume-0.4.2/hume/_batch/batch_job_state.py` & `hume-0.5.0rc1/hume/_measurement/batch/batch_job_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Batch job state."""
+
 from dataclasses import dataclass
 from typing import Optional
 
-from hume._batch.batch_job_status import BatchJobStatus
+from hume._measurement.batch.batch_job_status import BatchJobStatus
 
 
 @dataclass
 class BatchJobState:
     """Batch job state.
 
     Args:
```

### Comparing `hume-0.4.2/hume/_batch/batch_job_status.py` & `hume-0.5.0rc1/hume/_measurement/batch/batch_job_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Batch job status."""
+
 from enum import Enum
 
 
 class BatchJobStatus(Enum):
     """Batch job status."""
 
     COMPLETED = "COMPLETED"
```

### Comparing `hume-0.4.2/hume/_batch/hume_batch_client.py` & `hume-0.5.0rc1/hume/_measurement/batch/hume_batch_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Batch API client."""
+
 import json
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
-from requests import Session
-
-from hume._batch.batch_job import BatchJob
-from hume._batch.batch_job_details import BatchJobDetails
-from hume._batch.transcription_config import TranscriptionConfig
-from hume._common.api_type import ApiType
 from hume._common.client_base import ClientBase
-from hume._common.config_utils import serialize_configs
+from hume._common.utilities.config_utilities import serialize_configs
+from hume._measurement.batch.batch_job import BatchJob
+from hume._measurement.batch.batch_job_details import BatchJobDetails
+from hume._measurement.batch.transcription_config import TranscriptionConfig
 from hume.error.hume_client_exception import HumeClientException
 from hume.models.config.model_config_base import ModelConfigBase
 
 
 class HumeBatchClient(ClientBase):
     """Batch API client.
 
@@ -50,26 +48,15 @@
     ):
         """Construct a HumeBatchClient.
 
         Args:
             api_key (str): Hume API key.
             timeout (int): Time in seconds before canceling long-running Hume API requests.
         """
-        self._timeout = timeout
-        self._session = Session()
-        super().__init__(api_key, *args, **kwargs)
-
-    @classmethod
-    def get_api_type(cls) -> ApiType:
-        """Get the ApiType of the client.
-
-        Returns:
-            ApiType: API type of the client.
-        """
-        return ApiType.BATCH
+        super().__init__(api_key, http_timeout=timeout, *args, **kwargs)
 
     def get_job(self, job_id: str) -> BatchJob:
         """Rehydrate a job based on a Job ID.
 
         Args:
             job_id (str): ID of the job to rehydrate.
 
@@ -116,20 +103,16 @@
 
         Raises:
             HumeClientException: If the job details cannot be loaded.
 
         Returns:
             BatchJobDetails: Batch job details.
         """
-        endpoint = self._construct_endpoint(f"jobs/{job_id}")
-        response = self._session.get(
-            endpoint,
-            timeout=self._timeout,
-            headers=self._get_client_headers(),
-        )
+        endpoint = self._build_endpoint("batch", f"jobs/{job_id}")
+        response = self._http_client.get(endpoint, headers=self._get_client_headers())
 
         try:
             body = response.json()
         except json.JSONDecodeError:
             # pylint: disable=raise-missing-from
             raise HumeClientException("Unexpected error when getting job details")
 
@@ -146,20 +129,16 @@
 
         Raises:
             HumeClientException: If the job predictions cannot be loaded.
 
         Returns:
             Any: Batch job predictions.
         """
-        endpoint = self._construct_endpoint(f"jobs/{job_id}/predictions")
-        response = self._session.get(
-            endpoint,
-            timeout=self._timeout,
-            headers=self._get_client_headers(),
-        )
+        endpoint = self._build_endpoint("batch", f"jobs/{job_id}/predictions")
+        response = self._http_client.get(endpoint, headers=self._get_client_headers())
 
         try:
             body = response.json()
         except json.JSONDecodeError:
             # pylint: disable=raise-missing-from
             raise HumeClientException("Unexpected error when getting job predictions")
 
@@ -177,20 +156,16 @@
 
         Raises:
             HumeClientException: If the job artifacts cannot be loaded.
 
         Returns:
             Any: Batch job artifacts.
         """
-        endpoint = self._construct_endpoint(f"jobs/{job_id}/artifacts")
-        response = self._session.get(
-            endpoint,
-            timeout=self._timeout,
-            headers=self._get_client_headers(),
-        )
+        endpoint = self._build_endpoint("batch", f"jobs/{job_id}/artifacts")
+        response = self._http_client.get(endpoint, headers=self._get_client_headers())
 
         with Path(filepath).open("wb") as f:
             f.write(response.content)
 
     @classmethod
     def _construct_request(
         cls,
@@ -231,28 +206,26 @@
 
         Raises:
             HumeClientException: If the batch job fails to start.
 
         Returns:
             BatchJob: A `BatchJob` that wraps the batch computation.
         """
-        endpoint = self._construct_endpoint("jobs")
+        endpoint = self._build_endpoint("batch", "jobs")
 
         if filepaths is None:
-            response = self._session.post(
+            response = self._http_client.post(
                 endpoint,
                 json=request_body,
-                timeout=self._timeout,
                 headers=self._get_client_headers(),
             )
         else:
             form_data = self._get_multipart_form_data(request_body, filepaths)
-            response = self._session.post(
+            response = self._http_client.post(
                 endpoint,
-                timeout=self._timeout,
                 headers=self._get_client_headers(),
                 files=form_data,
             )
 
         try:
             body = response.json()
         except json.decoder.JSONDecodeError:
```

### Comparing `hume-0.4.2/hume/_batch/transcription_config.py` & `hume-0.5.0rc1/hume/_measurement/batch/transcription_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for speech transcription."""
+
 from dataclasses import dataclass
 from typing import Optional
 
 from hume._common.config_base import ConfigBase
 
 
 @dataclass
```

### Comparing `hume-0.4.2/hume/_common/config_base.py` & `hume-0.5.0rc1/hume/_common/config_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Abstract base class for model configurations."""
+
 import warnings
 from abc import ABC
 from dataclasses import asdict, dataclass, fields
 from typing import Any, Dict, Generic, TypeVar, cast
 
 T = TypeVar("T")  # Type for subclasses of ConfigBase
```

### Comparing `hume-0.4.2/hume/_common/config_utils.py` & `hume-0.5.0rc1/hume/_common/utilities/config_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Model configuration utilities."""
+
 from typing import Any, Dict, List, Type
 
 from hume.error.hume_client_exception import HumeClientException
 from hume.models import ModelType
 from hume.models.config import (
     BurstConfig,
     FaceConfig,
```

### Comparing `hume-0.4.2/hume/_common/retry_utils.py` & `hume-0.5.0rc1/hume/_common/utilities/retry_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Function retry utilities."""
+
 import logging
 import time
 from typing import Callable, Optional, Type, TypeVar, cast
 
 from typing_extensions import ParamSpec
 
 from hume.error.hume_client_exception import HumeClientException
```

### Comparing `hume-0.4.2/hume/_stream/stream_socket.py` & `hume-0.5.0rc1/hume/_measurement/stream/stream_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """Streaming socket connection."""
+
 import base64
 import json
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
-from hume._common.config_utils import serialize_configs
+from websockets.client import WebSocketClientProtocol
+
+from hume._common.utilities.config_utilities import serialize_configs
 from hume.error.hume_client_exception import HumeClientException
 from hume.models.config import FacemeshConfig, LanguageConfig, ModelConfigBase
 
-try:
-    from websockets.client import WebSocketClientProtocol
-
-    HAS_WEBSOCKETS = True
-except ModuleNotFoundError:
-    HAS_WEBSOCKETS = False
-
 
 class StreamSocket:
     """Streaming socket connection."""
 
     _FACE_LIMIT = 100
     _N_LANDMARKS = 478
     _N_SPATIAL = 3
@@ -36,21 +32,14 @@
             configs (Optional[List[ModelConfigBase]]): List of model configurations.
             stream_window_ms (Optional[int]): Length of the sliding window in milliseconds to use when
                 aggregating media across streaming payloads within one websocket connection.
 
         Raises:
             HumeClientException: If there is an error processing media over the socket connection.
         """
-        if not HAS_WEBSOCKETS:
-            raise HumeClientException(
-                "The websockets package is required to use HumeStreamClient. "
-                'Run `pip install "hume[stream]"` to install a version compatible with the'
-                "Hume Python SDK."
-            )
-
         self._protocol = protocol
         self._configs = configs
         self._stream_window_ms = stream_window_ms
 
         # Serialize configs once for full lifetime of socket
         self._serialized_configs = serialize_configs(configs)
```

### Comparing `hume-0.4.2/hume/error/hume_client_exception.py` & `hume-0.5.0rc1/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.4.2/hume/models/config/__init__.py` & `hume-0.5.0rc1/hume/models/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module init."""
+
 from hume.models.config.burst_config import BurstConfig
 from hume.models.config.face_config import FaceConfig
 from hume.models.config.facemesh_config import FacemeshConfig
 from hume.models.config.language_config import LanguageConfig
 from hume.models.config.model_config_base import ModelConfigBase
 from hume.models.config.ner_config import NerConfig
 from hume.models.config.prosody_config import ProsodyConfig
```

### Comparing `hume-0.4.2/hume/models/config/face_config.py` & `hume-0.5.0rc1/hume/models/config/face_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for the facial expression model."""
+
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from hume.models import ModelType
 from hume.models.config.model_config_base import ModelConfigBase
```

### Comparing `hume-0.4.2/hume/models/config/language_config.py` & `hume-0.5.0rc1/hume/models/config/language_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for the language emotion model."""
+
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
 from hume.models import ModelType
 from hume.models.config.model_config_base import ModelConfigBase
```

### Comparing `hume-0.4.2/hume/models/config/model_config_base.py` & `hume-0.5.0rc1/hume/models/config/model_config_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Abstract base class for model configurations."""
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Generic, TypeVar
 
 from hume._common.config_base import ConfigBase
 from hume.models import ModelType
```

### Comparing `hume-0.4.2/hume/models/config/ner_config.py` & `hume-0.5.0rc1/hume/models/config/ner_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for the named-entity emotion model."""
+
 from dataclasses import dataclass
 from typing import Optional
 
 from hume.models import ModelType
 from hume.models.config.model_config_base import ModelConfigBase
```

### Comparing `hume-0.4.2/hume/models/config/prosody_config.py` & `hume-0.5.0rc1/hume/models/config/prosody_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Configuration for the speech prosody model."""
+
 from dataclasses import dataclass
 from typing import Dict, Optional
 
 from hume.models import ModelType
 from hume.models.config.model_config_base import ModelConfigBase
```

### Comparing `hume-0.4.2/hume/models/model_type.py` & `hume-0.5.0rc1/hume/models/model_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Model type enum."""
+
 from enum import Enum
 
 
 class ModelType(Enum):
     """Model type enum."""
 
     BURST = "burst"
```

### Comparing `hume-0.4.2/pyproject.toml` & `hume-0.5.0rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,95 +3,101 @@
 classifiers = [
   "Development Status :: 4 - Beta",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
-description = "Hume AI Python Client"
+description = "Hume AI Python SDK"
 keywords = [
   "hume",
   "ai",
+  "evi",
+  "empathic",
   "multimodal",
   "expression",
   "analysis",
   "sentiment",
   "voice",
   "recognition",
   "detection",
   "emotion",
+  "interface",
   "speech",
   "audio",
   "vision",
   "expressive",
   "embeddings",
   "communication",
   "learning",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.4.2"
+version = "0.5.0rc1"
 
 [tool.poetry.dependencies]
+httpx = { extras = ["http2"], version = "^0.27.0" }
 jupyter = { version = "^1.0.0", optional = true }
-pydub = { version = "^0.25.1", optional = true }
-python = ">=3.8.1,<4"
-requests = "^2.28.2"
+pydantic = "^2.6.4"
+pydub = "^0.25.1"
+python = ">=3.9,<4"
+simpleaudio = { version = "^1.0.4", optional = true }
+sounddevice = { version = "^0.4.6", optional = true }
 typing-extensions = "^4.3.0"
-websockets = { version = "^10.3", optional = true }
+websockets = "^10.3"
 
 [tool.poetry.dev-dependencies]
-black = "^23.9.1"
+black = "^24.3.0"
 covcheck = { version = "^0.4.3", extras = ["toml"] }
 flake8 = "^6.0.0"
 ipykernel = "^6.22.0"
 mypy = "^1.0.1"
 pydocstyle = "^6.1.1"
 pylint = "^2.16.2"
 pyproject-flake8 = "^6.0.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.19.0"
 pytest-cov = "^4.0.0"
 pytest-forked = "^1.4.0"
 pytest-xdist = "^2.5.0"
 semver = "^2.13.0"
 testbook = "^0.4.2"
-types-requests = "^2.25.11"
 types-setuptools = "^57.4.4"
 types-toml = "^0.10.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mike = "^1.1.2"
 mkdocs = "^1.4.3"
 mkdocs-material = "^9.1.9"
 mkdocstrings = { version = "^0.21.2", extras = ["python"] }
 
 [tool.poetry.extras]
-examples = ["jupyter", "pydub"]
-stream = ["websockets"]
+playback = ["simpleaudio", "sounddevice"]
+examples = ["jupyter"]
+stream = []
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 line-length = 120
 
 [tool.covcheck.group.unit.coverage]
-branch = 63.0
-line = 80.0
+branch = 50.0
+line = 72.0
 
 [tool.covcheck.group.service.coverage]
-branch = 64.0
-line = 87.0
+branch = 58.0
+line = 80.0
 
 [tool.flake8]
 ignore = ""           # Required to disable default ignores
 max-line-length = 120
 
 [tool.isort]
 line_length = 120
```

### Comparing `hume-0.4.2/PKG-INFO` & `hume-0.5.0rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.4.2
-Summary: Hume AI Python Client
+Version: 0.5.0rc1
+Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
-Keywords: hume,ai,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,speech,audio,vision,expressive,embeddings,communication,learning
+Keywords: hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev
 Author-email: dev@hume.ai
-Requires-Python: >=3.8.1,<4
+Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: examples
+Provides-Extra: playback
 Provides-Extra: stream
+Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "examples"
-Requires-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "examples"
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: pydub (>=0.25.1,<0.26.0)
+Requires-Dist: simpleaudio (>=1.0.4,<2.0.0) ; extra == "playback"
+Requires-Dist: sounddevice (>=0.4.6,<0.5.0) ; extra == "playback"
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
-Requires-Dist: websockets (>=10.3,<11.0) ; extra == "stream"
+Requires-Dist: websockets (>=10.3,<11.0)
 Project-URL: Repository, https://github.com/HumeAI/hume-python-sdk
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img src="https://storage.googleapis.com/hume-public-logos/hume/hume-banner.png">
   <h1>Hume AI Python SDK</h1>
 
@@ -41,16 +46,16 @@
     <a href="https://github.com/HumeAI/hume-python-sdk/actions/workflows/ci.yml"><img src="https://github.com/HumeAI/hume-python-sdk/actions/workflows/ci.yaml/badge.svg" alt="CI"></a>
   </div>
   <br>
 </div>
 
 To get started, create an account at [beta.hume.ai](https://beta.hume.ai).
 
-> **Note**
-> Our current version is not yet considered a stable release. As we are still in the development phase, we have chosen to continue releasing under the 0 major release until we are ready to launch version 1.0.0. Our APIs might undergo breaking changes that are necessary for us to improve our tooling and ensure a more stable and reliable release in the future. We encourage you to keep up with our [API changelog](https://dev.hume.ai/changelog) and mailing list to stay up to date with the latest changes.
+> **Note:**
+> Our APIs might undergo breaking changes that are necessary for us to improve our tooling and ensure a more reliable release in the future. Early versions of this SDK may have partial support or support may be fully discontinued. We encourage you to [join our Discord](https://link.hume.ai/discord) to to stay up to date with the latest changes.
 
 ## Documentation & Examples
 
 For complete documentation check out the [Python SDK docs site](https://humeai.github.io/hume-python-sdk/) or [try some recipes](https://dev.hume.ai/recipes) from our platform documentation.
 
 Example notebooks can be found in the [examples folder](./examples/README.md).
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
-Metadata-Version: 2.1 Name: hume Version: 0.4.2 Summary: Hume AI Python Client
+Metadata-Version: 2.1 Name: hume Version: 0.5.0rc1 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
-hume,ai,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,speech,audio,vision,expressive,embeddings,communication,learning
-Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.8.1,<4
+hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
+Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: examples Provides-Extra:
-stream Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "examples" Requires-
-Dist: pydub (>=0.25.1,<0.26.0) ; extra == "examples" Requires-Dist: requests
-(>=2.28.2,<3.0.0) Requires-Dist: typing-extensions (>=4.3.0,<5.0.0) Requires-
-Dist: websockets (>=10.3,<11.0) ; extra == "stream" Project-URL: Repository,
-https://github.com/HumeAI/hume-python-sdk Description-Content-Type: text/
-markdown
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Provides-Extra: examples Provides-Extra: playback Provides-
+Extra: stream Requires-Dist: httpx[http2] (>=0.27.0,<0.28.0) Requires-Dist:
+jupyter (>=1.0.0,<2.0.0) ; extra == "examples" Requires-Dist: pydantic
+(>=2.6.4,<3.0.0) Requires-Dist: pydub (>=0.25.1,<0.26.0) Requires-Dist:
+simpleaudio (>=1.0.4,<2.0.0) ; extra == "playback" Requires-Dist: sounddevice
+(>=0.4.6,<0.5.0) ; extra == "playback" Requires-Dist: typing-extensions
+(>=4.3.0,<5.0.0) Requires-Dist: websockets (>=10.3,<11.0) Project-URL:
+Repository, https://github.com/HumeAI/hume-python-sdk Description-Content-Type:
+text/markdown
     [https://storage.googleapis.com/hume-public-logos/hume/hume-banner.png]
                        ************ HHuummee AAII PPyytthhoonn SSDDKK ************
            IInntteeggrraattee HHuummee AAPPIIss ddiirreeccttllyy iinnttoo yyoouurr PPyytthhoonn aapppplliiccaattiioonn
 
                           _[_D_o_c_s_]_[_D_o_w_n_l_o_a_d_s_]_[_P_y_P_I_]_[_C_I_]
 
 To get started, create an account at [beta.hume.ai](https://beta.hume.ai). >
-**Note** > Our current version is not yet considered a stable release. As we
-are still in the development phase, we have chosen to continue releasing under
-the 0 major release until we are ready to launch version 1.0.0. Our APIs might
-undergo breaking changes that are necessary for us to improve our tooling and
-ensure a more stable and reliable release in the future. We encourage you to
-keep up with our [API changelog](https://dev.hume.ai/changelog) and mailing
-list to stay up to date with the latest changes. ## Documentation & Examples
-For complete documentation check out the [Python SDK docs site](https://
-humeai.github.io/hume-python-sdk/) or [try some recipes](https://dev.hume.ai/
+**Note:** > Our APIs might undergo breaking changes that are necessary for us
+to improve our tooling and ensure a more reliable release in the future. Early
+versions of this SDK may have partial support or support may be fully
+discontinued. We encourage you to [join our Discord](https://link.hume.ai/
+discord) to to stay up to date with the latest changes. ## Documentation &
+Examples For complete documentation check out the [Python SDK docs site](https:
+//humeai.github.io/hume-python-sdk/) or [try some recipes](https://dev.hume.ai/
 recipes) from our platform documentation. Example notebooks can be found in the
 [examples folder](./examples/README.md). ## Other Resources - [Hume AI
 Homepage](https://hume.ai) - [Platform Documentation](https://help.hume.ai/
 basics/about-hume-ai) ## Citations Hume's expressive communication platform has
 been built on top of published scientific research. If you use this SDK in your
 work please see [our docs](https://dev.hume.ai/docs/published) for the best way
 to cite Hume's publications. ## Support If you have questions, require
```

