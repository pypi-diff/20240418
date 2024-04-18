# Comparing `tmp/phc-ingestion-0.8.2.tar.gz` & `tmp/phc-ingestion-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.8.2.tar", last modified: Thu Apr 11 21:19:02 2024, max compression
+gzip compressed data, was "phc-ingestion-0.8.3.tar", last modified: Thu Apr 18 09:25:14 2024, max compression
```

## Comparing `phc-ingestion-0.8.2.tar` & `phc-ingestion-0.8.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0       16 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/PYPI.md
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4441 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      507 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      770 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0    12312 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/ihc.py
--rw-r--r--   0        0        0      555 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4706 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/json.py
--rw-r--r--   0        0        0     9536 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     2051 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/specimen_details.py
--rw-r--r--   0        0        0     4599 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0      372 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tests.py
--rw-r--r--   0        0        0     1027 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tmb.py
--rw-r--r--   0        0        0     1595 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3440 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/process.py
--rw-r--r--   0        0        0      297 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     2284 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8522 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5451 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7341 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0     2047 2024-04-11 21:18:40.388471 phc-ingestion-0.8.2/ingestion/nextgen/util/variant_table.py
--rw-r--r--   0        0        0   408290 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0       68 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1010 2024-04-11 21:18:40.392471 phc-ingestion-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/PYPI.md
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1257 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4441 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      507 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      770 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0    12312 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/ihc.py
+-rw-r--r--   0        0        0      555 2024-04-18 09:24:50.890956 phc-ingestion-0.8.3/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4706 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0     9536 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     2051 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/specimen_details.py
+-rw-r--r--   0        0        0     4599 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0      372 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/tests.py
+-rw-r--r--   0        0        0     1027 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/tmb.py
+-rw-r--r--   0        0        0     1595 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3440 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0      297 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     2284 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8522 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5562 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7341 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0     2047 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/nextgen/util/variant_table.py
+-rw-r--r--   0        0        0   408290 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0      162 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/shared_util/open_maybe_gzipped.py
+-rw-r--r--   0        0        0       68 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.894956 phc-ingestion-0.8.3/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-04-18 09:24:50.898956 phc-ingestion-0.8.3/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-04-18 09:24:50.898956 phc-ingestion-0.8.3/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-18 09:24:50.898956 phc-ingestion-0.8.3/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-04-18 09:24:50.898956 phc-ingestion-0.8.3/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-04-18 09:24:50.898956 phc-ingestion-0.8.3/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1010 2024-04-18 09:24:50.898956 phc-ingestion-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.3/PKG-INFO
```

### Comparing `phc-ingestion-0.8.2/ingestion/caris/process.py` & `phc-ingestion-0.8.3/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/cnv.py` & `phc-ingestion-0.8.3/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.8.3/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/hla.py` & `phc-ingestion-0.8.3/ingestion/caris/util/hla.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/ihc.py` & `phc-ingestion-0.8.3/ingestion/caris/util/ihc.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.8.3/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/json.py` & `phc-ingestion-0.8.3/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/metadata.py` & `phc-ingestion-0.8.3/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/specimen_details.py` & `phc-ingestion-0.8.3/ingestion/caris/util/specimen_details.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/structural.py` & `phc-ingestion-0.8.3/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/tmb.py` & `phc-ingestion-0.8.3/ingestion/caris/util/tmb.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/tsv.py` & `phc-ingestion-0.8.3/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/caris/util/vcf.py` & `phc-ingestion-0.8.3/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/foundation/process.py` & `phc-ingestion-0.8.3/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.8.3/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.8.3/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.8.3/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.8.3/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/generic/process.py` & `phc-ingestion-0.8.3/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/generic/utils.py` & `phc-ingestion-0.8.3/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/nextgen/process.py` & `phc-ingestion-0.8.3/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.8.3/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.8.3/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.8.3/ingestion/nextgen/util/process_structural.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pandas as pd
 from logging import Logger
 from typing import TypedDict
 
 from ingestion.shared_util.coords_to_genes import coords_to_genes
 from ingestion.nextgen.util.variant_table import extract_variant_table
 from ingestion.nextgen.util.interpretation import map_interpretation
+from ingestion.shared_util.open_maybe_gzipped import open_maybe_gzipped
 
 
 class StructuralVariant(TypedDict):
     sample_id: str
     gene1: str
     gene2: str
     effect: str
-    position_one: tuple[str, str, str]
-    position_two: tuple[str, str, str]
+    position1: tuple[str, str, str]
+    position2: tuple[str, str, str]
     interpretation: str
     sequence_type: str
     in_frame: str
     attributes: dict
 
 
 def structural_variant_to_csv_row(structural_variant: StructuralVariant) -> str:
@@ -41,15 +42,15 @@
     structural_variant_table = extract_variant_table(
         xml_in_file=xml_in_file, variant_type="structural", log=log
     )
 
     structural_variant_path_name = f"{root_path}/{prefix}.structural.csv"
     sample_id = prefix
 
-    with open(sv_in_file, "r") as f:
+    with open_maybe_gzipped(sv_in_file, "r") as f:
         variants = [line for line in f.readlines() if not line.startswith("#")]
 
     if not variants:
         log.info(f"No structural variants found in {sv_in_file}")
         structural_status = False
         return None, structural_status
 
@@ -102,15 +103,15 @@
 
                 if ref_coords == variant_coords:
                     interpretation = map_interpretation(row["info"], log)
 
         # Hard-code
         sequence_type = "Somatic"
         in_frame = "Unknown"
-        attributes = {}
+        attributes: dict = {}
 
         structural_variants.append(
             {
                 "sample_id": sample_id,
                 "gene1": gene1,
                 "gene2": gene2,
                 "effect": effect,
@@ -120,15 +121,15 @@
                 "sequence_type": sequence_type,
                 "in_frame": in_frame,
                 "attributes": attributes,
             }
         )
 
     # Dedupe structural variants based on chromosome and positions
-    deduped_structural_variants = []
+    deduped_structural_variants: list[StructuralVariant] = []
     for sv in structural_variants:
         maybe_matching_variant = next(
             (
                 variant
                 for variant in deduped_structural_variants
                 if are_variants_duplicates(sv, variant)
             ),
```

### Comparing `phc-ingestion-0.8.2/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.8.3/ingestion/nextgen/util/process_vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/nextgen/util/variant_table.py` & `phc-ingestion-0.8.3/ingestion/nextgen/util/variant_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.8.3/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.8.3/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.8.3/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.8.3/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.8.3/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.8.3/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.8.3/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.8.3/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.8.3/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.2/pyproject.toml` & `phc-ingestion-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.8.2"
+version = "0.8.3"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

