# Comparing `tmp/gwas_sumstats_tools-1.0.8.tar.gz` & `tmp/gwas_sumstats_tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas_sumstats_tools-1.0.8.tar", max compression
+gzip compressed data, was "gwas_sumstats_tools-1.0.9.tar", max compression
```

## Comparing `gwas_sumstats_tools-1.0.8.tar` & `gwas_sumstats_tools-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.8/LICENSE
--rw-r--r--   0        0        0     6157 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.8/README.md
--rwxr-xr-x   0        0        0    14459 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/cli.py
--rwxr-xr-x   0        0        0     2262 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/config.py
--rwxr-xr-x   0        0        0     5380 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/format.py
--rw-r--r--   0        0        0     2929 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/gen_meta.py
--rwxr-xr-x   0        0        0    10291 2023-06-06 14:58:15.071099 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/interfaces/data_table.py
--rwxr-xr-x   0        0        0    14737 2024-02-12 11:42:54.286579 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/interfaces/metadata.py
--rwxr-xr-x   0        0        0     3913 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/read.py
--rwxr-xr-x   0        0        0     5815 2023-10-16 12:59:49.118532 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/schema/data_table.py
--rwxr-xr-x   0        0        0     2225 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/schema/metadata.py
--rwxr-xr-x   0        0        0     4773 2023-06-06 14:58:15.118099 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/utils.py
--rwxr-xr-x   0        0        0     8337 2023-06-06 14:58:15.119099 gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/validate.py
--rw-r--r--   0        0        0      727 2024-02-14 12:14:11.931183 gwas_sumstats_tools-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     6885 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.9/LICENSE
+-rw-r--r--   0        0        0     6157 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.9/README.md
+-rwxr-xr-x   0        0        0    14459 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/cli.py
+-rwxr-xr-x   0        0        0     2434 2024-03-21 12:32:53.318384 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/config.py
+-rwxr-xr-x   0        0        0     5380 2023-06-06 14:58:15.062099 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/format.py
+-rw-r--r--   0        0        0     2929 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/gen_meta.py
+-rwxr-xr-x   0        0        0    10291 2023-06-06 14:58:15.071099 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/interfaces/data_table.py
+-rwxr-xr-x   0        0        0    15078 2024-03-21 12:32:53.318384 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/interfaces/metadata.py
+-rwxr-xr-x   0        0        0     3913 2023-06-06 14:58:15.084099 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/read.py
+-rwxr-xr-x   0        0        0     5815 2023-10-16 12:59:49.118532 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/schema/data_table.py
+-rwxr-xr-x   0        0        0     2225 2023-12-20 11:57:00.548676 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/schema/metadata.py
+-rwxr-xr-x   0        0        0     4773 2023-06-06 14:58:15.118099 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/utils.py
+-rwxr-xr-x   0        0        0     8337 2023-06-06 14:58:15.119099 gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/validate.py
+-rw-r--r--   0        0        0      727 2024-03-21 12:32:53.318384 gwas_sumstats_tools-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6885 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.9/PKG-INFO
```

### Comparing `gwas_sumstats_tools-1.0.8/LICENSE` & `gwas_sumstats_tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/README.md` & `gwas_sumstats_tools-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/cli.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/cli.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/config.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 )
 
 GWAS_CAT_API_INGEST_STUDIES_URL = _env_variable_else(
     "GWAS_CAT_API_INGEST_STUDIES_URL",
     "https://www.ebi.ac.uk/gwas/ingest/api/v2/studies/",
 )
 
+GWAS_CAT_API_INGEST_STUDIES_URL_SANDBOX = _env_variable_else(
+    "GWAS_CAT_API_INGEST_STUDIES_URL_SANDBOX",
+    "https://wwwdev.ebi.ac.uk/gwas/ingest/api/v2/studies/",
+)
+
 GWAS_CAT_STUDY_MAPPINGS = {
     "genotyping_technology": "genotyping_technology",
     "traitDescription": "trait_description",
     "effect_allele_frequency_lower_limit": "minor_allele_freq_lower_limit",
     "minor_allele_frequency_lower_limit": "minor_allele_freq_lower_limit",
     "summary_statistics_assembly": "genome_assembly",
     "analysisSoftware": "analysis_software",
```

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/format.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/format.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/gen_meta.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/gen_meta.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/interfaces/data_table.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/interfaces/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/interfaces/metadata.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/interfaces/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from datetime import date
 from pathlib import Path
 import ruamel.yaml
 
 from pydantic import ValidationError
 from gwas_sumstats_tools.config import (GWAS_CAT_API_STUDIES_URL,
                                         GWAS_CAT_API_INGEST_STUDIES_URL,
+                                        GWAS_CAT_API_INGEST_STUDIES_URL_SANDBOX,
                                         GWAS_CAT_STUDY_MAPPINGS,
                                         REST_GWAS_CAT_STUDY_MAPPINGS,
                                         STUDY_FIELD_TO_SPLIT,
                                         SAMPLE_FIELD_TO_SPLIT,
                                         GWAS_CAT_SAMPLE_MAPPINGS,
                                         REST_GWAS_CAT_SAMPLE_MAPPINGS,
                                         GENOME_ASSEMBLY_MAPPINGS)
@@ -124,30 +125,36 @@
                 c[3] = []
             for com in after.split('\n'):
                 c[3].append(comment_token(com, start_mark))
     if not hasattr(ruamel.yaml.comments.CommentedMap,'yaml_set_comment_before_after_key'):
         ruamel.yaml.comments.CommentedMap.yaml_set_comment_before_after_key = yscbak
 
 def metadata_dict_from_gwas_cat(
-    accession_id: str, is_bypass_rest_api: bool = False
+    accession_id: str, 
+    is_bypass_rest_api: bool = False, 
+    is_sandbox: bool = False,
 ) -> dict:
     """Extract metadat from the GWAS Catalog API
 
     Arguments:
         accession_id(str): GWAS Catalog accession ID
         is_bypass_rest_api(bool, optional): A flag indicating whether the request comes from the sumstats
             service. If True, the function bypasses querying the REST API for additional study metadata.
             Defaults to False, which means the REST API response will be included in the metadata dict.
+        is_sandbox(bool, optional): A A flag indicating whether the request comes from the sandbox sumstats
+            service.
 
     Returns:
         Metadata dict
     """
     meta_dict = {}
     sample_list = []
     study_url = GWAS_CAT_API_INGEST_STUDIES_URL + accession_id
+    if is_sandbox:
+        study_url = GWAS_CAT_API_INGEST_STUDIES_URL_SANDBOX + accession_id
     sample_url = study_url + "/samples"
     rest_url = GWAS_CAT_API_STUDIES_URL + accession_id
 
     study_response = download_with_requests(url=study_url)
     sample_response = download_with_requests(url=sample_url, params={"size": 100})
 
     if not is_bypass_rest_api:
```

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/read.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/read.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/schema/data_table.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/schema/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/schema/metadata.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/utils.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/utils.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/gwas_sumstats_tools/validate.py` & `gwas_sumstats_tools-1.0.9/gwas_sumstats_tools/validate.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.8/pyproject.toml` & `gwas_sumstats_tools-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwas-sumstats-tools"
-version = "1.0.8"
+version = "1.0.9"
 description = ""
 authors = ["jdhayhurst <jhayhurst@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "gwas_sumstats_tools"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `gwas_sumstats_tools-1.0.8/PKG-INFO` & `gwas_sumstats_tools-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas-sumstats-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: jdhayhurst
 Author-email: jhayhurst@ebi.ac.uk
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

