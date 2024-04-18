# Comparing `tmp/mlflow_for_ml_dev-0.1.3.tar.gz` & `tmp/mlflow_for_ml_dev-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_for_ml_dev-0.1.3.tar", max compression
+gzip compressed data, was "mlflow_for_ml_dev-0.1.4.tar", max compression
```

## Comparing `mlflow_for_ml_dev-0.1.3.tar` & `mlflow_for_ml_dev-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,40 @@
--rw-r--r--   0        0        0        0 2024-03-17 16:07:31.105454 mlflow_for_ml_dev-0.1.3/mlflow_for_ml_dev/__init__.py
--rw-r--r--   0        0        0       46 2024-03-17 16:59:13.243555 mlflow_for_ml_dev-0.1.3/mlflow_for_ml_dev/utils/hello_world.py
--rw-r--r--   0        0        0      744 2024-03-18 01:29:24.214032 mlflow_for_ml_dev-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       41 2024-03-18 01:23:41.653458 mlflow_for_ml_dev-0.1.3/README.md
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 mlflow_for_ml_dev-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-26 02:04:42.435280 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/__init__.py
+-rw-r--r--   0        0        0      367 2024-04-18 01:56:50.549692 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/entrypoints/start_tutorial.py
+-rw-r--r--   0        0        0     5487 2024-03-31 20:22:23.619983 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/experiments/custom_models.py
+-rw-r--r--   0        0        0     2760 2024-04-03 03:46:11.241722 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/experiments/exp_utils.py
+-rw-r--r--   0        0        0     1304 2024-04-17 04:16:08.323550 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/exploration.ipynb
+-rw-r--r--   0        0        0    44319 2024-03-28 13:44:33.118570 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/images/mlflow_run.jpeg
+-rw-r--r--   0        0        0        9 2024-03-28 15:18:32.254786 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/images/text_file.txt
+-rw-r--r--   0        0        0     3045 2024-04-06 16:56:59.593873 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/1_experiments/1_main_concepts.ipynb
+-rw-r--r--   0        0        0     2696 2024-04-05 03:34:09.324384 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/1_experiments/2_create_experiment.ipynb
+-rw-r--r--   0        0        0     3128 2024-04-06 04:38:35.025431 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/1_experiments/3_retrieve_experiments.ipynb
+-rw-r--r--   0        0        0     4658 2024-04-06 04:38:36.147664 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/1_experiments/4_update_experiment.ipynb
+-rw-r--r--   0        0        0     2889 2024-04-06 04:38:37.642707 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/1_experiments/5_delete_experiment.ipynb
+-rw-r--r--   0        0        0     6704 2024-04-17 04:15:55.086252 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/1_create_run.ipynb
+-rw-r--r--   0        0        0     9000 2024-04-17 04:15:53.055555 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/2_logging_functions.ipynb
+-rw-r--r--   0        0        0     7760 2024-04-17 04:15:51.031887 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/3_example.ipynb
+-rw-r--r--   0        0        0     7045 2024-04-17 04:15:49.040669 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/4_logging_models.ipynb
+-rw-r--r--   0        0        0     6359 2024-04-17 04:15:43.652251 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/5_mlflow_autologing.ipynb
+-rw-r--r--   0        0        0    24046 2024-04-04 00:40:09.792313 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/artifacts_example/feature_importance.png
+-rw-r--r--   0        0        0      719 2024-04-04 00:40:09.897808 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/artifacts_example/predictions.csv
+-rw-r--r--   0        0        0   969530 2024-04-04 00:40:07.123213 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/2_runs/artifacts_example/rf_5trees.png
+-rw-r--r--   0        0        0     6872 2024-04-17 04:15:47.567542 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/3_custom_functions/1_custom_functions.ipynb
+-rw-r--r--   0        0        0     4454 2024-04-17 04:16:24.831037 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/3_custom_functions/2_custom_function_model_drift_usecase.ipynb
+-rw-r--r--   0        0        0     6785 2024-04-17 04:16:00.312873 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/3_custom_functions/3_custom_function_wrapping_multiple_models.ipynb
+-rw-r--r--   0        0        0   395413 2024-04-04 00:47:12.644313 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/mlflow_tracking/3_custom_functions/training_data.csv
+-rw-r--r--   0        0        0     2155 2024-04-02 02:58:59.298410 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/1_registering_a_model.ipynb
+-rw-r--r--   0        0        0     2896 2024-04-02 02:58:57.734651 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/2_registering_a_model.ipynb
+-rw-r--r--   0        0        0     3008 2024-04-02 02:58:56.546496 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/3_registering_a_model.ipynb
+-rw-r--r--   0        0        0     7289 2024-04-03 04:22:05.866503 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/4_update_registered_model.ipynb
+-rw-r--r--   0        0        0     3896 2024-04-03 04:22:07.086855 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/5_update_model_version.ipynb
+-rw-r--r--   0        0        0     5902 2024-04-03 04:22:07.767005 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/6_retrieve_model_info.ipynb
+-rw-r--r--   0        0        0    42476 2024-04-03 04:22:08.554687 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/7_retrieving_registered_models.ipynb
+-rw-r--r--   0        0        0     3291 2024-04-03 04:22:09.852332 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/model_registry/8_delete_registered_model_info.ipynb
+-rw-r--r--   0        0        0    12413 2024-04-05 03:34:07.740870 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/searching/1_search_experiments.ipynb
+-rw-r--r--   0        0        0     6594 2024-04-06 16:46:17.234834 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/searching/2_search_runs.ipynb
+-rw-r--r--   0        0        0     9376 2024-04-06 12:51:37.782951 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/notebooks/searching/3_search_models.ipynb
+-rw-r--r--   0        0        0       72 2024-03-26 03:06:46.085192 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/utils/hello_world.py
+-rw-r--r--   0        0        0      105 2024-03-27 14:37:58.529764 mlflow_for_ml_dev-0.1.4/mlflow_for_ml_dev/utils/utils.py
+-rw-r--r--   0        0        0      999 2024-04-18 03:14:33.071805 mlflow_for_ml_dev-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-03-26 02:04:42.435280 mlflow_for_ml_dev-0.1.4/README.md
+-rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 mlflow_for_ml_dev-0.1.4/PKG-INFO
```

### Comparing `mlflow_for_ml_dev-0.1.3/pyproject.toml` & `mlflow_for_ml_dev-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 [tool.poetry]
 name = "mlflow_for_ml_dev"
-version = "0.1.3"
+version = "0.1.4"
 description = "Code examples for the youtube playlist 'MLflow for Machine Learning Development' by Manuel Gil"
 authors = ["Manuel Gil <manuelgilsitio@gmail.com>"]
 readme = "README.md"
 maintainers = ["Manuel Gil <manuelgilsitio@gmail.com>"]
 repository = "https://github.com/manuelgilm/mlflow_for_ml_dev"
 license = "MIT"
 keywords = ["mlflow", "machine learning", "development", "youtube", "tutorial"]
 classifiers = [
     "Topic :: Software Development :: Build Tools",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
+include = [
+    { path = "mlflow_for_ml_dev/notebooks", format = ["sdist", "wheel"] }
+]
 
 [tool.poetry.dependencies]
 python = "^3.11"
+ipython = "^8.22.2"
+jupyter = "^1.0.0"
+mlflow = "^2.11.3"
+
+[tool.poetry.scripts]
+start_tutorial = 'mlflow_for_ml_dev.entrypoints.start_tutorial:run_notebook'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mlflow_for_ml_dev-0.1.3/PKG-INFO` & `mlflow_for_ml_dev-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: mlflow_for_ml_dev
-Version: 0.1.3
+Version: 0.1.4
 Summary: Code examples for the youtube playlist 'MLflow for Machine Learning Development' by Manuel Gil
 Home-page: https://github.com/manuelgilm/mlflow_for_ml_dev
 License: MIT
 Keywords: mlflow,machine learning,development,youtube,tutorial
 Author: Manuel Gil
 Author-email: manuelgilsitio@gmail.com
 Maintainer: Manuel Gil
 Maintainer-email: manuelgilsitio@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: ipython (>=8.22.2,<9.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: mlflow (>=2.11.3,<3.0.0)
 Project-URL: Repository, https://github.com/manuelgilm/mlflow_for_ml_dev
 Description-Content-Type: text/markdown
 
 # MLflow for Machine Learning Development
```

