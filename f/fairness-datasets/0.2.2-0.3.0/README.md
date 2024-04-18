# Comparing `tmp/fairness_datasets-0.2.2.tar.gz` & `tmp/fairness_datasets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairness_datasets-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fairness_datasets-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fairness_datasets-0.2.2.tar` & `fairness_datasets-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3105 2023-08-16 10:00:21.878984 fairness_datasets-0.2.2/.gitignore
--rw-r--r--   0        0        0     1070 2023-08-16 09:03:18.201486 fairness_datasets-0.2.2/LICENSE
--rw-r--r--   0        0        0     2427 2024-04-17 12:43:04.913550 fairness_datasets-0.2.2/README.md
--rw-r--r--   0        0        0      269 2024-04-17 13:09:38.656931 fairness_datasets-0.2.2/fairnessdatasets/__init__.py
--rw-r--r--   0        0        0     8846 2024-04-12 19:25:16.709746 fairness_datasets-0.2.2/fairnessdatasets/adult.py
--rw-r--r--   0        0        0    15346 2024-04-17 13:20:50.203052 fairness_datasets-0.2.2/fairnessdatasets/base.py
--rw-r--r--   0        0        0     5397 2024-04-12 15:59:57.756084 fairness_datasets-0.2.2/fairnessdatasets/default.py
--rw-r--r--   0        0        0     6637 2024-04-17 13:20:50.195052 fairness_datasets-0.2.2/fairnessdatasets/law_school.py
--rw-r--r--   0        0        0     7062 2024-04-12 16:06:33.386637 fairness_datasets-0.2.2/fairnessdatasets/south_german.py
--rw-r--r--   0        0        0      783 2024-02-01 14:45:15.232276 fairness_datasets-0.2.2/noxfile.py
--rw-r--r--   0        0        0     1148 2024-04-12 15:36:24.293920 fairness_datasets-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1463 2024-04-12 19:37:07.507233 fairness_datasets-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0     3980 2024-04-12 19:50:13.029406 fairness_datasets-0.2.2/tests/test_column_indices.py
--rw-r--r--   0        0        0     1837 2024-04-17 12:40:40.261954 fairness_datasets-0.2.2/tests/test_download.py
--rw-r--r--   0        0        0      587 2024-04-12 12:55:35.731613 fairness_datasets-0.2.2/tests/test_output.py
--rw-r--r--   0        0        0     2107 2024-04-17 13:21:42.666906 fairness_datasets-0.2.2/tests/test_shapes.py
--rw-r--r--   0        0        0     1318 2024-04-12 15:51:37.738349 fairness_datasets-0.2.2/tests/test_use.py
--rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 fairness_datasets-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3105 2023-08-16 10:00:21.878984 fairness_datasets-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 2023-08-16 09:03:18.201486 fairness_datasets-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2427 2024-04-17 12:43:04.913550 fairness_datasets-0.3.0/README.md
+-rw-r--r--   0        0        0      269 2024-04-18 20:26:44.673759 fairness_datasets-0.3.0/fairnessdatasets/__init__.py
+-rw-r--r--   0        0        0     8846 2024-04-12 19:25:16.709746 fairness_datasets-0.3.0/fairnessdatasets/adult.py
+-rw-r--r--   0        0        0    15346 2024-04-17 13:20:50.203052 fairness_datasets-0.3.0/fairnessdatasets/base.py
+-rw-r--r--   0        0        0     5397 2024-04-12 15:59:57.756084 fairness_datasets-0.3.0/fairnessdatasets/default.py
+-rw-r--r--   0        0        0     6637 2024-04-17 13:20:50.195052 fairness_datasets-0.3.0/fairnessdatasets/law_school.py
+-rw-r--r--   0        0        0     8225 2024-04-18 20:27:59.145520 fairness_datasets-0.3.0/fairnessdatasets/south_german.py
+-rw-r--r--   0        0        0      783 2024-02-01 14:45:15.232276 fairness_datasets-0.3.0/noxfile.py
+-rw-r--r--   0        0        0     1148 2024-04-12 15:36:24.293920 fairness_datasets-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1463 2024-04-12 19:37:07.507233 fairness_datasets-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     3972 2024-04-18 20:28:26.993433 fairness_datasets-0.3.0/tests/test_column_indices.py
+-rw-r--r--   0        0        0     1837 2024-04-17 12:40:40.261954 fairness_datasets-0.3.0/tests/test_download.py
+-rw-r--r--   0        0        0      587 2024-04-12 12:55:35.731613 fairness_datasets-0.3.0/tests/test_output.py
+-rw-r--r--   0        0        0     2107 2024-04-17 13:21:42.666906 fairness_datasets-0.3.0/tests/test_shapes.py
+-rw-r--r--   0        0        0     1318 2024-04-12 15:51:37.738349 fairness_datasets-0.3.0/tests/test_use.py
+-rw-r--r--   0        0        0     3513 1970-01-01 00:00:00.000000 fairness_datasets-0.3.0/PKG-INFO
```

### Comparing `fairness_datasets-0.2.2/.gitignore` & `fairness_datasets-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/LICENSE` & `fairness_datasets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/README.md` & `fairness_datasets-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/fairnessdatasets/adult.py` & `fairness_datasets-0.3.0/fairnessdatasets/adult.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/fairnessdatasets/base.py` & `fairness_datasets-0.3.0/fairnessdatasets/base.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/fairnessdatasets/default.py` & `fairness_datasets-0.3.0/fairnessdatasets/default.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/fairnessdatasets/law_school.py` & `fairness_datasets-0.3.0/fairnessdatasets/law_school.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/fairnessdatasets/south_german.py` & `fairness_datasets-0.3.0/fairnessdatasets/south_german.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     Class Attributes:
     - `dataset_url`: The URL the South German Credit dataset is downloaded from.
     - `file_to_download`: The file to download from `dataset_url`.
     - `checksums`: The checksums of the files to download from `dataset_url`.
     - `file`: The file containing the data after downloading.
     - `variables`: The variables of the South German Credit dataset,
        together with the values they may take on and the interpretation of the values.
+    - `english_columns_to_german`: A mapping from english column names as used
+      by this class to the german column names of the dataset.
 
     Attributes:
     - `columns`: Column labels for the tensors in this dataset
       (after one-hot encoding, if applied).
     - `files_dir`: Where the data files are stored or downloaded to.
       Value: Root path (user specified) / `type(self).__name__)`
     - `data`: The dataset features (x values)
@@ -152,14 +154,37 @@
             2: "no",
         },
     }
     _variables_no_desc = {
         variable: None if values is None else tuple(values)
         for variable, values in variables.items()
     }
+    english_columns_to_german = {
+        "status": "laufkont",
+        "duration": "laufzeit",
+        "credit_history": "moral",
+        "purpose": "verw",
+        "amount": "hoehe",
+        "savings": "sparkont",
+        "employment_duration": "beszeit",
+        "installment_rate": "rate",
+        "personal_status_sex": "famges",
+        "other_debtors": "buerge",
+        "present_residence": "wohnzeit",
+        "property": "verm",
+        "age": "alter",
+        "other_installment_plans": "weitkred",
+        "housing": "wohn",
+        "number_credits": "bishkred",
+        "job": "beruf",
+        "people_liable": "pers",
+        "telephone": "telef",
+        "foreign_worker": "gastarb",
+        "credit_risk": "kredit",
+    }
 
     def __init__(
         self,
         root: Union[str, os.PathLike],
         raw: bool = False,
         download: bool = False,
         output_fn: Optional[Callable[[str], None]] = print,
@@ -180,21 +205,21 @@
         """
         super().__init__(root, raw, download, output_fn)
 
     def _raw_files(self) -> tuple[str, ...]:
         return (self.file_to_download,)
 
     def _target_column(self) -> str:
-        return "credit_risk"
+        return self.english_columns_to_german["credit_risk"]
 
     def _download(self):
         self._download_zip(self.dataset_url, self.checksums)
 
     def _load_raw(self) -> Tuple[pandas.DataFrame]:
-        all_columns = list(self.variables.keys()) + [self._target_column()]
+        all_columns = list(self._variables().keys()) + [self._target_column()]
         data: pandas.DataFrame = pandas.read_csv(
             self.files_dir / self.file_to_download,
             index_col=False,
             names=all_columns,
             delimiter=" ",
             skiprows=1,  # skip first row since pandas does not recognize header row
             dtype=int,
@@ -204,8 +229,14 @@
     def _preprocess(self, *data: pandas.DataFrame) -> Tuple[pandas.DataFrame]:
         self._output("Preprocessing data...")
         data = super()._preprocess(*data)
         self._output("Preprocessing finished.")
         return data
 
     def _variables(self) -> Dict[str, Optional[Tuple[str, ...]]]:
-        return self._variables_no_desc
+        return {
+            self.english_columns_to_german[var]: vals
+            for var, vals in self._variables_no_desc.items()
+        }
+
+    def column_indices(self, variable: str) -> Tuple[int, ...]:
+        return super().column_indices(self.english_columns_to_german[variable])
```

### Comparing `fairness_datasets-0.2.2/noxfile.py` & `fairness_datasets-0.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/pyproject.toml` & `fairness_datasets-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/tests/conftest.py` & `fairness_datasets-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/tests/test_column_indices.py` & `fairness_datasets-0.3.0/tests/test_column_indices.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         (SouthGerman, {}, "south_german_path", "age", 1),
         (SouthGerman, {"raw": True}, "south_german_raw_path", "credit_history", 1),
         (SouthGerman, {"raw": True}, "south_german_raw_path", "personal_status_sex", 1),
         (SouthGerman, {"raw": True}, "south_german_raw_path", "foreign_worker", 1),
         (SouthGerman, {"raw": True}, "south_german_raw_path", "age", 1),
     ],
 )
-def test_column_indices_default(
+def test_column_indices(
     dataset_class,
     init_kwargs,
     dataset_path,
     variable,
     expected_num_columns,
     request,
 ):
```

### Comparing `fairness_datasets-0.2.2/tests/test_download.py` & `fairness_datasets-0.3.0/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/tests/test_output.py` & `fairness_datasets-0.3.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/tests/test_shapes.py` & `fairness_datasets-0.3.0/tests/test_shapes.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/tests/test_use.py` & `fairness_datasets-0.3.0/tests/test_use.py`

 * *Files identical despite different names*

### Comparing `fairness_datasets-0.2.2/PKG-INFO` & `fairness_datasets-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fairness-datasets
-Version: 0.2.2
+Version: 0.3.0
 Summary: PyTorch dataset wrapper for the
 Keywords: PyTorch,Dataset,Fairness,Adult,Census Income,Law School
 Author-email: David Boetius <david.boetius@uni-konstanz.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

