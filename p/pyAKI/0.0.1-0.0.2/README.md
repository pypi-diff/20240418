# Comparing `tmp/pyAKI-0.0.1.tar.gz` & `tmp/pyaki-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAKI-0.0.1.tar", last modified: Sat Nov 11 07:06:50 2023, max compression
+gzip compressed data, was "pyaki-0.0.2.tar", last modified: Thu Apr 18 09:33:07 2024, max compression
```

## Comparing `pyAKI-0.0.1.tar` & `pyaki-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,50 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-11-11 07:06:50.951913 pyAKI-0.0.1/
--rw-r--r--   0 christian   (501) staff       (20)     1062 2023-06-07 08:14:32.000000 pyAKI-0.0.1/LICENSE
--rw-r--r--   0 christian   (501) staff       (20)      756 2023-11-11 07:06:50.951826 pyAKI-0.0.1/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1129 2023-11-11 06:30:49.000000 pyAKI-0.0.1/README.md
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-11-11 07:06:50.947011 pyAKI-0.0.1/bin/
--rwxr-xr-x   0 christian   (501) staff       (20)     1988 2023-10-31 19:43:21.000000 pyAKI-0.0.1/bin/process_aki_stages.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-11-11 07:06:50.948645 pyAKI-0.0.1/pyAKI/
--rw-r--r--   0 christian   (501) staff       (20)      199 2023-06-30 09:17:26.000000 pyAKI-0.0.1/pyAKI/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     5645 2023-10-26 08:28:04.000000 pyAKI-0.0.1/pyAKI/kdigo.py
--rw-r--r--   0 christian   (501) staff       (20)     7300 2023-10-26 08:28:04.000000 pyAKI-0.0.1/pyAKI/preprocessors.py
--rw-r--r--   0 christian   (501) staff       (20)    15765 2023-10-26 08:28:04.000000 pyAKI-0.0.1/pyAKI/probes.py
--rw-r--r--   0 christian   (501) staff       (20)     4907 2023-10-26 08:28:04.000000 pyAKI-0.0.1/pyAKI/utils.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-11-11 07:06:50.949576 pyAKI-0.0.1/pyAKI.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)      756 2023-11-11 07:06:50.000000 pyAKI-0.0.1/pyAKI.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)      454 2023-11-11 07:06:50.000000 pyAKI-0.0.1/pyAKI.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-11-11 07:06:50.000000 pyAKI-0.0.1/pyAKI.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       11 2023-11-11 07:06:50.000000 pyAKI-0.0.1/pyAKI.egg-info/top_level.txt
--rw-r--r--   0 christian   (501) staff       (20)      830 2023-11-11 07:06:50.952253 pyAKI-0.0.1/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      141 2023-11-11 06:54:28.000000 pyAKI-0.0.1/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-11-11 07:06:50.949840 pyAKI-0.0.1/test/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/__init__.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-11-11 07:06:50.951343 pyAKI-0.0.1/test/probes/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/probes/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      626 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/probes/set_up.py
--rw-r--r--   0 christian   (501) staff       (20)     5519 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/probes/test_creatinine_probes.py
--rw-r--r--   0 christian   (501) staff       (20)     1776 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/probes/test_rrt_probe.py
--rw-r--r--   0 christian   (501) staff       (20)     6758 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/probes/test_urineoutput_probes.py
--rw-r--r--   0 christian   (501) staff       (20)     1200 2023-11-11 06:30:49.000000 pyAKI-0.0.1/test/test_mimic.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.875323 pyaki-0.0.2/
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.865711 pyaki-0.0.2/.github/
+-rw-r--r--   0 christian   (501) staff       (20)      597 2023-06-27 11:36:55.000000 pyaki-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.866068 pyaki-0.0.2/.github/workflows/
+-rw-r--r--   0 christian   (501) staff       (20)     1317 2024-02-07 11:00:44.000000 pyaki-0.0.2/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 christian   (501) staff       (20)      334 2024-04-18 09:33:06.000000 pyaki-0.0.2/AUTHORS
+-rw-r--r--   0 christian   (501) staff       (20)      749 2023-11-27 15:08:08.000000 pyaki-0.0.2/CITATION.cff
+-rw-r--r--   0 christian   (501) staff       (20)     7188 2024-04-18 09:33:06.000000 pyaki-0.0.2/ChangeLog
+-rw-r--r--   0 christian   (501) staff       (20)     1062 2023-06-07 08:14:32.000000 pyaki-0.0.2/LICENSE
+-rw-r--r--   0 christian   (501) staff       (20)     2782 2024-04-18 09:33:07.875226 pyaki-0.0.2/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1836 2024-04-18 09:27:54.000000 pyaki-0.0.2/README.md
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.866401 pyaki-0.0.2/bin/
+-rwxr-xr-x   0 christian   (501) staff       (20)     1988 2023-10-31 19:43:21.000000 pyaki-0.0.2/bin/process_aki_stages.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.866713 pyaki-0.0.2/img/
+-rw-r--r--   0 christian   (501) staff       (20)    91493 2023-11-11 07:04:14.000000 pyaki-0.0.2/img/kdigo_criteria.png
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.868819 pyaki-0.0.2/pyAKI/
+-rw-r--r--   0 christian   (501) staff       (20)      215 2023-11-19 15:20:55.000000 pyaki-0.0.2/pyAKI/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     6500 2024-02-07 11:00:44.000000 pyaki-0.0.2/pyAKI/kdigo.py
+-rw-r--r--   0 christian   (501) staff       (20)     7290 2023-12-05 16:56:03.000000 pyaki-0.0.2/pyAKI/preprocessors.py
+-rw-r--r--   0 christian   (501) staff       (20)    21750 2024-02-07 11:00:44.000000 pyaki-0.0.2/pyAKI/probes.py
+-rw-r--r--   0 christian   (501) staff       (20)     5311 2023-11-27 15:08:39.000000 pyaki-0.0.2/pyAKI/utils.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.874716 pyaki-0.0.2/pyAKI.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)     2782 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)      971 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/not-zip-safe
+-rw-r--r--   0 christian   (501) staff       (20)       46 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/pbr.json
+-rw-r--r--   0 christian   (501) staff       (20)       98 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)        6 2024-04-18 09:33:07.000000 pyaki-0.0.2/pyAKI.egg-info/top_level.txt
+-rw-r--r--   0 christian   (501) staff       (20)       97 2024-04-18 09:27:54.000000 pyaki-0.0.2/requirements.txt
+-rw-r--r--   0 christian   (501) staff       (20)      830 2024-04-18 09:33:07.875686 pyaki-0.0.2/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      141 2023-11-11 06:54:28.000000 pyaki-0.0.2/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.870510 pyaki-0.0.2/test/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-11-11 06:30:49.000000 pyaki-0.0.2/test/__init__.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.870774 pyaki-0.0.2/test/data/
+-rw-r--r--   0 christian   (501) staff       (20)   178172 2024-02-07 11:00:44.000000 pyaki-0.0.2/test/data/validation_data.csv
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.873232 pyaki-0.0.2/test/preprocessors/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-11-17 17:48:16.000000 pyaki-0.0.2/test/preprocessors/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2737 2023-11-17 17:48:16.000000 pyaki-0.0.2/test/preprocessors/test_creatinie_preprocessor.py
+-rw-r--r--   0 christian   (501) staff       (20)      750 2023-11-17 17:48:16.000000 pyaki-0.0.2/test/preprocessors/test_demographics_preprocessor.py
+-rw-r--r--   0 christian   (501) staff       (20)     1430 2023-11-17 17:48:16.000000 pyaki-0.0.2/test/preprocessors/test_rrt_preprocessor.py
+-rw-r--r--   0 christian   (501) staff       (20)     1177 2023-11-17 17:48:16.000000 pyaki-0.0.2/test/preprocessors/test_time_index_preprocessor.py
+-rw-r--r--   0 christian   (501) staff       (20)     2845 2023-12-05 16:56:03.000000 pyaki-0.0.2/test/preprocessors/test_urineoutput_preprocessor.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2024-04-18 09:33:07.874310 pyaki-0.0.2/test/probes/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-11-11 06:30:49.000000 pyaki-0.0.2/test/probes/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     9414 2024-02-07 11:00:44.000000 pyaki-0.0.2/test/probes/test_creatinine_probes.py
+-rw-r--r--   0 christian   (501) staff       (20)     1777 2023-12-05 16:56:03.000000 pyaki-0.0.2/test/probes/test_rrt_probe.py
+-rw-r--r--   0 christian   (501) staff       (20)     9563 2023-12-05 16:56:03.000000 pyaki-0.0.2/test/probes/test_urineoutput_probes.py
+-rw-r--r--   0 christian   (501) staff       (20)      626 2023-12-05 16:56:03.000000 pyaki-0.0.2/test/set_up.py
+-rw-r--r--   0 christian   (501) staff       (20)     3547 2024-02-07 12:42:32.000000 pyaki-0.0.2/test/test_analyser.py
```

### Comparing `pyAKI-0.0.1/LICENSE` & `pyaki-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAKI-0.0.1/bin/process_aki_stages.py` & `pyaki-0.0.2/bin/process_aki_stages.py`

 * *Files identical despite different names*

### Comparing `pyAKI-0.0.1/pyAKI/kdigo.py` & `pyaki-0.0.2/pyAKI/kdigo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from typing import Optional
 
 import pandas as pd
 
 from pyAKI.probes import (
     Probe,
     UrineOutputProbe,
@@ -16,14 +18,16 @@
     CreatininePreProcessor,
     DemographicsPreProcessor,
     RRTPreProcessor,
 )
 
 from pyAKI.utils import Dataset
 
+logger = logging.getLogger(__name__)
+
 
 class Analyser:
     """
     Class for data analysis using probes and preprocessors.
 
     This class provides functionality for analyzing data using a collection of probes and preprocessors.
     It processes the input data through the specified preprocessors and applies the probes to perform
@@ -80,41 +84,59 @@
                     stay_identifier=stay_identifier, time_identifier=time_identifier
                 ),
                 DemographicsPreProcessor(stay_identifier=stay_identifier),
                 RRTPreProcessor(
                     stay_identifier=stay_identifier, time_identifier=time_identifier
                 ),
             ]
+
+        # validate datasets
+        self.validate_data(data)
+
         # apply preprocessors to the input data
+        logger.info("Start preprocessing")
         for preprocessor in preprocessors:
             data = preprocessor.process(data)
 
+        logger.info("Finish preprocessing")
+
         self._data: list[Dataset] = data
         self._probes: list[Probe] = probes
         self._stay_identifier: str = stay_identifier
 
+    def validate_data(self, datasets: list[Dataset]) -> None:
+        for dtype, df in datasets:
+            try:
+                if (df < 0).values.any():
+                    raise ValueError(f"Dataset of Type {dtype} contains negative data")
+            except TypeError:
+                continue
+
     def process_stays(self) -> pd.DataFrame:
         """
         Process all stays in the input data.
 
         This method processes all stays in the input data by applying the configured probes.
         The analysis results for all stays are concatenated and returned as a single DataFrame.
 
         Returns:
             pd.DataFrame: The analysis results for all stays.
         """
+        logger.info("Start probing")
+
         (_, df), *datasets = self._data
         stay_ids: pd.Index = df.index.get_level_values("stay_id").unique()
         for _, df in datasets:
             stay_ids.join(df.index.get_level_values("stay_id").unique())
 
         data: pd.DataFrame = self.process_stay(stay_ids.values[0])
         for stay_id in stay_ids.values[1:]:
             data = pd.concat([data, self.process_stay(stay_id)])
-        # data = data.drop(columns=["stay_id"])  # remove additional stay_id column
+
+        logger.info("Finish probing")
         return data
 
     def process_stay(self, stay_id: str) -> pd.DataFrame:
         """
         Process a specific stay in the input data by patient identificator.
 
         This method processes a specific stay in the input data by applying the configured probes and preprocessors.
@@ -122,23 +144,34 @@
 
         Args:
             stay_id (str): The identifier of the stay to process.
 
         Returns:
             pd.DataFrame: The analysis results for the specific stay.
         """
+        logger.debug("Processing stay with id: %s", stay_id)
 
-        data = [(name, data.loc[stay_id]) for name, data in self._data]
+        datasets: list[Dataset] = [
+            Dataset(dtype, data.loc[stay_id])  # type: ignore
+            for dtype, data in self._data
+            if stay_id in data.index
+        ]
 
         for probe in self._probes:
-            data: Dataset = probe.probe(data)
+            datasets = probe.probe(datasets)
 
-        (_, df), *datasets = data
+        (_, df), *datasets = datasets
         for _, _df in datasets:
             if isinstance(_df, pd.Series):
                 _df = pd.DataFrame([_df], index=df.index)
-            df: pd.DataFrame = df.merge(
-                _df, how="outer", left_index=True, right_index=True
+            columns = set(_df.columns) - set(df.columns)
+            df = df.merge(
+                _df[[*columns]], how="outer", left_index=True, right_index=True
             )
 
         df["stage"] = df.filter(like="stage").max(axis=1)
-        return df.set_index([pd.Index([stay_id] * len(df), name="stay_id"), df.index])
+        return df.set_index(
+            pd.MultiIndex.from_arrays(
+                [[stay_id] * len(df), df.index.values],
+                names=(self._stay_identifier, df.index.name),
+            )
+        )
```

### Comparing `pyAKI-0.0.1/pyAKI/preprocessors.py` & `pyaki-0.0.2/pyAKI/preprocessors.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,48 +64,48 @@
     """Preprocessor for processing the urine output dataset."""
 
     def __init__(
         self,
         stay_identifier: str = "stay_id",
         time_identifier: str = "charttime",
         interpolate: bool = True,
-        threshold: Optional[int] = 1,
+        threshold: int = 6,
     ) -> None:
         """
         Initialize a new instance of the UrineOutputPreProcessor class.
 
         Parameters:
             stay_identifier (str, optional): The column name that identifies stays or admissions in the dataset. Defaults to MIMIC standard "stay_id".
             time_identifier (str, optional): The column name that identifies the timestamp or time variable in the dataset. Defaults to MIMIC standard "charttime".
             interpolate (bool, optional): Flag indicating whether to perform interpolation on missing values. Defaults to True.
-            threshold (int, optional): The threshold value for limiting the interpolation range. Defaults to 1.
+            threshold (int, optional): The threshold value for limiting the interpolation range. Defaults to 6.
         """
         super().__init__(stay_identifier, time_identifier)
-
         self._interpolate: bool = interpolate
-        self._threshold: Optional[int] = threshold
+        self._threshold: int = threshold
 
     @dataset_as_df(df=DatasetType.URINEOUTPUT)
     @df_to_dataset(DatasetType.URINEOUTPUT)
-    def process(self, df: pd.DataFrame = None) -> pd.DataFrame:
+    def process(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Process the urine output dataset by resampling, interpolating missing values, and applying threshold-based adjustments.
 
         Parameters:
             df (pd.DataFrame): The input urine output dataset as a pandas DataFrame.
 
         Returns:
             pd.DataFrame: The processed urine output dataset as a pandas DataFrame.
         """
 
-        df = df.groupby(self._stay_identifier).resample("1H").sum()
+        df = df.groupby(self._stay_identifier).resample("1H").sum()  # type: ignore
+        df[df["urineoutput"] == 0] = None
+
         if not self._interpolate:
             return df
 
-        df[df["urineoutput"] == 0] = None
         mask = df["urineoutput"].isnull()
         df["urineoutput"] /= (
             (mask.cumsum() - mask.cumsum().where(~mask).ffill().fillna(0))
             .shift(1)
             .clip(upper=self._threshold)
             .add(1)
             .fillna(1)
@@ -117,15 +117,15 @@
     """Preprocessor for processing the creatinine dataset."""
 
     def __init__(
         self,
         stay_identifier: str = "stay_id",
         time_identifier: str = "charttime",
         ffill: bool = True,
-        threshold: Optional[int] = 72,
+        threshold: int = 72,
     ) -> None:
         """
         Initialize a new instance of the CreatininePreProcessor class.
 
         Parameters:
             stay_identifier (str, optional): The column name that identifies stays or admissions in the dataset. Defaults to "stay_id".
             time_identifier (str, optional): The column name that identifies the timestamp or time variable in the dataset. Defaults to "charttime".
@@ -135,38 +135,38 @@
         super().__init__(stay_identifier, time_identifier)
 
         self._ffill: bool = ffill
         self._threshold: Optional[int] = threshold
 
     @dataset_as_df(df=DatasetType.CREATININE)
     @df_to_dataset(DatasetType.CREATININE)
-    def process(self, df: pd.DataFrame = None) -> pd.DataFrame:
+    def process(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Process the creatinine dataset by resampling and performing forward filling on missing values.
 
         Parameters:
             df (pd.DataFrame): The input creatinine dataset as a pandas DataFrame.
 
         Returns:
             pd.DataFrame: The processed creatinine dataset as a pandas DataFrame.
         """
-        df = df.groupby(self._stay_identifier).resample("1H").mean()
+        df = df.groupby(self._stay_identifier).resample("1H").mean()  # type: ignore
         if not self._ffill:
             return df
 
         df[df["creat"] == 0] = None
         return df.ffill(limit=self._threshold)
 
 
 class DemographicsPreProcessor(Preprocessor):
     """Preprocessor for processing the demographics dataset."""
 
     @dataset_as_df(df=DatasetType.DEMOGRAPHICS)
     @df_to_dataset(DatasetType.DEMOGRAPHICS)
-    def process(self, df: pd.DataFrame = None) -> pd.DataFrame:
+    def process(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Process the demographics dataset by aggregating the data based on stay identifiers.
 
         Parameters:
             df (pd.DataFrame): The input demographics dataset as a pandas DataFrame.
 
         Returns:
@@ -176,19 +176,19 @@
 
 
 class RRTPreProcessor(Preprocessor):
     """Preprocessor for processing the RRT dataset."""
 
     @dataset_as_df(df=DatasetType.RRT)
     @df_to_dataset(DatasetType.RRT)
-    def process(self, df: pd.DataFrame = None) -> pd.DataFrame:
+    def process(self, df: pd.DataFrame) -> pd.DataFrame:
         """
         Process the RRT dataset by upsampling the data and forward filling the last value. We expect the dataframe to contain a 1 for RRT in progress, and 0 for RRT not in progress.
 
         Parameters:
             df (pd.DataFrame): The input RRT dataset as a pandas DataFrame.
 
         Returns:
             pd.DataFrame: The processed RRT dataset as a pandas DataFrame.
         """
-        df = df.groupby(self._stay_identifier).resample("1H").last()
+        df = df.groupby(self._stay_identifier).resample("1H").last()  # type: ignore
         return df.ffill()
```

### Comparing `pyAKI-0.0.1/pyAKI/probes.py` & `pyaki-0.0.2/pyAKI/probes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """ This module contains the Probe abstract base class and its subclasses,
 used for probing for the different KDIGO criteria."""
 
 from abc import ABC, ABCMeta
 from enum import StrEnum, auto
-from typing import Optional, Dict
 
 import pandas as pd
 import numpy as np
 
-
+import logging
 from pyAKI.utils import dataset_as_df, df_to_dataset, approx_gte, Dataset, DatasetType
 
 
 class Probe(ABC):
     """
     Abstract base class representing a data analysis probe.
 
@@ -39,15 +38,15 @@
 
         my_probe = MyProbe()
         result_df = my_probe.probe(datasets=my_datasets, additional_arg=value)
     """
 
     RESNAME: str = ""  # name of the column that will be added to the dataframe
 
-    def probe(self, datasets: list[Dataset], **kwargs) -> pd.DataFrame:
+    def probe(self, datasets: list[Dataset], **kwargs) -> list[Dataset]:
         """
         Abstract method to be implemented by subclasses.
 
         This method performs data analysis on the provided datasets and returns a DataFrame
         with the analysis results. Subclasses must override this method.
 
         Args:
@@ -99,36 +98,39 @@
     """
 
     RESNAME = "urineoutput_stage"
 
     def __init__(
         self,
         column: str = "urineoutput",
+        patient_weight_column: str = "weight",
         anuria_limit: float = 0.1,
         method: UrineOutputMethod = UrineOutputMethod.MEAN,
     ) -> None:
         """
         Initialize the UrineOutputProbe instance.
 
         Args:
             column (str): The name of the column representing urine output in the DataFrame.
             anuria_limit (float): The anuria limit for urine output calculations. Defaults to 0.1ml/kg/h.
         """
         super().__init__()
 
         self._column: str = column
+        self._patient_weight_column: str = patient_weight_column
+
         self._anuria_limit: float = anuria_limit
         self._method: UrineOutputMethod = method
 
     @dataset_as_df(df=DatasetType.URINEOUTPUT, patient=DatasetType.DEMOGRAPHICS)
     @df_to_dataset(DatasetType.URINEOUTPUT)
     def probe(
         self,
-        df: pd.DataFrame = None,
-        patient: pd.DataFrame = None,
+        df: pd.DataFrame,
+        patient: pd.DataFrame,
         **kwargs,
     ) -> pd.DataFrame:
         """
         Perform urine output analysis on the provided DataFrame.
 
         This method calculates the KDIGO stage according to urine output based on the provided DataFrame and patient information DataFrame.
         It modifies the DataFrame by adding the urine output stage column with appropriate values based on the calculations.
@@ -136,17 +138,22 @@
         Args:
             df (pd.DataFrame): The DataFrame containing the urine output data. We expect the DataFrame to contain urine output values in ml, sampled hourly.
             patient (pd.DataFrame): The DataFrame containing patient information. Should contain the patients weight in kg.
 
         Returns:
             pd.DataFrame: The modified DataFrame with the urine output stage column added.
         """
-        weight: pd.Series = patient["weight"]
+        if self._patient_weight_column not in patient:
+            raise ValueError("Missing weight for stay")
+
+        weight: pd.Series = patient[self._patient_weight_column]
         # fmt: off
-        df[self.RESNAME] = 0 # set all urineoutput_stage values to 0
+        df.loc[:, self.RESNAME] = np.nan  # set all urineoutput_stage values to NaN
+        df.loc[df.rolling(6).min()[self._column] >= 0, self.RESNAME] = 0
+
         if self._method == UrineOutputMethod.STRICT:
             df.loc[(df.rolling(6).max()[self._column] / weight) < 0.5, self.RESNAME] = 1
             df.loc[(df.rolling(12).max()[self._column] / weight) < 0.5, self.RESNAME] = 2
             df.loc[(df.rolling(24).max()[self._column] / weight) < 0.3, self.RESNAME] = 3
             df.loc[(df.rolling(12).max()[self._column] / weight) < self._anuria_limit, self.RESNAME] = 3
         elif self._method == UrineOutputMethod.MEAN:
             df.loc[(df.rolling(6).mean()[self._column] / weight) < 0.5, self.RESNAME] = 1
@@ -167,22 +174,36 @@
     Enumeration class representing different methods for creatinine baseline calculations.
 
     This class defines the available methods for calculating creatinine values.
     It is a subclass of the `StrEnum` class, which is a string-based enumeration.
     The available methods are `MIN` and `FIRST`.
 
     Attributes:
-        MIN: Represents the minimum method for creatinine calculations. Minimum creatinine value within the specified time window before observation is used as baseline.
-        FIRST: Represents the first method for creatinine calculations. First creatinine value within the specified time window before observation is used as baseline.
-        FIXED: Represents the fixed method for creatinine calculations. A fixed window (default 7 days) ist used for baseline calculation. Values from the window are used as baseline throughout the observation period.
-    """
-
-    MIN = auto()
-    FIRST = auto()
-    FIXED = auto()
+        ROLLING_MIN: Minimum of a rolling window following the timepoint of observation is used as baseline.
+        ROLLING_FIRST: First value of a rolling window following the timepoint of observation is used as baseline.
+        ROLLING_MEAN: Mean of a rolling window following the timepoint of observation is used as baseline.
+        FIXED_MIN: Minimum of the first n days of observation is used as baseline.
+        FIXED_MEAN: Mean of the first n days of observation is used as baseline.
+        OVERALL_FIRST: First observed value is used as baseline.
+        OVERALL_MEAN: Mean of all observed values is used as baseline.
+        OVERALL_MIN: Minimum of all observed values is used as baseline.
+        CONSTANT: A constant value is used as baseline.
+        CALCULATED: A calculated value is used as baseline, based off of the Cockcroft-Gault-Formula using the Adjusted Body Weight.
+    """
+
+    ROLLING_MIN = auto()
+    ROLLING_FIRST = auto()
+    ROLLING_MEAN = auto()
+    FIXED_MIN = auto()
+    FIXED_MEAN = auto()
+    OVERALL_FIRST = auto()
+    OVERALL_MEAN = auto()
+    OVERALL_MIN = auto()
+    CONSTANT = auto()
+    CALCULATED = auto()
 
 
 class AbstractCreatinineProbe(Probe, metaclass=ABCMeta):
     """
     Abstract base class representing a creatinine probe.
 
     This class serves as an abstract base class for creatinine probes.
@@ -203,77 +224,174 @@
             def probe(self, df, **kwargs):
                 # Probe implementation specific to the derived class
     """
 
     def __init__(
         self,
         column: str = "creat",
+        baseline_constant_column: str = "baseline_constant",
+        patient_weight_column: str = "weight",
+        patient_age_column: str = "age",
+        patient_height_column: str = "height",
+        patient_gender_column: str = "gender",
         baseline_timeframe: str = "7d",
-        method: CreatinineBaselineMethod = CreatinineBaselineMethod.FIXED,
+        expected_clearance: float = 72,
+        method: CreatinineBaselineMethod = CreatinineBaselineMethod.ROLLING_MIN,
     ) -> None:
         super().__init__()
 
         self._column: str = column
+        self._baseline_constant_column: str = baseline_constant_column
+        self._patient_weight_column: str = patient_weight_column
+        self._patient_age_column: str = patient_age_column
+        self._patient_height_column: str = patient_height_column
+        self._patient_gender_column: str = patient_gender_column
+
         self._baseline_timeframe: str = baseline_timeframe
+        self._expected_clearance: float = expected_clearance
         self._method: CreatinineBaselineMethod = method
 
-    def creatinine_baseline(self, df: pd.DataFrame) -> pd.Series:
+    def creatinine_baseline(self, df: pd.DataFrame, patient: pd.DataFrame) -> pd.Series:
         """
         Calculate the creatinine baseline values.
 
         This method calculates the creatinine baseline values based on the configured
         parameters and the provided DataFrame.
 
         Args:
             df (pd.DataFrame): The DataFrame containing the creatinine data.
 
         Returns:
             pd.Series: The calculated creatinine baseline values.
-
         """
-        if self._method == CreatinineBaselineMethod.FIRST:
+
+        if self._method == CreatinineBaselineMethod.ROLLING_FIRST:
             return (
                 df[df[self._column] > 0]
                 .rolling(self._baseline_timeframe)
-                .agg(lambda rows: rows[0])
+                .agg(lambda rows: rows.iloc[0])
                 .resample("1h")
                 .first()
                 .ffill()[self._column]
             )
 
-        if self._method == CreatinineBaselineMethod.MIN:
+        if self._method == CreatinineBaselineMethod.ROLLING_MIN:
             return (
                 df[df[self._column] > 0]
                 .rolling(self._baseline_timeframe)
                 .min()
                 .resample("1h")
                 .min()
                 .ffill()[self._column]
             )
+        if self._method == CreatinineBaselineMethod.ROLLING_MEAN:
+            return (
+                df[df[self._column] > 0]
+                .rolling(self._baseline_timeframe)
+                .mean()
+                .resample("1h")
+                .mean()
+                .ffill()[self._column]
+            )
 
-        if self._method == CreatinineBaselineMethod.FIXED:
-            values = (
+        if self._method == CreatinineBaselineMethod.FIXED_MIN:
+            values: pd.Series = (
                 df[df[self._column] > 0]
                 .rolling(self._baseline_timeframe)
                 .min()
                 .resample("1h")
                 .min()
                 .ffill()[self._column]
             )
-            min_value = values[
+            min_value: pd.DatetimeIndex = values[
                 values.index
                 <= (values.index[0] + pd.Timedelta(self._baseline_timeframe))
             ].min()  # calculate min value for first 7 days
             values[
                 values.index
                 > (values.index[0] + pd.Timedelta(self._baseline_timeframe))
             ] = min_value  # set all values after first 7 days to min value
 
             return values
 
+        if self._method == CreatinineBaselineMethod.FIXED_MEAN:
+            time_delta = pd.to_timedelta(self._baseline_timeframe)
+            end_time = df.index[0] + time_delta
+            value = df[df.index <= end_time][self._column].mean()
+            values = self._to_df_length(df, value)
+            return values
+
+        if self._method == CreatinineBaselineMethod.OVERALL_FIRST:
+            value = df[df[self._column] > 0].iloc[0][self._column]
+            values = self._to_df_length(df, value)
+            return values
+
+        if self._method == CreatinineBaselineMethod.OVERALL_MIN:
+            value = df[df[self._column] > 0][self._column].min()
+            values = self._to_df_length(df, value)
+            return values
+
+        if self._method == CreatinineBaselineMethod.OVERALL_MEAN:
+            value = df[df[self._column] > 0][self._column].mean()
+            values = self._to_df_length(df, value)
+            return values
+
+        if self._method == CreatinineBaselineMethod.CONSTANT:
+            if self._baseline_constant_column not in patient:
+                raise ValueError(
+                    "Baseline constant method requires baseline constant values. Please provide a pd.Series containing baseline values for creatinine."
+                )
+
+            return pd.Series(
+                [patient[self._baseline_constant_column]] * len(df),
+                index=df.index,
+                name=self._column,
+            )
+
+        if self._method == CreatinineBaselineMethod.CALCULATED:
+            columns = [
+                self._patient_weight_column,
+                self._patient_age_column,
+                self._patient_height_column,
+                self._patient_gender_column,
+            ]
+            for column in columns:
+                if column not in patient:
+                    raise ValueError(
+                        f"Calculated baseline method requires patient {column}. Please provide a pd.Series containing patient {column}."
+                    )
+
+            weight = patient[self._patient_weight_column]
+            height = patient[self._patient_height_column]
+            gender = patient[self._patient_gender_column]
+            age = patient[self._patient_age_column]
+
+            ibw = (50.0 if gender == "M" else 45.5) + 2.3 * height / 2.54 - 60
+            abw = ibw + 0.4 * (weight - ibw)
+
+            # fmt: off
+            return pd.Series(
+                [
+                    ((140 - age) * abw * (1 if gender == "M" else 0.85)) /
+                    (70 * self._expected_clearance)
+                ] * len(df),
+                index=df.index,
+                name=self._column,
+            )
+            # fmt: on
+
+    def _to_df_length(self, df: pd.DataFrame, value: float) -> pd.Series:
+        """Helper function to create a series, the same length as the data frame."""
+        values = pd.Series(
+            [value] * len(df),
+            index=df.index,
+            name=self._column,
+        )
+        return values
+
 
 class AbsoluteCreatinineProbe(AbstractCreatinineProbe):
     """
     Probe class for absolute creatinine criterion, according to KDIGO criteria.
 
     This class represents a probe that calculates AKI stages according to absolute rises in creatinine, according to the KDIGO criteria.
     It extends the `AbstractCreCreatinineProbe` class.
@@ -284,33 +402,62 @@
     Example:
         probe = AbsoluteCreatinineProbe(column="creatinine", baseline_timeframe="7d", method=CreatinineMethod.MIN)
         df_result = probe.probe(df)
     """
 
     RESNAME = "abs_creatinine_stage"
 
-    @dataset_as_df(df=DatasetType.CREATININE)
+    def __init__(
+        self,
+        column: str = "creat",
+        baseline_constant_column: str = "baseline_constant",
+        patient_weight_column: str = "weight",
+        patient_age_column: str = "age",
+        patient_height_column: str = "height",
+        patient_gender_column: str = "gender",
+        baseline_timeframe: str = "2d",
+        expected_clearance: float = 72,
+        method: CreatinineBaselineMethod = CreatinineBaselineMethod.ROLLING_MIN,
+    ) -> None:
+        super().__init__(
+            column=column,
+            baseline_constant_column=baseline_constant_column,
+            patient_weight_column=patient_weight_column,
+            patient_age_column=patient_age_column,
+            patient_height_column=patient_height_column,
+            patient_gender_column=patient_gender_column,
+            baseline_timeframe=baseline_timeframe,
+            expected_clearance=expected_clearance,
+            method=method,
+        )
+
+    @dataset_as_df(df=DatasetType.CREATININE, patient=DatasetType.DEMOGRAPHICS)
     @df_to_dataset(DatasetType.CREATININE)
-    def probe(self, df: pd.DataFrame = None, **kwargs) -> pd.DataFrame:
+    def probe(
+        self,
+        df: pd.DataFrame,
+        patient: pd.DataFrame,
+        **kwargs,
+    ) -> pd.DataFrame:
         """
         Perform KDIGO stage calculation based on absolute creatinine elevations on the provided DataFrame.
 
         This method calculates the KDIGO stage based on the provided DataFrame
         and the configured baseline values. It calculates the stage according to KDIGO criteria.
 
         Args:
             df (pd.DataFrame): The DataFrame containing the creatinine data. It should have a column
                 with the name specified in the `column` attribute of the probe.
 
         Returns:
             pd.DataFrame: The modified DataFrame with the absolute creatinine stage column added.
         """
-        baseline_values: pd.Series = self.creatinine_baseline(df)
+        baseline_values: pd.Series = self.creatinine_baseline(df, patient)
 
-        df[self.RESNAME] = 0.0
+        df.loc[:, self.RESNAME] = 0
         df.loc[approx_gte((df[self._column] - baseline_values), 0.3), self.RESNAME] = 1
         df.loc[approx_gte(df[self._column], 4), self.RESNAME] = 3
 
         df.loc[pd.isna(df[self._column]), self.RESNAME] = np.nan
 
         return df
 
@@ -327,34 +474,34 @@
     Example:
         probe = RelativeCreatinineProbe(column="creatinine", baseline_timeframe="7d", method=CreatinineBaselineMethod.MIN)
         df_result = probe.probe(df)
     """
 
     RESNAME = "rel_creatinine_stage"
 
-    @dataset_as_df(df=DatasetType.CREATININE)
+    @dataset_as_df(df=DatasetType.CREATININE, patient=DatasetType.DEMOGRAPHICS)
     @df_to_dataset(DatasetType.CREATININE)
-    def probe(self, df: pd.DataFrame = None, **kwargs) -> pd.DataFrame:
+    def probe(self, df: pd.DataFrame, patient: pd.DataFrame, **kwargs) -> pd.DataFrame:
         """
         Perform calculation of relative creatinine elevations on the provided DataFrame.
 
         This method calculates the relative creatinine stage based on the provided DataFrame
         and the configured baseline values. It modifies the DataFrame by adding the relative
         creatinine stage column with appropriate values based on the calculations.
 
         Args:
             df (pd.DataFrame): The DataFrame containing the creatinine data. It should have a column
                 with the name specified in the `column` attribute of the probe.
 
         Returns:
             pd.DataFrame: The modified DataFrame with the relative creatinine stage column added.
         """
-        baseline_values: pd.Series = self.creatinine_baseline(df)
+        baseline_values: pd.Series = self.creatinine_baseline(df, patient)
 
-        df[self.RESNAME] = 0
+        df.loc[:, self.RESNAME] = 0
         df.loc[
             approx_gte((df[self._column] / baseline_values), 1.5), self.RESNAME
         ] = 1.0
         df.loc[approx_gte((df[self._column] / baseline_values), 2), self.RESNAME] = 2
         df.loc[approx_gte((df[self._column] / baseline_values), 3), self.RESNAME] = 3
 
         df.loc[pd.isna(df[self._column]), self.RESNAME] = np.nan
@@ -385,18 +532,16 @@
         """Initialize the probe."""
         super().__init__()
 
         self._column: str = column
 
     @dataset_as_df(df=DatasetType.RRT)
     @df_to_dataset(DatasetType.RRT)
-    def probe(
-        self, df: pd.DataFrame = None, **kwargs: Optional[Dict[str, str]]
-    ) -> pd.DataFrame:
+    def probe(self, df: pd.DataFrame) -> pd.DataFrame:
         """Perform calculation of RRT on the provided DataFrame."""
-        df[self.RESNAME] = 0
+        df.loc[:, self.RESNAME] = 0
         df.loc[df[self._column] == 1, self.RESNAME] = 3
 
         # transfer nans
         df.loc[pd.isna(df[self._column]), self.RESNAME] = np.nan
 
         return df
```

### Comparing `pyAKI-0.0.1/pyAKI/utils.py` & `pyaki-0.0.2/pyAKI/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from typing import NamedTuple
+import logging
+
+from typing import NamedTuple, cast
 from enum import StrEnum, auto
 from functools import wraps
 
 import numpy as np
 import pandas as pd
 
+logger = logging.getLogger(__name__)
+
 
 class DatasetType(StrEnum):
     """Enumeration class representing different types of datasets."""
 
     URINEOUTPUT = auto()
     CREATININE = auto()
     DEMOGRAPHICS = auto()
@@ -33,15 +37,15 @@
         dataset = Dataset(dataset_type=DatasetType.URINEOUTPUT, df=my_dataframe)
     """
 
     dataset_type: DatasetType
     df: pd.DataFrame
 
 
-def dataset_as_df(**mapping: dict[str, DatasetType]):
+def dataset_as_df(**mapping: DatasetType):
     """
     Decorator factory for methods that process datasets with dataframes.
 
     This decorator is intended to be used with methods in a class that handle datasets
     consisting of dataframes. It allows you to specify a mapping of dataset types to
     corresponding dataframe names. The decorator then replaces the dataframes of the
     specified types with the results of the decorated method.
@@ -68,27 +72,35 @@
         When you call `process_data` with a list of `Dataset` objects containing data
         and labels, the decorator will automatically replace the dataframes based on
         the mapping and pass them to the method:
 
         processed_datasets = my_instance.process_data(datasets)
     """
     # swap keys and values in the mapping
-    in_mapping: dict[DatasetType, str] = {v: k for k, v in mapping.items()}
+    in_mapping: dict[DatasetType, str] = {}
+    for k, v in mapping.items():
+        in_mapping[cast(DatasetType, v)] = k
+
+    # in_mapping: Dict[DatasetType, str] = {v: k for k, v in mapping.items()}
 
     def decorator(func):
         @wraps(func)
-        def wrapper(self, datasets: list[Dataset], *args: list, **kwargs: dict):
+        def wrapper(self, datasets: list[Dataset], *args, **kwargs) -> list[Dataset]:
             # map the dataset types to corresponding DataFrames
             _mapping: dict[str, pd.DataFrame] = {
                 in_mapping[dtype]: df
                 for dtype, df in datasets
                 if dtype in in_mapping.keys()
             }
             # check if all datasets are mapped, otherwise return the original datasets
             if len(in_mapping) != len(_mapping):
+                logger.warning(
+                    "Skip %s because one or more datasets are missing to probe",
+                    self.__class__.__name__,
+                )
                 return datasets
 
             # call the wrapped function with the converted DataFrames
             _dtype, _df = func(self, *args, **_mapping, **kwargs)
 
             # return the updated datasets
             return [
@@ -121,17 +133,17 @@
         def process_dataframe(self, *args: list, **kwargs: dict) -> pd.DataFrame:
             # Process the DataFrame
             ...
     """
 
     def decorator(func):
         @wraps(func)
-        def wrapper(self, *args: list, **kwargs: dict):
+        def wrapper(self, *args: list, **kwargs: dict) -> Dataset:
             return Dataset(dtype, func(self, *args, **kwargs))
 
         return wrapper
 
     return decorator
 
 
-def approx_gte(x: pd.Series, y: pd.Series) -> bool:
-    return (x >= y).values | np.isclose(x, y)
+def approx_gte(x: pd.Series, y: pd.Series | float) -> bool | np.ndarray:
+    return np.logical_or(np.asarray(x >= y), np.isclose(x, y))
```

### Comparing `pyAKI-0.0.1/test/probes/set_up.py` & `pyaki-0.0.2/test/set_up.py`

 * *Files identical despite different names*

### Comparing `pyAKI-0.0.1/test/probes/test_rrt_probe.py` & `pyaki-0.0.2/test/probes/test_rrt_probe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest import TestCase
 import pandas as pd
 
 from pyAKI.probes import RRTProbe, Dataset, DatasetType
 from pyAKI.kdigo import Analyser
 
-from .set_up import setup_validation_data
+from ..set_up import setup_validation_data
 
 
 class TestRRTProbe(TestCase):
     def setUp(self) -> None:
         self.validation_data, self.validation_data_unlabelled = setup_validation_data()
         self.probe = RRTProbe()
```

