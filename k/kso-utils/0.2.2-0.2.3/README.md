# Comparing `tmp/kso_utils-0.2.2.tar.gz` & `tmp/kso_utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kso_utils-0.2.2.tar", max compression
+gzip compressed data, was "kso_utils-0.2.3.tar", max compression
```

## Comparing `kso_utils-0.2.2.tar` & `kso_utils-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35126 2023-09-21 14:24:50.986126 kso_utils-0.2.2/LICENSE
--rw-r--r--   0        0        0    14312 2024-04-02 13:24:27.140946 kso_utils-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996729 kso_utils-0.2.2/kso_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996795 kso_utils-0.2.2/kso_utils/db_starter/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-02 13:24:18.424978 kso_utils-0.2.2/kso_utils/db_starter/cdn_projects_list.csv
--rw-r--r--   0        0        0     1461 2024-02-28 09:49:51.234739 kso_utils-0.2.2/kso_utils/db_starter/projects_list.csv
--rw-r--r--   0        0        0     1994 2024-04-02 13:24:18.425126 kso_utils-0.2.2/kso_utils/db_starter/schema.py
--rw-r--r--   0        0        0    17893 2024-04-02 13:24:18.425340 kso_utils-0.2.2/kso_utils/db_utils.py
--rw-r--r--   0        0        0     6741 2024-04-02 13:24:18.426034 kso_utils-0.2.2/kso_utils/frame_utils.py
--rw-r--r--   0        0        0     4091 2023-09-22 19:06:03.217864 kso_utils-0.2.2/kso_utils/general.py
--rw-r--r--   0        0        0    13317 2024-04-02 13:24:18.426336 kso_utils-0.2.2/kso_utils/koster_utils.py
--rw-r--r--   0        0        0    31563 2024-04-02 13:24:18.426758 kso_utils-0.2.2/kso_utils/movie_utils.py
--rw-r--r--   0        0        0    95930 2024-04-02 13:24:18.427610 kso_utils-0.2.2/kso_utils/project.py
--rw-r--r--   0        0        0     3606 2024-04-02 13:24:18.428216 kso_utils-0.2.2/kso_utils/project_utils.py
--rw-r--r--   0        0        0    14924 2024-04-02 13:24:18.428542 kso_utils-0.2.2/kso_utils/server_utils.py
--rw-r--r--   0        0        0     6295 2024-04-02 13:24:18.429109 kso_utils-0.2.2/kso_utils/sgu_utils.py
--rw-r--r--   0        0        0    10031 2024-04-02 13:24:18.429517 kso_utils-0.2.2/kso_utils/spyfish_utils.py
--rw-r--r--   0        0        0    13795 2024-04-02 13:24:18.430086 kso_utils-0.2.2/kso_utils/video_reader.py
--rw-r--r--   0        0        0    76147 2024-04-02 13:24:18.430796 kso_utils-0.2.2/kso_utils/widgets.py
--rw-r--r--   0        0        0    80905 2024-04-02 15:03:44.770676 kso_utils-0.2.2/kso_utils/yolo_utils.py
--rw-r--r--   0        0        0     3347 2023-09-21 14:24:50.998838 kso_utils-0.2.2/kso_utils/zenodo_utils.py
--rw-r--r--   0        0        0    85468 2024-04-02 13:24:18.432485 kso_utils-0.2.2/kso_utils/zooniverse_utils.py
--rw-r--r--   0        0        0     2535 2024-04-03 11:53:45.621712 kso_utils-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    15784 1970-01-01 00:00:00.000000 kso_utils-0.2.2/setup.py
--rw-r--r--   0        0        0    15879 1970-01-01 00:00:00.000000 kso_utils-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35126 2023-09-21 14:24:50.986126 kso_utils-0.2.3/LICENSE
+-rw-r--r--   0        0        0    14312 2024-04-02 13:24:27.140946 kso_utils-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996729 kso_utils-0.2.3/kso_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-21 14:24:50.996795 kso_utils-0.2.3/kso_utils/db_starter/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-02 13:24:18.424978 kso_utils-0.2.3/kso_utils/db_starter/cdn_projects_list.csv
+-rw-r--r--   0        0        0     1461 2024-02-28 09:49:51.234739 kso_utils-0.2.3/kso_utils/db_starter/projects_list.csv
+-rw-r--r--   0        0        0     1994 2024-04-02 13:24:18.425126 kso_utils-0.2.3/kso_utils/db_starter/schema.py
+-rw-r--r--   0        0        0    19167 2024-04-18 09:52:17.826297 kso_utils-0.2.3/kso_utils/db_utils.py
+-rw-r--r--   0        0        0     6741 2024-04-02 13:24:18.426034 kso_utils-0.2.3/kso_utils/frame_utils.py
+-rw-r--r--   0        0        0     4091 2023-09-22 19:06:03.217864 kso_utils-0.2.3/kso_utils/general.py
+-rw-r--r--   0        0        0    13317 2024-04-02 13:24:18.426336 kso_utils-0.2.3/kso_utils/koster_utils.py
+-rw-r--r--   0        0        0    31563 2024-04-02 13:24:18.426758 kso_utils-0.2.3/kso_utils/movie_utils.py
+-rw-r--r--   0        0        0    96393 2024-04-18 09:42:08.293845 kso_utils-0.2.3/kso_utils/project.py
+-rw-r--r--   0        0        0     3606 2024-04-02 13:24:18.428216 kso_utils-0.2.3/kso_utils/project_utils.py
+-rw-r--r--   0        0        0    14924 2024-04-02 13:24:18.428542 kso_utils-0.2.3/kso_utils/server_utils.py
+-rw-r--r--   0        0        0     6295 2024-04-02 13:24:18.429109 kso_utils-0.2.3/kso_utils/sgu_utils.py
+-rw-r--r--   0        0        0    10031 2024-04-02 13:24:18.429517 kso_utils-0.2.3/kso_utils/spyfish_utils.py
+-rw-r--r--   0        0        0    13795 2024-04-11 09:53:06.799605 kso_utils-0.2.3/kso_utils/video_reader.py
+-rw-r--r--   0        0        0    76147 2024-04-02 13:24:18.430796 kso_utils-0.2.3/kso_utils/widgets.py
+-rw-r--r--   0        0        0    81215 2024-04-03 13:05:07.486948 kso_utils-0.2.3/kso_utils/yolo_utils.py
+-rw-r--r--   0        0        0     3347 2023-09-21 14:24:50.998838 kso_utils-0.2.3/kso_utils/zenodo_utils.py
+-rw-r--r--   0        0        0    85468 2024-04-02 13:24:18.432485 kso_utils-0.2.3/kso_utils/zooniverse_utils.py
+-rw-r--r--   0        0        0     2535 2024-04-18 09:54:11.517050 kso_utils-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    15784 1970-01-01 00:00:00.000000 kso_utils-0.2.3/setup.py
+-rw-r--r--   0        0        0    15879 1970-01-01 00:00:00.000000 kso_utils-0.2.3/PKG-INFO
```

### Comparing `kso_utils-0.2.2/LICENSE` & `kso_utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/README.md` & `kso_utils-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/db_starter/cdn_projects_list.csv` & `kso_utils-0.2.3/kso_utils/db_starter/cdn_projects_list.csv`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/db_starter/projects_list.csv` & `kso_utils-0.2.3/kso_utils/db_starter/projects_list.csv`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/db_starter/schema.py` & `kso_utils-0.2.3/kso_utils/db_starter/schema.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/db_utils.py` & `kso_utils-0.2.3/kso_utils/db_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,14 +418,41 @@
 
     # Roadblock to prevent empty rows in id_columns
     test_table(local_df, init_key, [local_df.columns[0]])
 
     return local_df
 
 
+def check_basic_meta(csv_paths: dict, conn: sqlite3.Connection):
+    """
+    The function `check_basic_meta` reads CSV files, retrieves basic column names from a SQLite
+    database, selects relevant columns, and performs a data check before logging completion.
+
+    :param csv_paths: The `csv_paths` parameter is a dictionary where the keys represent meta keys and
+    the values represent file paths to CSV files containing movies information
+    :type csv_paths: dict
+    :param conn: sqlite3.Connection object representing a connection to a SQLite database
+    :type conn: sqlite3.Connection
+    """
+
+    for meta_key, meta_path in csv_paths.items():
+        # Remove extra information from key
+        meta_key = meta_key.split("_")[1]
+        # Load the csv with movies information
+        test_df = pd.read_csv(meta_path)
+        # Retrieve the names of the basic columns in the sql db
+        field_names = list(get_column_names_db(conn, meta_key).values())
+        # Select the basic fields for the db check
+        df_to_db = test_df[[c for c in test_df.columns if c in field_names]]
+        # Double-check to prevent missing key information
+        test_table(df_to_db, meta_key, df_to_db.columns)
+
+        logging.info(f"The {meta_key} dataframe is complete")
+
+
 def check_species_meta(csv_paths: dict, conn: sqlite3.Connection):
     """
     > The function `check_species_meta` loads the csv with species information and checks if it is empty
 
     :param csv_paths: a dictionary with the paths of the csv files with info to initiate the db
     :param conn: SQL connection object
     """
```

### Comparing `kso_utils-0.2.2/kso_utils/frame_utils.py` & `kso_utils-0.2.3/kso_utils/frame_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/general.py` & `kso_utils-0.2.3/kso_utils/general.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/koster_utils.py` & `kso_utils-0.2.3/kso_utils/koster_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/movie_utils.py` & `kso_utils-0.2.3/kso_utils/movie_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/project.py` & `kso_utils-0.2.3/kso_utils/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,17 @@
                 init_key=init_key,
             )
 
     #############
     # t1
     #############
 
+    def check_basic_meta(self):
+        return db_utils.check_basic_meta(csv_paths=self.csv_paths, conn=self.db_connection)
+
     def select_meta_range(self, meta_key: str):
         """
         > This function takes a meta key as input and returns a dataframe, range of rows, and range of
         columns
 
         :param meta_key: str
         :type meta_key: str
@@ -1042,19 +1045,19 @@
         # Add the site and movie information to the classifications based on the subject information
         class_df = zoo_utils.add_subject_site_movie_info_to_class(
             self.project, self.db_connection, self.csv_paths, class_df
         )
 
         # Download the processed classifications as a csv file
         csv_filename = (
-            self.project.csv_folder
-            + self.project.Project_name
+            self.project.Project_name
             + str(datetime.date.today())
             + "classifications.csv"
         )
+
         class_df.to_csv(csv_filename, index=False)
 
         logging.info(f"The classications have been downloaded to {csv_filename}")
 
     def get_annotations_viewer(self, folder_path: str, annotation_classes: list):
         """
         > This function takes in a folder path and a list of annotation classes and returns a widget that
@@ -1070,15 +1073,15 @@
                  - 'class': the class of the annotation
                  - 'bbox': the bounding box of the annotation
         """
         return yolo_utils.get_annotations_viewer(
             folder_path, species_list=annotation_classes
         )
 
-    def download_gbif_occurrences(self, classified_by, df):
+    def download_gbif_occurrences(self, classified_by, df, max_count=True):
         if classified_by == "citizen_scientists":
             # Add the site and movie information to the classifications based on the subject information
             df = zoo_utils.add_subject_site_movie_info_to_class(
                 self.project,
                 self.db_connection,
                 self.csv_paths,
                 df,
@@ -1090,21 +1093,35 @@
             self.db_connection,
             df,
             self.csv_paths,
             classified_by,
             self.zoo_info,
         )
 
+        if max_count:
+            # Group by species/date/location and get the maximum 'individualCount'
+            occurrence_df = (
+                occurrence_df.sort_values("individualCount", ascending=False)
+                .groupby(
+                    [
+                        "scientificName",
+                        "eventDate",
+                        "decimalLatitude",
+                        "decimalLongitude",
+                    ],
+                    as_index=False,
+                )
+                .first()
+            )
+
         # Download the processed classifications as a csv file
         csv_filename = (
-            self.project.csv_folder
-            + self.project.Project_name
-            + str(datetime.date.today())
-            + "occurrence.csv"
+            self.project.Project_name + str(datetime.date.today()) + "occurrence.csv"
         )
+
         occurrence_df.to_csv(csv_filename, index=False)
 
         logging.info(f"The occurences have been downloaded to {csv_filename}")
 
     def process_detections(
         self,
         project,
@@ -1152,18 +1169,15 @@
 
     #############
     # t9
     #############
     def download_detections_csv(self, df):
         # Download the processed detections as a csv file
         csv_filename = (
-            self.project.csv_folder
-            + self.project.Project_name
-            + str(datetime.date.today())
-            + "detections.csv"
+            self.project.Project_name + str(datetime.date.today()) + "detections.csv"
         )
 
         df.to_csv(csv_filename, index=False)
 
         logging.info(f"The detections have been downloaded to {csv_filename}")
 
     def download_detections_species_cols_csv(self, df):
@@ -1236,18 +1250,15 @@
         sorted_columns = columns_no_sp_group + columns_sp_group
 
         # Select the cols based on the sorted list
         merged_df = merged_df[sorted_columns]
 
         # Download the processed detections as a csv file
         csv_filename = (
-            self.project.csv_folder
-            + self.project.Project_name
-            + str(datetime.date.today())
-            + "detections.csv"
+            self.project.Project_name + str(datetime.date.today()) + "detections.csv"
         )
 
         merged_df.to_csv(csv_filename, index=False)
 
         logging.info(
             f"The detections organised by species cols have been downloaded to {csv_filename}"
         )
```

### Comparing `kso_utils-0.2.2/kso_utils/project_utils.py` & `kso_utils-0.2.3/kso_utils/project_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/server_utils.py` & `kso_utils-0.2.3/kso_utils/server_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/sgu_utils.py` & `kso_utils-0.2.3/kso_utils/sgu_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/spyfish_utils.py` & `kso_utils-0.2.3/kso_utils/spyfish_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/video_reader.py` & `kso_utils-0.2.3/kso_utils/video_reader.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/widgets.py` & `kso_utils-0.2.3/kso_utils/widgets.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/yolo_utils.py` & `kso_utils-0.2.3/kso_utils/yolo_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1935,24 +1935,24 @@
     else:
         logging.info(filtered_df["class_id"].value_counts())
     return filtered_df.to_csv(str(Path(tracking_folder, "tracking_clean.csv")))
 
 
 # Auxiliary function to obtain a dictionary with the mapping between the class ids used by the detection model and the species names
 def get_species_mapping(model, project_name, team_name="koster", registry="wandb"):
-    
     import yaml
 
     def read_yaml_file(file_path):
         with open(file_path, "r") as file:
             yaml_data = yaml.safe_load(file)
         return yaml_data
-    
+
     if registry == "wandb":
         import wandb
+
         api = wandb.Api()
 
         full_path = f"{team_name}/{project_name}"
         runs = api.runs(full_path)  # Get all runs in the project
         for r in runs:
             # Choose the run corresponding to the model given as parameter
             if r.id == model.split("_")[1]:
@@ -1974,25 +1974,36 @@
                 logging.error("Error reading species mapping from config or file.")
                 species_mapping = {}
     elif registry == "mlflow":
         from mlflow import MlflowClient
 
         experiment = mlflow.get_experiment_by_name(project_name)
         client = MlflowClient()
-        pattern = r'runs:/([^/]+)/weights/best\.pt'
+        pattern = r"runs:/([^/]+)/weights/best\.pt"
         # Use re.search() to find the match
         try:
             run_id = re.search(pattern, model).group(1)
         except:
             logging.error("No valid run found.")
         if experiment is not None:
-            artifacts = client.list_artifacts(run_id)
-            yaml_fpath = [af for af in artifacts if ".yaml" in af]
+            # Get the path of the artifact with the labels and class_id
+            artifacts = client.list_artifacts(run_id, path="input_datasets")
+            run = mlflow.get_run(run_id)
+            artifact_uri = run.info.artifact_uri
+            yaml_fpath = [
+                Path(artifact_uri, af.path)
+                for af in artifacts
+                if ".yaml" in af.path and "hyp.yaml" not in af.path
+            ][0]
+
+            # Temporarily download the artifact with mapping labels
+            local_artifact = mlflow.artifacts.download_artifacts(str(yaml_fpath))
+
             # Attempt to read species mapping from a YAML file specified in the configuration
-            data_dict = read_yaml_file(yaml_fpath)
+            data_dict = read_yaml_file(local_artifact)
             species_mapping = data_dict["names"]
             species_mapping = {str(i): sp for i, sp in enumerate(species_mapping)}
     else:
         logging.error("Registry invalid.")
 
     return species_mapping
 
@@ -2065,34 +2076,29 @@
 
     # Map the class id to species labels
     if model_registry == "wandb":
         # Set the name of the template project
         if project_name == "template_project":
             project_name = "spyfish_aotearoa"
 
-        # Obtain a dictionary with the mapping between the class ids and the species names
-        species_mapping = get_species_mapping(model, project_name, team_name)
-
-        # Add a column with the species name corresponding to each class id
-        df["commonName"] = df["class_id"].astype(str).map(species_mapping)
-
-        # Define the movie col of interest
-        sp_group_col = "commonName"
+    # Obtain a dictionary with the mapping between the class ids and the species names
+    species_mapping = get_species_mapping(
+        model, project_name, team_name, model_registry
+    )
 
-    else:
-        # Define the movie col of interest
-        sp_group_col = "class_id"
+    # Add a column with the species name corresponding to each class id
+    df["commonName"] = df["class_id"].astype(str).map(species_mapping)
 
     # Get max_n per class detected in each movie per frame
-    df["max_n"] = df.groupby([movie_group_col, "frame_no"])[sp_group_col].transform(
+    df["max_n"] = df.groupby([movie_group_col, "frame_no"])["commonName"].transform(
         "count"
     )
 
     # Specify the columns for which we want unique confidence values
-    columns_conf = [movie_group_col, "frame_no", sp_group_col]
+    columns_conf = [movie_group_col, "frame_no", "commonName"]
 
     # Get the confidence range of each detection per frame and add three columns
     df["min_conf"] = df.groupby(columns_conf)["conf"].transform("min")
     df["mean_conf"] = df.groupby(columns_conf)["conf"].transform("mean")
     df["max_conf"] = df.groupby(columns_conf)["conf"].transform("max")
 
     # Create a boolean mask for duplicated rows based on the specified columns
@@ -2186,15 +2192,15 @@
     )
 
     # Group by n-second intervals
     interval = pd.Grouper(key="seconds_since_reference", freq=str(int_length) + "S")
 
     # Group by species and minute, calculate the count
     max_count_per_species = (
-        df.groupby(["movie_id", "class_id", interval])["max_n"].max().reset_index()
+        df.groupby(["movie_id", "commonName", interval])["max_n"].max().reset_index()
     )
 
     # Enable plotting of matplotlib
     try:
         # Enable inline plotting for Matplotlib
         get_ipython().magic("matplotlib inline")
     except ImportError:
@@ -2211,19 +2217,19 @@
 
     for movie_id in movies:
         movie_data = max_count_per_species[
             max_count_per_species["movie_id"] == movie_id
         ]
 
         # Create a separate line plot for each species
-        species_list = movie_data["class_id"].unique()
+        species_list = movie_data["commonName"].unique()
         plt.figure(figsize=(10, 6))
 
         for species in species_list:
-            species_data = movie_data[movie_data["class_id"] == species]
+            species_data = movie_data[movie_data["commonName"] == species]
             plt.plot(
                 species_data["seconds_since_reference"],
                 species_data["max_n"],
                 label=species,
             )
 
             plt.xlabel("Timestamp (seconds)")
```

### Comparing `kso_utils-0.2.2/kso_utils/zenodo_utils.py` & `kso_utils-0.2.3/kso_utils/zenodo_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/kso_utils/zooniverse_utils.py` & `kso_utils-0.2.3/kso_utils/zooniverse_utils.py`

 * *Files identical despite different names*

### Comparing `kso_utils-0.2.2/pyproject.toml` & `kso_utils-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kso_utils"
-version = "0.2.2"
+version = "0.2.3"
 description = "A package containing utility scripts for use with KSO analysis notebooks."
 authors = ["Jurie Germishuys <jurie.germishuys@combine.se>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "kso_utils"}]
 
 [tool.poetry.dependencies]
```

### Comparing `kso_utils-0.2.2/setup.py` & `kso_utils-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  'split-folders==0.5.1',
  'tqdm==4.64.1',
  'ultralytics==8.0.200',
  'wandb==0.13.2']
 
 setup_kwargs = {
     'name': 'kso-utils',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'A package containing utility scripts for use with KSO analysis notebooks.',
     'long_description': '# KSO System\n\nThe Koster Seafloor Observatory is an open-source, citizen science and machine learning approach to analyse subsea movies.\n\n<!-- PROJECT SHIELDS -->\n<!--\n*** I\'m using markdown "reference style" links for readability.\n*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).\n*** See the bottom of this document for the declaration of the reference variables\n*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.\n*** https://www.markdownguide.org/basic-syntax/#reference-style-links\n-->\n[![Contributors][contributors-shield]][contributors-url]\n[![Forks][forks-shield]][forks-url]\n[![Stargazers][stars-shield]][stars-url]\n[![Issues][issues-shield]][issues-url]\n[![GPL License][license-shield]][license-url]\n\n### KSO overview\nThe KSO system has been developed to:\n* move and process underwater footage and its associated data (e.g. location, date, sampling device).\n* make this data available to citizen scientists in Zooniverse to annotate the data.\n* train and evaluate machine learning models (customise [Yolov5][YoloV5] or [Yolov8][YoloV8] models).\n  \n![koster_info_diag][high-level-overview]\n\nThe system is built around a series of easy-to-use [Jupyter Notebooks][Jupyter_site]. Each notebook allows users to perform a specific task of the system (e.g. upload footage to the citizen science platform or analyse the classified data).\n\nUsers can run these notebooks via Google Colab (by clicking on the Colab links in the table below), locally or on a High-Performance Computer environment.\n\n### Notebooks\n| Name                                              | Description                                                                                 | Try it!  | \n| ------------------------------------------------- | ------------------------------------------------------------------------------------------- | --------|\n| 1. Check footage and metadata                     | Check format and contents of footage and sites, media and species csv files                 | [![Open In Colab][colablogo]][colab_tut_1] [![binder][binderlogo]][binder_tut] | \n| 2. Upload new media to the system*                | Upload new underwater media to the cloud/server and update the csv files                    | WIP | \n| 3. Upload clips to Zooniverse                     | Prepare original footage and upload short clips to Zooniverse                               | [![Open In Colab][colablogo]][colab_tut_3] [![binder][binderlogo]][binder_tut] |\n| 4. Upload frames to Zooniverse                    | Extract frames of interest from the original footage and upload them to Zooniverse              | [![Open In Colab][colablogo]][colab_tut_4] [![binder][binderlogo]][binder_tut] |\n| 5. Train ML models                                | Prepare the training and test data, set model parameters and train models                   | [![Open In Colab][colablogo]][colab_tut_5] [![binder][binderlogo]][binder_tut] | \n| 6. Evaluate ML models                            | Use ecologically relevant metrics to test the models                                        | [![Open In Colab][colablogo]][colab_tut_6] [![binder][binderlogo]][binder_tut]   |\n| 7. Publish ML models                               | Publish the model to a public repository                                                   | [![Open In Colab][colablogo]][colab_tut_7] [![binder][binderlogo]][binder_tut]  | \n| 8. Analyse Zooniverse classifications             | Pull and analyse up-to-date classifications from Zooniverse and export observations to GBIF             | [![Open In Colab][colablogo]][colab_tut_8] [![binder][binderlogo]][binder_tut] |\n| 9. Run ML models on footage                      | Automatically classify new footage and export observations to GBIF                                                          | [![Open In Colab][colablogo]][colab_tut_9] [![binder][binderlogo]][binder_tut] |\n\n  \n\\* Project-specific notebook\n\n## Local Installation\n\n### Docker Installation\n#### Requirements\n* [Docker](https://www.docker.com/products/docker-desktop/)\n\n#### Pull KSO Docker image\n```\nBash\ndocker pull ghcr.io/ocean-data-factory-sweden/kso:dev\n```\n\n### Conda Installation\n#### Requirements\n* [Python 3.8](https://www.python.org/)\n* [Anaconda](https://docs.anaconda.com/anaconda/install/index.html)\n* [GIT](https://git-scm.com/downloads)\n\n#### Download this repository\nClone this repository using\n```python\ngit clone https://github.com/ocean-data-factory-sweden/kso.git\n``` \n\n#### Prepare your system\nDepending on your system (Windows/Linux/MacOS), you might need to install some extra tools. If this is the case, you will get a message about what you need to install in the next steps. \nFor example, [Microsoft Build Tools C++][Microsoft_C++] with a version higher than 14.0 is required for Windows systems.\n\n#### Set up the environment with Conda\n1. Open the Anaconda Prompt\n2. Navigate to the folder where you have cloned the repository or unzipped the manually downloaded repository. Then go into the kso folder.\n```\ncd kso\n```\n\n3. Create an Anaconda environment with Python 3.8. Remember to change the name env.\n```\nconda create -n <name env> python=3.8\n```\n\n4. Enter the environment: \n```\nconda activate <name env>\n```\n\n5. Specify your GPU details.\n\n  5a. Find out the [pytorch][pytorch] installation you need. Navigate to the system options (example below) and select your device/platform details.\n  <div style="text-align: center;">\n    <img src="https://github.com/ocean-data-factory-sweden/kso/blob/dev/assets/cuda_gpu_example_requirements.png?raw=true" alt="CUDA Requirements" width="450" height="150">\n  </div>\n  \n  5b. Add the recommended command to the KSO\'s gpu_requirements_user.txt file.\n\n6. Install all the requirements:\n```\npip install -r requirements.txt -r gpu_requirements_user.txt\n```\n\n## Cloudina \nCloudina is a hosted version of KSO (powered by JupyterHub) on NAISS Science Cloud. It allows users to scale and automate larger workflows using a powerful processing backend. This is currently an invitation-only service. To access the platform, please contact jurie.germishuys[at]combine.se.\n\nThe current portals are accessible as:\n1. Console (object storage) - [storage][cdn_bucket]\n2. Album (JupyterHub) - [notebooks][cdn_album]\n3. Vendor (MLFlow) - [mlflow][cdn_vendor]\n\n\n## Starting a new project\nTo start a new project you will need to:\n1. Create initial information for the database: Input the information about the underwater footage files, sites and species of interest. You can use a [template of the csv files](https://drive.google.com/file/d/1PZGRoSY_UpyLfMhRphMUMwDXw4yx1_Fn/view?usp=sharing) and move the directory to the "db_starter" folder.\n2. Link your footage to the database: You will need files of underwater footage to run this system. You can [download some samples](https://drive.google.com/drive/folders/1t2ce8euh3SEU2I8uhiZN1Tu-76ZDqB6w?usp=sharing) and move them to `db_starter`. You can also store your own files and specify their directory in the notebooks.\n\nPlease remember the format of the underwater media is standardised (typically .mp4 or .jpg) and the associated metadata captured in three CSV files (“movies”, “sites” and “species”) should follow the [Darwin Core standards (DwC)](https://dwc.tdwg.org/simple/). \n\n## Developer instructions\nIf you would like to expand and improve the KSO capabilities, please follow the instructions above to set the project up on your local computer.\n\nWhen you add any changes, please create your branch on top of the current \'dev\' branch. Before submitting a Merge Request, please:\n* Run Black on the code you have edited \n```shell\nblack filename \n```\n* Clean up your commit history on your branch, so that every commit represents a logical change. (so squash and edit commits so that it is understandable for others)\n* For the commit messages, we ask that you please follow the [conventional commits guidelines](https://www.conventionalcommits.org/en/v1.0.0/) (table below) to facilitate code sharing. Also, please describe the logic behind the commit in the body of the message.\n  #### Commit types\n\n| Commit Type | Title                    | Description                                                                                                 | Emoji | \n|:-----------:|--------------------------|-------------------------------------------------------------------------------------------------------------|:-----:|\n|   `feat`    | Features                 | A new feature                                                                                               |   ✨   |       \n|    `fix`    | Bug Fixes                | A bug Fix                                                                                                   |  🐛   |      \n|   `docs`    | Documentation            | Documentation only changes                                                                                  |  📚   |        \n|   `style`   | Styles                   | Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)      |  💎   |         \n| `refactor`  | Code Refactoring         | A code change that neither fixes a bug nor adds a feature                                                   |  📦   |         \n|   `perf`    | Performance Improvements | A code change that improves performance                                                                     |  🚀   |         \n|   `test`    | Tests                    | Adding missing tests or correcting existing tests                                                           |  🚨   |         \n|   `build`   | Builds                   | Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)         |  🛠   |       \n|    `ci`     | Continuous Integrations  | Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs) |  ⚙️   |       \n|   `chore`   | Chores                   | Other changes that don\'t modify src or test files                                                           |  ♻️   |        \n|  `revert`   | Reverts                  | Reverts a previous commit                                                                                   |  🗑   |        \n\n* Rebase on top of dev. (never merge, only use rebase)\n* Submit a Pull Request and link at least 2 reviewers\n\n\n## Citation\n\nIf you use this code or its models in your research, please cite:\n\nAnton V, Germishuys J, Bergström P, Lindegarth M, Obst M (2021) An open-source, citizen science and machine learning approach to analyse subsea movies. Biodiversity Data Journal 9: e60548. https://doi.org/10.3897/BDJ.9.e60548\n\n## Collaborations/Questions\nYou can find out more about the project at https://subsim.wnmedia.se.\n\nWe are always excited to collaborate and help other marine scientists. Please feel free to contact us (matthias.obst(at)marine.gu.se) with your questions.\n\n## Troubleshooting\n\nIf you experience issues with the Panoptes package and/or uploading movies to Zooniverse, it might be related to the libmagic package. In Windows, the following commands might fix the issue:\n```python\npip install python-libmagic\npip install python-magic-bin\n```\n\n<!-- MARKDOWN LINKS & IMAGES -->\n<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->\n[contributors-shield]: https://img.shields.io/github/contributors/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[contributors-url]: https://https://github.com/ocean-data-factory-sweden/kso/graphs/contributors\n[forks-shield]: https://img.shields.io/github/forks/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[forks-url]: https://github.com/ocean-data-factory-sweden/kso/network/members\n[stars-shield]: https://img.shields.io/github/stars/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[stars-url]: https://github.com/ocean-data-factory-sweden/kso/stargazers\n[issues-shield]: https://img.shields.io/github/issues/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[issues-url]: https://github.com/ocean-data-factory-sweden/kso/issues\n[license-shield]: https://img.shields.io/github/license/ocean-data-factory-sweden/kso.svg?style=for-the-badge\n[license-url]: https://github.com/ocean-data-factory-sweden/kso/blob/main/LICENSE.txt\n[high-level-overview]: https://github.com/ocean-data-factory-sweden/kso/blob/main/assets/high-level-overview.png?raw=true\n[Jupyter_site]: https://jupyter.org/\n[colablogo]: https://colab.research.google.com/assets/colab-badge.svg\n[binderlogo]: https://mybinder.org/badge_logo.svg\n[colab_tut_1]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/01_Check_and_update_csv_files.ipynb\n[binder_tut]: https://mybinder.org/v2/gh/ocean-data-factory-sweden/kso/main\n[colab_tut_2]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/02_Upload_new_footage.ipynb\n[colab_tut_3]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/03_Upload_clips_to_Zooniverse.ipynb\n[colab_tut_4]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/04_Upload_frames_to_Zooniverse.ipynb\n[colab_tut_5]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/05_Train_ML_models.ipynb\n[colab_tut_6]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/06_Evaluate_ML_Models.ipynb\n[colab_tut_7]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/07_Transfer_ML_Models.ipynb\n[colab_tut_8]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/08_Analyse_Aggregate_Zooniverse_Annotations.ipynb\n[colab_tut_9]: https://colab.research.google.com/github/ocean-data-factory-sweden/kso/blob/dev/notebooks/09_Run_ML_Models_on_footage.ipynb\n[Microsoft_C++]: https://visualstudio.microsoft.com/visual-cpp-build-tools/\n[pytorch]: https://pytorch.org/\n[YoloV5]: https://github.com/ultralytics/yolov5\n[YoloV8]: https://github.com/ultralytics/ultralytics\n[cdn_bucket]: https://console.cloudina.org/\n[cdn_album]: https://album.cloudina.org/\n[cdn_vendor]: https://vendor.cloudina.org/\n',
     'author': 'Jurie Germishuys',
     'author_email': 'jurie.germishuys@combine.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kso_utils-0.2.2/PKG-INFO` & `kso_utils-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kso-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: A package containing utility scripts for use with KSO analysis notebooks.
 License: MIT
 Author: Jurie Germishuys
 Author-email: jurie.germishuys@combine.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

