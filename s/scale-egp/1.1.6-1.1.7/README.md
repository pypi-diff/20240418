# Comparing `tmp/scale_egp-1.1.6.tar.gz` & `tmp/scale_egp-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_egp-1.1.6.tar", max compression
+gzip compressed data, was "scale_egp-1.1.7.tar", max compression
```

## Comparing `scale_egp-1.1.6.tar` & `scale_egp-1.1.7.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0    17873 2024-04-16 18:44:22.539571 scale_egp-1.1.6/README.md
--rw-r--r--   0        0        0     1101 2024-04-16 18:44:22.539571 scale_egp-1.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/__init__.py
--rw-r--r--   0        0        0       74 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/__init__.py
--rw-r--r--   0        0        0     4533 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/cli_main.py
--rw-r--r--   0        0        0    17966 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/collections.py
--rw-r--r--   0        0        0     7857 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/formatter.py
--rw-r--r--   0        0        0     1469 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/model_instance_description.py
--rw-r--r--   0        0        0     1828 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/cli/parser.py
--rw-r--r--   0        0        0     1733 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/__init__.py
--rw-r--r--   0        0        0    13096 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/client.py
--rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/__init__.py
--rw-r--r--   0        0        0     2914 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/application_specs.py
--rw-r--r--   0        0        0     3170 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/chunks.py
--rw-r--r--   0        0        0     5272 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/completions.py
--rw-r--r--   0        0        0     2500 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_configs.py
--rw-r--r--   0        0        0    25007 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_datasets.py
--rw-r--r--   0        0        0     8055 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/evaluations.py
--rw-r--r--   0        0        0     4918 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/fine_tuning.py
--rw-r--r--   0        0        0    25810 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/knowledge_bases.py
--rw-r--r--   0        0        0     2685 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/model_groups.py
--rw-r--r--   0        0        0     4798 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/model_templates.py
--rw-r--r--   0        0        0     7572 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/models.py
--rw-r--r--   0        0        0     1862 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/question_sets.py
--rw-r--r--   0        0        0     2588 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/questions.py
--rw-r--r--   0        0        0     1510 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/collections/users.py
--rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/constants/__init__.py
--rw-r--r--   0        0        0      762 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/constants/model_schemas.py
--rw-r--r--   0        0        0     9257 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/enums.py
--rw-r--r--   0        0        0        0 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/__init__.py
--rw-r--r--   0        0        0     2712 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/fine_tuning_jobs.py
--rw-r--r--   0        0        0     2069 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/model_enums.py
--rw-r--r--   0        0        0     8403 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/models/model_vendor_configuration.py
--rw-r--r--   0        0        0      647 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/types/__init__.py
--rw-r--r--   0        0        0     4651 2024-04-16 18:44:22.539571 scale_egp-1.1.6/scale_egp/sdk/types/agents.py
--rw-r--r--   0        0        0      741 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/application_specs.py
--rw-r--r--   0        0        0     6125 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/chunks.py
--rw-r--r--   0        0        0     6553 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/completions.py
--rw-r--r--   0        0        0     1016 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/embeddings.py
--rw-r--r--   0        0        0     1019 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_configs.py
--rw-r--r--   0        0        0     3170 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_dataset_test_cases.py
--rw-r--r--   0        0        0     1686 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_datasets.py
--rw-r--r--   0        0        0     4837 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluation_test_case_results.py
--rw-r--r--   0        0        0     1398 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/evaluations.py
--rw-r--r--   0        0        0     3401 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/fine_tuning.py
--rw-r--r--   0        0        0     1860 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_artifacts.py
--rw-r--r--   0        0        0     1559 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_chunks.py
--rw-r--r--   0        0        0    15686 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_uploads.py
--rw-r--r--   0        0        0     1863 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/knowledge_bases.py
--rw-r--r--   0        0        0     1112 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/memory_strategy.py
--rw-r--r--   0        0        0     2478 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/message.py
--rw-r--r--   0        0        0     3557 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/model_templates.py
--rw-r--r--   0        0        0    14065 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/models.py
--rw-r--r--   0        0        0     1086 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/models_group.py
--rw-r--r--   0        0        0      891 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/question_sets.py
--rw-r--r--   0        0        0     5234 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/questions.py
--rw-r--r--   0        0        0      410 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/sdk/types/user_info.py
--rw-r--r--   0        0        0        0 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/__init__.py
--rw-r--r--   0        0        0    11461 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/api_utils.py
--rw-r--r--   0        0        0     3639 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/model_utils.py
--rw-r--r--   0        0        0      107 2024-04-16 18:44:22.543572 scale_egp-1.1.6/scale_egp/utils/strenum_compat.py
--rw-r--r--   0        0        0    18869 1970-01-01 00:00:00.000000 scale_egp-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    17873 2024-04-18 15:16:35.856385 scale_egp-1.1.7/README.md
+-rw-r--r--   0        0        0     1138 2024-04-18 15:16:35.856385 scale_egp-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-18 15:16:35.856385 scale_egp-1.1.7/scale_egp/cli/__init__.py
+-rw-r--r--   0        0        0     4737 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/cli_main.py
+-rw-r--r--   0        0        0    18102 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/collections.py
+-rw-r--r--   0        0        0     7857 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/formatter.py
+-rw-r--r--   0        0        0     1469 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/model_instance_description.py
+-rw-r--r--   0        0        0     1828 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/parser.py
+-rw-r--r--   0        0        0    52384 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/cli/vpc_setup_commands.py
+-rw-r--r--   0        0        0     1733 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/client.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/__init__.py
+-rw-r--r--   0        0        0     2914 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/application_specs.py
+-rw-r--r--   0        0        0     3170 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/chunks.py
+-rw-r--r--   0        0        0     5272 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/completions.py
+-rw-r--r--   0        0        0     2500 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_configs.py
+-rw-r--r--   0        0        0    25007 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_datasets.py
+-rw-r--r--   0        0        0     8055 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/evaluations.py
+-rw-r--r--   0        0        0     4918 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/fine_tuning.py
+-rw-r--r--   0        0        0    25810 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/knowledge_bases.py
+-rw-r--r--   0        0        0     2685 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/model_groups.py
+-rw-r--r--   0        0        0     4798 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/model_templates.py
+-rw-r--r--   0        0        0     7667 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/models.py
+-rw-r--r--   0        0        0     1862 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/question_sets.py
+-rw-r--r--   0        0        0     2588 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/questions.py
+-rw-r--r--   0        0        0     1510 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/collections/users.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/constants/__init__.py
+-rw-r--r--   0        0        0      762 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/constants/model_schemas.py
+-rw-r--r--   0        0        0     9257 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/enums.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/__init__.py
+-rw-r--r--   0        0        0     2712 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/fine_tuning_jobs.py
+-rw-r--r--   0        0        0     2069 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/model_enums.py
+-rw-r--r--   0        0        0     8403 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/models/model_vendor_configuration.py
+-rw-r--r--   0        0        0      647 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/__init__.py
+-rw-r--r--   0        0        0     4651 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/agents.py
+-rw-r--r--   0        0        0      741 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/application_specs.py
+-rw-r--r--   0        0        0     6125 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/chunks.py
+-rw-r--r--   0        0        0     6553 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/completions.py
+-rw-r--r--   0        0        0     1016 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/embeddings.py
+-rw-r--r--   0        0        0     1019 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_configs.py
+-rw-r--r--   0        0        0     3170 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_dataset_test_cases.py
+-rw-r--r--   0        0        0     1686 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_datasets.py
+-rw-r--r--   0        0        0     4837 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluation_test_case_results.py
+-rw-r--r--   0        0        0     1398 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/evaluations.py
+-rw-r--r--   0        0        0     3401 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/fine_tuning.py
+-rw-r--r--   0        0        0     1860 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_artifacts.py
+-rw-r--r--   0        0        0     1559 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_chunks.py
+-rw-r--r--   0        0        0    15686 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_uploads.py
+-rw-r--r--   0        0        0     1863 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/knowledge_bases.py
+-rw-r--r--   0        0        0     1112 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/memory_strategy.py
+-rw-r--r--   0        0        0     2478 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/message.py
+-rw-r--r--   0        0        0     3557 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/model_templates.py
+-rw-r--r--   0        0        0    14065 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/models.py
+-rw-r--r--   0        0        0     1086 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/models_group.py
+-rw-r--r--   0        0        0      891 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/question_sets.py
+-rw-r--r--   0        0        0     5234 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/questions.py
+-rw-r--r--   0        0        0      410 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/sdk/types/user_info.py
+-rw-r--r--   0        0        0        0 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/__init__.py
+-rw-r--r--   0        0        0    11461 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/api_utils.py
+-rw-r--r--   0        0        0     3639 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/model_utils.py
+-rw-r--r--   0        0        0      107 2024-04-18 15:16:35.860385 scale_egp-1.1.7/scale_egp/utils/strenum_compat.py
+-rw-r--r--   0        0        0    18948 1970-01-01 00:00:00.000000 scale_egp-1.1.7/PKG-INFO
```

### Comparing `scale_egp-1.1.6/README.md` & `scale_egp-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/pyproject.toml` & `scale_egp-1.1.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "scale-egp"
-version = "1.1.6"
+version = "1.1.7"
 description = "SDK for Scale SGP API"
 license = "Apache 2.0 modified with Commons Clause"
 authors = ["Scale SGP team"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/sgp-py/"
 repository = "https://github.com/scaleapi/egp-py"
 packages = [{include = "scale_egp"}]
@@ -19,14 +19,16 @@
 pydantic = ">=1.10.11,<2.0"
 httpx = ">0.25.0,<1.0"
 strenum = "^0.4.15"
 rich = "^13.7.0"
 fastjsonschema = "^2.19.0"
 argh = "^0.30.4"
 mock = "^4.0.3"
+boto3 = "^1.34.81"
+docker = "^7.0.0"
 
 [tool.poetry.scripts]
 scale-egp = "scale_egp.cli.cli_main:exec_cli"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.4"
 pylint = "2.17.7"
```

### Comparing `scale_egp-1.1.6/scale_egp/cli/cli_main.py` & `scale_egp-1.1.7/scale_egp/cli/cli_main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 import sys
 from typing import List, Optional
 from argh import ArghParser
 from scale_egp.cli.collections import (
+    GenericCommands,
     CollectionCRUDCommandsForImmutable,
     EGPClientFactory,
     FineTuningJobCommands,
     ModelDeploymentCommands,
     ModelInstanceCommands,
     ModelTemplateCommands,
     TrainingDatasetCommands,
@@ -16,14 +17,16 @@
 from scale_egp.cli.formatter import AVAILABLE_FORMATTERS
 from scale_egp.cli.parser import get_parser, dispatch
 import itertools
 from asyncio import iscoroutinefunction, run
 from functools import wraps
 import traceback
 
+from scale_egp.cli.vpc_setup_commands import AwsVpcSetupCommands
+
 
 def async_to_sync(fn):
     if iscoroutinefunction(fn):
 
         @wraps(fn)
         def fn2(self, *args, **kwargs):
             # Note: not passing in self, since the function will be bound to that instance
@@ -34,15 +37,15 @@
         # title of the output table
         instance = fn.__self__
         bound_method = fn2.__get__(instance, instance.__class__)
         return bound_method
     return fn
 
 
-def add_commands_to_parser(parser: ArghParser, commands: CollectionCRUDCommandsForImmutable):
+def add_commands_to_parser(parser: ArghParser, commands: GenericCommands):
     parser.add_commands(
         [
             async_to_sync(getattr(commands, key))
             for key in dir(commands)
             if not key.startswith("_") and callable(getattr(commands, key))
         ],
         group_name=commands.command_group_name,
@@ -92,15 +95,17 @@
     add_commands_to_parser(parser, ModelGroupCommands(client_factory))
     add_commands_to_parser(parser, ModelInstanceCommands(client_factory))
     add_commands_to_parser(parser, ModelDeploymentCommands(client_factory))
     add_commands_to_parser(parser, ModelTemplateCommands(client_factory))
     add_commands_to_parser(parser, UserCommands(client_factory))
     add_commands_to_parser(parser, FineTuningJobCommands(client_factory))
     add_commands_to_parser(parser, TrainingDatasetCommands(client_factory))
+    add_commands_to_parser(parser, AwsVpcSetupCommands(client_factory))
     for plugin_command_cls in load_plugins(parser):
+        print(f"Loading plugin: {plugin_command_cls.__name__}")
         add_commands_to_parser(parser, plugin_command_cls(client_factory))
     args = parser.parse_args(argv)
     try:
         client_factory.set_client_kwargs(
             api_key=args.api_key,
             endpoint_url=args.endpoint_url,
             account_id=args.account_id,
```

### Comparing `scale_egp-1.1.6/scale_egp/cli/collections.py` & `scale_egp-1.1.7/scale_egp/cli/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,27 +60,38 @@
 
     def get_client(self) -> EGPClient:
         if self.client is None:
             self.client = EGPClient(**self._client_kwargs)
         return self.client
 
 
-class CollectionCRUDCommandsForImmutable(Generic[EntityT, RequestT]):
+class GenericCommands:
+    command_group_name = "generic"
+    command_group_title = "Generic commands"
+
+    def __init__(
+        self,
+        client_factory: EGPClientFactory,
+    ):
+        self._client_factory = client_factory
+
+
+class CollectionCRUDCommandsForImmutable(GenericCommands, Generic[EntityT, RequestT]):
     command_group_name = "CRUD"
     command_group_title: Optional[str] = None
     list_formatting_options: Optional[FormattingOptions] = None
 
     def __init__(
         self,
         client_factory: EGPClientFactory,
         entity_type: Type[EntityT],
         request_type: Type[RequestT],
         collection_type: Type[APIEngine],
     ):
-        self._client_factory = client_factory
+        super().__init__(client_factory)
         self._entity_type = entity_type
         self._request_type = request_type
         self._collection_type = collection_type
 
     def _get_collection_instance(self) -> APIEngine:
         return self._collection_type(self._client_factory.get_client())
 
@@ -347,26 +358,20 @@
                 "request_schema": schemas[0].schema(),
                 "response_schema": schemas[1].schema(),
             }
             for (model_type, schemas) in MODEL_SCHEMAS.items()
         ]
 
 
-class UserCommands:
+class UserCommands(GenericCommands):
     command_group_name = "user"
     command_group_title = "User management and account information"
 
-    def __init__(
-        self,
-        client_factory: EGPClientFactory,
-    ):
-        self.client_factory = client_factory
-
     def whoami(self) -> UserInfoResponse:
-        return self.client_factory.get_client().user_info()
+        return self._client_factory.get_client().user_info()
 
 
 class FineTuningJobCommands(
     CollectionCRUDCommandsForImmutable[FineTuningJob, FineTuningJobRequest]
 ):
     command_group_name = "fine-tuning-job"
     command_group_title = "Manage model fine tuning jobs"
```

### Comparing `scale_egp-1.1.6/scale_egp/cli/formatter.py` & `scale_egp-1.1.7/scale_egp/cli/formatter.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/cli/model_instance_description.py` & `scale_egp-1.1.7/scale_egp/cli/model_instance_description.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/cli/parser.py` & `scale_egp-1.1.7/scale_egp/cli/parser.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/exceptions.py` & `scale_egp-1.1.7/scale_egp/exceptions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/client.py` & `scale_egp-1.1.7/scale_egp/sdk/client.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/application_specs.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/chunks.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/completions.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_configs.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/evaluation_datasets.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/evaluations.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/fine_tuning.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/knowledge_bases.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/model_groups.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/model_groups.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/model_templates.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/models.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,25 +233,26 @@
         """
         response = self._get(
             sub_path=self._sub_path.format(model_id=model.id),
         )
         return [ModelDeployment.from_dict(deployment) for deployment in response.json()]
 
     def execute(
-        self, id: str, model: ModelInstance, request: BaseModelRequest
+        self, id: str, model: ModelInstance, request: BaseModelRequest, timeout: Optional[int] = None
     ) -> BaseModelResponse:
         """
         Execute the specified model deployment with the given request.
 
         Returns:
             The model deployment's response.
         """
+        timeout = timeout or 10 * 60 # 10 minutes
         # TODO: verify model_request_parameters matches model template's
         #  model_request_parameters_schema if set
         model_request_cls, model_response_cls = MODEL_SCHEMAS[model.model_type]
-        assert isinstance(request, model_request_cls)
+        assert isinstance(request, model_request_cls) or isinstance(request, dict)
         response = self._post(
             sub_path=f"{self._sub_path.format(model_id=model.id)}/{id}/execute",
             request=request,
-            timeout=10 * 60,  # 10 minutes
+            timeout=timeout
         )
         return model_response_cls(**response.json())
```

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/question_sets.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/questions.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/collections/users.py` & `scale_egp-1.1.7/scale_egp/sdk/collections/users.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/constants/model_schemas.py` & `scale_egp-1.1.7/scale_egp/sdk/constants/model_schemas.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/enums.py` & `scale_egp-1.1.7/scale_egp/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/models/fine_tuning_jobs.py` & `scale_egp-1.1.7/scale_egp/sdk/models/fine_tuning_jobs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/models/model_enums.py` & `scale_egp-1.1.7/scale_egp/sdk/models/model_enums.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/models/model_vendor_configuration.py` & `scale_egp-1.1.7/scale_egp/sdk/models/model_vendor_configuration.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/__init__.py` & `scale_egp-1.1.7/scale_egp/sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/agents.py` & `scale_egp-1.1.7/scale_egp/sdk/types/agents.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/application_specs.py` & `scale_egp-1.1.7/scale_egp/sdk/types/application_specs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/chunks.py` & `scale_egp-1.1.7/scale_egp/sdk/types/chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/completions.py` & `scale_egp-1.1.7/scale_egp/sdk/types/completions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/embeddings.py` & `scale_egp-1.1.7/scale_egp/sdk/types/embeddings.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_configs.py` & `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_configs.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_dataset_test_cases.py` & `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_dataset_test_cases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_datasets.py` & `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_datasets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/evaluation_test_case_results.py` & `scale_egp-1.1.7/scale_egp/sdk/types/evaluation_test_case_results.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/evaluations.py` & `scale_egp-1.1.7/scale_egp/sdk/types/evaluations.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/fine_tuning.py` & `scale_egp-1.1.7/scale_egp/sdk/types/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_artifacts.py` & `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_artifacts.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_chunks.py` & `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_chunks.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_base_uploads.py` & `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_base_uploads.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/knowledge_bases.py` & `scale_egp-1.1.7/scale_egp/sdk/types/knowledge_bases.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/memory_strategy.py` & `scale_egp-1.1.7/scale_egp/sdk/types/memory_strategy.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/message.py` & `scale_egp-1.1.7/scale_egp/sdk/types/message.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/model_templates.py` & `scale_egp-1.1.7/scale_egp/sdk/types/model_templates.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/models.py` & `scale_egp-1.1.7/scale_egp/sdk/types/models.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/models_group.py` & `scale_egp-1.1.7/scale_egp/sdk/types/models_group.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/question_sets.py` & `scale_egp-1.1.7/scale_egp/sdk/types/question_sets.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/sdk/types/questions.py` & `scale_egp-1.1.7/scale_egp/sdk/types/questions.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/utils/api_utils.py` & `scale_egp-1.1.7/scale_egp/utils/api_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/scale_egp/utils/model_utils.py` & `scale_egp-1.1.7/scale_egp/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `scale_egp-1.1.6/PKG-INFO` & `scale_egp-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: scale-egp
-Version: 1.1.6
+Version: 1.1.7
 Summary: SDK for Scale SGP API
 Home-page: https://scaleapi.github.io/sgp-py/
 License: Apache 2.0 modified with Commons Clause
 Author: Scale SGP team
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argh (>=0.30.4,<0.31.0)
+Requires-Dist: boto3 (>=1.34.81,<2.0.0)
+Requires-Dist: docker (>=7.0.0,<8.0.0)
 Requires-Dist: fastjsonschema (>=2.19.0,<3.0.0)
 Requires-Dist: httpx (>0.25.0,<1.0)
 Requires-Dist: mock (>=4.0.3,<5.0.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0)
 Requires-Dist: requests (>=2.22)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: strenum (>=0.4.15,<0.5.0)
```

