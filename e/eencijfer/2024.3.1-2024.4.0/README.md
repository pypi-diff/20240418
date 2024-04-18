# Comparing `tmp/eencijfer-2024.3.1.tar.gz` & `tmp/eencijfer-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eencijfer-2024.3.1.tar", max compression
+gzip compressed data, was "eencijfer-2024.4.0.tar", max compression
```

## Comparing `eencijfer-2024.3.1.tar` & `eencijfer-2024.4.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0     1069 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/LICENSE
--rw-r--r--   0        0        0      925 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/README.md
--rw-r--r--   0        0        0     1807 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/__init__.py
--rw-r--r--   0        0        0       43 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/__init__.py
--rw-r--r--   0        0        0    11868 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/cohorten.py
--rw-r--r--   0        0        0     1891 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/eencijfer.py
--rw-r--r--   0        0        0     3174 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/eindexamencijfers.py
--rw-r--r--   0        0        0        0 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/__init__py
--rw-r--r--   0        0        0     2159 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
--rw-r--r--   0        0        0     1639 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/diploma.py
--rw-r--r--   0        0        0       53 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/local_data.py
--rw-r--r--   0        0        0     7712 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/opleiding.py
--rw-r--r--   0        0        0     1455 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/postcodes.py
--rw-r--r--   0        0        0     1756 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/prestatieafspraken.py
--rw-r--r--   0        0        0     7437 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/assets/transformations/vooropleiding.py
--rw-r--r--   0        0        0     4433 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/cli.py
--rw-r--r--   0        0        0       61 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/__init__.py
--rw-r--r--   0        0        0     2712 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/column_converters.py
--rw-r--r--   0        0        0    10854 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/eencijfer.py
--rw-r--r--   0        0        0      710 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Croho.csv
--rw-r--r--   0        0        0      716 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Croho_vest.csv
--rw-r--r--   0        0        0      136 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
--rw-r--r--   0        0        0      349 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_brinnummer.csv
--rw-r--r--   0        0        0      527 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
--rw-r--r--   0        0        0      128 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_ho-inst.csv
--rw-r--r--   0        0        0      284 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
--rw-r--r--   0        0        0      126 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_isat.csv
--rw-r--r--   0        0        0      213 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
--rw-r--r--   0        0        0      264 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_landcode.csv
--rw-r--r--   0        0        0      282 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
--rw-r--r--   0        0        0      191 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
--rw-r--r--   0        0        0      191 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
--rw-r--r--   0        0        0      249 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_vakcode.csv
--rw-r--r--   0        0        0      237 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
--rw-r--r--   0        0        0      237 2024-04-16 18:12:42.336346 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
--rw-r--r--   0        0        0      213 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_vooropl.csv
--rw-r--r--   0        0        0      140 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_vopl.csv
--rw-r--r--   0        0        0     6244 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/convert/import_definitions/EV____24.csv
--rw-r--r--   0        0        0     1058 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/convert/import_definitions/VAKHAVW_____.csv
--rw-r--r--   0        0        0     6596 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/convert/pii.py
--rw-r--r--   0        0        0       28 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/io/__init__.py
--rw-r--r--   0        0        0     3893 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/io/files.py
--rw-r--r--   0        0        0     2049 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/settings.py
--rw-r--r--   0        0        0       33 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/utils/__init__.py
--rw-r--r--   0        0        0     4054 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/utils/detect_eencijfer_files.py
--rw-r--r--   0        0        0     2624 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/utils/init.py
--rw-r--r--   0        0        0      991 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/utils/local_data.py
--rw-r--r--   0        0        0     1944 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/eencijfer/utils/qa.py
--rw-r--r--   0        0        0     2505 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/tests/__init__.py
--rw-r--r--   0        0        0      450 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/tests/test_cli.py
--rw-r--r--   0        0        0      541 2024-04-16 18:12:42.340345 eencijfer-2024.3.1/tests/test_eencijfer.py
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 eencijfer-2024.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/LICENSE
+-rw-r--r--   0        0        0      925 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/README.md
+-rw-r--r--   0        0        0     1808 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/__init__.py
+-rw-r--r--   0        0        0    11868 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/cohorten.py
+-rw-r--r--   0        0        0     1891 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/eencijfer.py
+-rw-r--r--   0        0        0     3174 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/eindexamencijfers.py
+-rw-r--r--   0        0        0        0 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/__init__py
+-rw-r--r--   0        0        0     2159 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv
+-rw-r--r--   0        0        0     1639 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/diploma.py
+-rw-r--r--   0        0        0       53 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/local_data.py
+-rw-r--r--   0        0        0     7712 2024-04-18 19:42:47.078748 eencijfer-2024.4.0/eencijfer/assets/transformations/opleiding.py
+-rw-r--r--   0        0        0     1455 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/assets/transformations/postcodes.py
+-rw-r--r--   0        0        0     1756 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/assets/transformations/prestatieafspraken.py
+-rw-r--r--   0        0        0     7437 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/assets/transformations/vooropleiding.py
+-rw-r--r--   0        0        0     5221 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/cli.py
+-rw-r--r--   0        0        0       61 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/__init__.py
+-rw-r--r--   0        0        0     2712 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/column_converters.py
+-rw-r--r--   0        0        0    10854 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/eencijfer.py
+-rw-r--r--   0        0        0      710 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho.csv
+-rw-r--r--   0        0        0      716 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho_vest.csv
+-rw-r--r--   0        0        0      136 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_actuele_instelling.csv
+-rw-r--r--   0        0        0      349 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_brinnummer.csv
+-rw-r--r--   0        0        0      527 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv
+-rw-r--r--   0        0        0      128 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_ho-inst.csv
+-rw-r--r--   0        0        0      284 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_ho_ISCED.csv
+-rw-r--r--   0        0        0      126 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_isat.csv
+-rw-r--r--   0        0        0      213 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_land_naar_herkomstindikking.csv
+-rw-r--r--   0        0        0      264 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_landcode.csv
+-rw-r--r--   0        0        0      282 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_nationaliteitscode.csv
+-rw-r--r--   0        0        0      191 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_postcodecijfers_2023.csv
+-rw-r--r--   0        0        0      191 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_postcodecijfers_2024.csv
+-rw-r--r--   0        0        0      249 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vakcode.csv
+-rw-r--r--   0        0        0      237 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vestnr_ho.csv
+-rw-r--r--   0        0        0      237 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vestnr_ho_compleet.csv
+-rw-r--r--   0        0        0      213 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vooropl.csv
+-rw-r--r--   0        0        0      140 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_vopl.csv
+-rw-r--r--   0        0        0     6244 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/EV____24.csv
+-rw-r--r--   0        0        0     1058 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/import_definitions/VAKHAVW_____.csv
+-rw-r--r--   0        0        0     6596 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/convert/pii.py
+-rw-r--r--   0        0        0       28 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/io/__init__.py
+-rw-r--r--   0        0        0     2777 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/io/db.py
+-rw-r--r--   0        0        0     3915 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/io/files.py
+-rw-r--r--   0        0        0     2232 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/settings.py
+-rw-r--r--   0        0        0       33 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/__init__.py
+-rw-r--r--   0        0        0     4054 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/detect_eencijfer_files.py
+-rw-r--r--   0        0        0     2624 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/init.py
+-rw-r--r--   0        0        0      991 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/local_data.py
+-rw-r--r--   0        0        0     1944 2024-04-18 19:42:47.082748 eencijfer-2024.4.0/eencijfer/utils/qa.py
+-rw-r--r--   0        0        0     2525 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      450 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0      541 2024-04-18 19:42:47.086748 eencijfer-2024.4.0/tests/test_eencijfer.py
+-rw-r--r--   0        0        0     1873 1970-01-01 00:00:00.000000 eencijfer-2024.4.0/PKG-INFO
```

### Comparing `eencijfer-2024.3.1/LICENSE` & `eencijfer-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/README.md` & `eencijfer-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/__init__.py` & `eencijfer-2024.4.0/eencijfer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for eencijfer."""
 
 __author__ = """Bram Enning"""
 __email__ = 'bramenning@gmail.com'
-__version__ = '2024.3.1'
+__version__ = '2024.4.0'
 __app_name__ = 'eencijfer'
 
 import logging
 import shutil
 from importlib import import_module
 from pathlib import Path
 
@@ -58,8 +58,8 @@
 
 # import module so all column-converter-decorators are activated
 import_module("eencijfer.convert.column_converters")
 
 
 FORMAT = "[%(filename)s:%(lineno)s - %(funcName)20s() ] %(message)s"
 
-logging.basicConfig(format=FORMAT, level=logging.INFO)
+logging.basicConfig(format=FORMAT, level=logging.DEBUG)
```

### Comparing `eencijfer-2024.3.1/eencijfer/assets/cohorten.py` & `eencijfer-2024.4.0/eencijfer/assets/cohorten.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/eencijfer.py` & `eencijfer-2024.4.0/eencijfer/assets/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/eindexamencijfers.py` & `eencijfer-2024.4.0/eencijfer/assets/eindexamencijfers.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv` & `eencijfer-2024.4.0/eencijfer/assets/transformations/datasets/21RI/croho_naam_opleiding_faculteit.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/transformations/diploma.py` & `eencijfer-2024.4.0/eencijfer/assets/transformations/diploma.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/transformations/opleiding.py` & `eencijfer-2024.4.0/eencijfer/assets/transformations/opleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/transformations/postcodes.py` & `eencijfer-2024.4.0/eencijfer/assets/transformations/postcodes.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/transformations/prestatieafspraken.py` & `eencijfer-2024.4.0/eencijfer/assets/transformations/prestatieafspraken.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/assets/transformations/vooropleiding.py` & `eencijfer-2024.4.0/eencijfer/assets/transformations/vooropleiding.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/cli.py` & `eencijfer-2024.4.0/eencijfer/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 
 from eencijfer import APP_NAME, CONFIG_FILE, __version__
 from eencijfer.assets.cohorten import create_cohorten_met_indicatoren
 from eencijfer.assets.eencijfer import _create_eencijfer_df
 from eencijfer.assets.eindexamencijfers import _create_eindexamencijfer_df
 from eencijfer.convert.eencijfer import _convert_to_parquet
 from eencijfer.convert.pii import _replace_all_pgn_with_pseudo_id_remove_pii_local_id
+from eencijfer.io.db import _create_duckdb
 from eencijfer.io.files import ExportFormat, _convert_to_export_format, _save_to_file
 from eencijfer.settings import config
+from eencijfer.utils.detect_eencijfer_files import _get_eencijfer_datafile
 from eencijfer.utils.init import _create_default_config
 from eencijfer.utils.qa import compare_eencijfer_files_and_definitions
 
 logger = logging.getLogger(__name__)
 
 app = typer.Typer(name="eencijfer", help="ETL-tool for Dutch eencijfer", no_args_is_help=True)
 
@@ -64,45 +66,57 @@
 def init():
     """Initializes eencijfer-package."""
     _create_default_config(CONFIG_FILE)
 
 
 @app.command()
 def convert(
-    export_format: ExportFormat = ExportFormat.parquet,
+    source_dir: Annotated[Optional[Path], typer.Option(help="Directory containing eencijfer source files.")] = None,
+    result_dir: Annotated[Optional[Path], typer.Option(help="Directory where results are stored.")] = None,
+    export_format: Annotated[ExportFormat, typer.Option(help="File format of results.")] = ExportFormat.parquet,
+    # export_format: ExportFormat = ,
     use_column_converters: Annotated[bool, typer.Option("--use-column-converters/--not-use-column-converters", "-c/-C")] = True,
     remove_pii: Annotated[bool, typer.Option("--remove-pii/--do-not-remove-pii", "-p/-P")] = True,
     add_local_id: Annotated[bool, typer.Option("--add-local-id/--do-not-add-local-id", "-s/-S")] = False,
 ):
     """Convert eencijfer-files to desired exportformat, with or without PII."""
 
-    source_dir = config.getpath('default', 'source_dir')
+    if source_dir is None:
+        source_dir = config.getpath('default', 'source_dir')
 
-    result_dir = config.getpath('default', 'result_dir')
+    if result_dir is None:
+        result_dir = config.getpath('default', 'result_dir')
 
     working_dir = result_dir / '.temp_dir'
 
+    db_name = config.getpath('default', 'db_name')
+
     if not result_dir.is_dir():
         Path(result_dir).mkdir(parents=True, exist_ok=True)
 
     if not working_dir.is_dir():
         Path(working_dir).mkdir(parents=True, exist_ok=True)
 
     _convert_to_parquet(
         source_dir=source_dir,
         result_dir=working_dir,
         export_format=ExportFormat.parquet,
         use_column_converters=use_column_converters,
     )
 
-    _replace_all_pgn_with_pseudo_id_remove_pii_local_id(
-        eencijfer_dir=working_dir, remove_pii=remove_pii, add_local_id=add_local_id
-    )
-
-    _convert_to_export_format(source_dir=working_dir, result_dir=result_dir, export_format=export_format)
+    eencijfer_fname = _get_eencijfer_datafile(working_dir)
+    if eencijfer_fname:
+        _replace_all_pgn_with_pseudo_id_remove_pii_local_id(
+            eencijfer_dir=working_dir, remove_pii=remove_pii, add_local_id=add_local_id
+        )
+
+    if export_format.value == 'duckdb':
+        _create_duckdb(source_dir=working_dir, result_dir=result_dir, db_name=db_name)
+    else:
+        _convert_to_export_format(source_dir=working_dir, result_dir=result_dir, export_format=export_format)
 
     logger.debug(f'Removing working dir {working_dir}')
     shutil.rmtree(working_dir)
 
 
 @app.command()
 def qa():
```

### Comparing `eencijfer-2024.3.1/eencijfer/convert/column_converters.py` & `eencijfer-2024.4.0/eencijfer/convert/column_converters.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/eencijfer.py` & `eencijfer-2024.4.0/eencijfer/convert/eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/import_definitions/Croho.csv` & `eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/import_definitions/Croho_vest.csv` & `eencijfer-2024.4.0/eencijfer/convert/import_definitions/Croho_vest.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv` & `eencijfer-2024.4.0/eencijfer/convert/import_definitions/Dec_brinvestigingsnummer.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/import_definitions/EV____24.csv` & `eencijfer-2024.4.0/eencijfer/convert/import_definitions/EV____24.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/import_definitions/VAKHAVW_____.csv` & `eencijfer-2024.4.0/eencijfer/convert/import_definitions/VAKHAVW_____.csv`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/convert/pii.py` & `eencijfer-2024.4.0/eencijfer/convert/pii.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/io/files.py` & `eencijfer-2024.4.0/eencijfer/io/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         str (_type_): _description_
         Enum (_type_): _description_
     """
 
     csv = "csv"
     parquet = "parquet"
     xlsx = "xlsx"
+    duckdb = "duckdb"
 
 
 def _save_to_file(
     df: pd.DataFrame,
     dir: Path,
     fname: str,
     export_format: ExportFormat = ExportFormat.parquet,
```

### Comparing `eencijfer-2024.3.1/eencijfer/settings.py` & `eencijfer-2024.4.0/eencijfer/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 
 logger = logging.getLogger(__name__)
 
 default_source_dir = Path().absolute()
 default_assets_dir = Path().absolute() / "assets"
 default_result_dir = Path().absolute() / "result"
 default_import_definitions_dir = PACKAGE_PROVIDED_IMPORT_DEFINTIONS_DIR
+default_db_name = 'eencijfer.duckdb'
 
 
 def _get_config(
     CONFIG_FILE: Path,
     source_dir: Path = default_source_dir,
     result_dir: Path = default_result_dir,
     assets_dir: Path = default_assets_dir,
+    db_name: str = default_db_name,
     import_definitions_dir: Path = default_import_definitions_dir,
     use_column_converter: bool = False,
     remove_pii: bool = True,
 ) -> configparser.ConfigParser:
     config = configparser.ConfigParser(converters={"path": lambda x: Path(x), "list": lambda x: x.split(',')})
 
     try:
@@ -32,14 +34,16 @@
             config.add_section('default')
         if not config.has_option('default', 'source_dir'):
             config.set('default', 'source_dir', source_dir.as_posix())
         if not config.has_option('default', 'result_dir'):
             config.set('default', 'result_dir', result_dir.as_posix())
         if not config.has_option('default', 'assets_dir'):
             config.set('default', 'assets_dir', assets_dir.as_posix())
+        if not config.has_option('default', 'db_name'):
+            config.set('default', 'db_name', db_name)
         if not config.has_option('default', 'import_definitions_dir'):
             config.set('default', 'import_definitions_dir', import_definitions_dir.as_posix())
         if not config.has_option('default', 'use_column_converter'):
             config.set('default', 'use_column_converter', str(use_column_converter))
         if not config.has_option('default', 'remove_pii'):
             config.set('default', 'remove_pii', str(remove_pii))
```

### Comparing `eencijfer-2024.3.1/eencijfer/utils/detect_eencijfer_files.py` & `eencijfer-2024.4.0/eencijfer/utils/detect_eencijfer_files.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/utils/init.py` & `eencijfer-2024.4.0/eencijfer/utils/init.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/utils/local_data.py` & `eencijfer-2024.4.0/eencijfer/utils/local_data.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/eencijfer/utils/qa.py` & `eencijfer-2024.4.0/eencijfer/utils/qa.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/pyproject.toml` & `eencijfer-2024.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "eencijfer"
-version = "2024.3.1"
+version = "2024.4.0"
 homepage = "https://github.com/enningb/eencijfer"
 description = "ETL-tool for Dutch eencijfer."
 authors = ["Bram Enning <bramenning@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -24,14 +24,15 @@
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 pandas =">=2.0.0"
 numpy = ">=1.26.1"
 pyarrow= "^15.0.0"
 case-converter = ">=1.1.0"
+duckdb = "^0.10.1"
 
 [tool.poetry.dev-dependencies]
 black = "^23.12.1"
 isort = "^5.13.2"
 flake8 = "^6.1.0"
 flake8-docstrings = "^1.7.0"
 mypy = "^1.8.0"
@@ -86,15 +87,15 @@
 #skip_glob = docs/conf.py
 
 
 [tool.mypy]
 disable_error_code = ["attr-defined"]
 
 [tool.bumpversion]
-current_version = "2024.3.1"
+current_version = "2024.4.0"
 commit = true
 commit_args = "--no-verify"
 tag = true
 tag_name = "{new_version}"
 allow_dirty = true
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<dev>post)\\d+\\.dev\\d+)?"
 message = "Version updated from {current_version} to {new_version}"
@@ -110,14 +111,15 @@
 
 
 
 
 
 
 
+
 
 
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eencijfer-2024.3.1/tests/test_eencijfer.py` & `eencijfer-2024.4.0/tests/test_eencijfer.py`

 * *Files identical despite different names*

### Comparing `eencijfer-2024.3.1/PKG-INFO` & `eencijfer-2024.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eencijfer
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: ETL-tool for Dutch eencijfer.
 Home-page: https://github.com/enningb/eencijfer
 License: MIT
 Author: Bram Enning
 Author-email: bramenning@gmail.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: case-converter (>=1.1.0)
+Requires-Dist: duckdb (>=0.10.1,<0.11.0)
 Requires-Dist: numpy (>=1.26.1)
 Requires-Dist: pandas (>=2.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # eencijfer
```

