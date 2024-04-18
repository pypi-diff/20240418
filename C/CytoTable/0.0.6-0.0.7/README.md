# Comparing `tmp/cytotable-0.0.6.tar.gz` & `tmp/cytotable-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytotable-0.0.6.tar", max compression
+gzip compressed data, was "cytotable-0.0.7.tar", max compression
```

## Comparing `cytotable-0.0.6.tar` & `cytotable-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1528 2024-03-16 20:01:26.206865 cytotable-0.0.6/LICENSE
--rw-r--r--   0        0        0      315 2024-03-16 20:01:49.138877 cytotable-0.0.6/cytotable/__init__.py
--rw-r--r--   0        0        0     1872 2024-03-16 20:01:26.206865 cytotable-0.0.6/cytotable/constants.py
--rw-r--r--   0        0        0    51590 2024-03-16 20:01:26.206865 cytotable-0.0.6/cytotable/convert.py
--rw-r--r--   0        0        0      482 2024-03-16 20:01:26.210865 cytotable-0.0.6/cytotable/exceptions.py
--rw-r--r--   0        0        0    10771 2024-03-16 20:01:26.210865 cytotable-0.0.6/cytotable/presets.py
--rw-r--r--   0        0        0    11283 2024-03-16 20:01:26.210865 cytotable-0.0.6/cytotable/sources.py
--rw-r--r--   0        0        0    14344 2024-03-16 20:01:26.210865 cytotable-0.0.6/cytotable/utils.py
--rw-r--r--   0        0        0     1672 2024-03-16 20:01:49.138877 cytotable-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2107 2024-03-16 20:01:26.214865 cytotable-0.0.6/readme.md
--rw-r--r--   0        0        0     3189 1970-01-01 00:00:00.000000 cytotable-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1528 2024-04-18 20:40:33.489007 cytotable-0.0.7/LICENSE
+-rw-r--r--   0        0        0      315 2024-04-18 20:40:56.509095 cytotable-0.0.7/cytotable/__init__.py
+-rw-r--r--   0        0        0     1872 2024-04-18 20:40:33.489007 cytotable-0.0.7/cytotable/constants.py
+-rw-r--r--   0        0        0    51771 2024-04-18 20:40:33.489007 cytotable-0.0.7/cytotable/convert.py
+-rw-r--r--   0        0        0      482 2024-04-18 20:40:33.489007 cytotable-0.0.7/cytotable/exceptions.py
+-rw-r--r--   0        0        0    10773 2024-04-18 20:40:33.489007 cytotable-0.0.7/cytotable/presets.py
+-rw-r--r--   0        0        0    11283 2024-04-18 20:40:33.489007 cytotable-0.0.7/cytotable/sources.py
+-rw-r--r--   0        0        0    14476 2024-04-18 20:40:33.489007 cytotable-0.0.7/cytotable/utils.py
+-rw-r--r--   0        0        0     1878 2024-04-18 20:40:56.505095 cytotable-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2107 2024-04-18 20:40:33.493007 cytotable-0.0.7/readme.md
+-rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 cytotable-0.0.7/PKG-INFO
```

### Comparing `cytotable-0.0.6/LICENSE` & `cytotable-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cytotable-0.0.6/cytotable/constants.py` & `cytotable-0.0.7/cytotable/constants.py`

 * *Files identical despite different names*

### Comparing `cytotable-0.0.6/cytotable/convert.py` & `cytotable-0.0.7/cytotable/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,16 @@
         # read data with chunk size + offset
         # and export to parquet
         with _duckdb_reader() as ddb_reader:
             _write_parquet_table_with_metadata(
                 table=ddb_reader.execute(
                     f"""
                     {base_query}
+                    /* order by all columns for deterministic output */
+                    ORDER BY ALL
                     LIMIT {chunk_size} OFFSET {offset}
                     """
                 ).arrow(),
                 where=result_filepath,
             )
     # Include exception handling to read mixed-type data
     # using sqlite3 and special utility function.
@@ -746,14 +748,15 @@
     # writing data to a parquet file.
     # read data with chunk size + offset
     # and export to parquet
     with _duckdb_reader() as ddb_reader:
         result = ddb_reader.execute(
             f"""
                 {joins}
+                {"ORDER BY ALL" if "ORDER BY" not in joins.upper() else ""}
                 LIMIT {chunk_size} OFFSET {offset}
                 """
         ).arrow()
 
     # drop nulls if specified
     if drop_null:
         result = result.drop_null()
```

### Comparing `cytotable-0.0.6/cytotable/presets.py` & `cytotable-0.0.7/cytotable/presets.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,23 @@
                     COLUMNS('^Metadata_ImageNumber$|^Image_Metadata_Well$|^Image_Metadata_Plate$')
                 FROM
                     read_parquet('image.parquet')
                 )
             SELECT
                 *
             FROM
-                Image_Filtered AS image
-            LEFT JOIN read_parquet('cytoplasm.parquet') AS cytoplasm ON
-                cytoplasm.Metadata_ImageNumber = image.Metadata_ImageNumber
+                read_parquet('cytoplasm.parquet') AS cytoplasm
             LEFT JOIN read_parquet('cells.parquet') AS cells ON
                 cells.Metadata_ImageNumber = cytoplasm.Metadata_ImageNumber
                 AND cells.Metadata_ObjectNumber = cytoplasm.Metadata_Cytoplasm_Parent_Cells
             LEFT JOIN read_parquet('nuclei.parquet') AS nuclei ON
                 nuclei.Metadata_ImageNumber = cytoplasm.Metadata_ImageNumber
                 AND nuclei.Metadata_ObjectNumber = cytoplasm.Metadata_Cytoplasm_Parent_Nuclei
+            LEFT JOIN Image_Filtered AS image ON
+                image.Metadata_ImageNumber = cytoplasm.Metadata_ImageNumber
             """,
     },
     "cellprofiler_sqlite": {
         # version specifications using related references
         "CONFIG_SOURCE_VERSION": {
             "cellprofiler": "v4.2.4",
         },
@@ -81,23 +81,23 @@
                     Image_Metadata_Plate
                 FROM
                     read_parquet('per_image.parquet')
                 )
             SELECT
                 *
             FROM
-                Per_Image_Filtered AS per_image
-            LEFT JOIN read_parquet('per_cytoplasm.parquet') AS per_cytoplasm ON
-                per_cytoplasm.Metadata_ImageNumber = per_image.Metadata_ImageNumber
+                read_parquet('per_cytoplasm.parquet') AS per_cytoplasm
             LEFT JOIN read_parquet('per_cells.parquet') AS per_cells ON
                 per_cells.Metadata_ImageNumber = per_cytoplasm.Metadata_ImageNumber
                 AND per_cells.Cells_Number_Object_Number = per_cytoplasm.Cytoplasm_Parent_Cells
             LEFT JOIN read_parquet('per_nuclei.parquet') AS per_nuclei ON
                 per_nuclei.Metadata_ImageNumber = per_cytoplasm.Metadata_ImageNumber
                 AND per_nuclei.Nuclei_Number_Object_Number = per_cytoplasm.Cytoplasm_Parent_Nuclei
+            LEFT JOIN  Per_Image_Filtered AS per_image ON
+                per_image.Metadata_ImageNumber = per_cytoplasm.Metadata_ImageNumber
             """,
     },
     "cellprofiler_sqlite_pycytominer": {
         # version specifications using related references
         "CONFIG_SOURCE_VERSION": {
             "cellprofiler": "v4.2.4",
             "pycytominer": "c90438fd7c11ad8b1689c21db16dab1a5280de6c",
@@ -132,23 +132,23 @@
                     Image_Metadata_Plate
                 FROM
                     read_parquet('per_image.parquet')
                 )
             SELECT
                 *
             FROM
-                Per_Image_Filtered AS per_image
-            LEFT JOIN read_parquet('per_cytoplasm.parquet') AS per_cytoplasm ON
-                per_cytoplasm.Metadata_ImageNumber = per_image.Metadata_ImageNumber
+                read_parquet('per_cytoplasm.parquet') AS per_cytoplasm
             LEFT JOIN read_parquet('per_cells.parquet') AS per_cells ON
                 per_cells.Metadata_ImageNumber = per_cytoplasm.Metadata_ImageNumber
                 AND per_cells.Metadata_Cells_Number_Object_Number = per_cytoplasm.Metadata_Cytoplasm_Parent_Cells
             LEFT JOIN read_parquet('per_nuclei.parquet') AS per_nuclei ON
                 per_nuclei.Metadata_ImageNumber = per_cytoplasm.Metadata_ImageNumber
                 AND per_nuclei.Metadata_Nuclei_Number_Object_Number = per_cytoplasm.Metadata_Cytoplasm_Parent_Nuclei
+            LEFT JOIN Per_Image_Filtered AS per_image ON
+                per_image.Metadata_ImageNumber = per_cytoplasm.Metadata_ImageNumber
             """,
     },
     "cell-health-cellprofiler-to-cytominer-database": {
         # version specifications using related references
         "CONFIG_SOURCE_VERSION": {
             "cell-health-dataset": "v5",
             "cellprofiler": "v2.X",
@@ -186,26 +186,26 @@
                     Image_Metadata_Plate
                 FROM
                     read_parquet('image.parquet')
                 )
             SELECT
                 *
             FROM
-                Image_Filtered AS image
-            LEFT JOIN read_parquet('cytoplasm.parquet') AS cytoplasm ON
-                cytoplasm.Metadata_TableNumber = image.Metadata_TableNumber
-                AND cytoplasm.Metadata_ImageNumber = image.Metadata_ImageNumber
+                read_parquet('cytoplasm.parquet') AS cytoplasm
             LEFT JOIN read_parquet('cells.parquet') AS cells ON
                 cells.Metadata_TableNumber = cytoplasm.Metadata_TableNumber
                 AND cells.Metadata_ImageNumber = cytoplasm.Metadata_ImageNumber
                 AND cells.Cells_ObjectNumber = cytoplasm.Metadata_Cytoplasm_Parent_Cells
             LEFT JOIN read_parquet('nuclei.parquet') AS nuclei ON
                 nuclei.Metadata_TableNumber = cytoplasm.Metadata_TableNumber
                 AND nuclei.Metadata_ImageNumber = cytoplasm.Metadata_ImageNumber
                 AND nuclei.Nuclei_ObjectNumber = cytoplasm.Metadata_Cytoplasm_Parent_Nuclei
+            LEFT JOIN  Image_Filtered AS image ON
+                image.Metadata_TableNumber = cytoplasm.Metadata_TableNumber
+                AND image.Metadata_ImageNumber = cytoplasm.Metadata_ImageNumber
         """,
     },
     "in-carta": {
         # version specifications using related references
         "CONFIG_SOURCE_VERSION": {
             "in-carta": "v1.17.0412545",
         },
```

### Comparing `cytotable-0.0.6/cytotable/sources.py` & `cytotable-0.0.7/cytotable/sources.py`

 * *Files identical despite different names*

### Comparing `cytotable-0.0.6/cytotable/utils.py` & `cytotable-0.0.7/cytotable/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,15 +253,20 @@
             END AS {col['column_name']}
             """
             for col in column_info
         ]
 
         # perform the select using the cases built above and using chunksize + offset
         cursor.execute(
-            f'SELECT {", ".join(query_parts)} FROM {table_name} LIMIT {chunk_size} OFFSET {offset};'
+            f"""
+            SELECT {', '.join(query_parts)}
+            FROM {table_name}
+            ORDER BY {', '.join([col['column_name'] for col in column_info])}
+            LIMIT {chunk_size} OFFSET {offset};
+            """
         )
         # collect the results and include the column name with values
         results = [
             dict(zip([desc[0] for desc in cursor.description], row))
             for row in cursor.fetchall()
         ]
```

### Comparing `cytotable-0.0.6/pyproject.toml` & `cytotable-0.0.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "CytoTable"
 # note: version data is maintained by poetry-dynamic-versioning (do not edit)
-version = "0.0.6"
+version = "0.0.7"
 description = "Transform CellProfiler and DeepProfiler data for processing image-based profiling readouts with Pycytominer and other Cytomining tools."
 authors = ["Cytomining Community"]
 license = "BSD-3-Clause License"
 packages = [{include = "cytotable"}]
 readme = "readme.md"
 repository = "https://github.com/cytomining/CytoTable"
 documentation = "https://cytomining.github.io/CytoTable/"
@@ -21,17 +21,25 @@
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.setuptools_scm]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 pyarrow = ">=13.0.0"
-cloudpathlib = {extras = ["all"], version = "^0.15.0"}
-duckdb = ">=0.8.0,<0.10.0"
+cloudpathlib = {extras = ["all"], version = "^0.18.0"}
+duckdb = ">=0.8.0,!=0.10.0,>=0.10.1"
 parsl = ">=2023.9.25"
+numpy = [
+  {version = "<=1.24.4", python = "<3.12"},
+  {version = ">=1.26.0", python = ">=3.12"}
+]
+scipy = [
+  {version = "<1.12.0", python = "<3.9"},
+  {version = "^1.12.0", python = ">=3.9"}
+]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
 Sphinx = "^6.0.0"
 myst-parser = "^2.0.0"
 sphinxcontrib-mermaid = "^0.9.0"
```

### Comparing `cytotable-0.0.6/readme.md` & `cytotable-0.0.7/readme.md`

 * *Files identical despite different names*

### Comparing `cytotable-0.0.6/PKG-INFO` & `cytotable-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: CytoTable
-Version: 0.0.6
+Version: 0.0.7
 Summary: Transform CellProfiler and DeepProfiler data for processing image-based profiling readouts with Pycytominer and other Cytomining tools.
 Home-page: https://github.com/cytomining/CytoTable
 License: BSD-3-Clause License
 Keywords: python,cellprofiler,single-cell-analysis,way-lab
 Author: Cytomining Community
 Requires-Python: >=3.8,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cloudpathlib[all] (>=0.15.0,<0.16.0)
-Requires-Dist: duckdb (>=0.8.0,<0.10.0)
+Requires-Dist: cloudpathlib[all] (>=0.18.0,<0.19.0)
+Requires-Dist: duckdb (>=0.10.1)
+Requires-Dist: numpy (<=1.24.4) ; python_version < "3.12"
+Requires-Dist: numpy (>=1.26.0) ; python_version >= "3.12"
 Requires-Dist: parsl (>=2023.9.25)
 Requires-Dist: pyarrow (>=13.0.0)
+Requires-Dist: scipy (<1.12.0) ; python_version < "3.9"
+Requires-Dist: scipy (>=1.12.0,<2.0.0) ; python_version >= "3.9"
 Project-URL: Documentation, https://cytomining.github.io/CytoTable/
 Project-URL: Repository, https://github.com/cytomining/CytoTable
 Description-Content-Type: text/markdown
 
 <img height="200" src="https://raw.githubusercontent.com/cytomining/cytotable/main/logo/with-text-for-light-bg.png?raw=true">
 
 # CytoTable
```

