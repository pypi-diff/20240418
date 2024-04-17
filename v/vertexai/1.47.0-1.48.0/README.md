# Comparing `tmp/vertexai-1.47.0.tar.gz` & `tmp/vertexai-1.48.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertexai-1.47.0.tar", last modified: Tue Apr 16 18:10:52 2024, max compression
+gzip compressed data, was "vertexai-1.48.0.tar", last modified: Wed Apr 17 22:44:02 2024, max compression
```

## Comparing `vertexai-1.47.0.tar` & `vertexai-1.48.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-16 18:10:51.000000 vertexai-1.47.0/
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    11358 2023-05-05 15:54:43.000000 vertexai-1.47.0/LICENSE
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7570 2024-04-16 18:10:51.000000 vertexai-1.47.0/PKG-INFO
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      264 2024-03-07 21:35:24.000000 vertexai-1.47.0/README.md
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      490 2024-04-06 04:10:48.000000 vertexai-1.47.0/pyproject.toml
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)       38 2024-04-16 18:10:51.000000 vertexai-1.47.0/setup.cfg
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     6004 2024-03-14 23:52:24.000000 vertexai-1.47.0/setup.py
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      625 2024-04-08 20:24:36.000000 vertexai-1.47.0/version.py
-drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7570 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/PKG-INFO
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      242 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/SOURCES.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/dependency_links.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/not-zip-safe
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     2845 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/requires.txt
--rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        8 2024-04-16 18:10:51.000000 vertexai-1.47.0/vertexai.egg-info/top_level.txt
+drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-17 22:44:02.000000 vertexai-1.48.0/
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    11358 2023-05-05 15:54:43.000000 vertexai-1.48.0/LICENSE
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    10471 2024-04-17 22:44:02.000000 vertexai-1.48.0/PKG-INFO
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      264 2024-03-07 21:35:24.000000 vertexai-1.48.0/README.md
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      490 2024-04-06 04:10:48.000000 vertexai-1.48.0/pyproject.toml
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)       38 2024-04-17 22:44:02.000000 vertexai-1.48.0/setup.cfg
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     7616 2024-04-17 22:43:06.000000 vertexai-1.48.0/setup.py
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      625 2024-04-17 20:52:55.000000 vertexai-1.48.0/version.py
+drwxrwxr-x   0 wuamy    (518829) primarygroup (89939)        0 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)    10471 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/PKG-INFO
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)      242 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        1 2024-04-17 22:44:01.000000 vertexai-1.48.0/vertexai.egg-info/not-zip-safe
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)     4129 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/requires.txt
+-rw-rw-r--   0 wuamy    (518829) primarygroup (89939)        8 2024-04-17 22:44:02.000000 vertexai-1.48.0/vertexai.egg-info/top_level.txt
```

### Comparing `vertexai-1.47.0/LICENSE` & `vertexai-1.48.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vertexai-1.47.0/PKG-INFO` & `vertexai-1.48.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,188 @@
 Metadata-Version: 2.1
 Name: vertexai
-Version: 1.47.0
+Version: 1.48.0
 Summary: Please run pip install vertexai to use the Vertex SDK.
 Home-page: https://github.com/googleapis/python-aiplatform
 Author: Google LLC
 Author-email: Google LLC <googleapis-packages@google.com>
 License: Apache 2.0
 Project-URL: repository, https://github.com/googleapis/python-aiplatform.git
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: google-cloud-aiplatform==1.47.0
+Requires-Dist: google-cloud-aiplatform[all]==1.48.0
 Provides-Extra: endpoint
 Requires-Dist: requests>=2.28.1; extra == "endpoint"
 Provides-Extra: full
-Requires-Dist: lit-nlp==0.4.0; extra == "full"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
-Requires-Dist: cloudpickle<3.0; extra == "full"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "full"
+Requires-Dist: pandas>=1.0.0; extra == "full"
 Requires-Dist: numpy>=1.15.0; extra == "full"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "full"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "full"
+Requires-Dist: requests>=2.28.1; extra == "full"
+Requires-Dist: pydantic<2; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "full"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
+Requires-Dist: immutabledict; extra == "full"
+Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
+Requires-Dist: cloudpickle<3.0; extra == "full"
 Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
-Requires-Dist: google-cloud-logging<4.0; extra == "full"
 Requires-Dist: pyarrow>=6.0.1; extra == "full"
+Requires-Dist: google-vizier>=0.1.6; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: lit-nlp==0.4.0; extra == "full"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "full"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "full"
+Requires-Dist: pydantic<3; extra == "full"
 Requires-Dist: docker>=5.0.3; extra == "full"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
-Requires-Dist: pyyaml==5.3.1; extra == "full"
-Requires-Dist: google-vizier>=0.1.6; extra == "full"
-Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "full"
-Requires-Dist: pydantic<2; extra == "full"
-Requires-Dist: requests>=2.28.1; extra == "full"
-Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
-Requires-Dist: pandas>=1.0.0; extra == "full"
-Requires-Dist: google-cloud-bigquery; extra == "full"
+Requires-Dist: google-cloud-logging<4.0; extra == "full"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "full"
 Requires-Dist: google-cloud-bigquery-storage; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "full"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "full"
 Requires-Dist: starlette>=0.17.1; extra == "full"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "full"
+Requires-Dist: google-cloud-bigquery; extra == "full"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "full"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
 Provides-Extra: metadata
 Requires-Dist: pandas>=1.0.0; extra == "metadata"
 Requires-Dist: numpy>=1.15.0; extra == "metadata"
 Provides-Extra: tensorboard
-Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "tensorboard"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "tensorboard"
 Provides-Extra: testing
-Requires-Dist: lit-nlp==0.4.0; extra == "testing"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
-Requires-Dist: cloudpickle<3.0; extra == "testing"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "testing"
+Requires-Dist: pandas>=1.0.0; extra == "testing"
 Requires-Dist: numpy>=1.15.0; extra == "testing"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "testing"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "testing"
+Requires-Dist: requests>=2.28.1; extra == "testing"
+Requires-Dist: pydantic<2; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
+Requires-Dist: immutabledict; extra == "testing"
+Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
+Requires-Dist: cloudpickle<3.0; extra == "testing"
 Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
-Requires-Dist: google-cloud-logging<4.0; extra == "testing"
 Requires-Dist: pyarrow>=6.0.1; extra == "testing"
+Requires-Dist: google-vizier>=0.1.6; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: lit-nlp==0.4.0; extra == "testing"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "testing"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "testing"
+Requires-Dist: pydantic<3; extra == "testing"
 Requires-Dist: docker>=5.0.3; extra == "testing"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
-Requires-Dist: pyyaml==5.3.1; extra == "testing"
-Requires-Dist: google-vizier>=0.1.6; extra == "testing"
-Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "testing"
-Requires-Dist: pydantic<2; extra == "testing"
-Requires-Dist: requests>=2.28.1; extra == "testing"
-Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
-Requires-Dist: pandas>=1.0.0; extra == "testing"
-Requires-Dist: google-cloud-bigquery; extra == "testing"
+Requires-Dist: google-cloud-logging<4.0; extra == "testing"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "testing"
 Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "testing"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "testing"
 Requires-Dist: starlette>=0.17.1; extra == "testing"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "testing"
+Requires-Dist: google-cloud-bigquery; extra == "testing"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "testing"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: bigframes; python_version >= "3.10" and extra == "testing"
 Requires-Dist: google-api-core<3.0.0,>=2.11; extra == "testing"
 Requires-Dist: grpcio-testing; extra == "testing"
 Requires-Dist: ipython; extra == "testing"
 Requires-Dist: kfp<3.0.0,>=2.6.0; extra == "testing"
 Requires-Dist: pyfakefs; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: scikit-learn; extra == "testing"
-Requires-Dist: tensorflow<=2.12.0,>=2.3.0; extra == "testing"
-Requires-Dist: torch<2.1.0,>=2.0.0; extra == "testing"
-Requires-Dist: xgboost; extra == "testing"
-Requires-Dist: xgboost_ray; extra == "testing"
+Requires-Dist: tensorflow==2.13.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: tensorflow==2.16.1; python_version > "3.11" and extra == "testing"
+Requires-Dist: torch<2.1.0,>=2.0.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: torch>=2.2.0; python_version > "3.11" and extra == "testing"
 Requires-Dist: requests-toolbelt<1.0.0; extra == "testing"
+Requires-Dist: immutabledict; extra == "testing"
+Requires-Dist: xgboost; extra == "testing"
 Provides-Extra: xai
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "xai"
 Provides-Extra: lit
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "lit"
 Requires-Dist: pandas>=1.0.0; extra == "lit"
 Requires-Dist: lit-nlp==0.4.0; extra == "lit"
 Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "lit"
 Provides-Extra: cloud-profiler
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "cloud-profiler"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "cloud-profiler"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "cloud-profiler"
 Provides-Extra: pipelines
-Requires-Dist: pyyaml==5.3.1; extra == "pipelines"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "pipelines"
 Provides-Extra: vizier
 Requires-Dist: google-vizier>=0.1.6; extra == "vizier"
 Provides-Extra: prediction
 Requires-Dist: docker>=5.0.3; extra == "prediction"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "prediction"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "prediction"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "prediction"
 Requires-Dist: starlette>=0.17.1; extra == "prediction"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "prediction"
 Provides-Extra: datasets
 Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "datasets"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "datasets"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "datasets"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "datasets"
 Provides-Extra: private-endpoints
 Requires-Dist: urllib3<1.27,>=1.21.1; extra == "private-endpoints"
 Requires-Dist: requests>=2.28.1; extra == "private-endpoints"
 Provides-Extra: autologging
 Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "autologging"
 Provides-Extra: preview
 Requires-Dist: cloudpickle<3.0; extra == "preview"
 Requires-Dist: google-cloud-logging<4.0; extra == "preview"
 Provides-Extra: ray
 Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "ray"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "ray"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "ray"
 Requires-Dist: google-cloud-bigquery-storage; extra == "ray"
 Requires-Dist: google-cloud-bigquery; extra == "ray"
 Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "ray"
 Requires-Dist: pyarrow>=6.0.1; extra == "ray"
 Requires-Dist: pydantic<2; extra == "ray"
+Requires-Dist: immutabledict; extra == "ray"
+Provides-Extra: ray-testing
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "ray-testing"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "ray-testing"
+Requires-Dist: google-cloud-bigquery-storage; extra == "ray-testing"
+Requires-Dist: google-cloud-bigquery; extra == "ray-testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "ray-testing"
+Requires-Dist: pyarrow>=6.0.1; extra == "ray-testing"
+Requires-Dist: pydantic<2; extra == "ray-testing"
+Requires-Dist: immutabledict; extra == "ray-testing"
+Requires-Dist: pytest-xdist; extra == "ray-testing"
+Requires-Dist: ray[train]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; extra == "ray-testing"
+Requires-Dist: scikit-learn; extra == "ray-testing"
+Requires-Dist: tensorflow; extra == "ray-testing"
+Requires-Dist: torch<2.1.0,>=2.0.0; extra == "ray-testing"
+Requires-Dist: xgboost; extra == "ray-testing"
+Requires-Dist: xgboost_ray; extra == "ray-testing"
+Provides-Extra: reasoningengine
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "reasoningengine"
+Requires-Dist: pydantic<3; extra == "reasoningengine"
+Provides-Extra: rapid-evaluation
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "rapid-evaluation"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "rapid-evaluation"
+Provides-Extra: langchain
+Requires-Dist: langchain<0.2,>=0.1.13; extra == "langchain"
+Requires-Dist: langchain-core<0.2; extra == "langchain"
+Requires-Dist: langchain-google-vertexai<0.2; extra == "langchain"
+Provides-Extra: langchain-testing
+Requires-Dist: langchain<0.2,>=0.1.13; extra == "langchain-testing"
+Requires-Dist: langchain-core<0.2; extra == "langchain-testing"
+Requires-Dist: langchain-google-vertexai<0.2; extra == "langchain-testing"
+Requires-Dist: pytest-xdist; extra == "langchain-testing"
 
 vertexai
 ========
 
 To use the Vertex GAPIC clients, please install the `google-cloud-aiplatform` PyPi package by running `pip install google-cloud-aiplatform`.
 
 To use the Vertex AI SDK, please install the `vertexai` PyPi package by running `pip install vertexai`.
```

### Comparing `vertexai-1.47.0/setup.py` & `vertexai-1.48.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright 2024 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,31 +13,31 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import io
 import os
-import setuptools
 
+import setuptools  # type: ignore
 
 name = "vertexai"
 description = "Vertex AI API client library"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 readme_filename = os.path.join(package_root, "README.md")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 version = {}
 with open(os.path.join(package_root, "version.py")) as fp:
     exec(fp.read(), version)
 version = version["__version__"]
 
-tensorboard_extra_require = ["tensorflow >=2.3.0, <2.15.0"]
+tensorboard_extra_require = ["tensorflow >=2.3.0, <3.0.0dev; python_version<='3.11'"]
 metadata_extra_require = ["pandas >= 1.0.0", "numpy>=1.15.0"]
 xai_extra_require = ["tensorflow >=2.3.0, <3.0.0dev"]
 lit_extra_require = [
     "tensorflow >= 2.3.0, <3.0.0dev",
     "pandas >= 1.0.0",
     "lit-nlp == 0.4.0",
     "explainable-ai-sdk >= 1.0.0",
@@ -49,56 +49,104 @@
 ]
 featurestore_extra_require = [
     "google-cloud-bigquery-storage",
     "pandas >= 1.0.0",
     "pyarrow >= 6.0.1",
 ]
 pipelines_extra_require = [
-    "pyyaml==5.3.1",
+    "pyyaml>=5.3.1,<7",
 ]
 datasets_extra_require = [
     "pyarrow >= 3.0.0, < 8.0dev; python_version<'3.11'",
-    "pyarrow >= 10.0.1; python_version>='3.11'",
+    "pyarrow >= 10.0.1; python_version=='3.11'",
+    "pyarrow >= 14.0.0; python_version>='3.12'",
 ]
 
 vizier_extra_require = [
     "google-vizier>=0.1.6",
 ]
 
 prediction_extra_require = [
     "docker >= 5.0.3",
-    "fastapi >= 0.71.0, <0.103.1",
+    "fastapi >= 0.71.0, <=0.109.1",
     "httpx >=0.23.0, <0.25.0",  # Optional dependency of fastapi
     "starlette >= 0.17.1",
     "uvicorn[standard] >= 0.16.0",
 ]
 
 endpoint_extra_require = ["requests >= 2.28.1"]
 
-private_endpoints_extra_require = ["urllib3 >=1.21.1, <1.27", "requests >= 2.28.1"]
+private_endpoints_extra_require = [
+    "urllib3 >=1.21.1, <1.27",
+    "requests >= 2.28.1",
+]
 
 autologging_extra_require = ["mlflow>=1.27.0,<=2.1.1"]
 
 preview_extra_require = [
     "cloudpickle < 3.0",
     "google-cloud-logging < 4.0",
 ]
 
 ray_extra_require = [
     # Cluster only supports 2.4.0 and 2.9.3
-    "ray[default] >= 2.4, <= 2.9.3,!= 2.5.*,!= 2.6.*,!= 2.7.*,!= 2.8.*,!=2.9.0,!=2.9.1,!=2.9.2; python_version<'3.11'",
+    (
+        "ray[default] >= 2.4, <= 2.9.3,!= 2.5.*,!= 2.6.*,!= 2.7.*,!="
+        " 2.8.*,!=2.9.0,!=2.9.1,!=2.9.2; python_version<'3.11'"
+    ),
     # Ray Data v2.4 in Python 3.11 is broken, but got fixed in Ray v2.5.
-    "ray[default] >= 2.5, <= 2.9.3; python_version>='3.11'",
+    "ray[default] >= 2.5, <= 2.9.3; python_version=='3.11'",
     "google-cloud-bigquery-storage",
     "google-cloud-bigquery",
     "pandas >= 1.0.0, < 2.2.0",
     "pyarrow >= 6.0.1",
     # Workaround for https://github.com/ray-project/ray/issues/36990.
     # TODO(b/295406381): Remove this pin when we drop support of ray<=2.5.
     "pydantic < 2",
+    "immutabledict",
+]
+
+genai_requires = (
+    "pydantic < 3",
+    "docstring_parser < 1",
+)
+
+ray_testing_extra_require = ray_extra_require + [
+    "pytest-xdist",
+    # ray train extras required for prediction tests
+    (
+        "ray[train] >= 2.4, <= 2.9.3,!= 2.5.*,!= 2.6.*,!= 2.7.*,!="
+        " 2.8.*,!=2.9.0,!=2.9.1,!=2.9.2"
+    ),
+    # Framework version constraints copied from testing_extra_require
+    "scikit-learn",
+    "tensorflow",
+    "torch >= 2.0.0, < 2.1.0",
+    "xgboost",
+    "xgboost_ray",
+]
+
+reasoning_engine_extra_require = [
+    "cloudpickle >= 2.2.1, < 3.0",
+    "pydantic < 3",
+]
+
+rapid_evaluation_extra_require = [
+    "nest_asyncio >= 1.0.0, < 1.6.0",
+    "pandas >= 1.0.0, < 2.2.0",
+]
+
+langchain_extra_require = [
+    "langchain >= 0.1.13, < 0.2",
+    "langchain-core < 0.2",
+    "langchain-google-vertexai < 0.2",
+]
+
+langchain_testing_extra_require = langchain_extra_require + [
+    "pytest-xdist",
 ]
 
 full_extra_require = list(
     set(
         tensorboard_extra_require
         + metadata_extra_require
         + xai_extra_require
@@ -109,14 +157,16 @@
         + endpoint_extra_require
         + vizier_extra_require
         + prediction_extra_require
         + private_endpoints_extra_require
         + autologging_extra_require
         + preview_extra_require
         + ray_extra_require
+        + reasoning_engine_extra_require
+        + rapid_evaluation_extra_require
     )
 )
 testing_extra_require = (
     full_extra_require
     + profiler_extra_require
     + [
         "bigframes; python_version>='3.10'",
@@ -125,36 +175,40 @@
         "grpcio-testing",
         "ipython",
         "kfp >= 2.6.0, < 3.0.0",
         "pyfakefs",
         "pytest-asyncio",
         "pytest-xdist",
         "scikit-learn",
-        "tensorflow >= 2.3.0, <= 2.12.0",
+        # Lazy import requires > 2.12.0
+        "tensorflow == 2.13.0; python_version<='3.11'",
+        "tensorflow == 2.16.1; python_version>'3.11'",
         # TODO(jayceeli) torch 2.1.0 has conflict with pyfakefs, will check if
         # future versions fix this issue
-        "torch >= 2.0.0, < 2.1.0",
-        "xgboost",
-        "xgboost_ray",
+        "torch >= 2.0.0, < 2.1.0; python_version<='3.11'",
+        "torch >= 2.2.0; python_version>'3.11'",
         "requests-toolbelt < 1.0.0",
+        "immutabledict",
+        "xgboost",
     ]
 )
 
+
 setuptools.setup(
     name=name,
     version=version,
     description=description,
     long_description=readme,
     author="Google LLC",
     author_email="vertex-sdk-dev-pypi@google.com",
     license="Apache 2.0",
     url="https://github.com/googleapis/python-aiplatform",
     platforms="Posix; MacOS X; Windows",
     include_package_data=True,
-    install_requires=[f"google-cloud-aiplatform == {version}"],
+    install_requires=[f"google-cloud-aiplatform[all] == {version}"],
     extras_require={
         "endpoint": endpoint_extra_require,
         "full": full_extra_require,
         "metadata": metadata_extra_require,
         "tensorboard": tensorboard_extra_require,
         "testing": testing_extra_require,
         "xai": xai_extra_require,
@@ -164,14 +218,19 @@
         "vizier": vizier_extra_require,
         "prediction": prediction_extra_require,
         "datasets": datasets_extra_require,
         "private_endpoints": private_endpoints_extra_require,
         "autologging": autologging_extra_require,
         "preview": preview_extra_require,
         "ray": ray_extra_require,
+        "ray_testing": ray_testing_extra_require,
+        "reasoningengine": reasoning_engine_extra_require,
+        "rapid_evaluation": rapid_evaluation_extra_require,
+        "langchain": langchain_extra_require,
+        "langchain_testing": langchain_testing_extra_require,
     },
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

### Comparing `vertexai-1.47.0/version.py` & `vertexai-1.48.0/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "1.47.0"
+__version__ = "1.48.0"
```

### Comparing `vertexai-1.47.0/vertexai.egg-info/PKG-INFO` & `vertexai-1.48.0/vertexai.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,188 @@
 Metadata-Version: 2.1
 Name: vertexai
-Version: 1.47.0
+Version: 1.48.0
 Summary: Please run pip install vertexai to use the Vertex SDK.
 Home-page: https://github.com/googleapis/python-aiplatform
 Author: Google LLC
 Author-email: Google LLC <googleapis-packages@google.com>
 License: Apache 2.0
 Project-URL: repository, https://github.com/googleapis/python-aiplatform.git
 Platform: Posix; MacOS X; Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: google-cloud-aiplatform==1.47.0
+Requires-Dist: google-cloud-aiplatform[all]==1.48.0
 Provides-Extra: endpoint
 Requires-Dist: requests>=2.28.1; extra == "endpoint"
 Provides-Extra: full
-Requires-Dist: lit-nlp==0.4.0; extra == "full"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
-Requires-Dist: cloudpickle<3.0; extra == "full"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "full"
+Requires-Dist: pandas>=1.0.0; extra == "full"
 Requires-Dist: numpy>=1.15.0; extra == "full"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "full"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "full"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "full"
+Requires-Dist: requests>=2.28.1; extra == "full"
+Requires-Dist: pydantic<2; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "full"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "full"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
+Requires-Dist: immutabledict; extra == "full"
+Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
+Requires-Dist: cloudpickle<3.0; extra == "full"
 Requires-Dist: urllib3<1.27,>=1.21.1; extra == "full"
-Requires-Dist: google-cloud-logging<4.0; extra == "full"
 Requires-Dist: pyarrow>=6.0.1; extra == "full"
+Requires-Dist: google-vizier>=0.1.6; extra == "full"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: lit-nlp==0.4.0; extra == "full"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "full"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "full"
+Requires-Dist: pydantic<3; extra == "full"
 Requires-Dist: docker>=5.0.3; extra == "full"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "full"
-Requires-Dist: pyyaml==5.3.1; extra == "full"
-Requires-Dist: google-vizier>=0.1.6; extra == "full"
-Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "full"
-Requires-Dist: pydantic<2; extra == "full"
-Requires-Dist: requests>=2.28.1; extra == "full"
-Requires-Dist: uvicorn[standard]>=0.16.0; extra == "full"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "full"
-Requires-Dist: pandas>=1.0.0; extra == "full"
-Requires-Dist: google-cloud-bigquery; extra == "full"
+Requires-Dist: google-cloud-logging<4.0; extra == "full"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "full"
 Requires-Dist: google-cloud-bigquery-storage; extra == "full"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "full"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "full"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "full"
 Requires-Dist: starlette>=0.17.1; extra == "full"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "full"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "full"
+Requires-Dist: google-cloud-bigquery; extra == "full"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "full"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "full"
 Provides-Extra: metadata
 Requires-Dist: pandas>=1.0.0; extra == "metadata"
 Requires-Dist: numpy>=1.15.0; extra == "metadata"
 Provides-Extra: tensorboard
-Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "tensorboard"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "tensorboard"
 Provides-Extra: testing
-Requires-Dist: lit-nlp==0.4.0; extra == "testing"
-Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
-Requires-Dist: cloudpickle<3.0; extra == "testing"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "testing"
+Requires-Dist: pandas>=1.0.0; extra == "testing"
 Requires-Dist: numpy>=1.15.0; extra == "testing"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "testing"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "testing"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "testing"
+Requires-Dist: requests>=2.28.1; extra == "testing"
+Requires-Dist: pydantic<2; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "testing"
+Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
+Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
+Requires-Dist: immutabledict; extra == "testing"
+Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
+Requires-Dist: cloudpickle<3.0; extra == "testing"
 Requires-Dist: urllib3<1.27,>=1.21.1; extra == "testing"
-Requires-Dist: google-cloud-logging<4.0; extra == "testing"
 Requires-Dist: pyarrow>=6.0.1; extra == "testing"
+Requires-Dist: google-vizier>=0.1.6; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: lit-nlp==0.4.0; extra == "testing"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "testing"
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "testing"
+Requires-Dist: pydantic<3; extra == "testing"
 Requires-Dist: docker>=5.0.3; extra == "testing"
-Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "testing"
-Requires-Dist: pyyaml==5.3.1; extra == "testing"
-Requires-Dist: google-vizier>=0.1.6; extra == "testing"
-Requires-Dist: tensorflow<2.15.0,>=2.3.0; extra == "testing"
-Requires-Dist: pydantic<2; extra == "testing"
-Requires-Dist: requests>=2.28.1; extra == "testing"
-Requires-Dist: uvicorn[standard]>=0.16.0; extra == "testing"
-Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
-Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "testing"
-Requires-Dist: pandas>=1.0.0; extra == "testing"
-Requires-Dist: google-cloud-bigquery; extra == "testing"
+Requires-Dist: google-cloud-logging<4.0; extra == "testing"
+Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "testing"
 Requires-Dist: google-cloud-bigquery-storage; extra == "testing"
-Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "testing"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "testing"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "testing"
 Requires-Dist: starlette>=0.17.1; extra == "testing"
-Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "testing"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "testing"
+Requires-Dist: google-cloud-bigquery; extra == "testing"
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "testing"
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "testing"
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "testing"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "testing"
 Requires-Dist: bigframes; python_version >= "3.10" and extra == "testing"
 Requires-Dist: google-api-core<3.0.0,>=2.11; extra == "testing"
 Requires-Dist: grpcio-testing; extra == "testing"
 Requires-Dist: ipython; extra == "testing"
 Requires-Dist: kfp<3.0.0,>=2.6.0; extra == "testing"
 Requires-Dist: pyfakefs; extra == "testing"
 Requires-Dist: pytest-asyncio; extra == "testing"
 Requires-Dist: pytest-xdist; extra == "testing"
 Requires-Dist: scikit-learn; extra == "testing"
-Requires-Dist: tensorflow<=2.12.0,>=2.3.0; extra == "testing"
-Requires-Dist: torch<2.1.0,>=2.0.0; extra == "testing"
-Requires-Dist: xgboost; extra == "testing"
-Requires-Dist: xgboost_ray; extra == "testing"
+Requires-Dist: tensorflow==2.13.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: tensorflow==2.16.1; python_version > "3.11" and extra == "testing"
+Requires-Dist: torch<2.1.0,>=2.0.0; python_version <= "3.11" and extra == "testing"
+Requires-Dist: torch>=2.2.0; python_version > "3.11" and extra == "testing"
 Requires-Dist: requests-toolbelt<1.0.0; extra == "testing"
+Requires-Dist: immutabledict; extra == "testing"
+Requires-Dist: xgboost; extra == "testing"
 Provides-Extra: xai
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "xai"
 Provides-Extra: lit
 Requires-Dist: tensorflow<3.0.0dev,>=2.3.0; extra == "lit"
 Requires-Dist: pandas>=1.0.0; extra == "lit"
 Requires-Dist: lit-nlp==0.4.0; extra == "lit"
 Requires-Dist: explainable-ai-sdk>=1.0.0; extra == "lit"
 Provides-Extra: cloud-profiler
 Requires-Dist: tensorboard-plugin-profile<3.0.0dev,>=2.4.0; extra == "cloud-profiler"
 Requires-Dist: werkzeug<2.1.0dev,>=2.0.0; extra == "cloud-profiler"
 Requires-Dist: tensorflow<3.0.0dev,>=2.4.0; extra == "cloud-profiler"
 Provides-Extra: pipelines
-Requires-Dist: pyyaml==5.3.1; extra == "pipelines"
+Requires-Dist: pyyaml<7,>=5.3.1; extra == "pipelines"
 Provides-Extra: vizier
 Requires-Dist: google-vizier>=0.1.6; extra == "vizier"
 Provides-Extra: prediction
 Requires-Dist: docker>=5.0.3; extra == "prediction"
-Requires-Dist: fastapi<0.103.1,>=0.71.0; extra == "prediction"
+Requires-Dist: fastapi<=0.109.1,>=0.71.0; extra == "prediction"
 Requires-Dist: httpx<0.25.0,>=0.23.0; extra == "prediction"
 Requires-Dist: starlette>=0.17.1; extra == "prediction"
 Requires-Dist: uvicorn[standard]>=0.16.0; extra == "prediction"
 Provides-Extra: datasets
 Requires-Dist: pyarrow<8.0dev,>=3.0.0; python_version < "3.11" and extra == "datasets"
-Requires-Dist: pyarrow>=10.0.1; python_version >= "3.11" and extra == "datasets"
+Requires-Dist: pyarrow>=10.0.1; python_version == "3.11" and extra == "datasets"
+Requires-Dist: pyarrow>=14.0.0; python_version >= "3.12" and extra == "datasets"
 Provides-Extra: private-endpoints
 Requires-Dist: urllib3<1.27,>=1.21.1; extra == "private-endpoints"
 Requires-Dist: requests>=2.28.1; extra == "private-endpoints"
 Provides-Extra: autologging
 Requires-Dist: mlflow<=2.1.1,>=1.27.0; extra == "autologging"
 Provides-Extra: preview
 Requires-Dist: cloudpickle<3.0; extra == "preview"
 Requires-Dist: google-cloud-logging<4.0; extra == "preview"
 Provides-Extra: ray
 Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "ray"
-Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version >= "3.11" and extra == "ray"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "ray"
 Requires-Dist: google-cloud-bigquery-storage; extra == "ray"
 Requires-Dist: google-cloud-bigquery; extra == "ray"
 Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "ray"
 Requires-Dist: pyarrow>=6.0.1; extra == "ray"
 Requires-Dist: pydantic<2; extra == "ray"
+Requires-Dist: immutabledict; extra == "ray"
+Provides-Extra: ray-testing
+Requires-Dist: ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; python_version < "3.11" and extra == "ray-testing"
+Requires-Dist: ray[default]<=2.9.3,>=2.5; python_version == "3.11" and extra == "ray-testing"
+Requires-Dist: google-cloud-bigquery-storage; extra == "ray-testing"
+Requires-Dist: google-cloud-bigquery; extra == "ray-testing"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "ray-testing"
+Requires-Dist: pyarrow>=6.0.1; extra == "ray-testing"
+Requires-Dist: pydantic<2; extra == "ray-testing"
+Requires-Dist: immutabledict; extra == "ray-testing"
+Requires-Dist: pytest-xdist; extra == "ray-testing"
+Requires-Dist: ray[train]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4; extra == "ray-testing"
+Requires-Dist: scikit-learn; extra == "ray-testing"
+Requires-Dist: tensorflow; extra == "ray-testing"
+Requires-Dist: torch<2.1.0,>=2.0.0; extra == "ray-testing"
+Requires-Dist: xgboost; extra == "ray-testing"
+Requires-Dist: xgboost_ray; extra == "ray-testing"
+Provides-Extra: reasoningengine
+Requires-Dist: cloudpickle<3.0,>=2.2.1; extra == "reasoningengine"
+Requires-Dist: pydantic<3; extra == "reasoningengine"
+Provides-Extra: rapid-evaluation
+Requires-Dist: nest_asyncio<1.6.0,>=1.0.0; extra == "rapid-evaluation"
+Requires-Dist: pandas<2.2.0,>=1.0.0; extra == "rapid-evaluation"
+Provides-Extra: langchain
+Requires-Dist: langchain<0.2,>=0.1.13; extra == "langchain"
+Requires-Dist: langchain-core<0.2; extra == "langchain"
+Requires-Dist: langchain-google-vertexai<0.2; extra == "langchain"
+Provides-Extra: langchain-testing
+Requires-Dist: langchain<0.2,>=0.1.13; extra == "langchain-testing"
+Requires-Dist: langchain-core<0.2; extra == "langchain-testing"
+Requires-Dist: langchain-google-vertexai<0.2; extra == "langchain-testing"
+Requires-Dist: pytest-xdist; extra == "langchain-testing"
 
 vertexai
 ========
 
 To use the Vertex GAPIC clients, please install the `google-cloud-aiplatform` PyPi package by running `pip install google-cloud-aiplatform`.
 
 To use the Vertex AI SDK, please install the `vertexai` PyPi package by running `pip install vertexai`.
```

### Comparing `vertexai-1.47.0/vertexai.egg-info/requires.txt` & `vertexai-1.48.0/vertexai.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,155 +1,222 @@
-google-cloud-aiplatform==1.47.0
+google-cloud-aiplatform[all]==1.48.0
 
 [autologging]
 mlflow<=2.1.1,>=1.27.0
 
 [cloud_profiler]
 tensorboard-plugin-profile<3.0.0dev,>=2.4.0
 werkzeug<2.1.0dev,>=2.0.0
 tensorflow<3.0.0dev,>=2.4.0
 
 [datasets]
 
 [datasets:python_version < "3.11"]
 pyarrow<8.0dev,>=3.0.0
 
-[datasets:python_version >= "3.11"]
+[datasets:python_version == "3.11"]
 pyarrow>=10.0.1
 
+[datasets:python_version >= "3.12"]
+pyarrow>=14.0.0
+
 [endpoint]
 requests>=2.28.1
 
 [full]
-lit-nlp==0.4.0
-pandas<2.2.0,>=1.0.0
-cloudpickle<3.0
+pandas>=1.0.0
 numpy>=1.15.0
 httpx<0.25.0,>=0.23.0
+requests>=2.28.1
+pydantic<2
+pandas<2.2.0,>=1.0.0
+mlflow<=2.1.1,>=1.27.0
+immutabledict
+uvicorn[standard]>=0.16.0
+cloudpickle<3.0
 urllib3<1.27,>=1.21.1
-google-cloud-logging<4.0
 pyarrow>=6.0.1
+google-vizier>=0.1.6
 tensorflow<3.0.0dev,>=2.3.0
+lit-nlp==0.4.0
+fastapi<=0.109.1,>=0.71.0
+cloudpickle<3.0,>=2.2.1
+pydantic<3
 docker>=5.0.3
-mlflow<=2.1.1,>=1.27.0
-pyyaml==5.3.1
-google-vizier>=0.1.6
-tensorflow<2.15.0,>=2.3.0
-pydantic<2
-requests>=2.28.1
-uvicorn[standard]>=0.16.0
-pandas>=1.0.0
-google-cloud-bigquery
+google-cloud-logging<4.0
+explainable-ai-sdk>=1.0.0
+pyyaml<7,>=5.3.1
 google-cloud-bigquery-storage
 starlette>=0.17.1
-explainable-ai-sdk>=1.0.0
-fastapi<0.103.1,>=0.71.0
+google-cloud-bigquery
+nest_asyncio<1.6.0,>=1.0.0
 
 [full:python_version < "3.11"]
-ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 pyarrow<8.0dev,>=3.0.0
+ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
+
+[full:python_version <= "3.11"]
+tensorflow<3.0.0dev,>=2.3.0
 
-[full:python_version >= "3.11"]
+[full:python_version == "3.11"]
 ray[default]<=2.9.3,>=2.5
 pyarrow>=10.0.1
 
+[full:python_version >= "3.12"]
+pyarrow>=14.0.0
+
+[langchain]
+langchain<0.2,>=0.1.13
+langchain-core<0.2
+langchain-google-vertexai<0.2
+
+[langchain_testing]
+langchain<0.2,>=0.1.13
+langchain-core<0.2
+langchain-google-vertexai<0.2
+pytest-xdist
+
 [lit]
 tensorflow<3.0.0dev,>=2.3.0
 pandas>=1.0.0
 lit-nlp==0.4.0
 explainable-ai-sdk>=1.0.0
 
 [metadata]
 pandas>=1.0.0
 numpy>=1.15.0
 
 [pipelines]
-pyyaml==5.3.1
+pyyaml<7,>=5.3.1
 
 [prediction]
 docker>=5.0.3
-fastapi<0.103.1,>=0.71.0
+fastapi<=0.109.1,>=0.71.0
 httpx<0.25.0,>=0.23.0
 starlette>=0.17.1
 uvicorn[standard]>=0.16.0
 
 [preview]
 cloudpickle<3.0
 google-cloud-logging<4.0
 
 [private_endpoints]
 urllib3<1.27,>=1.21.1
 requests>=2.28.1
 
+[rapid_evaluation]
+nest_asyncio<1.6.0,>=1.0.0
+pandas<2.2.0,>=1.0.0
+
 [ray]
 google-cloud-bigquery-storage
 google-cloud-bigquery
 pandas<2.2.0,>=1.0.0
 pyarrow>=6.0.1
 pydantic<2
+immutabledict
 
 [ray:python_version < "3.11"]
 ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 
-[ray:python_version >= "3.11"]
+[ray:python_version == "3.11"]
 ray[default]<=2.9.3,>=2.5
 
+[ray_testing]
+google-cloud-bigquery-storage
+google-cloud-bigquery
+pandas<2.2.0,>=1.0.0
+pyarrow>=6.0.1
+pydantic<2
+immutabledict
+pytest-xdist
+ray[train]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
+scikit-learn
+tensorflow
+torch<2.1.0,>=2.0.0
+xgboost
+xgboost_ray
+
+[ray_testing:python_version < "3.11"]
+ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
+
+[ray_testing:python_version == "3.11"]
+ray[default]<=2.9.3,>=2.5
+
+[reasoningengine]
+cloudpickle<3.0,>=2.2.1
+pydantic<3
+
 [tensorboard]
-tensorflow<2.15.0,>=2.3.0
+
+[tensorboard:python_version <= "3.11"]
+tensorflow<3.0.0dev,>=2.3.0
 
 [testing]
-lit-nlp==0.4.0
-pandas<2.2.0,>=1.0.0
-cloudpickle<3.0
+pandas>=1.0.0
 numpy>=1.15.0
 httpx<0.25.0,>=0.23.0
+requests>=2.28.1
+pydantic<2
+pandas<2.2.0,>=1.0.0
+mlflow<=2.1.1,>=1.27.0
+immutabledict
+uvicorn[standard]>=0.16.0
+cloudpickle<3.0
 urllib3<1.27,>=1.21.1
-google-cloud-logging<4.0
 pyarrow>=6.0.1
+google-vizier>=0.1.6
 tensorflow<3.0.0dev,>=2.3.0
+lit-nlp==0.4.0
+fastapi<=0.109.1,>=0.71.0
+cloudpickle<3.0,>=2.2.1
+pydantic<3
 docker>=5.0.3
-mlflow<=2.1.1,>=1.27.0
-pyyaml==5.3.1
-google-vizier>=0.1.6
-tensorflow<2.15.0,>=2.3.0
-pydantic<2
-requests>=2.28.1
-uvicorn[standard]>=0.16.0
-pandas>=1.0.0
-google-cloud-bigquery
+google-cloud-logging<4.0
+explainable-ai-sdk>=1.0.0
+pyyaml<7,>=5.3.1
 google-cloud-bigquery-storage
 starlette>=0.17.1
-explainable-ai-sdk>=1.0.0
-fastapi<0.103.1,>=0.71.0
+google-cloud-bigquery
+nest_asyncio<1.6.0,>=1.0.0
 tensorboard-plugin-profile<3.0.0dev,>=2.4.0
 werkzeug<2.1.0dev,>=2.0.0
 tensorflow<3.0.0dev,>=2.4.0
 google-api-core<3.0.0,>=2.11
 grpcio-testing
 ipython
 kfp<3.0.0,>=2.6.0
 pyfakefs
 pytest-asyncio
 pytest-xdist
 scikit-learn
-tensorflow<=2.12.0,>=2.3.0
-torch<2.1.0,>=2.0.0
-xgboost
-xgboost_ray
 requests-toolbelt<1.0.0
+xgboost
 
 [testing:python_version < "3.11"]
-ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 pyarrow<8.0dev,>=3.0.0
+ray[default]!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.0,!=2.9.1,!=2.9.2,<=2.9.3,>=2.4
 
-[testing:python_version >= "3.10"]
-bigframes
+[testing:python_version <= "3.11"]
+tensorflow<3.0.0dev,>=2.3.0
+tensorflow==2.13.0
+torch<2.1.0,>=2.0.0
 
-[testing:python_version >= "3.11"]
+[testing:python_version == "3.11"]
 ray[default]<=2.9.3,>=2.5
 pyarrow>=10.0.1
 
+[testing:python_version > "3.11"]
+tensorflow==2.16.1
+torch>=2.2.0
+
+[testing:python_version >= "3.10"]
+bigframes
+
+[testing:python_version >= "3.12"]
+pyarrow>=14.0.0
+
 [vizier]
 google-vizier>=0.1.6
 
 [xai]
 tensorflow<3.0.0dev,>=2.3.0
```

