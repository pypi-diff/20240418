# Comparing `tmp/automated_ml_pack-1.0.6.tar.gz` & `tmp/automated_ml_pack-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automated_ml_pack-1.0.6.tar", last modified: Tue Mar 26 21:47:28 2024, max compression
+gzip compressed data, was "automated_ml_pack-1.0.7.tar", last modified: Thu Apr 18 08:01:40 2024, max compression
```

## Comparing `automated_ml_pack-1.0.6.tar` & `automated_ml_pack-1.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:47:28.527561 automated_ml_pack-1.0.6/
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     1076 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/LICENSE.txt
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       82 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/MANIFEST.in
--rw-r--r--   0 cnjume    (1000) cnjume    (1000)     7364 2024-03-26 21:47:28.527561 automated_ml_pack-1.0.6/PKG-INFO
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     6226 2024-03-26 21:45:33.000000 automated_ml_pack-1.0.6/README.md
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      192 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/requirements.txt
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       38 2024-03-26 21:47:28.527561 automated_ml_pack-1.0.6/setup.cfg
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     1616 2024-03-26 21:45:51.000000 automated_ml_pack-1.0.6/setup.py
-drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:47:28.519561 automated_ml_pack-1.0.6/src/
-drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:47:28.523561 automated_ml_pack-1.0.6/src/automated_ml_pack/
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        9 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/__init__.py
-drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:47:28.523561 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        9 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/__init__.py
-drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:47:28.527561 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/__init__.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     3386 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/data_ingestion.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     9398 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/data_transformation.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     6021 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/model_trainer.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      667 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/exception.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      414 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/logger.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     2320 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/params.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     3817 2024-03-26 21:44:12.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/run_train_pipeline.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)    18566 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/modules/utils.py
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     9323 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.6/src/automated_ml_pack/train_pipeline.py
-drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:47:28.527561 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/
--rw-r--r--   0 cnjume    (1000) cnjume    (1000)     7364 2024-03-26 21:47:28.000000 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/PKG-INFO
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      895 2024-03-26 21:47:28.000000 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/SOURCES.txt
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        1 2024-03-26 21:47:28.000000 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/dependency_links.txt
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       77 2024-03-26 21:47:28.000000 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/entry_points.txt
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      187 2024-03-26 21:47:28.000000 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/requires.txt
--rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       18 2024-03-26 21:47:28.000000 automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/top_level.txt
+drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-04-18 08:01:40.135648 automated_ml_pack-1.0.7/
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     1076 2024-04-17 12:13:29.000000 automated_ml_pack-1.0.7/LICENSE.txt
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       82 2024-04-17 12:13:29.000000 automated_ml_pack-1.0.7/MANIFEST.in
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     7131 2024-04-18 08:01:40.135648 automated_ml_pack-1.0.7/PKG-INFO
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     6345 2024-04-18 07:26:01.000000 automated_ml_pack-1.0.7/README.md
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      192 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/requirements.txt
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       38 2024-04-18 08:01:40.135648 automated_ml_pack-1.0.7/setup.cfg
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     1616 2024-04-17 12:22:00.000000 automated_ml_pack-1.0.7/setup.py
+drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-04-18 08:01:40.131648 automated_ml_pack-1.0.7/src/
+drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-04-18 08:01:40.131648 automated_ml_pack-1.0.7/src/automated_ml_pack/
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        9 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/__init__.py
+drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-04-18 08:01:40.135648 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        9 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/__init__.py
+drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-04-18 08:01:40.135648 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        0 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/__init__.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     3386 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/data_ingestion.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     9398 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/data_transformation.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     6210 2024-04-18 06:37:20.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/model_trainer.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      667 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/exception.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      414 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/logger.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     2320 2024-03-26 21:17:51.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/params.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     3911 2024-04-18 07:03:06.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/run_train_pipeline.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)    18965 2024-04-18 07:53:59.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/modules/utils.py
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     9557 2024-04-18 07:00:07.000000 automated_ml_pack-1.0.7/src/automated_ml_pack/train_pipeline.py
+drwxrwxr-x   0 cnjume    (1000) cnjume    (1000)        0 2024-04-18 08:01:40.131648 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)     7131 2024-04-18 08:01:39.000000 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/PKG-INFO
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      895 2024-04-18 08:01:40.000000 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/SOURCES.txt
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)        1 2024-04-18 08:01:39.000000 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/dependency_links.txt
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       77 2024-04-18 08:01:39.000000 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/entry_points.txt
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)      187 2024-04-18 08:01:39.000000 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/requires.txt
+-rw-rw-r--   0 cnjume    (1000) cnjume    (1000)       18 2024-04-18 08:01:39.000000 automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/top_level.txt
```

### Comparing `automated_ml_pack-1.0.6/LICENSE.txt` & `automated_ml_pack-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automated_ml_pack-1.0.6/PKG-INFO` & `automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 Metadata-Version: 2.1
-Name: automated_ml_pack
-Version: 1.0.6
+Name: automated-ml-pack
+Version: 1.0.7
 Summary: This package is designed for swift and automated machine learning practice, catering to both classification and regression tasks. It facilitates model training, grid search application, and the preservation of the best model. Furthermore, it stores and visualizes the best scores attained by other models using commonly employed evaluation metrics.
 Home-page: https://github.com/CyrilleMesue/automated_ml_pack
 Author: Cyrille
 Author-email: cyrillemesue@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: auto_mix_prep==0.2.0
-Requires-Dist: catboost==1.2.3
-Requires-Dist: dill==0.3.8
-Requires-Dist: feature_engine==1.6.2
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.1
-Requires-Dist: scikit_learn==1.4.1.post1
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: xgboost==2.0.3
 
 # AutomatedMLPack
 ## _A Comprehensive Package for Automated Machine Learning_
 [![scikit-learn](https://github.com/CyrilleMesue/archives/blob/main/images/mlpack.png?raw=true)](https://pypi.org/project/automated-ml-pack/)
 
 **Project Overview:**
 This package is designed for swift and automated machine learning practice, catering to both classification and regression tasks. It facilitates model training, grid search application, and the preservation of the best model. Furthermore, it stores and visualizes the best scores attained by other models using commonly employed evaluation metrics.    
@@ -78,15 +67,16 @@
                        test_size=0.2, 
                        no_standard_scaling=False,
                        feature_selection=False, 
                        feature_selection_method="addition",
                        selectkbest_num_features=32, 
                        output_dir="outputs",
                        verbose = True,
-                       no_param_finetune = False
+                       no_param_finetune = False,
+                       finetune_fraction = 1.0
                       )
 ```
 
 ### Command Line Interface
 
 ```USAGE```:     
 run_train_pipeline -[INPUT_FILE] [options]
@@ -115,14 +105,15 @@
                      Specify between recursive feature addition and recursive feature elimination algorithms for classification. By default, recursive feature addition is applied. For regression tasks, SelectKBest is used for feature selection.    
 ```--selectkbest_num_features``` SELECTKBEST_NUM_FEATURES
                      Number of top features to select. For regression only.     
 ```--output_dir``` OUTPUT_DIR   
                      Custom Name of Output Folder.     
 ```--return_data```         Select to include raw data, training data and test data in the output folders.    
 ```--no_param_finetune```    If true, hyperparameter search will not be performed for each model. Otherwise, hyperparameter tunning is performed.
+```--finetune_fraction```    Percentage of data used for fine tunning.
 
 ## Tutorials
 
 The data must be in csv or tsv format and the user must provide the column name that contains the targets. The following is an example of how the tool can be used for classification tasks.       
 
 ```sh
 run_train_pipeline --input_file heart.csv --target_column HeartDisease --training_type clf --test_size 0.2 --feature_selection --feature_selection_method addition --output_dir heart_disease_classification
```

### Comparing `automated_ml_pack-1.0.6/README.md` & `automated_ml_pack-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,16 @@
                        test_size=0.2, 
                        no_standard_scaling=False,
                        feature_selection=False, 
                        feature_selection_method="addition",
                        selectkbest_num_features=32, 
                        output_dir="outputs",
                        verbose = True,
-                       no_param_finetune = False
+                       no_param_finetune = False,
+                       finetune_fraction = 1.0
                       )
 ```
 
 ### Command Line Interface
 
 ```USAGE```:     
 run_train_pipeline -[INPUT_FILE] [options]
@@ -89,14 +90,15 @@
                      Specify between recursive feature addition and recursive feature elimination algorithms for classification. By default, recursive feature addition is applied. For regression tasks, SelectKBest is used for feature selection.    
 ```--selectkbest_num_features``` SELECTKBEST_NUM_FEATURES
                      Number of top features to select. For regression only.     
 ```--output_dir``` OUTPUT_DIR   
                      Custom Name of Output Folder.     
 ```--return_data```         Select to include raw data, training data and test data in the output folders.    
 ```--no_param_finetune```    If true, hyperparameter search will not be performed for each model. Otherwise, hyperparameter tunning is performed.
+```--finetune_fraction```    Percentage of data used for fine tunning.
 
 ## Tutorials
 
 The data must be in csv or tsv format and the user must provide the column name that contains the targets. The following is an example of how the tool can be used for classification tasks.       
 
 ```sh
 run_train_pipeline --input_file heart.csv --target_column HeartDisease --training_type clf --test_size 0.2 --feature_selection --feature_selection_method addition --output_dir heart_disease_classification
```

### Comparing `automated_ml_pack-1.0.6/setup.py` & `automated_ml_pack-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
 name = "automated_ml_pack",
-version= "1.0.6",
+version= "1.0.7",
 author="Cyrille",
 author_email="cyrillemesue@gmail.com",
 description='This package is designed for swift and automated machine learning practice, catering to both classification and regression tasks. It facilitates model training, grid search application, and the preservation of the best model. Furthermore, it stores and visualizes the best scores attained by other models using commonly employed evaluation metrics.',
 package_dir={"": "src"},
 packages=find_packages('src'),
 long_description=long_description,
 long_description_content_type="text/markdown",
```

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/data_ingestion.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/data_transformation.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/data_transformation.py`

 * *Files identical despite different names*

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/components/model_trainer.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/components/model_trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,26 @@
     model_report_path = os.path.join("outputs",f"{basename_tag}report.json")
 
 class ModelTrainer:
     def __init__(self,
                  modeling_type = "reg",
                  output_base:str = "",
                  output_dir:str="outputs",
-                 param_finetune:bool = True
+                 param_finetune:bool = True,
+                 finetune_fraction:float = 1.0
                  ):
         self.model_trainer_config=ModelTrainerConfig()
         self.basename_tag = self.model_trainer_config.basename_tag
         self.output_base = output_base
         self.model_trainer_config.model_report_path = self.model_trainer_config.model_report_path.replace(self.basename_tag,f"{modeling_type}_{output_base}_")
         self.model_trainer_config.model_report_path = self.model_trainer_config.model_report_path.replace("outputs",f"{output_dir}")
         self.modeling_type = modeling_type
         self.output_dir = output_dir
         self.param_finetune = param_finetune
+        self.finetune_fraction = finetune_fraction
 
 
     def initiate_model_trainer(self,train_array,test_array):
         try:
             logging.info("Split training and test input data")
             X_train,y_train,X_test,y_test=(
                 train_array[:,:-1],
@@ -83,15 +85,16 @@
             model_report:dict=evaluate_models(X_train=X_train,
                                               y_train=y_train,
                                               X_test=X_test,
                                               y_test=y_test,
                                               models=models,
                                               param=params,
                                               modeling_type = self.modeling_type,
-                                              param_finetune = self.param_finetune
+                                              param_finetune = self.param_finetune,
+                                              finetune_fraction = self.finetune_fraction
                                               )
             
             ## To get best model score from dict
             best_model_score = 0
             best_model_name = ""
 
             for model_name in model_report:
```

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/exception.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/exception.py`

 * *Files identical despite different names*

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/params.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/params.py`

 * *Files identical despite different names*

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/run_train_pipeline.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/run_train_pipeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
                        no_standard_scaling:bool = False,
                        feature_selection:bool = False, 
                        feature_selection_method:str = "addition",
                        selectkbest_num_features: int = 32, 
                        output_dir:str = None,
                        return_data:bool = False,
                        no_param_finetune:bool = False,
+                       finetune_fraction:float = 1.0,
                        verbose:bool = True
                       ):
     """
     Function to facilitate the training of multiple machine learning models,
     optimize the models, and save the trained models. It also conducts model
     evaluation using diverse methods. Additionally, the function is capable
     of handling both regression and classification tasks.
@@ -69,13 +70,13 @@
         output_base = f" --output_base {output_base}"
     if no_param_finetune:
         no_param_finetune = " --no_param_finetune"
     else:
         no_param_finetune = ""
         
     # handle options
-    script = f"run_train_pipeline --input_file {input_file} --target_column {target_column} --selectkbest_num_features {selectkbest_num_features} --training_type {training_type} --test_size {test_size} --feature_selection_method {feature_selection_method} --output_dir {output_dir}" + feature_selection + engineer_new_features + no_standard_scaling + output_base + no_param_finetune
+    script = f"run_train_pipeline --input_file {input_file} --target_column {target_column} --selectkbest_num_features {selectkbest_num_features} --training_type {training_type} --test_size {test_size} --feature_selection_method {feature_selection_method} --output_dir {output_dir} --finetune_fraction {finetune_fraction}" + feature_selection + engineer_new_features + no_standard_scaling + output_base + no_param_finetune
 
     if verbose:
         print(script)
     # Your code to execute the training pipeline goes here
     os.system(script)
```

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/modules/utils.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/modules/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,33 +26,42 @@
 
         with open(file_path, "wb") as file_obj:
             pickle.dump(obj, file_obj)
 
     except Exception as e:
         raise CustomException(e, sys)
 
-def evaluate_models(X_train, y_train,X_test,y_test,models,param, modeling_type = "reg", param_finetune = True):
+def evaluate_models(X_train, y_train,X_test,y_test,models,param, modeling_type = "reg", param_finetune = True, finetune_fraction = 1.0):
     try:
         report = {}
 
         if modeling_type =="reg":
             kfold = KFold(n_splits=5, random_state=32, shuffle = True)
             scoring = "r2"
         else:
             kfold = StratifiedKFold(n_splits=5, random_state=32, shuffle = True)
             scoring = "accuracy"
 	
         for i in tqdm(range(len(list(models)))):
             model = list(models.values())[i]
             
+            print(finetune_fraction)
             if param_finetune:
+                print(finetune_fraction)
+                n_samples = int(finetune_fraction * 100)
+                X_train_cv = pd.DataFrame(X_train).sample(n_samples, random_state = 32).values
+                y_train_cv = pd.DataFrame(y_train).sample(n_samples, random_state = 32).values
+                print(X_train_cv.shape)
+
+
+
                 para=param[list(models.keys())[i]]
 
                 gs = GridSearchCV(model,para,cv=kfold, scoring = scoring)
-                gs.fit(X_train,y_train)
+                gs.fit(X_train_cv,y_train_cv)
                 model_best_params = gs.best_params_
                 model.set_params(**model_best_params)
 
             model.fit(X_train,y_train)
 
             #get cross validation and test report
             cross_val_report = get_cross_validation_scores(model, X_train,y_train, cv= kfold, training_type = modeling_type)
```

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack/train_pipeline.py` & `automated_ml_pack-1.0.7/src/automated_ml_pack/train_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     parser.add_argument('--no_standard_scaling', default = False, action="store_true", help='Whether or not to apply scikit-learn standard scaler on the data.')
     parser.add_argument('--feature_selection', default=False, action="store_true",help='Whether or not to perform feature selection on the dataset.')
     parser.add_argument('--feature_selection_method', type=str, default = "addition", choices = ["addition", "elimination"], help='Specify between recursive feature addition and recursive feature elimination algorithms for classification. By default, recursive feature addition is applied. For regression tasks, SelectKBest is used for feature selection.')
     parser.add_argument('--selectkbest_num_features', type=int, default = 32, help='Number of top features to select. For regression only.')
     parser.add_argument('--output_dir', type=str, default = "outputs", help='Custom Name of Output Folder.')
     parser.add_argument('--return_data', default = False, action="store_true", help='Select to include raw data, training data and test data in the output folders.')
     parser.add_argument('--no_param_finetune', default = False, action="store_true", help='If true, hyperparameter search will not be performed for each model. Otherwise, hyperparameter tunning is performed.')
+    parser.add_argument('--finetune_fraction', default = 1.0, help='Percentage of data used for fine tunning.')
+
+
 
     args = parser.parse_args()
 
     # Load dataframe from input file
     logging.info("Loading input data")
     try:
         if args.input_file:
@@ -85,14 +88,15 @@
         test_size = args.test_size
         standard_scaling = not args.no_standard_scaling
         feature_selection = args.feature_selection
         selectkbest_num_features = args.selectkbest_num_features
         output_dir = args.output_dir
         return_data = args.return_data
         param_finetune = not args.no_param_finetune
+        finetune_fraction = args.finetune_fraction
 
 
     except Exception as e:
         raise CustomException(e, sys)
     logging.info("Completed setting configurations!")
 
     obj=DataIngestion(input_data = data, 
@@ -118,15 +122,16 @@
                                            output_dir = output_dir
                                            )
     train_arr,test_arr,_,selected_columns, reverse_encode=data_transformation.initiate_data_transformation(train_data,test_data)
 
     modeltrainer=ModelTrainer(modeling_type = training_type,
                               output_base = output_base,
                               output_dir = output_dir,
-                              param_finetune = param_finetune
+                              param_finetune = param_finetune,
+                              finetune_fraction = finetune_fraction
                               )
 
     best_model_name, __ = modeltrainer.initiate_model_trainer(train_arr,test_arr)
     print(__)
 
     if training_type == "clf":
         # plot results
```

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/PKG-INFO` & `automated_ml_pack-1.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 Metadata-Version: 2.1
 Name: automated_ml_pack
-Version: 1.0.6
+Version: 1.0.7
 Summary: This package is designed for swift and automated machine learning practice, catering to both classification and regression tasks. It facilitates model training, grid search application, and the preservation of the best model. Furthermore, it stores and visualizes the best scores attained by other models using commonly employed evaluation metrics.
 Home-page: https://github.com/CyrilleMesue/automated_ml_pack
 Author: Cyrille
 Author-email: cyrillemesue@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: auto_mix_prep==0.2.0
-Requires-Dist: catboost==1.2.3
-Requires-Dist: dill==0.3.8
-Requires-Dist: feature_engine==1.6.2
-Requires-Dist: matplotlib==3.8.3
-Requires-Dist: numpy==1.26.4
-Requires-Dist: pandas==2.2.1
-Requires-Dist: scikit_learn==1.4.1.post1
-Requires-Dist: seaborn==0.13.2
-Requires-Dist: tqdm==4.66.2
-Requires-Dist: xgboost==2.0.3
 
 # AutomatedMLPack
 ## _A Comprehensive Package for Automated Machine Learning_
 [![scikit-learn](https://github.com/CyrilleMesue/archives/blob/main/images/mlpack.png?raw=true)](https://pypi.org/project/automated-ml-pack/)
 
 **Project Overview:**
 This package is designed for swift and automated machine learning practice, catering to both classification and regression tasks. It facilitates model training, grid search application, and the preservation of the best model. Furthermore, it stores and visualizes the best scores attained by other models using commonly employed evaluation metrics.    
@@ -78,15 +67,16 @@
                        test_size=0.2, 
                        no_standard_scaling=False,
                        feature_selection=False, 
                        feature_selection_method="addition",
                        selectkbest_num_features=32, 
                        output_dir="outputs",
                        verbose = True,
-                       no_param_finetune = False
+                       no_param_finetune = False,
+                       finetune_fraction = 1.0
                       )
 ```
 
 ### Command Line Interface
 
 ```USAGE```:     
 run_train_pipeline -[INPUT_FILE] [options]
@@ -115,14 +105,15 @@
                      Specify between recursive feature addition and recursive feature elimination algorithms for classification. By default, recursive feature addition is applied. For regression tasks, SelectKBest is used for feature selection.    
 ```--selectkbest_num_features``` SELECTKBEST_NUM_FEATURES
                      Number of top features to select. For regression only.     
 ```--output_dir``` OUTPUT_DIR   
                      Custom Name of Output Folder.     
 ```--return_data```         Select to include raw data, training data and test data in the output folders.    
 ```--no_param_finetune```    If true, hyperparameter search will not be performed for each model. Otherwise, hyperparameter tunning is performed.
+```--finetune_fraction```    Percentage of data used for fine tunning.
 
 ## Tutorials
 
 The data must be in csv or tsv format and the user must provide the column name that contains the targets. The following is an example of how the tool can be used for classification tasks.       
 
 ```sh
 run_train_pipeline --input_file heart.csv --target_column HeartDisease --training_type clf --test_size 0.2 --feature_selection --feature_selection_method addition --output_dir heart_disease_classification
```

### Comparing `automated_ml_pack-1.0.6/src/automated_ml_pack.egg-info/SOURCES.txt` & `automated_ml_pack-1.0.7/src/automated_ml_pack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

