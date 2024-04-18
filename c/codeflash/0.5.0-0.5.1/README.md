# Comparing `tmp/codeflash-0.5.0.tar.gz` & `tmp/codeflash-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeflash-0.5.0.tar", max compression
+gzip compressed data, was "codeflash-0.5.1.tar", max compression
```

## Comparing `codeflash-0.5.0.tar` & `codeflash-0.5.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.5.0/README.md
--rw-r--r--   0        0        0     4405 2024-04-11 20:54:38.441461 codeflash-0.5.0/codeflash/LICENSE
--rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.5.0/codeflash/__init__.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.5.0/codeflash/api/__init__.py
--rw-r--r--   0        0        0     8122 2024-04-10 21:49:12.465747 codeflash-0.5.0/codeflash/api/aiservice.py
--rw-r--r--   0        0        0     4703 2024-03-06 13:45:57.132901 codeflash-0.5.0/codeflash/api/cfapi.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.5.0/codeflash/cli_cmds/__init__.py
--rw-r--r--   0        0        0     5655 2024-04-10 20:56:46.198285 codeflash-0.5.0/codeflash/cli_cmds/cli.py
--rw-r--r--   0        0        0    22938 2024-03-30 21:18:28.910786 codeflash-0.5.0/codeflash/cli_cmds/cmd_init.py
--rw-r--r--   0        0        0      156 2024-02-01 23:15:04.021654 codeflash-0.5.0/codeflash/cli_cmds/logging_config.py
--rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.5.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.5.0/codeflash/code_utils/__init__.py
--rw-r--r--   0        0        0     7170 2024-04-10 21:49:12.465898 codeflash-0.5.0/codeflash/code_utils/code_extractor.py
--rw-r--r--   0        0        0     9450 2024-04-10 21:49:12.466063 codeflash-0.5.0/codeflash/code_utils/code_replacer.py
--rw-r--r--   0        0        0     2618 2024-03-27 23:33:18.926667 codeflash-0.5.0/codeflash/code_utils/code_utils.py
--rw-r--r--   0        0        0      273 2024-03-09 12:14:07.997779 codeflash-0.5.0/codeflash/code_utils/compat.py
--rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.5.0/codeflash/code_utils/config_consts.py
--rw-r--r--   0        0        0     3906 2024-04-02 23:26:25.038599 codeflash-0.5.0/codeflash/code_utils/config_parser.py
--rw-r--r--   0        0        0     2908 2024-03-30 02:05:25.997181 codeflash-0.5.0/codeflash/code_utils/env_utils.py
--rw-r--r--   0        0        0     1988 2024-03-29 22:03:45.051414 codeflash-0.5.0/codeflash/code_utils/formatter.py
--rw-r--r--   0        0        0     3308 2024-04-08 00:04:34.442696 codeflash-0.5.0/codeflash/code_utils/git_utils.py
--rw-r--r--   0        0        0    22288 2024-03-27 23:33:18.927147 codeflash-0.5.0/codeflash/code_utils/instrument_existing_tests.py
--rw-r--r--   0        0        0     3501 2024-03-28 19:16:33.995378 codeflash-0.5.0/codeflash/code_utils/shell_utils.py
--rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.5.0/codeflash/code_utils/sqlalchemy_utils.py
--rw-r--r--   0        0        0     1860 2024-01-24 20:13:21.332617 codeflash-0.5.0/codeflash/code_utils/time_utils.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.5.0/codeflash/discovery/__init__.py
--rw-r--r--   0        0        0    16183 2024-03-13 16:48:07.259994 codeflash-0.5.0/codeflash/discovery/discover_unit_tests.py
--rw-r--r--   0        0        0    12182 2024-04-10 20:56:46.198974 codeflash-0.5.0/codeflash/discovery/functions_to_optimize.py
--rw-r--r--   0        0        0     1229 2024-02-13 02:11:11.092168 codeflash-0.5.0/codeflash/github/PrComment.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.5.0/codeflash/github/__init__.py
--rw-r--r--   0        0        0    44529 2024-04-10 21:49:12.466361 codeflash-0.5.0/codeflash/main.py
--rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.5.0/codeflash/optimization/__init__.py
--rw-r--r--   0        0        0    11557 2024-04-10 21:49:12.466508 codeflash-0.5.0/codeflash/optimization/function_context.py
--rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.5.0/codeflash/result/__init__.py
--rw-r--r--   0        0        0     3959 2024-03-02 17:26:31.551442 codeflash-0.5.0/codeflash/result/create_pr.py
--rw-r--r--   0        0        0     1982 2024-02-01 23:15:04.024170 codeflash-0.5.0/codeflash/result/explanation.py
--rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.5.0/codeflash/telemetry/__init__.py
--rw-r--r--   0        0        0     1257 2024-03-19 02:04:16.181201 codeflash-0.5.0/codeflash/telemetry/posthog.py
--rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.5.0/codeflash/telemetry/sentry.py
--rw-r--r--   0        0        0        0 2024-04-10 20:56:46.199644 codeflash-0.5.0/codeflash/tracing/__init__.py
--rw-r--r--   0        0        0     4908 2024-04-10 20:56:46.200028 codeflash-0.5.0/codeflash/tracing/replay_test.py
--rw-r--r--   0        0        0     5174 2024-04-10 20:56:46.200480 codeflash-0.5.0/codeflash/tracing/tracer.py
--rw-r--r--   0        0        0     1910 2024-03-24 21:57:44.197591 codeflash-0.5.0/codeflash/update_license_version.py
--rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.5.0/codeflash/verification/__init__.py
--rw-r--r--   0        0        0     4733 2024-04-04 03:26:48.352761 codeflash-0.5.0/codeflash/verification/comparator.py
--rw-r--r--   0        0        0     1139 2024-03-30 00:35:38.112124 codeflash-0.5.0/codeflash/verification/equivalence.py
--rw-r--r--   0        0        0    14539 2024-04-08 00:04:34.443972 codeflash-0.5.0/codeflash/verification/parse_test_output.py
--rw-r--r--   0        0        0     6681 2024-04-08 00:04:34.444171 codeflash-0.5.0/codeflash/verification/test_results.py
--rw-r--r--   0        0        0     1580 2024-03-24 21:57:44.197705 codeflash-0.5.0/codeflash/verification/test_runner.py
--rw-r--r--   0        0        0     2366 2024-04-10 20:56:46.200732 codeflash-0.5.0/codeflash/verification/verification_utils.py
--rw-r--r--   0        0        0     4242 2024-03-24 21:57:44.198063 codeflash-0.5.0/codeflash/verification/verifier.py
--rw-r--r--   0        0        0      150 2024-04-11 20:55:45.133024 codeflash-0.5.0/codeflash/version.py
--rw-r--r--   0        0        0     2915 2024-04-11 20:55:45.132371 codeflash-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 codeflash-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-01-05 04:36:50.272525 codeflash-0.5.1/README.md
+-rw-r--r--   0        0        0     4405 2024-04-18 06:54:49.015842 codeflash-0.5.1/codeflash/LICENSE
+-rw-r--r--   0        0        0        0 2024-02-13 02:11:11.085505 codeflash-0.5.1/codeflash/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274581 codeflash-0.5.1/codeflash/api/__init__.py
+-rw-r--r--   0        0        0     7886 2024-04-16 22:27:44.246474 codeflash-0.5.1/codeflash/api/aiservice.py
+-rw-r--r--   0        0        0     4681 2024-04-18 03:01:28.772476 codeflash-0.5.1/codeflash/api/cfapi.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.274847 codeflash-0.5.1/codeflash/cli_cmds/__init__.py
+-rw-r--r--   0        0        0     7606 2024-04-18 19:11:45.874124 codeflash-0.5.1/codeflash/cli_cmds/cli.py
+-rw-r--r--   0        0        0    22865 2024-04-18 03:01:28.773022 codeflash-0.5.1/codeflash/cli_cmds/cmd_init.py
+-rw-r--r--   0        0        0      440 2024-04-16 22:27:44.247326 codeflash-0.5.1/codeflash/cli_cmds/logging_config.py
+-rw-r--r--   0        0        0     1827 2024-03-24 21:57:44.196107 codeflash-0.5.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.275400 codeflash-0.5.1/codeflash/code_utils/__init__.py
+-rw-r--r--   0        0        0     7170 2024-04-16 22:27:44.247484 codeflash-0.5.1/codeflash/code_utils/code_extractor.py
+-rw-r--r--   0        0        0     9450 2024-04-16 22:27:44.247642 codeflash-0.5.1/codeflash/code_utils/code_replacer.py
+-rw-r--r--   0        0        0     2572 2024-04-16 22:27:44.247908 codeflash-0.5.1/codeflash/code_utils/code_utils.py
+-rw-r--r--   0        0        0      273 2024-04-15 22:14:14.315668 codeflash-0.5.1/codeflash/code_utils/compat.py
+-rw-r--r--   0        0        0      224 2024-02-10 04:17:44.568348 codeflash-0.5.1/codeflash/code_utils/config_consts.py
+-rw-r--r--   0        0        0     3908 2024-04-18 03:01:28.775259 codeflash-0.5.1/codeflash/code_utils/config_parser.py
+-rw-r--r--   0        0        0     2880 2024-04-18 03:01:28.775549 codeflash-0.5.1/codeflash/code_utils/env_utils.py
+-rw-r--r--   0        0        0     1979 2024-04-18 03:01:28.775777 codeflash-0.5.1/codeflash/code_utils/formatter.py
+-rw-r--r--   0        0        0     3305 2024-04-18 03:01:28.775937 codeflash-0.5.1/codeflash/code_utils/git_utils.py
+-rw-r--r--   0        0        0    22720 2024-04-18 06:54:04.081262 codeflash-0.5.1/codeflash/code_utils/instrument_existing_tests.py
+-rw-r--r--   0        0        0     3497 2024-04-18 03:01:28.776414 codeflash-0.5.1/codeflash/code_utils/shell_utils.py
+-rw-r--r--   0        0        0     1007 2024-01-05 04:36:50.277228 codeflash-0.5.1/codeflash/code_utils/sqlalchemy_utils.py
+-rw-r--r--   0        0        0     1860 2024-01-24 20:13:21.332617 codeflash-0.5.1/codeflash/code_utils/time_utils.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277391 codeflash-0.5.1/codeflash/discovery/__init__.py
+-rw-r--r--   0        0        0    16173 2024-04-18 03:01:28.777556 codeflash-0.5.1/codeflash/discovery/discover_unit_tests.py
+-rw-r--r--   0        0        0    12401 2024-04-18 19:11:45.875161 codeflash-0.5.1/codeflash/discovery/functions_to_optimize.py
+-rw-r--r--   0        0        0     1230 2024-04-18 03:01:28.780898 codeflash-0.5.1/codeflash/github/PrComment.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.277833 codeflash-0.5.1/codeflash/github/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-16 22:27:44.248364 codeflash-0.5.1/codeflash/main.py
+-rw-r--r--   0        0        0        0 2024-01-05 04:36:50.278392 codeflash-0.5.1/codeflash/optimization/__init__.py
+-rw-r--r--   0        0        0    11557 2024-04-16 22:27:44.248501 codeflash-0.5.1/codeflash/optimization/function_context.py
+-rw-r--r--   0        0        0    46035 2024-04-16 22:27:44.248849 codeflash-0.5.1/codeflash/optimization/optimizer.py
+-rw-r--r--   0        0        0        0 2024-01-29 22:33:50.970495 codeflash-0.5.1/codeflash/result/__init__.py
+-rw-r--r--   0        0        0     4625 2024-04-16 22:27:44.249419 codeflash-0.5.1/codeflash/result/create_pr.py
+-rw-r--r--   0        0        0     1982 2024-02-01 23:15:04.024170 codeflash-0.5.1/codeflash/result/explanation.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:04:16.181069 codeflash-0.5.1/codeflash/telemetry/__init__.py
+-rw-r--r--   0        0        0     1247 2024-04-18 03:01:28.781066 codeflash-0.5.1/codeflash/telemetry/posthog.py
+-rw-r--r--   0        0        0      579 2024-03-19 02:04:16.181306 codeflash-0.5.1/codeflash/telemetry/sentry.py
+-rw-r--r--   0        0        0        0 2024-04-18 19:11:45.875236 codeflash-0.5.1/codeflash/tracing/__init__.py
+-rw-r--r--   0        0        0     4938 2024-04-18 19:11:45.876501 codeflash-0.5.1/codeflash/tracing/replay_test.py
+-rw-r--r--   0        0        0     5160 2024-04-18 19:11:45.876985 codeflash-0.5.1/codeflash/tracing/tracer.py
+-rw-r--r--   0        0        0     1905 2024-04-18 03:01:28.781529 codeflash-0.5.1/codeflash/update_license_version.py
+-rw-r--r--   0        0        0        0 2024-01-20 20:41:44.799451 codeflash-0.5.1/codeflash/verification/__init__.py
+-rw-r--r--   0        0        0     4738 2024-04-18 03:01:28.781696 codeflash-0.5.1/codeflash/verification/comparator.py
+-rw-r--r--   0        0        0     1139 2024-03-30 00:35:38.112124 codeflash-0.5.1/codeflash/verification/equivalence.py
+-rw-r--r--   0        0        0    14520 2024-04-18 06:54:04.082484 codeflash-0.5.1/codeflash/verification/parse_test_output.py
+-rw-r--r--   0        0        0     6581 2024-04-16 22:27:44.249777 codeflash-0.5.1/codeflash/verification/test_results.py
+-rw-r--r--   0        0        0     1606 2024-04-18 03:01:28.782090 codeflash-0.5.1/codeflash/verification/test_runner.py
+-rw-r--r--   0        0        0     2327 2024-04-18 19:11:45.877370 codeflash-0.5.1/codeflash/verification/verification_utils.py
+-rw-r--r--   0        0        0     4126 2024-04-18 03:01:28.782490 codeflash-0.5.1/codeflash/verification/verifier.py
+-rw-r--r--   0        0        0      150 2024-04-18 19:13:22.432539 codeflash-0.5.1/codeflash/version.py
+-rw-r--r--   0        0        0     2894 2024-04-18 19:13:22.431563 codeflash-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 codeflash-0.5.1/PKG-INFO
```

### Comparing `codeflash-0.5.0/codeflash/LICENSE` & `codeflash-0.5.1/codeflash/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Business Source License 1.1
 
 Parameters
 
 Licensor:             CodeFlash Inc.
-Licensed Work:        Codeflash Client version 0.4.x
+Licensed Work:        Codeflash Client version 0.5.x
                       The Licensed Work is (c) 2024 CodeFlash Inc.
 
 Additional Use Grant: None. Production use of the Licensed Work is only permitted
                       if you have entered into a separate written agreement
                       with CodeFlash Inc. for production use in connection
                       with a subscription to CodeFlash's Code Optimization
                       Platform. Please visit codeflash.ai for further
                       information.
 
-Change Date:          2028-03-24
+Change Date:          2028-04-11
 
 Change License:       MIT
 
 Notice
 
 The Business Source License (this document, or the “License”) is not an Open
 Source license. However, the Licensed Work will eventually be made available
```

### Comparing `codeflash-0.5.0/codeflash/api/aiservice.py` & `codeflash-0.5.1/codeflash/api/aiservice.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import json
 import logging
 import os
 import platform
+from functools import lru_cache
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 from pydantic.dataclasses import dataclass
 from pydantic.json import pydantic_encoder
 
 from codeflash.code_utils.env_utils import get_codeflash_api_key
 from codeflash.discovery.functions_to_optimize import FunctionToOptimize
 from codeflash.telemetry.posthog import ph
 
-if os.environ.get("AIS_SERVER", default="prod").lower() == "local":
-    AI_SERVICE_BASE_URL = "http://localhost:8000/"
-    logging.info(f"Using local AI Service at {AI_SERVICE_BASE_URL}.")
-else:
-    AI_SERVICE_BASE_URL = "https://app.codeflash.ai"
+
+@lru_cache(maxsize=1)
+def get_aiservice_base_url() -> str:
+    if os.environ.get("AIS_SERVER", default="prod").lower() == "local":
+        logging.info("Using local AI Service at http://localhost:8000/")
+        return "http://localhost:8000/"
+    return "https://app.codeflash.ai"
 
 
 def make_ai_service_request(
     endpoint: str,
     method: str = "POST",
     payload: Optional[Dict[str, Any]] = None,
     timeout: float = None,
@@ -28,15 +31,15 @@
     """Make an API request to the given endpoint on the AI service.
     :param endpoint: The endpoint to call, e.g., "/optimize".
     :param method: The HTTP method to use ('GET' or 'POST').
     :param payload: Optional JSON payload to include in the POST request body.
     :param timeout: The timeout for the request.
     :return: The response object from the API.
     """
-    url = f"{AI_SERVICE_BASE_URL}/ai{endpoint}"
+    url = f"{get_aiservice_base_url()}/ai{endpoint}"
     ai_service_headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
     if method.upper() == "POST":
         json_payload = json.dumps(payload, indent=None, default=pydantic_encoder)
         ai_service_headers["Content-Type"] = "application/json"
         response = requests.post(
             url,
             data=json_payload,
@@ -52,70 +55,62 @@
 @dataclass(frozen=True)
 class Optimization:
     source_code: str
     explanation: str
     optimization_id: str
 
 
-@dataclass(frozen=True)
-class Optimizations:
-    optimizations: List[Optimization]
-
-
-def optimize_python_code(source_code: str, trace_id: str, num_variants: int = 10) -> Optimizations:
+def optimize_python_code(source_code: str, trace_id: str, num_variants: int = 10) -> List[Optimization]:
     """Optimize the given python code for performance by making a request to the Django endpoint.
 
     Parameters
     ----------
     - source_code (str): The python code to optimize.
     - num_variants (int): Number of optimization variants to generate. Default is 10.
 
     Returns
     -------
-    - List[Tuple[str, str]]: A list of tuples where the first element is the optimized code and the second is the explanation.
+    - List[Optimization]: A list of Optimization objects.
 
     """
     payload = {
         "source_code": source_code,
         "num_variants": num_variants,
         "trace_id": trace_id,
         "python_version": platform.python_version(),
     }
     logging.info("Generating optimized candidates ...")
     try:
         response = make_ai_service_request("/optimize", payload=payload, timeout=600)
     except requests.exceptions.RequestException as e:
         logging.exception(f"Error generating optimized candidates: {e}")
         ph("cli-optimize-error-caught", {"error": str(e)})
-        return Optimizations(optimizations=[])
+        return []
 
     if response.status_code == 200:
-        optimizations = response.json()["optimizations"]
-        logging.info(f"Generated {len(optimizations)} candidates.")
-        return Optimizations(
-            [
-                Optimization(
-                    source_code=opt["source_code"],
-                    explanation=opt["explanation"],
-                    optimization_id=opt["optimization_id"],
-                )
-                for opt in optimizations
-            ],
-        )
-    else:
-        try:
-            error = response.json()["error"]
-        except Exception:
-            error = response.text
-        logging.error(f"Error generating optimized candidates: {response.status_code} - {error}")
-        ph(
-            "cli-optimize-error-response",
-            {"response_status_code": response.status_code, "error": error},
-        )
-        return Optimizations(optimizations=[])
+        optimizations_json = response.json()["optimizations"]
+        logging.info(f"Generated {len(optimizations_json)} candidates.")
+        return [
+            Optimization(
+                source_code=opt["source_code"],
+                explanation=opt["explanation"],
+                optimization_id=opt["optimization_id"],
+            )
+            for opt in optimizations_json
+        ]
+    try:
+        error = response.json()["error"]
+    except Exception:
+        error = response.text
+    logging.error(f"Error generating optimized candidates: {response.status_code} - {error}")
+    ph(
+        "cli-optimize-error-response",
+        {"response_status_code": response.status_code, "error": error},
+    )
+    return []
 
 
 def log_results(
     function_trace_id: str,
     speedup_ratio: Optional[Dict[str, float]],
     original_runtime: Optional[float],
     optimized_runtime: Optional[Dict[str, float]],
```

### Comparing `codeflash-0.5.0/codeflash/api/cfapi.py` & `codeflash-0.5.1/codeflash/api/cfapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import json
 import logging
 import os
-import requests
 from functools import lru_cache
+from typing import Any, Dict, Optional
+
+import requests
 from pydantic.json import pydantic_encoder
 from requests import Response
-from typing import Optional, Dict, Any
 
 from codeflash.code_utils.env_utils import get_codeflash_api_key
-from codeflash.github.PrComment import PrComment, FileDiffContent
+from codeflash.github.PrComment import FileDiffContent, PrComment
 
 if os.environ.get("CFAPI_SERVER", default="prod").lower() == "local":
     CFAPI_BASE_URL = "http://localhost:3001"
     logging.info(f"Using local CF API at {CFAPI_BASE_URL}.")
 else:
     CFAPI_BASE_URL = "https://app.codeflash.ai"
 
 
 def make_cfapi_request(
-    endpoint: str, method: str, payload: Optional[Dict[str, Any]] = None
+    endpoint: str, method: str, payload: Optional[Dict[str, Any]] = None,
 ) -> requests.Response:
-    """
-    Make an HTTP request using the specified method, URL, headers, and JSON payload.
+    """Make an HTTP request using the specified method, URL, headers, and JSON payload.
     :param endpoint: The endpoint URL to send the request to.
     :param method: The HTTP method to use ('GET', 'POST', etc.).
     :param payload: Optional JSON payload to include in the POST request body.
     :return: The response object from the API.
     """
     url = f"{CFAPI_BASE_URL}/cfapi{endpoint}"
     cfapi_headers = {"Authorization": f"Bearer {get_codeflash_api_key()}"}
@@ -36,39 +36,37 @@
     else:
         response = requests.get(url, headers=cfapi_headers)
     return response
 
 
 @lru_cache(maxsize=1)
 def get_user_id() -> Optional[str]:
-    """
-    Retrieve the user's userid by making a request to the /cfapi/cli-get-user endpoint.
+    """Retrieve the user's userid by making a request to the /cfapi/cli-get-user endpoint.
     :return: The userid or None if the request fails.
     """
     response = make_cfapi_request(endpoint="/cli-get-user", method="GET")
     if response.status_code == 200:
         return response.text
     else:
         logging.error(
-            f"Failed to look up your userid; is your CF API key valid? ({response.reason})"
+            f"Failed to look up your userid; is your CF API key valid? ({response.reason})",
         )
         return None
 
 
 def suggest_changes(
     owner: str,
     repo: str,
     pr_number: int,
     file_changes: dict[str, FileDiffContent],
     pr_comment: PrComment,
     existing_tests: str,
     generated_tests: str,
 ) -> Response:
-    """
-    Suggest changes to a pull request.
+    """Suggest changes to a pull request.
     Will make a review suggestion when possible;
     or create a new dependent pull request with the suggested changes.
     :param owner: The owner of the repository.
     :param repo: The name of the repository.
     :param pr_number: The number of the pull request.
     :param file_changes: A dictionary of file changes.
     :param pr_comment: The pull request comment object, containing the optimization explanation, best runtime, etc.
@@ -93,16 +91,15 @@
     repo: str,
     base_branch: str,
     file_changes: dict[str, FileDiffContent],
     pr_comment: PrComment,
     existing_tests: str,
     generated_tests: str,
 ) -> Response:
-    """
-    Create a pull request, targeting the specified branch. (usually 'main')
+    """Create a pull request, targeting the specified branch. (usually 'main')
     :param owner: The owner of the repository.
     :param repo: The name of the repository.
     :param base_branch: The base branch to target.
     :param file_changes: A dictionary of file changes.
     :param pr_comment: The pull request comment object, containing the optimization explanation, best runtime, etc.
     :param generated_tests: The generated tests.
     :return: The response object.
@@ -117,16 +114,15 @@
         "generatedTests": generated_tests,
     }
     response = make_cfapi_request(endpoint="/create-pr", method="POST", payload=payload)
     return response
 
 
 def check_github_app_installed_on_repo(owner: str, repo: str) -> Response:
-    """
-    Check if the Codeflash GitHub App is installed on the specified repository.
+    """Check if the Codeflash GitHub App is installed on the specified repository.
     :param owner: The owner of the repository.
     :param repo: The name of the repository.
     :return: The response object.
     """
     return make_cfapi_request(
         endpoint=f"/is-github-app-installed?repo={repo}&owner={owner}",
         method="GET",
```

### Comparing `codeflash-0.5.0/codeflash/cli_cmds/cmd_init.py` & `codeflash-0.5.1/codeflash/cli_cmds/cmd_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import os
 import re
 import subprocess
 import sys
 import time
-from typing import Optional, NoReturn
+from typing import NoReturn, Optional
 
 import click
 import inquirer
 import inquirer.themes
 import tomlkit
 from git import Repo
 from pydantic.dataclasses import dataclass
@@ -16,16 +16,16 @@
 
 from codeflash.code_utils.compat import LF
 from codeflash.code_utils.env_utils import (
     get_codeflash_api_key,
 )
 from codeflash.code_utils.git_utils import get_github_secrets_page_url
 from codeflash.code_utils.shell_utils import (
-    save_api_key_to_rc,
     get_shell_rc_path,
+    save_api_key_to_rc,
 )
 from codeflash.telemetry.posthog import ph
 from codeflash.version import __version__ as version
 
 CODEFLASH_LOGO: str = (
     f"{LF}"
     r"              __    _____         __ " + f"{LF}"
@@ -65,19 +65,19 @@
             f"{LF}"
             f"⚡️ Codeflash is now set up! You can now run:{LF}"
             f"    codeflash --file <path-to-file> --function <function-name> to optimize a function within a file{LF}"
             f"    codeflash --file <path-to-file> to optimize all functions in a file{LF}"
             f"    codeflash --all to optimize all functions in all files in the module you selected ({setup_info.module_root}){LF}"
             # f"    codeflash --pr <pr-number> to optimize a PR{LF}"
             f"-or-{LF}"
-            f"    codeflash --help to see all options{LF}"
+            f"    codeflash --help to see all options{LF}",
         )
         if did_add_new_key:
             click.echo(
-                "🐚 Don't forget to restart your shell to load the CODEFLASH_API_KEY environment variable!"
+                "🐚 Don't forget to restart your shell to load the CODEFLASH_API_KEY environment variable!",
             )
             click.echo("Or run the following command to reload:")
             if os.name == "nt":
                 click.echo(f"  call {get_shell_rc_path()}")
             else:
                 click.echo(f"  source {get_shell_rc_path()}")
 
@@ -97,15 +97,15 @@
 
 
 def collect_setup_info() -> SetupInfo:
     curdir = os.getcwd()
     # Check if the cwd is writable
     if not os.access(curdir, os.W_OK):
         click.echo(
-            f"❌ The current directory isn't writable, please check your folder permissions and try again.{LF}"
+            f"❌ The current directory isn't writable, please check your folder permissions and try again.{LF}",
         )
         click.echo("It's likely you don't have write permissions for this folder.")
         sys.exit(1)
 
     # Check for the existence of pyproject.toml or setup.py
     project_name = check_for_toml_or_setup_file()
 
@@ -128,15 +128,15 @@
 
     valid_module_subdirs = [dir for dir in valid_subdirs if dir != "tests"]
 
     curdir_option = "current directory (" + curdir + ")"
     module_subdir_options = valid_module_subdirs + [curdir_option]
 
     module_root_answer = inquirer.list_input(
-        message=f"Which Python module do you want me to optimize going forward? (Usually the top-most directory with all of your Python source code)",
+        message="Which Python module do you want me to optimize going forward? (Usually the top-most directory with all of your Python source code)",
         choices=module_subdir_options,
         default=(
             project_name if project_name in module_subdir_options else module_subdir_options[0]
         ),
     )
     module_root = "." if module_root_answer == curdir_option else module_root_answer
     ph("cli-project-root-provided")
@@ -168,15 +168,15 @@
                 inquirer.Path(
                     "path",
                     message=f"Enter the path to your tests directory inside {os.path.abspath(module_root) + os.pathsep} ",
                     path_type=inquirer.Path.DIRECTORY,
                     exists=True,
                     normalize_to_absolute_path=True,
                 ),
-            ]
+            ],
         )
         tests_root = (
             custom_tests_root_answer["path"] if custom_tests_root_answer else apologize_and_exit()
         )
     else:
         tests_root = tests_root_answer
     tests_root = os.path.relpath(tests_root, curdir)
@@ -220,25 +220,25 @@
         "pyproject.toml": "[tool.pytest.ini_options]",
         "tox.ini": "[pytest]",
         "setup.cfg": "[tool:pytest]",
     }
     for pytest_file in pytest_files:
         file_path = os.path.join(curdir, pytest_file)
         if os.path.exists(file_path):
-            with open(file_path, "r", encoding="utf8") as file:
+            with open(file_path, encoding="utf8") as file:
                 contents = file.read()
                 if pytest_config_patterns[pytest_file] in contents:
                     test_framework = "pytest"
                     break
         test_framework = "pytest"
     else:
         # Check if any python files contain a class that inherits from unittest.TestCase
         for filename in os.listdir(tests_root):
             if filename.endswith(".py"):
-                with open(os.path.join(tests_root, filename), "r", encoding="utf8") as file:
+                with open(os.path.join(tests_root, filename), encoding="utf8") as file:
                     contents = file.read()
                     try:
                         node = ast.parse(contents)
                     except SyntaxError:
                         continue
                     if any(
                         isinstance(item, ast.ClassDef)
@@ -261,46 +261,46 @@
     click.echo("Checking for pyproject.toml or setup.py ...\r", nl=False)
     curdir = os.getcwd()
     pyproject_toml_path = os.path.join(curdir, "pyproject.toml")
     setup_py_path = os.path.join(curdir, "setup.py")
     project_name = None
     if os.path.exists(pyproject_toml_path):
         try:
-            with open(pyproject_toml_path, "r", encoding="utf8") as f:
+            with open(pyproject_toml_path, encoding="utf8") as f:
                 pyproject_toml_content = f.read()
             project_name = tomlkit.parse(pyproject_toml_content)["tool"]["poetry"]["name"]
             click.echo(f"✅ I found a pyproject.toml for your project {project_name}.")
             ph("cli-pyproject-toml-found-name")
-        except Exception as e:
-            click.echo(f"✅ I found a pyproject.toml for your project.")
+        except Exception:
+            click.echo("✅ I found a pyproject.toml for your project.")
             ph("cli-pyproject-toml-found")
     else:
         if os.path.exists(setup_py_path):
-            with open(setup_py_path, "r", encoding="utf8") as f:
+            with open(setup_py_path, encoding="utf8") as f:
                 setup_py_content = f.read()
             project_name_match = re.search(
-                r"setup\s*\([^)]*?name\s*=\s*['\"](.*?)['\"]", setup_py_content, re.DOTALL
+                r"setup\s*\([^)]*?name\s*=\s*['\"](.*?)['\"]", setup_py_content, re.DOTALL,
             )
             if project_name_match:
                 project_name = project_name_match.group(1)
                 click.echo(f"✅ Found setup.py for your project {project_name}")
                 ph("cli-setup-py-found-name")
             else:
-                click.echo(f"✅ Found setup.py.")
+                click.echo("✅ Found setup.py.")
                 ph("cli-setup-py-found")
         click.echo(
             f"💡 I couldn't find a pyproject.toml in the current directory ({curdir}).{LF}"
             f"(make sure you're running `codeflash init` from your project's root directory!){LF}"
-            f"I need this file to store my configuration settings."
+            f"I need this file to store my configuration settings.",
         )
         ph("cli-no-pyproject-toml-or-setup-py")
 
         # Create a pyproject.toml file because it doesn't exist
         create_toml = inquirer.confirm(
-            f"Do you want me to create a pyproject.toml file in the current directory?",
+            "Do you want me to create a pyproject.toml file in the current directory?",
             default=True,
             show_default=False,
         )
         if create_toml:
             ph("cli-create-pyproject-toml")
             # Define a minimal pyproject.toml content
             new_pyproject_toml = tomlkit.document()
@@ -310,29 +310,29 @@
                     pyproject_file.write(tomlkit.dumps(new_pyproject_toml))
 
                 # Check if the pyproject.toml file was created
                 if os.path.exists(pyproject_toml_path):
                     click.echo(f"✅ Created a pyproject.toml file at {pyproject_toml_path}")
                     click.pause()
                 ph("cli-created-pyproject-toml")
-            except IOError as e:
+            except OSError:
                 click.echo(
-                    "❌ Failed to create pyproject.toml. Please check your disk permissions and available space."
+                    "❌ Failed to create pyproject.toml. Please check your disk permissions and available space.",
                 )
                 apologize_and_exit()
         else:
             click.echo("⏩️ Skipping pyproject.toml creation.")
             apologize_and_exit()
     click.echo()
     return project_name
 
 
 def apologize_and_exit() -> NoReturn:
     click.echo(
-        "💡 If you're having trouble, see https://app.codeflash.ai/app/getting-started for further help getting started with Codeflash!"
+        "💡 If you're having trouble, see https://app.codeflash.ai/app/getting-started for further help getting started with Codeflash!",
     )
     click.echo("👋 Exiting...")
     sys.exit(1)
 
 
 # Ask if the user wants Codeflash to optimize new GitHub PRs
 def prompt_github_action(setup_info: SetupInfo) -> None:
@@ -359,18 +359,18 @@
             os.makedirs(workflows_path, exist_ok=True)
             from importlib.resources import read_text
 
             py_version = sys.version_info
             python_version_string = f" {py_version.major}.{py_version.minor}"
 
             optimize_yml_content = read_text(
-                "codeflash.cli_cmds.workflows", "codeflash-optimize.yaml"
+                "codeflash.cli_cmds.workflows", "codeflash-optimize.yaml",
             )
             optimize_yml_content = optimize_yml_content.replace(
-                " {{ python_version }}", python_version_string
+                " {{ python_version }}", python_version_string,
             )
             with open(optimize_yaml_path, "w", encoding="utf8") as optimize_yml_file:
                 optimize_yml_file.write(optimize_yml_content)
             click.echo(f"✅ Created {optimize_yaml_path}{LF}")
             click.prompt(
                 f"Next, you'll need to add your CODEFLASH_API_KEY as a secret to your GitHub repo.{LF}"
                 + f"Press Enter to open your repo's secrets page at {get_github_secrets_page_url(repo)} ...{LF}"
@@ -396,55 +396,55 @@
                 type=click.STRING,
                 prompt_suffix="",
                 show_default=False,
             )
             click.launch(optimize_yaml_path)
             click.echo(
                 "📝 I opened the workflow file in your editor! You'll need to edit the steps that install the right Python "
-                + f"version and any project dependencies. See the comments in the file for more details.{LF}"
+                + f"version and any project dependencies. See the comments in the file for more details.{LF}",
             )
             click.pause()
             click.echo()
             click.echo(
-                f"🚀 Codeflash is now configured to automatically optimize new Github PRs!{LF}"
+                f"🚀 Codeflash is now configured to automatically optimize new Github PRs!{LF}",
             )
             ph("cli-github-workflow-created")
         else:
             click.echo("⏩️ Skipping GitHub workflow creation.")
             ph("cli-github-workflow-skipped")
 
 
 # Create or update the pyproject.toml file with the Codeflash dependency & configuration
 def configure_pyproject_toml(setup_info: SetupInfo) -> None:
     toml_path = os.path.join(os.getcwd(), "pyproject.toml")
     try:
-        with open(toml_path, "r", encoding="utf8") as pyproject_file:
+        with open(toml_path, encoding="utf8") as pyproject_file:
             pyproject_data = tomlkit.parse(pyproject_file.read())
     except FileNotFoundError:
         click.echo(
             f"I couldn't find a pyproject.toml in the current directory.{LF}"
-            f"Please create a new empty pyproject.toml file here, OR if you use poetry then run `poetry init`, OR run `codeflash init` again from a directory with an existing pyproject.toml file."
+            f"Please create a new empty pyproject.toml file here, OR if you use poetry then run `poetry init`, OR run `codeflash init` again from a directory with an existing pyproject.toml file.",
         )
         apologize_and_exit()
 
     codeflash_section = tomlkit.table()
     codeflash_section.add(
-        tomlkit.comment("All paths are relative to this pyproject.toml's directory.")
+        tomlkit.comment("All paths are relative to this pyproject.toml's directory."),
     )
     codeflash_section["module-root"] = setup_info.module_root
     codeflash_section["tests-root"] = setup_info.tests_root
     codeflash_section["test-framework"] = setup_info.test_framework
     codeflash_section["ignore-paths"] = setup_info.ignore_paths
 
     # Add the 'codeflash' section, ensuring 'tool' section exists
     tool_section = pyproject_data.get("tool", tomlkit.table())
     tool_section["codeflash"] = codeflash_section
     pyproject_data["tool"] = tool_section
 
-    click.echo(f"Writing Codeflash configuration ...\r", nl=False)
+    click.echo("Writing Codeflash configuration ...\r", nl=False)
     with open(toml_path, "w", encoding="utf8") as pyproject_file:
         pyproject_file.write(tomlkit.dumps(pyproject_data))
     click.echo(f"✅ Added Codeflash configuration to {toml_path}")
     click.echo()
 
 
 class CFAPIKeyType(click.ParamType):
@@ -462,15 +462,15 @@
             )
 
 
 # Returns True if the user entered a new API key, False if they used an existing one
 def prompt_api_key() -> bool:
     try:
         existing_api_key = get_codeflash_api_key()
-    except EnvironmentError:
+    except OSError:
         existing_api_key = None
     if existing_api_key:
         display_key = f"{existing_api_key[:3]}****{existing_api_key[-4:]}"
         click.echo(f"🔑 I found a CODEFLASH_API_KEY in your environment [{display_key}]!")
 
         use_existing_key = inquirer.confirm(
             message="Do you want to use this key?",
@@ -495,22 +495,21 @@
             hide_input=False,
             default="",
             type=CFAPIKeyType(),
             show_default=False,
         ).strip()
         if api_key:
             break
-        else:
-            if not browser_launched:
-                click.echo(
-                    f"Opening your Codeflash API key page. Grab a key from there!{LF}"
-                    "You can also open this link manually: https://app.codeflash.ai/app/apikeys"
-                )
-                click.launch("https://app.codeflash.ai/app/apikeys")
-                browser_launched = True  # This does not work on remote consoles
+        elif not browser_launched:
+            click.echo(
+                f"Opening your Codeflash API key page. Grab a key from there!{LF}"
+                "You can also open this link manually: https://app.codeflash.ai/app/apikeys",
+            )
+            click.launch("https://app.codeflash.ai/app/apikeys")
+            browser_launched = True  # This does not work on remote consoles
     shell_rc_path = get_shell_rc_path()
     if not shell_rc_path.exists() and os.name == "nt":
         # On Windows, create a batch file in the user's home directory (not auto-run, just used to store api key)
         shell_rc_path.touch()
         click.echo(f"✅ Created {shell_rc_path}")
     result = save_api_key_to_rc(api_key)
     if is_successful(result):
@@ -577,9 +576,9 @@
     os.remove(bubble_sort_path)
     click.echo(f"{LF}🗑️ Deleted {bubble_sort_path}")
 
     if process.returncode == 0:
         click.echo(f"{LF}✅ End-to-end test passed. Codeflash has been correctly set up!")
     else:
         click.echo(
-            f"{LF}❌ End-to-end test failed. Please check the logs above, and take a look at https://app.codeflash.ai/app/getting-started for help and troubleshooting."
+            f"{LF}❌ End-to-end test failed. Please check the logs above, and take a look at https://app.codeflash.ai/app/getting-started for help and troubleshooting.",
         )
```

### Comparing `codeflash-0.5.0/codeflash/cli_cmds/workflows/codeflash-optimize.yaml` & `codeflash-0.5.1/codeflash/cli_cmds/workflows/codeflash-optimize.yaml`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/code_utils/code_extractor.py` & `codeflash-0.5.1/codeflash/code_utils/code_extractor.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/code_utils/code_replacer.py` & `codeflash-0.5.1/codeflash/code_utils/code_replacer.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/code_utils/code_utils.py` & `codeflash-0.5.1/codeflash/code_utils/code_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ast
 import logging
 import os
 import site
 from tempfile import TemporaryDirectory
-from typing import Optional, List, Union, Tuple
+from typing import List, Optional, Tuple, Union
 
 
 def module_name_from_file_path(file_path: str, project_root: str) -> str:
     relative_path = os.path.relpath(file_path, project_root)
     module_path = relative_path.replace(os.sep, ".")
     if module_path.lower().endswith(".py"):
         module_path = module_path[:-3]
@@ -17,49 +17,48 @@
 def file_path_from_module_name(module_name: str, project_root: str) -> str:
     """Get file path from module path"""
     return os.path.join(project_root, module_name.replace(".", os.sep) + ".py")
 
 
 def ellipsis_in_ast(module: ast.AST) -> bool:
     for node in ast.walk(module):
-        if isinstance(node, ast.Constant):
-            if node.value == ...:
-                return True
+        if isinstance(node, ast.Constant) and node.value == ...:
+            return True
     return False
 
 
 def get_imports_from_file(
     file_path: Optional[str] = None,
     file_string: Optional[str] = None,
     file_ast: Optional[ast.AST] = None,
 ) -> List[Union[ast.Import, ast.ImportFrom]]:
     assert (
         sum([file_path is not None, file_string is not None, file_ast is not None]) == 1
     ), "Must provide exactly one of file_path, file_string, or file_ast"
     if file_path:
-        with open(file_path, "r", encoding="utf8") as file:
+        with open(file_path, encoding="utf8") as file:
             file_string = file.read()
     if file_ast is None:
         try:
             file_ast = ast.parse(file_string)
         except SyntaxError as e:
-            logging.error(f"Syntax error in code: {e}")
+            logging.exception(f"Syntax error in code: {e}")
             return []
     imports = []
     for node in ast.walk(file_ast):
         if isinstance(node, (ast.Import, ast.ImportFrom)):
             imports.append(node)
     return imports
 
 
 def get_all_function_names(code: str) -> Tuple[bool, List[str]]:
     try:
         module = ast.parse(code)
     except SyntaxError as e:
-        logging.error(f"Syntax error in code: {e}")
+        logging.exception(f"Syntax error in code: {e}")
         return False, []
 
     function_names = []
     for node in ast.walk(module):
         if isinstance(node, (ast.FunctionDef, ast.AsyncFunctionDef)):
             function_names.append(node.name)
     return True, function_names
@@ -69,12 +68,9 @@
     if not hasattr(get_run_tmp_file, "tmpdir"):
         get_run_tmp_file.tmpdir = TemporaryDirectory(prefix="codeflash_")
     return os.path.join(get_run_tmp_file.tmpdir.name, file_path)
 
 
 def path_belongs_to_site_packages(file_path: str) -> bool:
     return any(  # The definition is not part of a site-package Python library
-        [
-            file_path.startswith(site_package_path + os.sep)
-            for site_package_path in site.getsitepackages()
-        ]
+        [file_path.startswith(site_package_path + os.sep) for site_package_path in site.getsitepackages()],
     )
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/config_parser.py` & `codeflash-0.5.1/codeflash/code_utils/config_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,54 +7,54 @@
 
 def find_pyproject_toml(config_file=None):
     # Find the pyproject.toml file on the root of the project
 
     if config_file is not None:
         if not config_file.lower().endswith(".toml"):
             raise ValueError(
-                f"Config file {config_file} is not a valid toml file. Please recheck the path to pyproject.toml"
+                f"Config file {config_file} is not a valid toml file. Please recheck the path to pyproject.toml",
             )
         if not os.path.exists(config_file):
             raise ValueError(
-                f"Config file {config_file} does not exist. Please recheck the path to pyproject.toml"
+                f"Config file {config_file} does not exist. Please recheck the path to pyproject.toml",
             )
         return config_file
 
     else:
         dir_path = os.getcwd()
 
-        while not os.path.dirname(dir_path) == dir_path:
+        while os.path.dirname(dir_path) != dir_path:
             config_file = os.path.join(dir_path, "pyproject.toml")
             if os.path.exists(config_file):
                 return config_file
             # Search for pyproject.toml in the parent directories
             dir_path = os.path.dirname(dir_path)
         raise ValueError(
-            f"Could not find pyproject.toml in the current directory {os.getcwd()} or any of the parent directories. Please create it by running `poetry init`, or pass the path to pyproject.toml with the --config-file argument."
+            f"Could not find pyproject.toml in the current directory {os.getcwd()} or any of the parent directories. Please create it by running `poetry init`, or pass the path to pyproject.toml with the --config-file argument.",
         )
 
 
 def parse_config_file(config_file_path=None):
     config_file_path = find_pyproject_toml(config_file_path)
     try:
         with open(config_file_path, "rb") as f:
             data = tomlkit.parse(f.read())
     except tomlkit.exceptions.ParseError as e:
         raise ValueError(
-            f"Error while parsing the config file {config_file_path}. Please recheck the file for syntax errors. Error: {e}"
+            f"Error while parsing the config file {config_file_path}. Please recheck the file for syntax errors. Error: {e}",
         )
 
     try:
         tool = data["tool"]
         assert isinstance(tool, dict)
         config = tool["codeflash"]
     except tomlkit.exceptions.NonExistentKey:
         raise ValueError(
             f"Could not find the 'codeflash' block in the config file {config_file_path}. "
-            f"Please run 'codeflash init' to create the config file."
+            f"Please run 'codeflash init' to create the config file.",
         )
     assert isinstance(config, dict)
 
     # default values:
     path_keys = ["module-root", "tests-root"]
     path_list_keys = ["ignore-paths"]
     # TODO: minimum-peformance-gain should become a more dynamic auto-detection in the future
@@ -84,15 +84,15 @@
         if key in config:
             config[key] = bool(config[key])
         else:
             config[key] = bool_keys[key]
     for key in path_keys:
         if key in config:
             config[key] = os.path.realpath(
-                os.path.join(os.path.dirname(config_file_path), config[key])
+                os.path.join(os.path.dirname(config_file_path), config[key]),
             )
 
     for key in path_list_keys:
         if key in config:
             config[key] = [
                 os.path.realpath(os.path.join(os.path.dirname(config_file_path), path))
                 for path in config[key]
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/env_utils.py` & `codeflash-0.5.1/codeflash/code_utils/env_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 from codeflash.code_utils.shell_utils import read_api_key_from_shell_config
 
 
 @lru_cache(maxsize=1)
 def get_codeflash_api_key() -> Optional[str]:
     api_key = os.environ.get("CODEFLASH_API_KEY") or read_api_key_from_shell_config()
     if not api_key:
-        raise EnvironmentError(
+        raise OSError(
             "I didn't find a Codeflash API key in your environment.\n"
             + "You can generate one at https://app.codeflash.ai/app/apikeys,\n"
-            + "then set it as a CODEFLASH_API_KEY environment variable."
+            + "then set it as a CODEFLASH_API_KEY environment variable.",
         )
     if not api_key.startswith("cf-"):
-        raise EnvironmentError(
+        raise OSError(
             f"Your Codeflash API key seems to be invalid. It should start with a 'cf-' prefix; I found '{api_key}' instead.\n"
             + "You can generate one at https://app.codeflash.ai/app/apikeys,\n"
-            + "then set it as a CODEFLASH_API_KEY environment variable."
+            + "then set it as a CODEFLASH_API_KEY environment variable.",
         )
     return api_key
 
 
 def ensure_codeflash_api_key() -> bool:
     try:
         get_codeflash_api_key()
-    except EnvironmentError:
-        logging.error(
+    except OSError:
+        logging.exception(
             "Codeflash API key not found in your environment.\n"
             + "You can generate one at https://app.codeflash.ai/app/apikeys,\n"
-            + "then set it as a CODEFLASH_API_KEY environment variable."
+            + "then set it as a CODEFLASH_API_KEY environment variable.",
         )
         return False
     return True
 
 
 @lru_cache(maxsize=1)
 def get_codeflash_org_key() -> Optional[str]:
@@ -54,16 +54,16 @@
         return None
     else:
         return int(pr_number)
 
 
 def ensure_pr_number() -> bool:
     if not get_pr_number():
-        raise EnvironmentError(
-            "CODEFLASH_PR_NUMBER not found in environment variables; make sure the Github Action is setting this so Codeflash can comment on the right PR"
+        raise OSError(
+            "CODEFLASH_PR_NUMBER not found in environment variables; make sure the Github Action is setting this so Codeflash can comment on the right PR",
         )
     return True
 
 
 def ensure_git_repo(module_root: str) -> bool:
     try:
         _ = git.Repo(module_root, search_parent_directories=True).git_dir
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/formatter.py` & `codeflash-0.5.1/codeflash/code_utils/formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 import logging
 import os.path
 import subprocess
+
 import isort
 
 
 def format_code(
-    formatter_cmd: str, imports_sort_cmd: str, should_sort_imports: bool, path: str
+    formatter_cmd: str, imports_sort_cmd: str, should_sort_imports: bool, path: str,
 ) -> str:
     # TODO: Only allow a particular whitelist of formatters here to prevent arbitrary code execution
     if formatter_cmd.lower() == "disabled":
         if should_sort_imports:
             return sort_imports(imports_sort_cmd, should_sort_imports, path)
 
-        with open(path, "r", encoding="utf8") as f:
+        with open(path, encoding="utf8") as f:
             new_code = f.read()
         return new_code
 
     formatter_cmd_list = [chunk for chunk in formatter_cmd.split(" ") if chunk != ""]
     logging.info(f"Formatting code with {formatter_cmd} ...")
     # black currently does not have a stable public API, so we are using the CLI
     # the main problem is custom config parsing https://github.com/psf/black/issues/779
     assert os.path.exists(path), f"File {path} does not exist. Cannot format the file. Exiting..."
     result = subprocess.run(
-        formatter_cmd_list + [path], stdout=subprocess.PIPE, stderr=subprocess.PIPE
+        formatter_cmd_list + [path], stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False,
     )
     if result.returncode == 0:
         logging.info("OK")
     else:
         logging.error(f"Failed to format code with {formatter_cmd}")
 
     if should_sort_imports:
         return sort_imports(imports_sort_cmd, should_sort_imports, path)
 
-    with open(path, "r", encoding="utf8") as f:
+    with open(path, encoding="utf8") as f:
         new_code = f.read()
 
     return new_code
 
 
 def sort_imports(imports_sort_cmd: str, should_sort_imports: bool, path: str) -> str:
     if imports_sort_cmd.lower() == "disabled":
-        with open(path, "r", encoding="utf8") as f:
+        with open(path, encoding="utf8") as f:
             code = f.read()
         return code
 
     if should_sort_imports:
         # Deduplicate and sort imports
         isort.file(path)
 
-        with open(path, "r", encoding="utf8") as f:
+        with open(path, encoding="utf8") as f:
             new_code = f.read()
         return new_code
     else:
         # Return original code
-        with open(path, "r", encoding="utf8") as f:
+        with open(path, encoding="utf8") as f:
             code = f.read()
         return code
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/git_utils.py` & `codeflash-0.5.1/codeflash/code_utils/git_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import git
 from git import Repo
 from unidiff import PatchSet
 
 
 def get_git_diff(
-    repo_directory: str = os.getcwd(), uncommitted_changes: bool = False
+    repo_directory: str = os.getcwd(), uncommitted_changes: bool = False,
 ) -> dict[str, list[int]]:
     repository = git.Repo(repo_directory, search_parent_directories=True)
     commit = repository.head.commit
     if uncommitted_changes:
         uni_diff_text = repository.git.diff(
-            None, "HEAD", ignore_blank_lines=True, ignore_space_at_eol=True
+            None, "HEAD", ignore_blank_lines=True, ignore_space_at_eol=True,
         )
     else:
         uni_diff_text = repository.git.diff(
             commit.hexsha + "^1",
             commit.hexsha,
             ignore_blank_lines=True,
             ignore_space_at_eol=True,
@@ -50,16 +50,15 @@
         logging.debug("deleted lines : " + str(del_line_no))
 
         change_list[file_path] = add_line_no
     return change_list
 
 
 def get_current_branch(repo: Optional[Repo] = None) -> str:
-    """
-    Returns the name of the current branch in the given repository.
+    """Returns the name of the current branch in the given repository.
 
     :param repo: An optional Repo object. If not provided, the function will
                  search for a repository in the current and parent directories.
     :return: The name of the current branch.
     """
     repository: Repo = repo if repo else git.Repo(search_parent_directories=True)
     return repository.active_branch.name
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/instrument_existing_tests.py` & `codeflash-0.5.1/codeflash/code_utils/instrument_existing_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ast
 from _ast import ClassDef
 from typing import Any, Optional, Tuple
 
-from codeflash.code_utils.code_utils import module_name_from_file_path, get_run_tmp_file
+from codeflash.code_utils.code_utils import get_run_tmp_file, module_name_from_file_path
 
 
 class ReplaceCallNodeWithName(ast.NodeTransformer):
     def __init__(self, only_function_name, new_variable_name="codeflash_return_value"):
         self.only_function_name = only_function_name
         self.new_variable_name = new_variable_name
 
@@ -22,15 +22,19 @@
 
 class InjectPerfOnly(ast.NodeTransformer):
     def __init__(self, function_name, module_path):
         self.only_function_name = function_name
         self.module_path = module_path
 
     def update_line_node(
-        self, test_node, node_name, index: str, test_class_name: Optional[str] = None
+        self,
+        test_node,
+        node_name,
+        index: str,
+        test_class_name: Optional[str] = None,
     ):
         call_node = None
         for node in ast.walk(test_node):
             if isinstance(node, ast.Call) and (
                 (hasattr(node.func, "id") and node.func.id == self.only_function_name)
                 or (hasattr(node.func, "attr") and node.func.attr == self.only_function_name)
             ):
@@ -118,25 +122,26 @@
                                 attr="connect",
                                 ctx=ast.Load(),
                             ),
                             args=[
                                 ast.JoinedStr(
                                     values=[
                                         ast.Constant(
-                                            value=f"{get_run_tmp_file('test_return_values_')}"
+                                            value=f"{get_run_tmp_file('test_return_values_')}",
                                         ),
                                         ast.FormattedValue(
                                             value=ast.Name(
-                                                id="codeflash_iteration", ctx=ast.Load()
+                                                id="codeflash_iteration",
+                                                ctx=ast.Load(),
                                             ),
                                             conversion=-1,
                                         ),
                                         ast.Constant(value=".sqlite"),
-                                    ]
-                                )
+                                    ],
+                                ),
                             ],
                             keywords=[],
                         ),
                         lineno=node.lineno + 2,
                         col_offset=node.col_offset,
                     ),
                     ast.Assign(
@@ -160,16 +165,16 @@
                                 attr="execute",
                                 ctx=ast.Load(),
                             ),
                             args=[
                                 ast.Constant(
                                     value="CREATE TABLE IF NOT EXISTS test_results (test_module_path TEXT,"
                                     " test_class_name TEXT, test_function_name TEXT, function_getting_tested TEXT,"
-                                    " iteration_id TEXT, runtime INTEGER, return_value BLOB)"
-                                )
+                                    " iteration_id TEXT, runtime INTEGER, return_value BLOB)",
+                                ),
                             ],
                             keywords=[],
                         ),
                         lineno=node.lineno + 4,
                         col_offset=node.col_offset,
                     ),
                 ]
@@ -180,62 +185,68 @@
                             func=ast.Attribute(
                                 value=ast.Name(id="codeflash_con", ctx=ast.Load()),
                                 attr="close",
                                 ctx=ast.Load(),
                             ),
                             args=[],
                             keywords=[],
-                        )
-                    )
+                        ),
+                    ),
                 ]
             )
             i = len(node.body) - 1
             while i >= 0:
                 line_node = node.body[i]
                 # TODO: Validate if the functional call actually did not raise any exceptions
 
                 if isinstance(line_node, (ast.With, ast.For, ast.While)):
                     j = len(line_node.body) - 1
                     while j >= 0:
                         compound_line_node = line_node.body[j]
                         for internal_node in ast.walk(compound_line_node):
                             if self.is_target_function_line(internal_node):
                                 line_node.body[j : j + 1] = self.update_line_node(
-                                    internal_node, node.name, str(i) + "_" + str(j), test_class_name
+                                    internal_node,
+                                    node.name,
+                                    str(i) + "_" + str(j),
+                                    test_class_name,
                                 )
                                 break
                         j -= 1
-                else:
-                    if self.is_target_function_line(line_node):
-                        node.body[i : i + 1] = self.update_line_node(
-                            line_node, node.name, str(i), test_class_name
-                        )
+                elif self.is_target_function_line(line_node):
+                    node.body[i : i + 1] = self.update_line_node(
+                        line_node,
+                        node.name,
+                        str(i),
+                        test_class_name,
+                    )
                 i -= 1
         return node
 
 
 class FunctionImportedAsVisitor(ast.NodeVisitor):
     """This checks if a function has been imported as an alias. We only care about the alias then.
     from numpy import array as np_array
-    np_array is what we want"""
+    np_array is what we want
+    """
 
     def __init__(self, original_function_name):
         self.original_function_name = original_function_name
         self.imported_as_function_name = original_function_name
 
     # TODO: Validate if the function imported is actually from the right module
     def visit_ImportFrom(self, node: ast.ImportFrom):
         for alias in node.names:
             if alias.name == self.original_function_name:
-                if hasattr(alias, "asname") and not alias.asname is None:
+                if hasattr(alias, "asname") and alias.asname is not None:
                     self.imported_as_function_name = alias.asname
 
 
 def inject_profiling_into_existing_test(test_path, function_name, root_path) -> Tuple[bool, str]:
-    with open(test_path, "r", encoding="utf8") as f:
+    with open(test_path, encoding="utf8") as f:
         test_code = f.read()
     try:
         tree = ast.parse(test_code)
     except SyntaxError as e:
         print(f"Syntax error in code: {e}")
         return False, None
     # TODO: Pass the full name of function here, otherwise we can run into namespace clashes
@@ -245,15 +256,15 @@
     module_path = module_name_from_file_path(test_path, root_path)
     tree = InjectPerfOnly(function_name, module_path).visit(tree)
     new_imports = [
         ast.Import(names=[ast.alias(name="time")]),
         ast.Import(names=[ast.alias(name="gc")]),
         ast.Import(names=[ast.alias(name="os")]),
         ast.Import(names=[ast.alias(name="sqlite3")]),
-        ast.Import(names=[ast.alias(name="pickle")]),
+        ast.Import(names=[ast.alias(name="dill", asname="pickle")]),
     ]
     tree.body = new_imports + [create_wrapper_function(function_name, module_path)] + tree.body
 
     return True, ast.unparse(tree)
 
 
 def create_wrapper_function(function_name, module_path):
@@ -280,29 +291,33 @@
         ),
         body=[
             ast.Assign(
                 targets=[ast.Name(id="test_id", ctx=ast.Store())],
                 value=ast.JoinedStr(
                     values=[
                         ast.FormattedValue(
-                            value=ast.Name(id="test_module_name", ctx=ast.Load()), conversion=-1
+                            value=ast.Name(id="test_module_name", ctx=ast.Load()),
+                            conversion=-1,
                         ),
                         ast.Constant(value=":"),
                         ast.FormattedValue(
-                            value=ast.Name(id="test_class_name", ctx=ast.Load()), conversion=-1
+                            value=ast.Name(id="test_class_name", ctx=ast.Load()),
+                            conversion=-1,
                         ),
                         ast.Constant(value=":"),
                         ast.FormattedValue(
-                            value=ast.Name(id="test_name", ctx=ast.Load()), conversion=-1
+                            value=ast.Name(id="test_name", ctx=ast.Load()),
+                            conversion=-1,
                         ),
                         ast.Constant(value=":"),
                         ast.FormattedValue(
-                            value=ast.Name(id="line_id", ctx=ast.Load()), conversion=-1
+                            value=ast.Name(id="line_id", ctx=ast.Load()),
+                            conversion=-1,
                         ),
-                    ]
+                    ],
                 ),
                 lineno=lineno + 1,
             ),
             ast.If(
                 test=ast.UnaryOp(
                     op=ast.Not(),
                     operand=ast.Call(
@@ -317,33 +332,33 @@
                 body=[
                     ast.Assign(
                         targets=[
                             ast.Attribute(
                                 value=ast.Name(id="codeflash_wrap", ctx=ast.Load()),
                                 attr="index",
                                 ctx=ast.Store(),
-                            )
+                            ),
                         ],
                         value=ast.Dict(keys=[], values=[]),
                         lineno=lineno + 3,
-                    )
+                    ),
                 ],
                 orelse=[],
                 lineno=lineno + 2,
             ),
             ast.If(
                 test=ast.Compare(
                     left=ast.Name(id="test_id", ctx=ast.Load()),
                     ops=[ast.In()],
                     comparators=[
                         ast.Attribute(
                             value=ast.Name(id="codeflash_wrap", ctx=ast.Load()),
                             attr="index",
                             ctx=ast.Load(),
-                        )
+                        ),
                     ],
                 ),
                 body=[
                     ast.AugAssign(
                         target=ast.Subscript(
                             value=ast.Attribute(
                                 value=ast.Name(id="codeflash_wrap", ctx=ast.Load()),
@@ -352,32 +367,32 @@
                             ),
                             slice=ast.Name(id="test_id", ctx=ast.Load()),
                             ctx=ast.Store(),
                         ),
                         op=ast.Add(),
                         value=ast.Constant(value=1),
                         lineno=lineno + 5,
-                    )
+                    ),
                 ],
                 orelse=[
                     ast.Assign(
                         targets=[
                             ast.Subscript(
                                 value=ast.Attribute(
                                     value=ast.Name(id="codeflash_wrap", ctx=ast.Load()),
                                     attr="index",
                                     ctx=ast.Load(),
                                 ),
                                 slice=ast.Name(id="test_id", ctx=ast.Load()),
                                 ctx=ast.Store(),
-                            )
+                            ),
                         ],
                         value=ast.Constant(value=0),
                         lineno=lineno + 6,
-                    )
+                    ),
                 ],
                 lineno=lineno + 4,
             ),
             ast.Assign(
                 targets=[
                     ast.Name(id="codeflash_test_index", ctx=ast.Store()),
                 ],
@@ -393,21 +408,23 @@
                 lineno=lineno + 7,
             ),
             ast.Assign(
                 targets=[ast.Name(id="invocation_id", ctx=ast.Store())],
                 value=ast.JoinedStr(
                     values=[
                         ast.FormattedValue(
-                            value=ast.Name(id="line_id", ctx=ast.Load()), conversion=-1
+                            value=ast.Name(id="line_id", ctx=ast.Load()),
+                            conversion=-1,
                         ),
                         ast.Constant(value="_"),
                         ast.FormattedValue(
-                            value=ast.Name(id="codeflash_test_index", ctx=ast.Load()), conversion=-1
+                            value=ast.Name(id="codeflash_test_index", ctx=ast.Load()),
+                            conversion=-1,
                         ),
-                    ]
+                    ],
                 ),
                 lineno=lineno + 8,
             ),
             ast.Expr(
                 value=ast.Call(
                     func=ast.Attribute(
                         value=ast.Name(id="gc", ctx=ast.Load()),
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/shell_utils.py` & `codeflash-0.5.1/codeflash/code_utils/shell_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 from returns.result import Failure, Result, Success
 
 from codeflash.code_utils.compat import LF
 
 if os.name == "nt":  # Windows
     SHELL_RC_EXPORT_PATTERN = re.compile(r"^set CODEFLASH_API_KEY=(cf-.*)$", re.M)
-    SHELL_RC_EXPORT_PREFIX = f"set CODEFLASH_API_KEY="
+    SHELL_RC_EXPORT_PREFIX = "set CODEFLASH_API_KEY="
 else:
     SHELL_RC_EXPORT_PATTERN = re.compile(r'^export CODEFLASH_API_KEY="?(cf-[^\s"]+)"?$', re.M)
-    SHELL_RC_EXPORT_PREFIX = f"export CODEFLASH_API_KEY="
+    SHELL_RC_EXPORT_PREFIX = "export CODEFLASH_API_KEY="
 
 
 def read_api_key_from_shell_config() -> Optional[str]:
     try:
         shell_rc_path = get_shell_rc_path()
-        with open(shell_rc_path, "r", encoding="utf8") as shell_rc:
+        with open(shell_rc_path, encoding="utf8") as shell_rc:
             shell_contents = shell_rc.read()
             matches = SHELL_RC_EXPORT_PATTERN.findall(shell_contents)
             return matches[-1] if matches else None
     except FileNotFoundError:
         return None
 
 
@@ -35,15 +35,15 @@
         shell_rc_filename = {
             "zsh": ".zshrc",
             "ksh": ".kshrc",
             "csh": ".cshrc",
             "tcsh": ".cshrc",
             "dash": ".profile",
         }.get(
-            shell, ".bashrc"
+            shell, ".bashrc",
         )  # map each shell to its config file and default to .bashrc
         return Path.home() / shell_rc_filename
 
 
 def get_api_key_export_line(api_key: str) -> str:
     return f"{SHELL_RC_EXPORT_PREFIX}{api_key}"
 
@@ -58,30 +58,30 @@
                 if not shell_contents:
                     shell_contents = "@echo off"
             existing_api_key = read_api_key_from_shell_config()
 
             if existing_api_key:
                 # Replace the existing API key line
                 updated_shell_contents = re.sub(
-                    SHELL_RC_EXPORT_PATTERN, api_key_line, shell_contents
+                    SHELL_RC_EXPORT_PATTERN, api_key_line, shell_contents,
                 )
                 action = "Updated CODEFLASH_API_KEY in"
             else:
                 # Append the new API key line
                 updated_shell_contents = shell_contents.rstrip() + f"{LF}{api_key_line}{LF}"
                 action = "Added CODEFLASH_API_KEY to"
 
             shell_file.seek(0)
             shell_file.write(updated_shell_contents)
             shell_file.truncate()
         return Success(f"✅ {action} {shell_rc_path}")
     except PermissionError:
         return Failure(
             f"💡 I tried adding your Codeflash API key to {shell_rc_path} - but seems like I don't have permissions to do so.{LF}"
-            f"You'll need to open it yourself and add the following line:{LF}{LF}{api_key_line}{LF}"
+            f"You'll need to open it yourself and add the following line:{LF}{LF}{api_key_line}{LF}",
         )
     except FileNotFoundError:
         return Failure(
             f"💡 I went to save your Codeflash API key to {shell_rc_path}, but noticed that it doesn't exist.{LF}"
             f"To ensure your Codeflash API key is automatically loaded into your environment at startup, you can create {shell_rc_path} and add the following line:{LF}"
             f"{LF}{api_key_line}{LF}",
         )
```

### Comparing `codeflash-0.5.0/codeflash/code_utils/sqlalchemy_utils.py` & `codeflash-0.5.1/codeflash/code_utils/sqlalchemy_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/code_utils/time_utils.py` & `codeflash-0.5.1/codeflash/code_utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/discovery/discover_unit_tests.py` & `codeflash-0.5.1/codeflash/discovery/discover_unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     test_function: str
     test_suite: Optional[str]
 
     @classmethod
     def from_pytest_stdout_line_co(cls, module: str, function: str, directory: str):
         absolute_test_path = os.path.join(directory, module)
         assert os.path.exists(
-            absolute_test_path
+            absolute_test_path,
         ), f"Test discovery failed - Test file does not exist {absolute_test_path}"
         return cls(
             test_file=absolute_test_path,
             test_class=None,
             test_function=function,
             test_suite=None,
         )
 
     @classmethod
     def from_pytest_stdout_line_q(cls, line: str, pytest_rootdir: str):
         parts = line.split("::")
         absolute_test_path = os.path.join(pytest_rootdir, parts[0])
         assert os.path.exists(
-            absolute_test_path
+            absolute_test_path,
         ), f"Test discovery failed - Test file does not exist {absolute_test_path}"
         if len(parts) == 3:
             return cls(
                 test_file=absolute_test_path,
                 test_class=parts[1],
                 test_function=parts[2],
                 test_suite=None,
@@ -117,15 +117,15 @@
 def discover_tests_pytest(cfg: TestConfig) -> Dict[str, List[TestsInFile]]:
     tests_root = cfg.tests_root
     project_root = cfg.project_root_path
     pytest_cmd_list = [chunk for chunk in cfg.pytest_cmd.split(" ") if chunk != ""]
     pytest_result = subprocess.run(
         pytest_cmd_list + [f"{tests_root}", "--co", "-q", "-m", "not skip"],
         stdout=subprocess.PIPE,
-        cwd=project_root,
+        cwd=project_root, check=False,
     )
 
     pytest_stdout = pytest_result.stdout.decode("utf-8")
 
     parse_type = ParseType.Q
     if "rootdir: " not in pytest_stdout:
         pytest_rootdir = get_pytest_rootdir_only(pytest_cmd_list, tests_root, project_root)
@@ -181,38 +181,38 @@
                             continue
                         details = get_test_details(test_2)
                         if details is not None:
                             file_to_test_map[details.test_module_path].append(
                                 {
                                     "test_function": details.test_function,
                                     "test_suite_name": details.test_suite_name,
-                                }
+                                },
                             )
                 else:
                     details = get_test_details(test)
                     if details is not None:
                         file_to_test_map[details.test_module_path].append(
                             {
                                 "test_function": details.test_function,
                                 "test_suite_name": details.test_suite_name,
-                            }
+                            },
                         )
     return process_test_files(file_to_test_map, cfg)
 
 
 def discover_parameters_unittest(function_name: str):
     function_name = function_name.split("_")
     if len(function_name) > 1 and function_name[-1].isdigit():
         return True, "_".join(function_name[:-1]), function_name[-1]
 
     return False, function_name, None
 
 
 def process_test_files(
-    file_to_test_map: Dict[str, List[Dict[str, str]]], cfg: TestConfig
+    file_to_test_map: Dict[str, List[Dict[str, str]]], cfg: TestConfig,
 ) -> Dict[str, List[TestsInFile]]:
     project_root_path = cfg.project_root_path
     test_framework = cfg.test_framework
     function_to_test_map = defaultdict(list)
     jedi_project = jedi.Project(path=project_root_path)
 
     for test_file, functions in file_to_test_map.items():
@@ -227,18 +227,17 @@
                 functions_to_search = [elem["test_function"] for elem in functions]
                 for function in functions_to_search:
                     if "[" in function:
                         function_name = re.split(r"\[|\]", function)[0]
                         parameters = re.split(r"\[|\]", function)[1]
                         if name.name == function_name and name.type == "function":
                             test_functions.add(TestFunction(name.name, None, parameters))
-                    else:
-                        if name.name == function and name.type == "function":
-                            test_functions.add(TestFunction(name.name, None, None))
-                            break
+                    elif name.name == function and name.type == "function":
+                        test_functions.add(TestFunction(name.name, None, None))
+                        break
             if test_framework == "unittest":
                 functions_to_search = [elem["test_function"] for elem in functions]
                 test_suites = [elem["test_suite_name"] for elem in functions]
                 if name.name in test_suites and name.type == "class":
                     for def_name in all_defs:
                         if (
                             def_name.type == "function"
@@ -250,15 +249,15 @@
                                     is_parameterized,
                                     new_function,
                                     parameters,
                                 ) = discover_parameters_unittest(function)
 
                                 if is_parameterized and new_function == def_name.name:
                                     test_functions.add(
-                                        TestFunction(def_name.name, name.name, parameters)
+                                        TestFunction(def_name.name, name.name, parameters),
                                     )
                                 elif function == def_name.name:
                                     test_functions.add(TestFunction(def_name.name, name.name, None))
 
         test_functions_list = list(test_functions)
         test_functions_raw = [elem.function_name for elem in test_functions_list]
 
@@ -278,15 +277,15 @@
                     definition = script.goto(
                         line=name.line,
                         column=name.column,
                         follow_imports=True,
                         follow_builtin_imports=False,
                     )
                 except Exception as e:
-                    logging.error(str(e))
+                    logging.exception(str(e))
                     continue
                 if definition and definition[0].type == "function":
                     definition_path = str(definition[0].module_path)
                     # The definition is part of this project and not defined within the original function
                     if (
                         definition_path.startswith(str(project_root_path) + os.sep)
                         and definition[0].module_name != name.module_name
@@ -294,24 +293,24 @@
                         if scope_parameters is not None:
                             if test_framework == "pytest":
                                 scope_test_function += "[" + scope_parameters + "]"
                             if test_framework == "unittest":
                                 scope_test_function += "_" + scope_parameters
 
                         function_to_test_map[definition[0].full_name].append(
-                            TestsInFile(test_file, None, scope_test_function, scope_test_suite)
+                            TestsInFile(test_file, None, scope_test_function, scope_test_suite),
                         )
     deduped_function_to_test_map = {}
     for function, tests in function_to_test_map.items():
         deduped_function_to_test_map[function] = list(set(tests))
     return deduped_function_to_test_map
 
 
 def parse_pytest_stdout(
-    pytest_stdout: str, pytest_rootdir: str, tests_root: str, parse_type: ParseType
+    pytest_stdout: str, pytest_rootdir: str, tests_root: str, parse_type: ParseType,
 ) -> List[TestsInFile]:
     test_results = []
     if parse_type == ParseType.Q:
         for line in pytest_stdout.splitlines():
             if line.startswith("==") or line.startswith("\n") or line == "":
                 break
             try:
@@ -380,14 +379,14 @@
 
         elif "<Function " in line and module is not None:
             function = re.match(r"\s*<Function (.+)>", line)
             if function:
                 function = function.group(1)
                 try:
                     test_result = TestsInFile.from_pytest_stdout_line_co(
-                        module, function, directory
+                        module, function, directory,
                     )
                     test_results.append(test_result)
                 except ValueError as e:
                     logging.warning(str(e))
 
     return test_results
```

### Comparing `codeflash-0.5.0/codeflash/discovery/functions_to_optimize.py` & `codeflash-0.5.1/codeflash/discovery/functions_to_optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import ast
 import logging
 import os
 import random
-from _ast import ClassDef, FunctionDef, AsyncFunctionDef
-from typing import Dict, Optional, List, Tuple, Union
+from _ast import AsyncFunctionDef, ClassDef, FunctionDef
+from typing import Dict, List, Optional, Tuple, Union
 
 import git
 import libcst as cst
 from libcst import CSTNode
 from libcst.metadata import CodeRange
 from pydantic.dataclasses import dataclass
 
-from codeflash.code_utils.code_utils import (
-    path_belongs_to_site_packages,
-    module_name_from_file_path,
-)
+from codeflash.code_utils.code_utils import module_name_from_file_path, path_belongs_to_site_packages
 from codeflash.code_utils.git_utils import get_git_diff
 from codeflash.verification.verification_utils import TestConfig
 
 
 class ReturnStatementVisitor(cst.CSTVisitor):
     def __init__(self) -> None:
         super().__init__()
@@ -41,42 +38,40 @@
         node.visit(return_visitor)
         if return_visitor.has_return_statement:
             pos: CodeRange = self.get_metadata(cst.metadata.PositionProvider, node)
             parents: Optional[CSTNode] = self.get_metadata(cst.metadata.ParentNodeProvider, node)
             ast_parents: list[FunctionParent] = []
             while parents is not None:
                 if isinstance(parents, (cst.FunctionDef, cst.ClassDef)):
-                    ast_parents.append(
-                        FunctionParent(parents.name.value, parents.__class__.__name__)
-                    )
+                    ast_parents.append(FunctionParent(parents.name.value, parents.__class__.__name__))
                 parents = self.get_metadata(cst.metadata.ParentNodeProvider, parents, default=None)
             self.functions.append(
                 FunctionToOptimize(
                     function_name=node.name.value,
                     file_path=self.file_path,
                     parents=list(reversed(ast_parents)),
                     starting_line=pos.start.line,
                     ending_line=pos.end.line,
-                )
+                ),
             )
 
 
 class FunctionWithReturnStatement(ast.NodeVisitor):
     def __init__(self, file_path: str) -> None:
         self.functions: List[FunctionToOptimize] = []
         self.ast_path: List[FunctionParent] = []
         self.file_path: str = file_path
 
     def visit_FunctionDef(self, node: FunctionDef) -> None:
         # Check if the function has a return statement and add it to the list
         if function_has_return_statement(node):
             self.functions.append(
                 FunctionToOptimize(
-                    function_name=node.name, file_path=self.file_path, parents=self.ast_path[:]
-                )
+                    function_name=node.name, file_path=self.file_path, parents=self.ast_path[:],
+                ),
             )
         # Continue visiting the body of the function to find nested functions
         self.generic_visit(node)
 
     def generic_visit(self, node: ast.AST) -> None:
         if isinstance(node, (FunctionDef, AsyncFunctionDef, ClassDef)):
             self.ast_path.append(FunctionParent(node.name, node.__class__.__name__))
@@ -108,14 +103,27 @@
 
     def __str__(self) -> str:
         return (
             f"{self.file_path}:{'.'.join([p.name for p in self.parents])}"
             f"{'.' if self.parents else ''}{self.function_name}"
         )
 
+    @property
+    def qualified_name(self):
+        return (
+            self.function_name
+            if self.parents == []
+            else ".".join(
+                [
+                    self.parents[0].name,
+                    self.function_name,
+                ],
+            )
+        )
+
 
 def get_functions_to_optimize_by_file(
     optimize_all: str,
     file: Optional[str],
     function: Optional[str],
     test_cfg: TestConfig,
     ignore_paths: List[str],
@@ -133,39 +141,39 @@
             found_function = None
             for fn in functions[file]:
                 if only_function_name == fn.function_name:
                     found_function = fn
             if found_function is None:
                 raise ValueError(
                     f"Function {only_function_name} not found in file {file} or"
-                    f" the function does not have a 'return' statement."
+                    f" the function does not have a 'return' statement.",
                 )
             functions[file] = [found_function]
     else:
         logging.info("Finding all functions modified in the current git diff ...")
         functions = get_functions_within_git_diff()
     filtered_modified_functions, functions_count = filter_functions(
-        functions, test_cfg.tests_root, ignore_paths, project_root, module_root
+        functions, test_cfg.tests_root, ignore_paths, project_root, module_root,
     )
     logging.info("Found %d functions to optimize", functions_count)
     return filtered_modified_functions, functions_count
 
 
 def get_functions_within_git_diff() -> Dict[str, List[FunctionToOptimize]]:
     modified_lines: dict[str, list[int]] = get_git_diff(uncommitted_changes=False)
     modified_functions: Dict[str, List[FunctionToOptimize]] = {}
     for path in modified_lines:
         if not os.path.exists(path):
             continue
-        with open(path, "r", encoding="utf8") as f:
+        with open(path, encoding="utf8") as f:
             file_content = f.read()
             try:
                 wrapper = cst.metadata.MetadataWrapper(cst.parse_module(file_content))
             except Exception as e:
-                logging.error(e)
+                logging.exception(e)
                 continue
             function_lines = FunctionVisitor(file_path=path)
             wrapper.visit(function_lines)
             modified_functions[path] = [
                 function_to_optimize
                 for function_to_optimize in function_lines.functions
                 if (start_line := function_to_optimize.starting_line) is not None
@@ -191,19 +199,19 @@
     random.shuffle(files_list)
     functions_shuffled = dict(files_list)
     return functions_shuffled
 
 
 def find_all_functions_in_file(file_path: str) -> Dict[str, List[FunctionToOptimize]]:
     functions: Dict[str, List[FunctionToOptimize]] = {}
-    with open(file_path, "r", encoding="utf8") as f:
+    with open(file_path, encoding="utf8") as f:
         try:
             ast_module = ast.parse(f.read())
         except Exception as e:
-            logging.error(e)
+            logging.exception(e)
             return functions
         function_name_visitor = FunctionWithReturnStatement(file_path)
         function_name_visitor.visit(ast_module)
         functions[file_path] = function_name_visitor.functions
     return functions
 
 
@@ -230,17 +238,15 @@
     module_root: str,
 ) -> Tuple[Dict[str, List[FunctionToOptimize]], int]:
     # Remove any function that we don't want to optimize
 
     # Ignore files with submodule path
     submodule_paths = []
     if is_git_repo(module_root):
-        submodule_paths = ignored_submodule_paths(
-            git.Repo(module_root, search_parent_directories=True)
-        )
+        submodule_paths = ignored_submodule_paths(git.Repo(module_root, search_parent_directories=True))
     filtered_modified_functions: Dict[str, List[FunctionToOptimize]] = {}
     functions_count: int = 0
     test_functions_removed_count: int = 0
     non_modules_removed_count: int = 0
     site_packages_removed_count: int = 0
     ignore_paths_removed_count: int = 0
     malformed_paths_count: int = 0
```

### Comparing `codeflash-0.5.0/codeflash/github/PrComment.py` & `codeflash-0.5.1/codeflash/github/PrComment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Union
 
-from codeflash.verification.test_results import TestResults
 from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
+from codeflash.verification.test_results import TestResults
+
 
 @dataclass(frozen=True, config={"arbitrary_types_allowed": True})
 class PrComment:
     optimization_explanation: str
     best_runtime: int
     original_runtime: int
     function_name: str
```

### Comparing `codeflash-0.5.0/codeflash/main.py` & `codeflash-0.5.1/codeflash/optimization/optimizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-"""Thanks for being curious about how codeflash works! If you might want to work with us on finally making performance a
-solved problem, please reach out to us at careers@codeflash.ai. We're hiring!
-"""
-
-from __future__ import annotations
-
 import concurrent.futures
 import logging
 import os
 import pathlib
 import uuid
-from argparse import SUPPRESS, ArgumentParser, Namespace
+from argparse import Namespace
 from collections import defaultdict
-from typing import IO, Dict, Tuple, Union
+from typing import IO, Dict, List, Optional, Tuple, Union
 
 import libcst as cst
+from pydantic import BaseModel
+from returns.pipeline import is_successful
+from returns.result import Failure, Result, Success
 
-from codeflash.api.aiservice import log_results, optimize_python_code
-from codeflash.cli_cmds.cli import process_cmd_args
-from codeflash.cli_cmds.cmd_init import CODEFLASH_LOGO
+from codeflash.api.aiservice import Optimization, log_results, optimize_python_code
 from codeflash.code_utils import env_utils
 from codeflash.code_utils.code_extractor import extract_code
 from codeflash.code_utils.code_replacer import replace_function_definitions_in_module
 from codeflash.code_utils.code_utils import (
     get_all_function_names,
     get_run_tmp_file,
     module_name_from_file_path,
@@ -31,94 +26,68 @@
     MAX_CUMULATIVE_TEST_RUNTIME_NANOSECONDS,
     MAX_FUNCTION_TEST_SECONDS,
     MAX_TEST_FUNCTION_RUNS,
     MAX_TEST_RUN_ITERATIONS,
     N_CANDIDATES,
 )
 from codeflash.code_utils.formatter import format_code, sort_imports
-from codeflash.code_utils.instrument_existing_tests import (
-    inject_profiling_into_existing_test,
-)
+from codeflash.code_utils.instrument_existing_tests import inject_profiling_into_existing_test
 from codeflash.code_utils.time_utils import humanize_runtime
 from codeflash.discovery.discover_unit_tests import TestsInFile, discover_unit_tests
 from codeflash.discovery.functions_to_optimize import (
     FunctionParent,
     FunctionToOptimize,
     get_functions_to_optimize_by_file,
 )
 from codeflash.optimization.function_context import (
     Source,
     get_constrained_function_context_and_dependent_functions,
 )
-from codeflash.result.create_pr import check_create_pr
+from codeflash.result.create_pr import check_create_pr, existing_tests_source_for
 from codeflash.result.explanation import Explanation
 from codeflash.telemetry import posthog
 from codeflash.telemetry.posthog import ph
 from codeflash.telemetry.sentry import init_sentry
 from codeflash.verification.equivalence import compare_results
 from codeflash.verification.parse_test_output import parse_test_results
-from codeflash.verification.test_results import (
-    TestResults,
-    TestType,
-)
+from codeflash.verification.test_results import TestResults, TestType
 from codeflash.verification.test_runner import run_tests
-from codeflash.verification.verification_utils import (
-    TestConfig,
-    get_test_file_path,
-)
+from codeflash.verification.verification_utils import TestConfig, get_test_file_path
 from codeflash.verification.verifier import generate_tests
 
 
-def parse_args() -> Namespace:
-    parser = ArgumentParser()
-    parser.add_argument("command", nargs="?", help="The command to run (e.g., 'init')")
-    parser.add_argument("--file", help="Try to optimize only this file")
-    parser.add_argument(
-        "--function",
-        help="Try to optimize only this function within the given file path",
-    )
-    parser.add_argument(
-        "--all",
-        help="Try to optimize all functions. Can take a really long time. Can pass an optional starting directory to"
-        " optimize code from. If no args specified (just --all), will optimize all code in the project.",
-        nargs="?",
-        const="",
-        default=SUPPRESS,
-    )
-    parser.add_argument(
-        "--module-root",
-        type=str,
-        help="Path to the project's Python module that you want to optimize."
-        " This is the top-level root directory where all the Python source code is located.",
-    )
-    parser.add_argument(
-        "--tests-root",
-        type=str,
-        help="Path to the test directory of the project, where all the tests are located.",
-    )
-    parser.add_argument("--test-framework", choices=["pytest", "unittest"], default="pytest")
-    parser.add_argument(
-        "--config-file",
-        type=str,
-        help="Path to the pyproject.toml with codeflash configs.",
-    )
-    parser.add_argument(
-        "--pytest-cmd",
-        type=str,
-        help="Command that codeflash will use to run pytest. If not specified, codeflash will use 'pytest'",
-    )
-    parser.add_argument(
-        "--use-cached-tests",
-        action="store_true",
-        help="Use cached tests from a specified file for debugging.",
-    )
-    parser.add_argument("-v", "--verbose", action="store_true", help="Print verbose debug logs")
-    parser.add_argument("--version", action="store_true", help="Print the version of codeflash")
-    args: Namespace = parser.parse_args()
-    return process_cmd_args(args)
+class OptimizedCandidateResult(BaseModel):
+    times_run: int
+    best_test_runtime: int
+    best_test_results: TestResults
+
+
+class OriginalCodeBaseline(BaseModel):
+    generated_test_results: TestResults
+    overall_test_results: Optional[TestResults]
+    runtime: int
+
+
+class TestsAndOptimizationsResult(BaseModel):
+    generated_original_test_source: str
+    instrumented_test_source: str
+    optimizations: List[Optimization]
+
+
+class BestOptimization(BaseModel):
+    source_code: str
+    explanation: str
+    dependent_functions: list[Tuple[Source, str, str]]
+
+
+class CodeOptimizationContext(BaseModel):
+    code_to_optimize_with_dependents: str
+    contextual_dunder_methods: set[tuple[str, str]]
+    dependent_functions: List[Tuple[Source, str, str]]
+    preexisting_functions: List[str]
 
 
 class Optimizer:
     def __init__(self, args: Namespace):
         self.args = args
         init_sentry(not args.disable_telemetry)
         posthog.initialize_posthog(not args.disable_telemetry)
@@ -128,15 +97,14 @@
             project_root_path=args.project_root,
             test_framework=args.test_framework,
             pytest_cmd=args.pytest_cmd,
         )
 
     def run(self) -> None:
         ph("cli-optimize-run-start")
-        logging.info(CODEFLASH_LOGO)
         logging.info("Running optimizer.")
         if not env_utils.ensure_codeflash_api_key():
             return
         if not env_utils.ensure_git_repo(module_root=self.args.module_root):
             logging.error("No git repository detected and user aborted run. Exiting...")
             exit(1)
 
@@ -177,386 +145,430 @@
                 logging.info(f"Examining file {path} ...")
                 # TODO: Sequence the functions one goes through intelligently. If we are optimizing f(g(x)),
                 #  then we might want to first optimize f rather than g because optimizing f would already
                 #  optimize g as it is a dependency
                 f: IO[str]
                 with open(path, encoding="utf8") as f:
                     original_code: str = f.read()
-                should_sort_imports = True
-                if (
-                    sort_imports(self.args.imports_sort_cmd, should_sort_imports, path)
-                    != original_code
-                ):
-                    should_sort_imports = False
 
                 function_to_optimize: FunctionToOptimize
                 for function_to_optimize in file_to_funcs_to_optimize[path]:
                     function_trace_id: str = str(uuid.uuid4())
                     ph("cli-optimize-function-start", {"function_trace_id": function_trace_id})
-                    function_name: str = (
-                        function_to_optimize.function_name
-                        if function_to_optimize.parents == []
-                        else ".".join(
-                            [
-                                function_to_optimize.parents[0].name,
-                                function_to_optimize.function_name,
-                            ],
-                        )
-                    )
                     function_iterator_count += 1
                     logging.info(
-                        f"Optimizing function {function_iterator_count} of {num_optimizable_functions} - {function_name}",
+                        f"Optimizing function {function_iterator_count} of {num_optimizable_functions} - {function_to_optimize.qualified_name}",
                     )
                     winning_test_results = None
-                    # remove leftovers from previous run
-                    pathlib.Path(get_run_tmp_file("test_return_values_0.bin")).unlink(
-                        missing_ok=True,
-                    )
-                    pathlib.Path(get_run_tmp_file("test_return_values_0.sqlite")).unlink(
-                        missing_ok=True,
-                    )
-                    code_to_optimize, contextual_dunder_methods = extract_code(
-                        [function_to_optimize],
-                    )
-                    if code_to_optimize is None:
-                        logging.error("Could not find function to optimize.")
+                    self.cleanup_leftover_test_return_values()
+                    ctx_result = self.get_code_optimization_context(function_to_optimize)
+                    if not is_successful(ctx_result):
+                        logging.error(ctx_result.failure())
                         continue
-
-                    success, preexisting_functions = get_all_function_names(code_to_optimize)
-                    if not success:
-                        logging.error("Error in parsing the code, skipping optimization.")
+                    code_context: CodeOptimizationContext = ctx_result.unwrap()
+                    dependent_functions_by_module_abspath = defaultdict(set)
+                    for _, module_abspath, qualified_name in code_context.dependent_functions:
+                        dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
+                    original_dependent_code = {}
+                    for module_abspath in dependent_functions_by_module_abspath.keys():
+                        with open(module_abspath, encoding="utf8") as f:
+                            dependent_code = f.read()
+                            original_dependent_code[module_abspath] = dependent_code
+                    logging.info(f"Code to be optimized:\n{code_context.code_to_optimize_with_dependents}")
+                    module_path = module_name_from_file_path(path, self.args.project_root)
+
+                    instrumented_unittests_created_for_function = self.instrument_existing_tests(
+                        function_name=function_to_optimize.qualified_name,
+                        module_path=module_path,
+                        function_to_tests=function_to_tests,
+                    )
+                    instrumented_unittests_created.update(
+                        instrumented_unittests_created_for_function,
+                    )
+
+                    tests_result = self.generate_tests_and_optimizations(
+                        code_context.code_to_optimize_with_dependents,
+                        function_to_optimize,
+                        code_context.dependent_functions,
+                        module_path,
+                        function_trace_id,
+                    )
+                    if not is_successful(tests_result):
+                        logging.error(tests_result.failure())
                         continue
+                    tests_and_optimizations: TestsAndOptimizationsResult = tests_result.unwrap()
 
-                    dependent_code, dependent_functions = (
-                        get_constrained_function_context_and_dependent_functions(
-                            function_to_optimize,
-                            self.args.project_root,
-                            code_to_optimize,
-                        )
-                    )
-                    if function_to_optimize.parents:
-                        function_class = function_to_optimize.parents[0].name
-                        dependent_methods = [
-                            df
-                            for df in dependent_functions
-                            if df[2].count(".") > 0 and df[2].split(".")[0] == function_class
-                        ]
-                        optimizable_methods = [function_to_optimize] + [
-                            FunctionToOptimize(
-                                df[2].split(".")[0],
-                                "",
-                                [FunctionParent(df[2].split(".")[0], "ClassDef")],
-                                None,
-                                None,
-                            )
-                            for df in dependent_methods
-                        ]
-                        if len(optimizable_methods) > 1:
-                            code_to_optimize, contextual_dunder_methods = extract_code(
-                                optimizable_methods,
-                            )
-                            if code_to_optimize is None:
-                                logging.error("Could not find function to optimize.")
-                                continue
-                    code_to_optimize_with_dependents = dependent_code + "\n" + code_to_optimize
-                preexisting_functions.extend(
-                    [fn[0].full_name.split(".")[-1] for fn in dependent_functions],
-                )
-                dependent_functions_by_module_abspath = defaultdict(set)
-                for _, module_abspath, qualified_name in dependent_functions:
-                    dependent_functions_by_module_abspath[module_abspath].add(qualified_name)
-                original_dependent_code = {}
-                for module_abspath in dependent_functions_by_module_abspath.keys():
-                    with open(module_abspath, encoding="utf8") as f:
-                        dependent_code = f.read()
-                        original_dependent_code[module_abspath] = dependent_code
-                logging.info(f"Code to be optimized:\n{code_to_optimize_with_dependents}")
-                module_path = module_name_from_file_path(path, self.args.project_root)
-
-                instrumented_unittests_created_for_function = self.prepare_existing_tests(
-                    function_name=function_name,
-                    module_path=module_path,
-                    function_to_tests=function_to_tests,
-                )
-                instrumented_unittests_created.update(
-                    instrumented_unittests_created_for_function,
-                )
-
-                (
-                    success,
-                    generated_original_test_source,
-                    instrumented_test_source,
-                    optimizations,
-                ) = self.generate_tests_and_optimizations(
-                    code_to_optimize_with_dependents,
-                    function_to_optimize,
-                    dependent_functions,
-                    module_path,
-                    function_trace_id,
-                )
-                if not success:
-                    continue
-
-                generated_tests_path = get_test_file_path(
-                    self.args.tests_root,
-                    function_to_optimize.function_name,
-                    0,
-                )
-                with open(generated_tests_path, "w", encoding="utf8") as file:
-                    file.write(instrumented_test_source)
+                    generated_tests_path = get_test_file_path(
+                        self.args.tests_root,
+                        function_to_optimize.function_name,
+                        0,
+                    )
+                    with open(generated_tests_path, "w", encoding="utf8") as file:
+                        file.write(tests_and_optimizations.instrumented_test_source)
 
-                test_files_created.add(generated_tests_path)
-                (
-                    success,
-                    original_gen_results,
-                    overall_original_test_results,
-                    original_runtime,
-                ) = self.establish_original_code_baseline(
-                    function_name,
-                    instrumented_unittests_created_for_function,
-                    generated_tests_path,
-                )
-                if not success:
-                    continue
-                best_runtime = original_runtime  # The fastest code runtime until now
-                logging.info("Optimizing code ...")
-                # TODO: Postprocess the optimized function to include the original docstring and such
-
-                best_optimization = []
-                speedup_ratios: Dict[str, float | None] = dict()
-                optimized_runtimes = dict()
-                is_correct = dict()
-
-                for i, optimization in enumerate(optimizations.optimizations):
-                    j = i + 1
-                    if optimization.source_code is None:
+                    test_files_created.add(generated_tests_path)
+                    baseline_result = self.establish_original_code_baseline(
+                        function_to_optimize.qualified_name,
+                        instrumented_unittests_created_for_function,
+                        generated_tests_path,
+                    )
+                    if not is_successful(baseline_result):
+                        logging.error(baseline_result.failure())
                         continue
-                    # remove left overs from previous run
-                    pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
-                        missing_ok=True,
-                    )
-                    pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
-                        missing_ok=True,
-                    )
-                    logging.info("Optimized candidate:")
-                    logging.info(optimization.source_code)
-                    try:
-                        replace_function_definitions_in_module(
-                            [function_name],
-                            optimization.source_code,
-                            path,
-                            preexisting_functions,
-                            contextual_dunder_methods,
+                    original_code_baseline: OriginalCodeBaseline = baseline_result.unwrap()
+                    best_runtime = original_code_baseline.runtime  # The fastest code runtime until now
+                    logging.info("Optimizing code ...")
+                    # TODO: Postprocess the optimized function to include the original docstring and such
+
+                    best_optimization: Optional[BestOptimization] = None
+                    speedup_ratios: Dict[str, float | None] = dict()
+                    optimized_runtimes = dict()
+                    is_correct = dict()
+
+                    for i, optimization in enumerate(tests_and_optimizations.optimizations):
+                        j = i + 1
+                        if optimization.source_code is None:
+                            continue
+                        # remove left overs from previous run
+                        pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.bin")).unlink(
+                            missing_ok=True,
+                        )
+                        pathlib.Path(get_run_tmp_file(f"test_return_values_{j}.sqlite")).unlink(
+                            missing_ok=True,
                         )
-                        for (
-                            module_abspath,
-                            qualified_names,
-                        ) in dependent_functions_by_module_abspath.items():
+                        logging.info("Optimized candidate:")
+                        logging.info(optimization.source_code)
+                        try:
                             replace_function_definitions_in_module(
-                                list(qualified_names),
+                                [function_to_optimize.qualified_name],
                                 optimization.source_code,
+                                path,
+                                code_context.preexisting_functions,
+                                code_context.contextual_dunder_methods,
+                            )
+                            for (
                                 module_abspath,
-                                [],
-                                contextual_dunder_methods,
+                                qualified_names,
+                            ) in dependent_functions_by_module_abspath.items():
+                                replace_function_definitions_in_module(
+                                    list(qualified_names),
+                                    optimization.source_code,
+                                    module_abspath,
+                                    [],
+                                    code_context.contextual_dunder_methods,
+                                )
+                        except (
+                            ValueError,
+                            SyntaxError,
+                            cst.ParserSyntaxError,
+                            AttributeError,
+                        ) as e:
+                            logging.exception(e)
+                            self.write_code_and_dependents(
+                                original_code,
+                                original_dependent_code,
+                                path,
+                                dependent_functions_by_module_abspath,
                             )
-                    except (
-                        ValueError,
-                        SyntaxError,
-                        cst.ParserSyntaxError,
-                        AttributeError,
-                    ) as e:
-                        logging.exception(e)
-                        with open(path, "w", encoding="utf8") as f:
-                            f.write(original_code)
-                        for module_abspath in dependent_functions_by_module_abspath.keys():
-                            with open(module_abspath, "w", encoding="utf8") as f:
-                                f.write(original_dependent_code[module_abspath])
-                        continue
-
-                    (
-                        success,
-                        times_run,
-                        best_test_runtime,
-                        best_test_results,
-                    ) = self.run_optimized_candidate(
-                        optimization_index=j,
-                        instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
-                        overall_original_test_results=overall_original_test_results,
-                        original_gen_results=original_gen_results,
-                        generated_tests_path=generated_tests_path,
-                        best_runtime_until_now=best_runtime,
-                    )
-                    optimized_runtimes[optimization.optimization_id] = best_test_runtime
-                    speedup_ratios[optimization.optimization_id] = None
-                    is_correct[optimization.optimization_id] = success
-
-                    if success:
-                        speedup_ratios[optimization.optimization_id] = (
-                            original_runtime - best_test_runtime
-                        ) / best_test_runtime
+                            continue
 
-                        logging.info(
-                            f"Candidate runtime measured over {times_run} run{'s' if times_run > 1 else ''}: "
-                            f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
-                            f"{((original_runtime - best_test_runtime) / best_test_runtime):.3f}",
+                        run_results = self.run_optimized_candidate(
+                            optimization_index=j,
+                            instrumented_unittests_created_for_function=instrumented_unittests_created_for_function,
+                            overall_original_test_results=original_code_baseline.overall_test_results,
+                            original_gen_results=original_code_baseline.generated_test_results,
+                            generated_tests_path=generated_tests_path,
+                            best_runtime_until_now=best_runtime,
                         )
-                        if (
-                            ((original_runtime - best_test_runtime) / best_test_runtime)
-                            > self.args.minimum_performance_gain
-                        ) and best_test_runtime < best_runtime:
-                            logging.info(
-                                "This candidate is better than the previous best candidate.",
-                            )
+                        if not is_successful(run_results):
+                            optimized_runtimes[optimization.optimization_id] = None
+                            is_correct[optimization.optimization_id] = False
+                            speedup_ratios[optimization.optimization_id] = None
+                        else:
+                            candidate_result: OptimizedCandidateResult = run_results.unwrap()
+                            best_test_runtime = candidate_result.best_test_runtime
+                            optimized_runtimes[optimization.optimization_id] = best_test_runtime
+                            is_correct[optimization.optimization_id] = True
+                            speedup_ratios[optimization.optimization_id] = (
+                                original_code_baseline.runtime - best_test_runtime
+                            ) / best_test_runtime
 
                             logging.info(
-                                f"Original runtime: {humanize_runtime(original_runtime)} Best test runtime: "
-                                f"{humanize_runtime(best_test_runtime)}, ratio = "
-                                f"{((original_runtime - best_test_runtime) / best_test_runtime)}",
+                                f"Candidate runtime measured over {candidate_result.times_run} run{'s' if candidate_result.times_run > 1 else ''}: "
+                                f"{humanize_runtime(best_test_runtime)}, speedup ratio = "
+                                f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime):.3f}",
                             )
-                            best_optimization = [
-                                optimization.source_code,
-                                optimization.explanation,
-                                dependent_functions,
-                            ]
-                            best_runtime = best_test_runtime
-                            winning_test_results = best_test_results
-                    with open(path, "w", encoding="utf8") as f:
-                        f.write(original_code)
-                    for module_abspath in dependent_functions_by_module_abspath.keys():
-                        with open(module_abspath, "w", encoding="utf8") as f:
-                            f.write(original_dependent_code[module_abspath])
-                    logging.info("----------------")
-                logging.info(f"Best optimization: {best_optimization[0:2]}")
-
-                log_results(
-                    function_trace_id=function_trace_id,
-                    speedup_ratio=speedup_ratios,
-                    original_runtime=original_runtime,
-                    optimized_runtime=optimized_runtimes,
-                    is_correct=is_correct,
-                )
-                ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
-
-                if best_optimization:
-                    optimizations_found += 1
-                    logging.info(f"Best candidate:\n{best_optimization[0]}")
-
-                    optimized_code = best_optimization[0]
-                    replace_function_definitions_in_module(
-                        [function_name],
-                        optimized_code,
-                        path,
-                        preexisting_functions,
-                        contextual_dunder_methods,
-                    )
-                    for (
-                        module_abspath,
-                        qualified_names,
-                    ) in dependent_functions_by_module_abspath.items():
-                        replace_function_definitions_in_module(
-                            list(qualified_names),
-                            optimized_code,
-                            module_abspath,
-                            [],
-                            contextual_dunder_methods,
-                        )
-                    explanation_final = Explanation(
-                        raw_explanation_message=best_optimization[1],
-                        winning_test_results=winning_test_results,
-                        original_runtime_ns=original_runtime,
-                        best_runtime_ns=best_runtime,
-                        function_name=function_name,
-                        path=path,
-                    )
-                    logging.info(f"Explanation: \n{explanation_final.to_console_string()}")
-
-                    new_code = format_code(
-                        self.args.formatter_cmd,
-                        self.args.imports_sort_cmd,
-                        should_sort_imports,
-                        path,
-                    )
-                    new_dependent_code: dict[str, str] = {
-                        module_abspath: format_code(
-                            self.args.formatter_cmd,
-                            self.args.imports_sort_cmd,
-                            should_sort_imports,
-                            module_abspath,
+                            if (
+                                ((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)
+                                > self.args.minimum_performance_gain
+                            ) and best_test_runtime < best_runtime:
+                                logging.info(
+                                    "This candidate is better than the previous best candidate.",
+                                )
+
+                                logging.info(
+                                    f"Original runtime: {humanize_runtime(original_code_baseline.runtime)} Best test runtime: "
+                                    f"{humanize_runtime(best_test_runtime)}, ratio = "
+                                    f"{((original_code_baseline.runtime - best_test_runtime) / best_test_runtime)}",
+                                )
+                                best_optimization = BestOptimization(
+                                    source_code=optimization.source_code,
+                                    explanation=optimization.explanation,
+                                    dependent_functions=code_context.dependent_functions,
+                                )
+                                best_runtime = best_test_runtime
+                                winning_test_results = candidate_result.best_test_results
+                        self.write_code_and_dependents(
+                            original_code,
+                            original_dependent_code,
+                            path,
+                            dependent_functions_by_module_abspath,
                         )
-                        for module_abspath in dependent_functions_by_module_abspath.keys()
-                    }
-                    logging.info(
-                        f"Optimization was validated for correctness by running the following tests - "
-                        f"\n{generated_original_test_source}",
+                        logging.info("----------------")
+                    log_results(
+                        function_trace_id=function_trace_id,
+                        speedup_ratio=speedup_ratios,
+                        original_runtime=original_code_baseline.runtime,
+                        optimized_runtime=optimized_runtimes,
+                        is_correct=is_correct,
                     )
+                    ph("cli-optimize-function-finished", {"function_trace_id": function_trace_id})
 
-                    logging.info(f"⚡️ Optimization successful! 📄 {function_name} in {path}")
-                    logging.info(f"📈 {explanation_final.perf_improvement_line}")
+                    if best_optimization:
+                        optimizations_found += 1
+                        logging.info(
+                            f"Best candidate:\n{best_optimization.source_code}, {best_optimization.explanation}",
+                        )
+
+                        optimized_code = best_optimization.source_code
+                        explanation = Explanation(
+                            raw_explanation_message=best_optimization.explanation,
+                            winning_test_results=winning_test_results,
+                            original_runtime_ns=original_code_baseline.runtime,
+                            best_runtime_ns=best_runtime,
+                            function_name=function_to_optimize.qualified_name,
+                            path=path,
+                        )
 
-                    ph(
-                        "cli-optimize-success",
-                        {
-                            "function_trace_id": function_trace_id,
-                            "speedup_x": explanation_final.speedup_x,
-                            "speedup_pct": explanation_final.speedup_pct,
-                            "best_runtime": explanation_final.best_runtime_ns,
-                            "original_runtime": explanation_final.original_runtime_ns,
-                            "winning_test_results": {
-                                tt.to_name(): v
-                                for tt, v in explanation_final.winning_test_results.get_test_pass_fail_report_by_type().items()
+                        logging.info(
+                            f"⚡️ Optimization successful! 📄 {function_to_optimize.qualified_name} in {explanation.path}",
+                        )
+                        logging.info(f"📈 {explanation.perf_improvement_line}")
+                        logging.info(f"Explanation: \n{explanation.to_console_string()}")
+                        logging.info(
+                            f"Optimization was validated for correctness by running the following tests - "
+                            f"\n{tests_and_optimizations.generated_original_test_source}",
+                        )
+
+                        ph(
+                            "cli-optimize-success",
+                            {
+                                "function_trace_id": function_trace_id,
+                                "speedup_x": explanation.speedup_x,
+                                "speedup_pct": explanation.speedup_pct,
+                                "best_runtime": explanation.best_runtime_ns,
+                                "original_runtime": explanation.original_runtime_ns,
+                                "winning_test_results": {
+                                    tt.to_name(): v
+                                    for tt, v in explanation.winning_test_results.get_test_pass_fail_report_by_type().items()
+                                },
                             },
-                        },
-                    )
-                    test_files = function_to_tests.get(module_path + "." + function_name)
-                    existing_tests = ""
-                    if test_files:
-                        for test_file in test_files:
-                            with open(test_file.test_file, encoding="utf8") as f:
-                                new_test = "".join(f.readlines())
-                                if new_test not in existing_tests:
-                                    existing_tests += new_test
-
-                    check_create_pr(
-                        optimize_all=self.args.all,
-                        path=path,
-                        original_code=original_dependent_code | {path: original_code},
-                        new_code=new_dependent_code | {path: new_code},
-                        explanation=explanation_final,
-                        existing_tests_source=existing_tests,
-                        generated_original_test_source=generated_original_test_source,
-                    )
-                    if self.args.all or env_utils.get_pr_number():
-                        # Reverting to original code, because optimizing functions in a sequence can lead to
-                        #  a) Error propagation, where error in one function can cause the next optimization to fail
-                        #  b) Performance estimates become unstable, as the runtime of an optimization might be
-                        #     dependent on the runtime of the previous optimization
-                        with open(path, "w", encoding="utf8") as f:
-                            f.write(original_code)
-                        for module_abspath in dependent_functions_by_module_abspath.keys():
-                            with open(module_abspath, "w", encoding="utf8") as f:
-                                f.write(original_dependent_code[module_abspath])
-                # Delete all the generated tests to not cause any clutter.
-                pathlib.Path(generated_tests_path).unlink(missing_ok=True)
-                for test_paths in instrumented_unittests_created_for_function:
-                    pathlib.Path(test_paths).unlink(missing_ok=True)
+                        )
+
+                        existing_tests = existing_tests_source_for(
+                            function_to_optimize.qualified_name,
+                            module_path,
+                            function_to_tests,
+                        )
+
+                        self.replace_function_and_dependents_with_optimized_code(
+                            code_context,
+                            dependent_functions_by_module_abspath,
+                            explanation,
+                            optimized_code,
+                            function_to_optimize.qualified_name,
+                        )
+
+                        new_code, new_dependent_code = self.reformat_code_and_dependents(
+                            dependent_functions_by_module_abspath,
+                            explanation.path,
+                            original_code,
+                        )
+
+                        original_code_combined = original_dependent_code.copy()
+                        original_code_combined[explanation.path] = original_code
+                        new_code_combined = new_dependent_code.copy()
+                        new_code_combined[explanation.path] = new_code
+                        check_create_pr(
+                            optimize_all=self.args.all,
+                            original_code=original_code_combined,
+                            new_code=new_code_combined,
+                            explanation=explanation,
+                            existing_tests_source=existing_tests,
+                            generated_original_test_source=tests_and_optimizations.generated_original_test_source,
+                        )
+                        if self.args.all or env_utils.get_pr_number():
+                            # Reverting to original code, because optimizing functions in a sequence can lead to
+                            #  a) Error propagation, where error in one function can cause the next optimization to fail
+                            #  b) Performance estimates become unstable, as the runtime of an optimization might be
+                            #     dependent on the runtime of the previous optimization
+                            self.write_code_and_dependents(
+                                original_code,
+                                original_dependent_code,
+                                path,
+                                dependent_functions_by_module_abspath,
+                            )
+                    # Delete all the generated tests to not cause any clutter.
+                    pathlib.Path(generated_tests_path).unlink(missing_ok=True)
+                    for test_paths in instrumented_unittests_created_for_function:
+                        pathlib.Path(test_paths).unlink(missing_ok=True)
             ph("cli-optimize-run-finished", {"optimizations_found": optimizations_found})
             if optimizations_found == 0:
                 logging.info("❌ No optimizations found.")
             elif self.args.all:
                 logging.info("✨ All functions have been optimized! ✨")
         finally:
             # TODO: Also revert the file/function being optimized if the process did not succeed
             for test_file in instrumented_unittests_created:
                 pathlib.Path(test_file).unlink(missing_ok=True)
             for test_file in test_files_created:
                 pathlib.Path(test_file).unlink(missing_ok=True)
             if hasattr(get_run_tmp_file, "tmpdir"):
                 get_run_tmp_file.tmpdir.cleanup()
 
-    def prepare_existing_tests(
+    def write_code_and_dependents(
+        self,
+        original_code: str,
+        original_dependent_code: Dict[str, str],
+        path: str,
+        dependent_functions_by_module_abspath: Dict[str, set[str]],
+    ) -> None:
+        with open(path, "w", encoding="utf8") as f:
+            f.write(original_code)
+        for module_abspath in dependent_functions_by_module_abspath:
+            with open(module_abspath, "w", encoding="utf8") as f:
+                f.write(original_dependent_code[module_abspath])
+
+    def reformat_code_and_dependents(
+        self,
+        dependent_functions_by_module_abspath: Dict[str, set[str]],
+        path: str,
+        original_code: str,
+    ) -> Tuple[str, Dict[str, str]]:
+        should_sort_imports = True
+        if sort_imports(self.args.imports_sort_cmd, should_sort_imports, path) != original_code:
+            should_sort_imports = False
+
+        new_code = format_code(
+            self.args.formatter_cmd,
+            self.args.imports_sort_cmd,
+            should_sort_imports,
+            path,
+        )
+        new_dependent_code: dict[str, str] = {
+            module_abspath: format_code(
+                self.args.formatter_cmd,
+                self.args.imports_sort_cmd,
+                should_sort_imports,
+                module_abspath,
+            )
+            for module_abspath in dependent_functions_by_module_abspath
+        }
+        return new_code, new_dependent_code
+
+    def replace_function_and_dependents_with_optimized_code(
+        self,
+        code_context: CodeOptimizationContext,
+        dependent_functions_by_module_abspath: Dict[str, set[str]],
+        explanation: Explanation,
+        optimized_code: str,
+        qualified_function_name: str,
+    ) -> None:
+        replace_function_definitions_in_module(
+            [qualified_function_name],
+            optimized_code,
+            explanation.path,
+            code_context.preexisting_functions,
+            code_context.contextual_dunder_methods,
+        )
+        for (
+            module_abspath,
+            qualified_names,
+        ) in dependent_functions_by_module_abspath.items():
+            replace_function_definitions_in_module(
+                list(qualified_names),
+                optimized_code,
+                module_abspath,
+                [],
+                code_context.contextual_dunder_methods,
+            )
+
+    def get_code_optimization_context(
+        self,
+        function_to_optimize: FunctionToOptimize,
+    ) -> Result[CodeOptimizationContext, str]:
+        code_to_optimize, contextual_dunder_methods = extract_code(
+            [function_to_optimize],
+        )
+        if code_to_optimize is None:
+            return Failure("Could not find function to optimize.")
+        success, preexisting_functions = get_all_function_names(code_to_optimize)
+        if not success:
+            return Failure("Error in parsing the code, skipping optimization.")
+        dependent_code, dependent_functions = get_constrained_function_context_and_dependent_functions(
+            function_to_optimize,
+            self.args.project_root,
+            code_to_optimize,
+        )
+        if function_to_optimize.parents:
+            function_class = function_to_optimize.parents[0].name
+            dependent_methods = [
+                df
+                for df in dependent_functions
+                if df[2].count(".") > 0 and df[2].split(".")[0] == function_class
+            ]
+            optimizable_methods = [function_to_optimize] + [
+                FunctionToOptimize(
+                    df[2].split(".")[0],
+                    "",
+                    [FunctionParent(df[2].split(".")[0], "ClassDef")],
+                    None,
+                    None,
+                )
+                for df in dependent_methods
+            ]
+            if len(optimizable_methods) > 1:
+                code_to_optimize, contextual_dunder_methods = extract_code(
+                    optimizable_methods,
+                )
+                if code_to_optimize is None:
+                    return Failure("Could not find function to optimize.")
+        code_to_optimize_with_dependents = dependent_code + "\n" + code_to_optimize
+        preexisting_functions.extend(
+            [fn[0].full_name.split(".")[-1] for fn in dependent_functions],
+        )
+        return Success(
+            CodeOptimizationContext(
+                code_to_optimize_with_dependents=code_to_optimize_with_dependents,
+                contextual_dunder_methods=contextual_dunder_methods,
+                dependent_functions=dependent_functions,
+                preexisting_functions=preexisting_functions,
+            ),
+        )
+
+    def cleanup_leftover_test_return_values(self):
+        # remove leftovers from previous run
+        pathlib.Path(get_run_tmp_file("test_return_values_0.bin")).unlink(
+            missing_ok=True,
+        )
+        pathlib.Path(get_run_tmp_file("test_return_values_0.sqlite")).unlink(
+            missing_ok=True,
+        )
+
+    def instrument_existing_tests(
         self,
         function_name: str,
         module_path: str,
         function_to_tests: dict[str, list[TestsInFile]],
     ):
         relevant_test_files_count = 0
         unique_original_test_files = set()
@@ -598,18 +610,17 @@
     def generate_tests_and_optimizations(
         self,
         code_to_optimize_with_dependents: str,
         function_to_optimize: FunctionToOptimize,
         dependent_functions: list[Tuple[Source, str, str]],
         module_path: str,
         function_trace_id: str,
-    ):
+    ) -> Result[TestsAndOptimizationsResult, str]:
         generated_original_test_source = None
         instrumented_test_source = None
-        success = True
         with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
             future_tests = executor.submit(
                 self.generate_and_instrument_tests,
                 code_to_optimize_with_dependents,
                 function_to_optimize,
                 [definition[0].full_name for definition in dependent_functions],
                 module_path,
@@ -619,47 +630,39 @@
                 optimize_python_code,
                 code_to_optimize_with_dependents,
                 function_trace_id,
                 N_CANDIDATES,
             )
 
             future_tests_result = future_tests.result()
-            optimizations = future_optimization.result()
-        if (
-            future_tests_result
-            and isinstance(future_tests_result, tuple)
-            and len(future_tests_result) == 2
-        ):
+            optimizations: List[Optimization] = future_optimization.result()
+        if future_tests_result and isinstance(future_tests_result, tuple) and len(future_tests_result) == 2:
             (
                 generated_original_test_source,
                 instrumented_test_source,
             ) = future_tests_result
 
         else:
-            logging.error("/!\\ NO TESTS GENERATED for %s", function_to_optimize.function_name)
-            success = False
-        if len(optimizations.optimizations) == 0:
-            logging.error(
-                "/!\\ NO OPTIMIZATIONS GENERATED for %s",
-                function_to_optimize.function_name,
-            )
-            success = False
-        return (
-            success,
-            generated_original_test_source,
-            instrumented_test_source,
-            optimizations,
+            return Failure(f"/!\\ NO TESTS GENERATED for {function_to_optimize.function_name}")
+        if not optimizations:
+            return Failure(f"/!\\ NO OPTIMIZATIONS GENERATED for {function_to_optimize.function_name}")
+        return Success(
+            TestsAndOptimizationsResult(
+                generated_original_test_source=generated_original_test_source,
+                instrumented_test_source=instrumented_test_source,
+                optimizations=optimizations,
+            ),
         )
 
     def establish_original_code_baseline(
         self,
         function_name: str,
         instrumented_unittests_created_for_function: set[str],
         generated_tests_path: str,
-    ):
+    ) -> Result[OriginalCodeBaseline, str]:
         original_runtime = None
         best_runtime = None
         original_gen_results = None
         overall_original_test_results = None
         times_run = 0
         success = True
         # Keep the runtime in some acceptable range
@@ -757,29 +760,36 @@
                 break
 
         if times_run == 0:
             logging.warning(
                 "Failed to run the tests for the original function, skipping optimization",
             )
             success = False
-        if success:
-            logging.info(
-                f"Original code runtime measured over {times_run} run{'s' if times_run > 1 else ''}: {humanize_runtime(original_runtime)}",
-            )
-        return success, original_gen_results, overall_original_test_results, best_runtime
+        if not success:
+            return Failure("Failed to establish a baseline for the original code.")
+        logging.info(
+            f"Original code runtime measured over {times_run} run{'s' if times_run > 1 else ''}: {humanize_runtime(original_runtime)}",
+        )
+        return Success(
+            OriginalCodeBaseline(
+                generated_test_results=original_gen_results,
+                overall_test_results=overall_original_test_results,
+                runtime=best_runtime,
+            ),
+        )
 
     def run_optimized_candidate(
         self,
         optimization_index: int,
         instrumented_unittests_created_for_function: set[str],
         overall_original_test_results: TestResults,
         original_gen_results: TestResults,
         generated_tests_path: str,
         best_runtime_until_now: int,
-    ):
+    ) -> Result[OptimizedCandidateResult, str]:
         success = True
         best_test_runtime = None
         best_test_results = None
         equal_results = True
         generated_tests_elapsed_time = 0.0
 
         times_run = 0
@@ -894,19 +904,22 @@
         )
         pathlib.Path(get_run_tmp_file(f"test_return_values_{optimization_index}.sqlite")).unlink(
             missing_ok=True,
         )
         if not (equal_results and times_run > 0):
             success = False
 
-        return (
-            success,
-            times_run,
-            best_test_runtime,
-            best_test_results,
+        if not success:
+            return Failure("Failed to run the optimized candidate.")
+        return Success(
+            OptimizedCandidateResult(
+                times_run=times_run,
+                best_test_runtime=best_test_runtime,
+                best_test_results=best_test_results,
+            ),
         )
 
     def run_and_parse_tests(
         self,
         test_env: dict[str, str],
         test_file: str,
         test_type: TestType,
@@ -962,14 +975,10 @@
             return None
 
         generated_original_test_source, instrumented_test_source = tests
 
         return generated_original_test_source, instrumented_test_source
 
 
-def main() -> None:
-    """Entry point for the codeflash command-line interface."""
-    Optimizer(parse_args()).run()
-
-
-if __name__ == "__main__":
-    main()
+def run_with_args(args: Namespace) -> None:
+    optimizer = Optimizer(args)
+    optimizer.run()
```

### Comparing `codeflash-0.5.0/codeflash/optimization/function_context.py` & `codeflash-0.5.1/codeflash/optimization/function_context.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/result/create_pr.py` & `codeflash-0.5.1/codeflash/result/create_pr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 import logging
 import os.path
 import pathlib
-from typing import Optional
+from typing import Dict, List, Optional
 
 from codeflash.api import cfapi
 from codeflash.code_utils import env_utils
 from codeflash.code_utils.git_utils import (
+    get_current_branch,
     get_repo_owner_and_name,
     git_root_dir,
-    get_current_branch,
 )
+from codeflash.discovery.discover_unit_tests import TestsInFile
 from codeflash.github.PrComment import FileDiffContent, PrComment
 from codeflash.result.explanation import Explanation
 
 
+def existing_tests_source_for(
+    qualified_function_name: str,
+    module_path: str,
+    function_to_tests: Dict[str, List[TestsInFile]],
+) -> str:
+    test_files = function_to_tests.get(module_path + "." + qualified_function_name)
+    existing_tests = ""
+    if test_files:
+        for test_file in test_files:
+            with open(test_file.test_file, encoding="utf8") as f:
+                new_test = "".join(f.readlines())
+                if new_test not in existing_tests:
+                    existing_tests += new_test
+    return existing_tests
+
+
 def check_create_pr(
     optimize_all: bool,
-    path: str,
     original_code: dict[str, str],
     new_code: dict[str, str],
     explanation: Explanation,
     existing_tests_source: str,
     generated_original_test_source: str,
 ):
     pr_number: Optional[int] = env_utils.get_pr_number()
 
     if pr_number is not None:
         logging.info(f"Suggesting changes to PR #{pr_number} ...")
         owner, repo = get_repo_owner_and_name()
-        relative_path = str(pathlib.Path(os.path.relpath(path, git_root_dir())).as_posix())
+        relative_path = str(pathlib.Path(os.path.relpath(explanation.path, git_root_dir())).as_posix())
         response = cfapi.suggest_changes(
             owner=owner,
             repo=repo,
             pr_number=pr_number,
             file_changes={
                 str(pathlib.Path(os.path.relpath(p, git_root_dir())).as_posix()): FileDiffContent(
-                    oldContent=original_code[p], newContent=new_code[p]
+                    oldContent=original_code[p],
+                    newContent=new_code[p],
                 )
-                for p in original_code.keys()
+                for p in original_code
             },
             pr_comment=PrComment(
                 optimization_explanation=explanation.explanation_message(),
                 best_runtime=explanation.best_runtime_ns,
                 original_runtime=explanation.original_runtime_ns,
                 function_name=explanation.function_name,
                 relative_file_path=relative_path,
@@ -49,36 +66,37 @@
                 speedup_pct=explanation.speedup_pct,
                 winning_test_results=explanation.winning_test_results,
             ),
             existing_tests=existing_tests_source,
             generated_tests=generated_original_test_source,
         )
         if response.ok:
-            logging.info("Suggestions were successfully made to PR #" + str(pr_number))
+            logging.info(f"Suggestions were successfully made to PR #{pr_number}")
         else:
             logging.error(
                 f"Optimization was successful, but I failed to suggest changes to PR #{pr_number}."
-                f" Response from server was: {response.text}"
+                f" Response from server was: {response.text}",
             )
 
     elif optimize_all:
         logging.info("Creating a new PR with the optimized code...")
         owner, repo = get_repo_owner_and_name()
 
-        relative_path = str(pathlib.Path(os.path.relpath(path, git_root_dir())).as_posix())
+        relative_path = str(pathlib.Path(os.path.relpath(explanation.path, git_root_dir())).as_posix())
         base_branch = get_current_branch()
         response = cfapi.create_pr(
             owner=owner,
             repo=repo,
             base_branch=base_branch,
             file_changes={
                 str(pathlib.Path(os.path.relpath(p, git_root_dir())).as_posix()): FileDiffContent(
-                    oldContent=original_code[p], newContent=new_code[p]
+                    oldContent=original_code[p],
+                    newContent=new_code[p],
                 )
-                for p in original_code.keys()
+                for p in original_code
             },
             pr_comment=PrComment(
                 optimization_explanation=explanation.explanation_message(),
                 best_runtime=explanation.best_runtime_ns,
                 original_runtime=explanation.original_runtime_ns,
                 function_name=explanation.function_name,
                 relative_file_path=relative_path,
@@ -90,9 +108,9 @@
             generated_tests=generated_original_test_source,
         )
         if response.ok:
             logging.info(f"Successfully created a new PR #{response.text} with the optimized code.")
         else:
             logging.error(
                 f"Optimization was successful, but I failed to create a PR with the optimized code."
-                f" Response from server was: {response.text}"
+                f" Response from server was: {response.text}",
             )
```

### Comparing `codeflash-0.5.0/codeflash/result/explanation.py` & `codeflash-0.5.1/codeflash/result/explanation.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/telemetry/posthog.py` & `codeflash-0.5.1/codeflash/telemetry/posthog.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import logging
-from typing import Dict, Any, Optional
+from typing import Any, Dict, Optional
 
 from posthog import Posthog
 
 from codeflash.api.cfapi import get_user_id
 from codeflash.version import __version__, __version_tuple__
 
 _posthog = None
 
 
 def initialize_posthog(enabled: bool) -> None:
-    """
-    Enable or disable PostHog.
+    """Enable or disable PostHog.
     :param enabled: Whether to enable PostHog.
     """
     if not enabled:
         return
 
     global _posthog
     _posthog = Posthog(
         project_api_key="phc_aUO790jHd7z1SXwsYCz8dRApxueplZlZWeDSpKc5hol",
         host="https://us.posthog.com",
     )
     ph("cli-telemetry-enabled")
 
 
 def ph(event: str, properties: Optional[Dict[str, Any]] = None) -> None:
-    """
-    Log an event to PostHog.
+    """Log an event to PostHog.
     :param event: The name of the event.
     :param properties: A dictionary of properties to attach to the event.
     """
     if _posthog is None:
         return
 
     properties = properties or {}
```

### Comparing `codeflash-0.5.0/codeflash/telemetry/sentry.py` & `codeflash-0.5.1/codeflash/telemetry/sentry.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/tracing/replay_test.py` & `codeflash-0.5.1/codeflash/tracing/replay_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 import sqlite3
 import textwrap
 from collections import defaultdict
 from typing import Any, Dict, Generator, List, Tuple
 
 
 def get_next_arg_and_return(
-    trace_file: str, function_name: str, num_to_get: int = 3
+    trace_file: str,
+    function_name: str,
+    num_to_get: int = 3,
 ) -> Generator[Tuple[Any, Any], None, None]:
     db = sqlite3.connect(trace_file)
     cur = db.cursor()
     limit = num_to_get * 2 + 100
     data = cur.execute(
         "SELECT * FROM events WHERE function = ? ORDER BY time_ns ASC LIMIT ?",
         (function_name, limit),
@@ -23,22 +25,22 @@
             break
 
         event_type, frame_address = val[0], val[4]
         if event_type == "call":
             matched_arg_return[frame_address].append(val[7])
             if len(matched_arg_return[frame_address]) > 1:
                 logging.warning(
-                    f"Pre-existing call to the function {function_name} with same frame address."
+                    f"Pre-existing call to the function {function_name} with same frame address.",
                 )
         elif event_type == "return":
             matched_arg_return[frame_address].append(val[6])
             arg_return_length = len(matched_arg_return[frame_address])
             if arg_return_length > 2:
                 logging.warning(
-                    f"Pre-existing return to the function {function_name} with same frame address."
+                    f"Pre-existing return to the function {function_name} with same frame address.",
                 )
             elif arg_return_length == 1:
                 logging.warning(f"No call before return for {function_name}!")
             elif arg_return_length == 2:
                 yield matched_arg_return[frame_address]
                 counts += 1
                 del matched_arg_return[frame_address]
@@ -47,19 +49,21 @@
 
 
 def get_function_alias(module: str, function_name: str) -> str:
     return "_".join(module.split(".")) + "_" + function_name
 
 
 def create_trace_replay_test(
-    trace_file: str, functions: List[Tuple[str, str]], test_framework: str = "pytest"
+    trace_file: str,
+    functions: List[Tuple[str, str]],
+    test_framework: str = "pytest",
 ) -> str:
     assert test_framework in ["pytest", "unittest"]
 
-    imports = f"""import pickle
+    imports = f"""import dill as pickle
 import {test_framework}
 from codeflash.tracing.replay_test import get_next_arg_and_return
 from codeflash.validation.comparators import comparator
 """
 
     # TODO: Module can have "-" character if the module-root is ".". Need to handle that case
     function_imports = [
@@ -80,15 +84,15 @@
     test_function_body = textwrap.dedent(
         """\
         for arg_val_pkl, return_val_pkl in get_next_arg_and_return('{trace_file}', '{orig_function_name}', 3):
             args = pickle.loads(arg_val_pkl)
             return_val = pickle.loads(return_val_pkl)
             ret = {function_name}(**args)
             self.assertTrue(comparator(return_val, ret))
-    """
+    """,
     )
 
     test_template = "\nclass TestTracedFunctions(unittest.TestCase):\n"
     for module, function_name in functions:
         function_name_alias = get_function_alias(module, function_name)
         formatted_test_body = textwrap.indent(
             test_function_body.format(
@@ -107,15 +111,15 @@
     test_function_body = textwrap.dedent(
         """\
         for arg_val_pkl, return_val_pkl in get_next_arg_and_return('{trace_file}', '{orig_function_name}', 3):
             args = pickle.loads(arg_val_pkl)
             return_val = pickle.loads(return_val_pkl)
             ret = {function_name}(**args)
             assert comparator(return_val, ret)
-    """
+    """,
     )
 
     test_template = ""
     for module, function_name in functions:
         function_name_alias = get_function_alias(module, function_name)
         formatted_test_body = textwrap.indent(
             test_function_body.format(
```

### Comparing `codeflash-0.5.0/codeflash/tracing/tracer.py` & `codeflash-0.5.1/codeflash/tracing/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import logging
 import os
 import pathlib
-import pickle
 import sqlite3
 import sys
 import time
 from collections import defaultdict
 from typing import Any, Dict, Optional
 
+import dill as pickle
+
 from codeflash.code_utils.code_utils import module_name_from_file_path
 from codeflash.code_utils.config_parser import parse_config_file
 from codeflash.tracing.replay_test import create_trace_replay_test
 from codeflash.verification.verification_utils import get_test_file_path
 
 
 class Tracer:
-    """
-    Use this class as a 'with' context manager to trace a function call,
+    """Use this class as a 'with' context manager to trace a function call,
     input arguments, and return value.
     """
 
     def __init__(
         self,
         output: str = "script.trace",
         functions=None,
         disable: bool = False,
         config_file_path: Optional[str] = None,
     ) -> None:
         if functions is None:
             functions = []
         self.disable = disable
         self.con = None
-        self.flag = (
-            False  # To ignore the first call to trace_callback due to return from trace_callback
-        )
+        self.flag = False  # To ignore the first call to trace_callback due to return from trace_callback
         self.output_file = os.path.abspath(output)
         self.functions = functions
         self.function_modules: Dict[str, str] = {}
         self.function_filenames: Dict[str, str] = {}
         self.function_count = defaultdict(int)
         self.max_function_count = 50
         self.config, found_config_path = parse_config_file(config_file_path)
@@ -53,54 +51,55 @@
         pathlib.Path(self.output_file).unlink(missing_ok=True)
 
         self.con = sqlite3.connect(self.output_file)
         cur = self.con.cursor()
         # TODO: Check out if we need to export the function test name as well
         cur.execute(
             "CREATE TABLE events(type TEXT, function TEXT, filename TEXT, line_number INTEGER, "
-            "last_frame_address INTEGER, time_ns INTEGER, arg BLOB, locals BLOB)"
+            "last_frame_address INTEGER, time_ns INTEGER, arg BLOB, locals BLOB)",
         )
         sys.setprofile(self.trace_callback)
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         sys.setprofile(None)
         # TODO: Check if the self.disable condition can be moved before the sys.setprofile call.
         #  Currently, it is below to see if the self.disable check doesn't add extra steps in the tracing
         if self.disable:
             return
 
         self.con.close()
 
         module_function = [
-            (module, function_name) for function_name, module in self.function_modules.items()
+            (module, function_name)
+            for function_name, module in self.function_modules.items()
         ]
         replay_test = create_trace_replay_test(
             trace_file=self.output_file,
             functions=module_function,
             test_framework=self.config["test_framework"],
         )
         function_path = "_".join([func for _, func in module_function])
         test_file_path = get_test_file_path(
-            self.config["tests_root"], function_path, test_type="replay"
+            self.config["tests_root"], function_path, test_type="replay",
         )
         with open(test_file_path, "w", encoding="utf8") as file:
             file.write(replay_test)
 
         logging.info(
-            f"Codeflash: Function Traced successfully and replay test created! Path - {test_file_path}"
+            f"Codeflash: Function Traced successfully and replay test created! Path - {test_file_path}",
         )
 
     def trace_callback(self, frame: Any, event: str, arg: Any) -> None:
         if event not in ["call", "return"]:
-            return None
+            return
 
         code = frame.f_code
         if self.functions:
             if code.co_name not in self.functions:
-                return None
+                return
             if self.function_count[code.co_name] >= self.max_function_count:
                 return
             self.function_count[code.co_name] += 1
             if code.co_name in self.function_filenames:
                 assert self.function_filenames[code.co_name] == code.co_filename, (
                     f"Function {code.co_name} is defined in multiple files. "
                     f"Can only trace a unique function name at the moment. Aborting..."
@@ -110,15 +109,15 @@
         #         # TODO: Also check if this function arguments are unique from the values logged earlier
         elif not self.flag:
             self.flag = True
             return
 
         project_root = os.path.realpath(os.path.join(self.config["module_root"], ".."))
         self.function_modules[code.co_name] = module_name_from_file_path(
-            code.co_filename, project_root=project_root
+            code.co_filename, project_root=project_root,
         )
         cur = self.con.cursor()
 
         t_ns = time.perf_counter_ns()
         try:
             local_vars = pickle.dumps(frame.f_locals, protocol=pickle.HIGHEST_PROTOCOL)
             arg = pickle.dumps(arg, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `codeflash-0.5.0/codeflash/update_license_version.py` & `codeflash-0.5.1/codeflash/update_license_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     major_minor_version = ".".join(map(str, version[:2]))
 
     # Define the pattern to search for and the replacement string for the version
     version_pattern = re.compile(r"(Licensed Work:\s+Codeflash Client version\s+)(0\.\d+)(\.x)")
     version_replacement = r"\g<1>" + major_minor_version + r".x"
 
     # Read the LICENSE file
-    with open("codeflash/LICENSE", "r", encoding="utf8") as file:
+    with open("codeflash/LICENSE", encoding="utf8") as file:
         license_text = file.read()
 
     # Replace the version in the LICENSE file
     updated_license_text = version_pattern.sub(version_replacement, license_text)
 
     # Extract the current version from the LICENSE file
     current_version_match = re.search(r"version\s+(\d+\.\d+)\.x", license_text)
```

### Comparing `codeflash-0.5.0/codeflash/verification/comparator.py` & `codeflash-0.5.1/codeflash/verification/comparator.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 pandas.Categorical,
                 pandas.arrays.SparseArray,
             ),
         ):
             return orig.equals(new)
 
         if HAS_PANDAS and isinstance(
-            orig, (pandas.CategoricalDtype, pandas.Interval, pandas.Period)
+            orig, (pandas.CategoricalDtype, pandas.Interval, pandas.Period),
         ):
             return orig == new
 
         # This should be at the end of all numpy checking
         try:
             if HAS_NUMPY and np.isnan(orig):
                 return np.isnan(new)
@@ -141,10 +141,10 @@
         except Exception:
             pass
 
         # TODO : Add other types here
         logging.warning(f"Unknown comparator input type: {type(orig)}")
         return True
     except RecursionError as e:
-        logging.error(f"RecursionError while comparing objects: {e}")
+        logging.exception(f"RecursionError while comparing objects: {e}")
         sentry_sdk.capture_exception(e)
         return False
```

### Comparing `codeflash-0.5.0/codeflash/verification/equivalence.py` & `codeflash-0.5.1/codeflash/verification/equivalence.py`

 * *Files identical despite different names*

### Comparing `codeflash-0.5.0/codeflash/verification/parse_test_output.py` & `codeflash-0.5.1/codeflash/verification/parse_test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import logging
 import os
 import pathlib
-import pickle
 import sqlite3
 import subprocess
 from collections import defaultdict
 from typing import Optional
 
+import dill as pickle
 import sentry_sdk
 from junitparser.xunit2 import JUnitXml
 
 from codeflash.code_utils.code_utils import (
-    module_name_from_file_path,
     get_run_tmp_file,
+    module_name_from_file_path,
 )
 from codeflash.discovery.discover_unit_tests import discover_parameters_unittest
 from codeflash.verification.test_results import (
-    TestResults,
     FunctionTestInvocation,
-    TestType,
     InvocationId,
+    TestResults,
+    TestType,
 )
 from codeflash.verification.verification_utils import TestConfig
 
 
 def parse_test_return_values_bin(
-    file_location: str, test_framework: str, test_type: TestType, test_file_path: str
+    file_location: str,
+    test_framework: str,
+    test_type: TestType,
+    test_file_path: str,
 ) -> TestResults:
     test_results = TestResults()
     if not os.path.exists(file_location):
         logging.warning(f"No test results for {file_location} found.")
         return test_results
     with open(file_location, "rb") as file:
         while file:
@@ -43,15 +46,15 @@
             len_next = file.read(4)
             if not len_next:
                 return test_results
             len_next = int.from_bytes(len_next, byteorder="big")
             try:
                 test_pickle = pickle.loads(file.read(len_next))
             except Exception as e:
-                logging.error(f"Failed to load pickle file. Exception: {e}")
+                logging.exception(f"Failed to load pickle file. Exception: {e}")
                 return test_results
             len_next = file.read(4)
             len_next = int.from_bytes(len_next, byteorder="big")
             invocation_id = file.read(len_next).decode("ascii")
             # TODO : Remove the fully loaded unpickled object from the test_results.
             #  replace it with a link to the pickle object. Load it only on demand.
             #  The problem is that the unpickled object might be huge. This could cause codeflash to crash
@@ -61,15 +64,15 @@
                     id=InvocationId.from_str_id(encoded_test_name, invocation_id),
                     file_name=test_file_path,
                     did_pass=True,
                     runtime=duration,
                     test_framework=test_framework,
                     test_type=test_type,
                     return_value=test_pickle,
-                )
+                ),
             )
             # Hardcoding the test result to True because the test did execute and we are only interested in the return values,
             # the did_pass comes from the xml results file
     return test_results
 
 
 def parse_sqlite_test_results(
@@ -100,15 +103,15 @@
                 ),
                 file_name=test_py_file_path,
                 did_pass=True,
                 runtime=val[5],
                 test_framework=test_config.test_framework,
                 test_type=test_type,
                 return_value=None,
-            )
+            ),
         )
         # return_value is only None temporarily as this is only being used for the existing tests. This should generalize
         # to read the return_value from the sqlite file as well.
         # Hardcoding the test result to True because the test did execute and we are only interested in the return values,
         # the did_pass comes from the xml results file
     return test_results
 
@@ -132,27 +135,27 @@
         logging.warning(f"Failed to parse {test_xml_file_path} as JUnitXml. Exception: {e}")
         return test_results
 
     for suite in xml:
         for testcase in suite:
             class_name = testcase.classname
             file_name = suite._elem.attrib.get(
-                "file"
+                "file",
             )  # file_path_from_module_name(generated_tests_path, test_config.project_root_path)
             if (
                 file_name == f"unittest{os.sep}loader.py"
                 and class_name == "unittest.loader._FailedTest"
                 and suite.errors == 1
                 and suite.tests == 1
             ):
                 # This means that the test failed to load, so we don't want to crash on it
-                logging.info(f"Test failed to load, skipping it.")
+                logging.info("Test failed to load, skipping it.")
                 if run_result is not None:
                     logging.info(
-                        f"Test log - STDOUT : {run_result.stdout.decode()} \n STDERR : {run_result.stderr.decode()}"
+                        f"Test log - STDOUT : {run_result.stdout.decode()} \n STDERR : {run_result.stderr.decode()}",
                     )
                 return test_results
             file_name = test_py_file_path
 
             assert os.path.exists(file_name), f"File {file_name} doesn't exist."
             result = testcase.is_passed  # TODO: See for the cases of ERROR and SKIPPED
             test_module_path = module_name_from_file_path(file_name, test_config.project_root_path)
@@ -166,15 +169,15 @@
                 test_module_path = test_module_path[: -len("__perfinstrumented")]
             test_function = testcase.name
             if test_function is None:
                 with sentry_sdk.push_scope() as scope:
                     xml_file_contents = open(test_xml_file_path).read()
                     scope.set_extra("file", xml_file_contents)
                     sentry_sdk.capture_message(
-                        f"testcase.name is None in parse_test_xml for testcase {repr(testcase)} in file {xml_file_contents}"
+                        f"testcase.name is None in parse_test_xml for testcase {testcase!r} in file {xml_file_contents}",
                     )
                 continue
             # Parse test timing
             # system_out_content = ""
             # for system_out in testcase.system_out:
 
             #     system_out_content += system_out.text
@@ -189,57 +192,53 @@
                     ),
                     file_name=file_name,
                     runtime=None,
                     test_framework=test_config.test_framework,
                     did_pass=result,
                     test_type=test_type,
                     return_value=None,
-                )
+                ),
             )
     if len(test_results) == 0:
         logging.info(f"Test '{test_py_file_path}' failed to run, skipping it")
         if run_result is not None:
             logging.info(
-                f"Test log - STDOUT : {run_result.stdout.decode()} \n STDERR : {run_result.stderr.decode()}"
+                f"Test log - STDOUT : {run_result.stdout.decode()} \n STDERR : {run_result.stderr.decode()}",
             )
     return test_results
 
 
 def merge_test_results(
-    xml_test_results: TestResults, bin_test_results: TestResults, test_framework: str
+    xml_test_results: TestResults,
+    bin_test_results: TestResults,
+    test_framework: str,
 ) -> TestResults:
     merged_test_results = TestResults()
 
     grouped_xml_results = defaultdict(TestResults)
     grouped_bin_results = defaultdict(TestResults)
 
     # This is done to match the right iteration_id which might not be available in the xml
     for result in xml_test_results:
         if test_framework == "pytest":
             if "[" in result.id.test_function_name:  # handle parameterized test
-                test_function_name = result.id.test_function_name[
-                    : result.id.test_function_name.index("[")
-                ]
+                test_function_name = result.id.test_function_name[: result.id.test_function_name.index("[")]
             else:
                 test_function_name = result.id.test_function_name
 
         if test_framework == "unittest":
             test_function_name = result.id.test_function_name
             is_parameterized, new_test_function_name, _ = discover_parameters_unittest(
-                test_function_name
+                test_function_name,
             )
             if is_parameterized:  # handle parameterized test
                 test_function_name = new_test_function_name
 
         grouped_xml_results[
-            result.id.test_module_path
-            + ":"
-            + (result.id.test_class_name or "")
-            + ":"
-            + test_function_name
+            result.id.test_module_path + ":" + (result.id.test_class_name or "") + ":" + test_function_name
         ].add(result)
     for result in bin_test_results:
         grouped_bin_results[
             result.id.test_module_path
             + ":"
             + (result.id.test_class_name or "")
             + ":"
@@ -262,15 +261,15 @@
                         id=result_bin.id,
                         file_name=xml_result.file_name,
                         runtime=result_bin.runtime,
                         test_framework=xml_result.test_framework,
                         did_pass=xml_result.did_pass,
                         test_type=xml_result.test_type,
                         return_value=result_bin.return_value,
-                    )
+                    ),
                 )
         else:
             for i in range(len(bin_results.test_results)):
                 bin_result = bin_results.test_results[i]
                 try:
                     xml_result = xml_results.test_results[i]
                 except IndexError:
@@ -286,15 +285,15 @@
                         id=bin_result.id,
                         file_name=bin_result.file_name,
                         runtime=bin_result.runtime,
                         test_framework=bin_result.test_framework,
                         did_pass=bin_result.did_pass,
                         test_type=bin_result.test_type,
                         return_value=bin_result.return_value,
-                    )
+                    ),
                 )
 
     return merged_test_results
 
 
 def parse_test_results(
     test_xml_path: str,
@@ -317,39 +316,41 @@
             test_results_bin_file = parse_test_return_values_bin(
                 get_run_tmp_file(f"test_return_values_{optimization_iteration}.bin"),
                 test_framework=test_config.test_framework,
                 test_type=TestType.GENERATED_REGRESSION,
                 test_file_path=test_py_path,
             )
         except AttributeError as e:
-            logging.error(e)
+            logging.exception(e)
             test_results_bin_file = TestResults()
             pathlib.Path(
-                get_run_tmp_file(f"test_return_values_{optimization_iteration}.bin")
+                get_run_tmp_file(f"test_return_values_{optimization_iteration}.bin"),
             ).unlink(missing_ok=True)
     elif test_type == TestType.EXISTING_UNIT_TEST:
         try:
             test_results_bin_file = parse_sqlite_test_results(
                 get_run_tmp_file(f"test_return_values_{optimization_iteration}.sqlite"),
                 test_py_file_path=test_py_path,
                 test_type=TestType.EXISTING_UNIT_TEST,
                 test_config=test_config,
             )
         except AttributeError as e:
-            logging.error(e)
+            logging.exception(e)
             test_results_bin_file = TestResults()
     else:
         raise ValueError(f"Invalid test type: {test_type}")
 
     # We Probably want to remove deleting this file here later, because we want to preserve the reference to the
     # pickle blob in the test_results
     pathlib.Path(get_run_tmp_file(f"test_return_values_{optimization_iteration}.bin")).unlink(
-        missing_ok=True
+        missing_ok=True,
     )
     pathlib.Path(get_run_tmp_file(f"test_return_values_{optimization_iteration}.sqlite")).unlink(
-        missing_ok=True
+        missing_ok=True,
     )
 
     merged_results = merge_test_results(
-        test_results_xml, test_results_bin_file, test_config.test_framework
+        test_results_xml,
+        test_results_bin_file,
+        test_config.test_framework,
     )
     return merged_results
```

### Comparing `codeflash-0.5.0/codeflash/verification/test_results.py` & `codeflash-0.5.1/codeflash/verification/test_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import sys
 from enum import Enum
-from typing import Optional, Iterator, List
+from typing import Iterator, List, Optional
 
+from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
 from codeflash.verification.comparator import comparator
 
 
 class TestType(Enum):
     EXISTING_UNIT_TEST = 1
@@ -33,15 +34,15 @@
     iteration_id: Optional[str]
 
     # test_module_path:TestSuiteClass.test_function_name:function_tested:iteration_id
     def id(self):
         return f"{self.test_module_path}:{self.test_class_name or ''}.{self.test_function_name}:{self.function_getting_tested}:{self.iteration_id}"
 
     @staticmethod
-    def from_str_id(string_id: str, iteration_id: Optional[str] = None) -> "InvocationId":
+    def from_str_id(string_id: str, iteration_id: Optional[str] = None) -> InvocationId:
         components = string_id.split(":")
         assert len(components) == 4
         second_components = components[1].split(".")
         if len(second_components) == 1:
             test_class_name = None
             test_function_name = second_components[0]
         else:
@@ -63,26 +64,21 @@
     did_pass: bool  # Whether the test this function invocation was part of, passed or failed
     runtime: Optional[int]  # Time in nanoseconds
     test_framework: str  # unittest or pytest
     test_type: TestType
     return_value: Optional[object]  # The return value of the function invocation
 
 
-class TestResults:
-    test_results: list[FunctionTestInvocation]
-
-    def __init__(self, test_results=None):
-        if test_results is None:
-            test_results = []
-        self.test_results = test_results
+class TestResults(BaseModel):
+    test_results: List[FunctionTestInvocation] = []
 
     def add(self, function_test_invocation: FunctionTestInvocation) -> None:
         self.test_results.append(function_test_invocation)
 
-    def merge(self, other: "TestResults") -> None:
+    def merge(self, other: TestResults) -> None:
         self.test_results.extend(other.test_results)
 
     def get_by_id(self, invocation_id: InvocationId) -> Optional[FunctionTestInvocation]:
         return next((r for r in self.test_results if r.id == invocation_id), None)
 
     def get_all_ids(self) -> List[InvocationId]:
         return [test_result.id for test_result in self.test_results]
@@ -110,27 +106,27 @@
 
     @staticmethod
     def report_to_string(report: dict[TestType, dict[str, int]]) -> str:
         return " ".join(
             [
                 f"{test_type.to_name()}- (Passed: {report[test_type]['passed']}, Failed: {report[test_type]['failed']})"
                 for test_type in TestType
-            ]
+            ],
         )
 
     def total_passed_runtime(self) -> int:
         for result in self.test_results:
             if result.did_pass and result.runtime is None:
                 logging.debug(f"Ignoring test case that passed but had no runtime -> {result.id}")
         timing = sum(
             [
                 result.runtime
                 for result in self.test_results
                 if (result.did_pass and result.runtime is not None)
-            ]
+            ],
         )
         return timing
 
     def __iter__(self) -> Iterator[FunctionTestInvocation]:
         return iter(self.test_results)
 
     def __len__(self) -> int:
@@ -147,15 +143,15 @@
 
     def __contains__(self, value: FunctionTestInvocation) -> bool:
         return value in self.test_results
 
     def __bool__(self) -> bool:
         return bool(self.test_results)
 
-    def __eq__(self, other: TestResults):
+    def __eq__(self, other: object) -> bool:
         # Unordered comparison
         if type(self) != type(other):
             return False
         if len(self) != len(other):
             return False
         original_recursion_limit = sys.getrecursionlimit()
         for test_result in self:
```

### Comparing `codeflash-0.5.0/codeflash/verification/test_runner.py` & `codeflash-0.5.1/codeflash/verification/test_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import subprocess
-from typing import Tuple, Optional
+from typing import Optional, Tuple
 
 from codeflash.code_utils.code_utils import get_run_tmp_file
 
 
 def run_tests(
     test_path,
     test_framework: str,
@@ -24,24 +24,24 @@
                 "-q",
                 f"--timeout={pytest_timeout}",
                 f"--junitxml={result_file_path}",
             ],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
-            env=test_env,
+            env=test_env, check=False,
         )
     elif test_framework == "unittest":
         result_file_path = get_run_tmp_file("unittest_results.xml")
         results = subprocess.run(
             ["python", "-m", "xmlrunner"]
             + (["-v"] if verbose else [])
             + [test_path]
             + ["--output-file", result_file_path],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             cwd=cwd,
-            env=test_env,
+            env=test_env, check=False,
         )
     else:
         raise ValueError("Invalid test framework -- I only support Pytest and Unittest currently.")
     return result_file_path, results
```

### Comparing `codeflash-0.5.0/codeflash/verification/verification_utils.py` & `codeflash-0.5.1/codeflash/verification/verification_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import ast
 import os
 
 from pydantic.dataclasses import dataclass
 
 
 def get_test_file_path(
-    test_dir: str, function_name: str, iteration: int = 0, test_type: str = "unit"
+    test_dir: str, function_name: str, iteration: int = 0, test_type: str = "unit",
 ) -> str:
     assert test_type in ["unit", "inspired", "replay"]
     function_name = function_name.replace(".", "_")
     path = os.path.join(test_dir, f"test_{function_name}__{test_type}_test_{iteration}.py")
     if os.path.exists(path):
         return get_test_file_path(test_dir, function_name, iteration + 1)
     return path
@@ -35,19 +35,17 @@
 
     def __init__(self, import_list, test_framework):
         self.import_list = import_list
         self.test_framework = test_framework
 
     def visit_Import(self, node: ast.Import):
         self.import_list.append(node)
-        return None
 
     def visit_ImportFrom(self, node: ast.ImportFrom):
         self.import_list.append(node)
-        return None
 
     def visit_ClassDef(self, node: ast.ClassDef):
         if self.test_framework != "unittest":
             return node
         found = False
         if node.bases:
             for base in node.bases:
```

### Comparing `codeflash-0.5.0/codeflash/verification/verifier.py` & `codeflash-0.5.1/codeflash/verification/verifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import ast
 import logging
-from typing import Tuple, Optional
+from typing import Optional, Tuple
 
 from codeflash.api.aiservice import generate_regression_tests
-from codeflash.code_utils.code_utils import get_run_tmp_file
-from codeflash.code_utils.code_utils import module_name_from_file_path
+from codeflash.code_utils.code_utils import get_run_tmp_file, module_name_from_file_path
 from codeflash.discovery.functions_to_optimize import FunctionToOptimize
 from codeflash.verification.verification_utils import (
     ModifyInspiredTests,
-    get_test_file_path,
     TestConfig,
+    delete_multiple_if_name_main,
+    get_test_file_path,
 )
-from codeflash.verification.verification_utils import delete_multiple_if_name_main
 
 
 def generate_tests(
     source_code_being_tested: str,
     function_to_optimize: FunctionToOptimize,
     dependent_function_names: list[str],
     module_path: str,
@@ -31,15 +30,15 @@
         import importlib
 
         module = importlib.import_module(module_path)
         generated_test_source = module.CACHED_TESTS
         instrumented_test_source = module.CACHED_INSTRUMENTED_TESTS
         path = get_run_tmp_file("").replace("\\", "\\\\")  # Escape backslash for windows paths
         instrumented_test_source = instrumented_test_source.replace(
-            "{codeflash_run_tmp_dir_client_side}", path
+            "{codeflash_run_tmp_dir_client_side}", path,
         )
         logging.info(f"Using cached tests from {module_path}.CACHED_TESTS")
     else:
         test_module_path = module_name_from_file_path(
             get_test_file_path(test_cfg.tests_root, function_to_optimize.function_name, 0),
             test_cfg.project_root_path,
         )
@@ -53,20 +52,18 @@
             test_timeout=test_timeout,
             trace_id=function_trace_id,
         )
         if response and isinstance(response, tuple) and len(response) == 2:
             generated_test_source, instrumented_test_source = response
             path = get_run_tmp_file("").replace("\\", "\\\\")  # Escape backslash for windows paths
             instrumented_test_source = instrumented_test_source.replace(
-                "{codeflash_run_tmp_dir_client_side}", path
+                "{codeflash_run_tmp_dir_client_side}", path,
             )
         else:
-            logging.error(
-                f"Failed to generate and instrument tests for {function_to_optimize.function_name}"
-            )
+            logging.error(f"Failed to generate and instrument tests for {function_to_optimize.function_name}")
             return None
 
     # TODO: Add support for inspired tests
     # inspired_unit_tests = ""
 
     # merged_test_source = merge_unit_tests(
     #     instrumented_test_source, inspired_unit_tests, test_cfg.test_framework
@@ -76,15 +73,15 @@
 
 
 def merge_unit_tests(unit_test_source: str, inspired_unit_tests: str, test_framework: str) -> str:
     try:
         inspired_unit_tests_ast = ast.parse(inspired_unit_tests)
         unit_test_source_ast = ast.parse(unit_test_source)
     except SyntaxError as e:
-        logging.error(f"Syntax error in code: {e}")
+        logging.exception(f"Syntax error in code: {e}")
         return unit_test_source
     import_list: list[ast.stmt] = list()
     modified_ast = ModifyInspiredTests(import_list, test_framework).visit(inspired_unit_tests_ast)
     if test_framework == "pytest":
         # Because we only want to modify the top level test functions
         for node in ast.iter_child_nodes(modified_ast):
             if isinstance(node, ast.FunctionDef):
```

### Comparing `codeflash-0.5.0/pyproject.toml` & `codeflash-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "codeflash"
-version = "0.5.0" # Determined by poetry-dynamic-versioning during `poetry build`
+version = "0.5.1" # Determined by poetry-dynamic-versioning during `poetry build`
 description = "Client for codeflash.ai - automatic code performance optimization, powered by AI"
 license = "BSL-1.1"
 authors = ["CodeFlash Inc. <contact@codeflash.ai>"]
 homepage = "https://codeflash.ai"
 readme = "README.md"
 packages = [
     { include = "codeflash" },
@@ -30,23 +30,25 @@
 humanize = ">=4.0.0"
 posthog = ">=3.0.0"
 click = ">=8.1.0"
 inquirer = ">=3.0.0"
 sentry-sdk = "^1.40.6"
 parameterized = ">=0.9.0"
 returns = "^0.22.0"
-isort = "5.13.2"
+isort = ">=5.11.0"
+dill = "^0.3.8"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.12.0"
 mypy = "^1.9.0"
 ruff = "^0.3.5"
+ruff-lsp = "^0.0.53"
 
 
 [tool.poetry.build]
 script = "codeflash/update_license_version.py"
 
 [tool.poetry.scripts]
 codeflash = "codeflash.main:main"
@@ -92,19 +94,14 @@
 
 [tool.ruff]
 line-length = 110
 
 [tool.ruff.format]
 docstring-code-format = true
 
-
-[tool.black]
-line-length = 110
-target-version = ['py312']
-
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 vcs = "git"
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["codeflash/version.py"]
```

### Comparing `codeflash-0.5.0/PKG-INFO` & `codeflash-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: codeflash
-Version: 0.5.0
+Version: 0.5.1
 Summary: Client for codeflash.ai - automatic code performance optimization, powered by AI
 Home-page: https://codeflash.ai
 License: BSL-1.1
 Keywords: codeflash,performance,optimization,ai,code,machine learning,LLM
 Author: CodeFlash Inc.
 Author-email: contact@codeflash.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=22.3.0)
 Requires-Dist: click (>=8.1.0)
+Requires-Dist: dill (>=0.3.8,<0.4.0)
 Requires-Dist: gitpython (>=3.1.31)
 Requires-Dist: humanize (>=4.0.0)
 Requires-Dist: inquirer (>=3.0.0)
-Requires-Dist: isort (==5.13.2)
+Requires-Dist: isort (>=5.11.0)
 Requires-Dist: jedi (>=0.19.0)
 Requires-Dist: junitparser (>=3.1.0)
 Requires-Dist: libcst (>=1.0.1)
 Requires-Dist: parameterized (>=0.9.0)
 Requires-Dist: posthog (>=3.0.0)
 Requires-Dist: pydantic (>=1.10.1)
 Requires-Dist: pytest (>=7.0.0)
```

