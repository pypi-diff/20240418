# Comparing `tmp/bblocks-1.3.0.tar.gz` & `tmp/bblocks-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblocks-1.3.0.tar", max compression
+gzip compressed data, was "bblocks-1.3.1.tar", max compression
```

## Comparing `bblocks-1.3.0.tar` & `bblocks-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1074 2024-04-09 11:05:37.224790 bblocks-1.3.0/LICENSE
--rw-r--r--   0        0        0    17113 2024-04-09 11:05:37.224790 bblocks-1.3.0/README.md
--rw-r--r--   0        0        0      138 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/.raw_data/README.md
--rw-r--r--   0        0        0     1223 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/analysis_tools/__init__.py
--rw-r--r--   0        0        0     4393 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/analysis_tools/get.py
--rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/cleaning_tools/__init__.py
--rw-r--r--   0        0        0     9126 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/cleaning_tools/clean.py
--rw-r--r--   0        0        0     5259 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/cleaning_tools/filter.py
--rw-r--r--   0        0        0      573 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/config.py
--rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/dataframe_tools/__init__.py
--rw-r--r--   0        0        0    25549 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/dataframe_tools/add.py
--rw-r--r--   0        0        0     3613 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/dataframe_tools/common.py
--rw-r--r--   0        0        0        0 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/__init__.py
--rw-r--r--   0        0        0     3359 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/common.py
--rw-r--r--   0        0        0      140 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/__init__.py
--rw-r--r--   0        0        0     2584 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/common.py
--rw-r--r--   0        0        0     3299 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/get_data.py
--rw-r--r--   0        0        0     1116 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_service_indicators.json
--rw-r--r--   0        0        0      541 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_stocks_indicators.json
--rw-r--r--   0        0        0   306280 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/settings/ids_indicators.json
--rw-r--r--   0        0        0     9462 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/debt/wb_ids.py
--rw-r--r--   0        0        0     1800 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/fao.py
--rw-r--r--   0        0        0     8253 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/hdr.py
--rw-r--r--   0        0        0     8322 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/ilo.py
--rw-r--r--   0        0        0     7347 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/imf.py
--rw-r--r--   0        0        0    12893 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/imf_weo.py
--rw-r--r--   0        0        0     9036 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/sdr.py
--rw-r--r--   0        0        0     4200 2024-04-09 11:05:37.224790 bblocks-1.3.0/bblocks/import_tools/settings/aids_indicators.json
--rw-r--r--   0        0        0  2744667 2024-04-09 11:05:37.236790 bblocks-1.3.0/bblocks/import_tools/settings/flourish_geometries.csv
--rw-r--r--   0        0        0     6288 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/settings/ids_codes.csv
--rw-r--r--   0        0        0      450 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/settings/oecd_codes.csv
--rw-r--r--   0        0        0     9495 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/unaids.py
--rw-r--r--   0        0        0     6793 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/wfp.py
--rw-r--r--   0        0        0     4675 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/who.py
--rw-r--r--   0        0        0     9952 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/import_tools/world_bank.py
--rw-r--r--   0        0        0      571 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/logger.py
--rw-r--r--   0        0        0        0 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/other_tools/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/other_tools/common.py
--rw-r--r--   0        0        0     3950 2024-04-09 11:05:37.240790 bblocks-1.3.0/bblocks/other_tools/dictionaries.py
--rw-r--r--   0        0        0     1195 2024-04-09 11:05:37.240790 bblocks-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    18331 1970-01-01 00:00:00.000000 bblocks-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-18 06:45:26.800626 bblocks-1.3.1/LICENSE
+-rw-r--r--   0        0        0    17113 2024-04-18 06:45:26.800626 bblocks-1.3.1/README.md
+-rw-r--r--   0        0        0      138 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/.raw_data/README.md
+-rw-r--r--   0        0        0     1223 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/analysis_tools/__init__.py
+-rw-r--r--   0        0        0     4393 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/analysis_tools/get.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/cleaning_tools/__init__.py
+-rw-r--r--   0        0        0     9126 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/cleaning_tools/clean.py
+-rw-r--r--   0        0        0     5259 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/cleaning_tools/filter.py
+-rw-r--r--   0        0        0      573 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/config.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/dataframe_tools/__init__.py
+-rw-r--r--   0        0        0    25549 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/dataframe_tools/add.py
+-rw-r--r--   0        0        0     3613 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/dataframe_tools/common.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/__init__.py
+-rw-r--r--   0        0        0     3359 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/common.py
+-rw-r--r--   0        0        0      140 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/__init__.py
+-rw-r--r--   0        0        0     2584 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/common.py
+-rw-r--r--   0        0        0     3299 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/get_data.py
+-rw-r--r--   0        0        0     1116 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/settings/debt_service_indicators.json
+-rw-r--r--   0        0        0      541 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/settings/debt_stocks_indicators.json
+-rw-r--r--   0        0        0   306280 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/settings/ids_indicators.json
+-rw-r--r--   0        0        0     9462 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/debt/wb_ids.py
+-rw-r--r--   0        0        0     1800 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/fao.py
+-rw-r--r--   0        0        0     8253 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/hdr.py
+-rw-r--r--   0        0        0     8322 2024-04-18 06:45:26.800626 bblocks-1.3.1/bblocks/import_tools/ilo.py
+-rw-r--r--   0        0        0     5578 2024-04-18 06:45:26.804626 bblocks-1.3.1/bblocks/import_tools/imf.py
+-rw-r--r--   0        0        0    14308 2024-04-18 06:45:26.804626 bblocks-1.3.1/bblocks/import_tools/imf_weo.py
+-rw-r--r--   0        0        0     9036 2024-04-18 06:45:26.804626 bblocks-1.3.1/bblocks/import_tools/sdr.py
+-rw-r--r--   0        0        0     4200 2024-04-18 06:45:26.804626 bblocks-1.3.1/bblocks/import_tools/settings/aids_indicators.json
+-rw-r--r--   0        0        0  2744667 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/settings/flourish_geometries.csv
+-rw-r--r--   0        0        0     6288 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/settings/ids_codes.csv
+-rw-r--r--   0        0        0      450 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/settings/oecd_codes.csv
+-rw-r--r--   0        0        0     9495 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/unaids.py
+-rw-r--r--   0        0        0     6793 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/wfp.py
+-rw-r--r--   0        0        0     4675 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/who.py
+-rw-r--r--   0        0        0     9952 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/import_tools/world_bank.py
+-rw-r--r--   0        0        0      571 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/logger.py
+-rw-r--r--   0        0        0        0 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/other_tools/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/other_tools/common.py
+-rw-r--r--   0        0        0     3950 2024-04-18 06:45:26.816626 bblocks-1.3.1/bblocks/other_tools/dictionaries.py
+-rw-r--r--   0        0        0     1180 2024-04-18 06:45:26.816626 bblocks-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0    18295 1970-01-01 00:00:00.000000 bblocks-1.3.1/PKG-INFO
```

### Comparing `bblocks-1.3.0/LICENSE` & `bblocks-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/README.md` & `bblocks-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/__init__.py` & `bblocks-1.3.1/bblocks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 
 # Easy access to importers
 from bblocks.import_tools.world_bank import WorldBankData
 from bblocks.import_tools.who import GHED
 from bblocks.import_tools.wfp import WFPData
 from bblocks.import_tools.imf import WorldEconomicOutlook
 from bblocks.import_tools.unaids import Aids
```

### Comparing `bblocks-1.3.0/bblocks/analysis_tools/get.py` & `bblocks-1.3.1/bblocks/analysis_tools/get.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/cleaning_tools/clean.py` & `bblocks-1.3.1/bblocks/cleaning_tools/clean.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/cleaning_tools/filter.py` & `bblocks-1.3.1/bblocks/cleaning_tools/filter.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/config.py` & `bblocks-1.3.1/bblocks/config.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/dataframe_tools/add.py` & `bblocks-1.3.1/bblocks/dataframe_tools/add.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/dataframe_tools/common.py` & `bblocks-1.3.1/bblocks/dataframe_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/common.py` & `bblocks-1.3.1/bblocks/import_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/debt/common.py` & `bblocks-1.3.1/bblocks/import_tools/debt/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/debt/get_data.py` & `bblocks-1.3.1/bblocks/import_tools/debt/get_data.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_service_indicators.json` & `bblocks-1.3.1/bblocks/import_tools/debt/settings/debt_service_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/debt/settings/debt_stocks_indicators.json` & `bblocks-1.3.1/bblocks/import_tools/debt/settings/debt_stocks_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/debt/settings/ids_indicators.json` & `bblocks-1.3.1/bblocks/import_tools/debt/settings/ids_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/debt/wb_ids.py` & `bblocks-1.3.1/bblocks/import_tools/debt/wb_ids.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/fao.py` & `bblocks-1.3.1/bblocks/import_tools/fao.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/hdr.py` & `bblocks-1.3.1/bblocks/import_tools/hdr.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/ilo.py` & `bblocks-1.3.1/bblocks/import_tools/ilo.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/imf_weo.py` & `bblocks-1.3.1/bblocks/import_tools/imf_weo.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from zipfile import ZipFile
 from dataclasses import dataclass
 import pandas as pd
 from datetime import datetime
 from bs4 import BeautifulSoup
 import io
 import requests
+import numpy as np
 
 from bblocks.import_tools.common import ImportData, get_response, unzip
 from bblocks.config import BBPaths
 from bblocks.logger import logger
 from bblocks.cleaning_tools import clean
 
 
@@ -379,7 +380,41 @@
 
         return (
             self._raw_data.loc[:, ["concept_code", "concept"]]
             .drop_duplicates()
             .set_index("concept_code")["concept"]
             .to_dict()
         )
+
+    def get_old_format_data(self) -> pd.DataFrame:
+        """This function returns the data in the old format that weo-reader returns
+
+        NOTE: This will return all the data in the object in the old format, regardless of the indicators loaded
+        Not all columns that existed in weo-reader are returned as they don't exist in the sdmx data files. However,
+        this should not cause issues are they are metadata columns not used in analysis.
+        """
+
+        logger.warning(
+            "This method is a temporary fix used to patch the output format that weo-reader returns. "
+            "It will be removed in the future."
+        )
+
+        col_mapper = {
+            "concept_code": "WEO Subject Code",
+            "ref_area_code": "WEO Country Code",
+            "lastactualdate": "Estimates Start After",
+            "notes": "Country/Series-specific Notes",
+            "unit": "Units",
+            "concept": "Subject Descriptor",
+            "ref_area": "Country",
+            "scale": "Scale",
+        }
+
+        return (
+            self.get_data()
+            .rename(columns=col_mapper)
+            .pivot(index=col_mapper.values(), columns="time_period", values="obs_value")
+            .reset_index()
+            .assign(ISO=lambda d: clean.convert_id(d.Country, not_found=np.nan))
+            .dropna(subset="ISO")
+            .reset_index(drop=True)
+        )
```

### Comparing `bblocks-1.3.0/bblocks/import_tools/sdr.py` & `bblocks-1.3.1/bblocks/import_tools/sdr.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/settings/aids_indicators.json` & `bblocks-1.3.1/bblocks/import_tools/settings/aids_indicators.json`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/settings/flourish_geometries.csv` & `bblocks-1.3.1/bblocks/import_tools/settings/flourish_geometries.csv`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/settings/ids_codes.csv` & `bblocks-1.3.1/bblocks/import_tools/settings/ids_codes.csv`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/unaids.py` & `bblocks-1.3.1/bblocks/import_tools/unaids.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/wfp.py` & `bblocks-1.3.1/bblocks/import_tools/wfp.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/who.py` & `bblocks-1.3.1/bblocks/import_tools/who.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/import_tools/world_bank.py` & `bblocks-1.3.1/bblocks/import_tools/world_bank.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/logger.py` & `bblocks-1.3.1/bblocks/logger.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/other_tools/common.py` & `bblocks-1.3.1/bblocks/other_tools/common.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/bblocks/other_tools/dictionaries.py` & `bblocks-1.3.1/bblocks/other_tools/dictionaries.py`

 * *Files identical despite different names*

### Comparing `bblocks-1.3.0/pyproject.toml` & `bblocks-1.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblocks"
-version = "1.3.0"
+version = "1.3.1"
 description = "A package with tools to download and analyse international development data. These tools are meant to be the building blocks of further analysis."
 authors = ["The ONE Campaign <data@one.org>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
@@ -21,27 +21,26 @@
 python = "^3.10"
 pandas = "^2"
 numpy = "^1"
 country-converter = "^1"
 openpyxl = "^3.0.10"
 requests = "^2.28"
 opencv-python = "^4.7.0"
-weo = "^0.7.4"
 beautifulsoup4 = "^4.12"
 pyjstat = "^2.3"
 pyarrow = "^15"
 wbgapi = "<1.1"
 camelot-py = "^0.11"
 pypdf = "^3.17"
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
 black = "^24"
 pytest = "^8"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 myst-nb = {version = "^1", python = "^3.1"}
 sphinx-autoapi = "^3.0"
 #sphinx-rtd-theme = "^1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bblocks-1.3.0/PKG-INFO` & `bblocks-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblocks
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package with tools to download and analyse international development data. These tools are meant to be the building blocks of further analysis.
 License: MIT
 Author: The ONE Campaign
 Author-email: data@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,14 @@
 Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
 Requires-Dist: pandas (>=2,<3)
 Requires-Dist: pyarrow (>=15,<16)
 Requires-Dist: pyjstat (>=2.3,<3.0)
 Requires-Dist: pypdf (>=3.17,<4.0)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: wbgapi (<1.1)
-Requires-Dist: weo (>=0.7.4,<0.8.0)
 Description-Content-Type: text/markdown
 
 [![pypi](https://img.shields.io/pypi/v/bblocks.svg)](https://pypi.org/project/bblocks/)
 [![python](https://img.shields.io/pypi/pyversions/bblocks.svg)](https://pypi.org/project/bblocks/)
 [![codecov](https://codecov.io/gh/ONEcampaign/bblocks/branch/main/graph/badge.svg?token=YN8S1719NH)](https://codecov.io/gh/ONEcampaign/bblocks)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

