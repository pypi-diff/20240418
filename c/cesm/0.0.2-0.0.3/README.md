# Comparing `tmp/cesm-0.0.2-py3-none-any.whl.zip` & `tmp/cesm-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17617 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat     7557 b- defN 24-Apr-11 15:21 cesm.py
+Zip file size: 17781 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat     6695 b- defN 24-Apr-17 17:58 cesm.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Oct-24 14:59 Core/__init__.py
 -rw-rw-rw-  2.0 fat    12046 b- defN 24-Apr-16 15:04 Core/data_access.py
 -rw-rw-rw-  2.0 fat    12672 b- defN 24-Apr-17 12:35 Core/input_parser.py
 -rw-rw-rw-  2.0 fat    19682 b- defN 24-Apr-16 13:57 Core/model.py
 -rw-rw-rw-  2.0 fat     2035 b- defN 24-Apr-16 09:39 Core/params.py
 -rw-rw-rw-  2.0 fat    12206 b- defN 24-Apr-11 15:21 Core/plotter.py
--rw-rw-rw-  2.0 fat     1118 b- defN 24-Apr-17 14:32 cesm-0.0.2.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat      533 b- defN 24-Apr-17 14:32 cesm-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 14:32 cesm-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-17 14:32 cesm-0.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-17 14:32 cesm-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      969 b- defN 24-Apr-17 14:32 cesm-0.0.2.dist-info/RECORD
-13 files, 68954 bytes uncompressed, 16031 bytes compressed:  76.8%
+-rw-rw-rw-  2.0 fat     1118 b- defN 24-Apr-17 19:32 cesm-0.0.3.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat     1251 b- defN 24-Apr-17 19:32 cesm-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-17 19:32 cesm-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       34 b- defN 24-Apr-17 19:32 cesm-0.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       10 b- defN 24-Apr-17 19:32 cesm-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      970 b- defN 24-Apr-17 19:32 cesm-0.0.3.dist-info/RECORD
+13 files, 68811 bytes uncompressed, 16195 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: Core/params.py
 Comment: 
 
 Filename: Core/plotter.py
 Comment: 
 
-Filename: cesm-0.0.2.dist-info/LICENSE.md
+Filename: cesm-0.0.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: cesm-0.0.2.dist-info/METADATA
+Filename: cesm-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cesm-0.0.2.dist-info/WHEEL
+Filename: cesm-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cesm-0.0.2.dist-info/entry_points.txt
+Filename: cesm-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: cesm-0.0.2.dist-info/top_level.txt
+Filename: cesm-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cesm-0.0.2.dist-info/RECORD
+Filename: cesm-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cesm.py

```diff
@@ -4,112 +4,93 @@
 #  mail@juliabarbosa.net
 # -------------------------------------------------- 
 
 import click
 import os
 import time 
 from pathlib import Path
-
+from distutils.dir_util import copy_tree
+import pkg_resources
 from InquirerPy import prompt
 
 # -- internal imports -- #
 from Core.input_parser import Parser
 from Core.model import Model
-# from Core.datacls import save_input_output, read_input_output
 from Core.plotter import Plotter, PlotType
 from Core.data_access import DAO
 import sqlite3
 
 # Constants
+DATA_DIR_PATH = Path(".").joinpath('Data')
 TECHMAP_DIR_PATH = Path(".").joinpath('Data', 'Techmap')
 TS_DIR_PATH = Path(".").joinpath('Data', 'TimeSeries')
 RUNS_DIR_PATH = Path(".").joinpath('Runs')
+
 FNAME_MODEL = 'db.sqlite'
 # -- Helpers -- #
 def get_existing_models():
       """Return a list of existing models"""
-      files = os.listdir(TECHMAP_DIR_PATH)
+      # files = os.listdir(TECHMAP_DIR_PATH)
+      files = [file.name for file in TECHMAP_DIR_PATH.glob("*") if file.is_file()]
       return [tm.split('.')[0] for tm in files if tm.endswith('.xlsx')]
 
-class ModelChoice(click.Choice):
-    def convert(self, value, param, ctx):
-         try:
-               return super().convert(value, param, ctx)
-         except click.exceptions.BadParameter:
-               # print each model in one line   
-               available_models = '\n\t '.join(get_existing_models())
-               raise click.BadParameter(f"Model {value} not found.\n \tAvailable models are:\n\t {available_models}")
-
 def get_runs():
    """Return a list of existing runs"""
-   return os.listdir(RUNS_DIR_PATH)
-
-class RunsChoice(click.Choice):
-   def convert(self, value, param, ctx):
-      try:
-         return super().convert(value, param, ctx)
-      except click.exceptions.BadParameter:
-         # print each model in one line   
-         available_runs = '\n\t '.join(get_runs())
-         raise click.BadParameter(f"Run {value} not found.\n \tComputed model runs are:\n\t {available_runs}")
+   return [entry.name for entry in RUNS_DIR_PATH.iterdir() if entry.is_dir()]
 
 def get_list_inquirer_choices(choices, name=None, message=None, type='list'):
    """Return a dict of choices in the format required by PyInquirer"""
    return {
       'type': type,
       'name': name,
       'message': message,
       'choices': choices,
    }
 
-def prompt_commodities(doa):
-      cos = [str(c) for c in doa.get_set("commodity")]
+def prompt_commodities(dao):
+      cos = [str(c) for c in dao.get_set("commodity")]
       # remove Dummy
       cos.remove('Dummy')
 
       return prompt(get_list_inquirer_choices(cos, name='commodities', type='checkbox', message='Select commodities: Select with spacebar and confirm with enter'))['commodities']
 
-def prompt_years(doa):
-    yy = [int(y) for y in doa.get_set("year")]
+def prompt_years(dao):
+    yy = [int(y) for y in dao.get_set("year")]
     return prompt(get_list_inquirer_choices(yy, name='years', type='checkbox', message='Select years: Select with spacebar and confirm with enter'))['years']
    
 
 # -- Main CLI Application -- #
 @click.group()
 def app():
    """Welcome to the Compact Energy System Modelling Tool (CESM)"""
-   
+
 @app.command(name='run')
-@click.option("--model_name",'-m', type=ModelChoice(get_existing_models()))
-@click.option("--scenario",'-s', type=click.STRING)
-def run(model_name, scenario):
+def run():
    """Run the Model"""
-   print(f'Running model {model_name} with scenario {scenario}')
+   # print(f'Running model {model_name} with scenario {scenario}')
 
    # If no scenario or model is provided, prompt the user to choose one
-   if model_name is None:
-      model_name = prompt(get_list_inquirer_choices(get_existing_models(), name='model_name', message='Please choose a model to run'))['model_name']
-   if scenario is None:
-      scenario = click.prompt('Please enter a scenario name', type=click.STRING)
+   # if model_name is None:
+   model_name = prompt(get_list_inquirer_choices(get_existing_models(), name='model_name', message='Please choose a model to run'))['model_name']
+   # if scenario is None:
+   scenario = click.prompt('Please enter a scenario name', type=click.STRING)
 
    # Create a directory for the model if it does not exist
    db_dir_path = RUNS_DIR_PATH.joinpath(model_name+'-'+scenario)
    if not os.path.exists(db_dir_path):
       os.mkdir(db_dir_path)
 
    # Create and Run the model
    conn = sqlite3.connect(":memory:")
    parser = Parser(model_name, techmap_dir_path=TECHMAP_DIR_PATH, ts_dir_path=TS_DIR_PATH, db_conn = conn, scenario = scenario)
-   # (self, name, techmap_dir_path, ts_dir_path, db_conn, scenario)
 
    # Parse
    print("\n#-- Parsing started --#")
    st = time.time()
    parser.parse()
-   # model_input = parser.get_input()
    print(f"Parsing finished in {time.time()-st:.2f} seconds")
 
    # Build
    print("\n#-- Building model started --#")
    st = time.time()
    model_instance = Model(conn=conn)
    print(f"Building model finished in {time.time()-st:.2f} seconds")
@@ -131,28 +112,22 @@
       # Delete the file using unlink()
       db_path.unlink()
    
    # write the in-memory db to disk
    disk_db_conn = sqlite3.connect(db_path)
    conn.backup(disk_db_conn)
    
-
-   
-   # save_input_output(input=model_input, output=model_output,filename=os.path.join(path, FNAME_MODEL))
    print(f"Saving model finished in {time.time()-st:.2f} seconds")
      
 @app.command(name='plot')
-@click.option("--simulation", '-s', type=RunsChoice(get_runs()), help="Name of the simulation to visualize. If not provided user will be prompted to choose one.")
-def plot(simulation):
+def plot():
    """Visualize the results of a simulation"""
 
-   if simulation is None:
-      simulation = prompt(get_list_inquirer_choices(get_runs(), name='simulation', message='Please choose a simulation to visualize'))['simulation'] 
+   simulation = prompt(get_list_inquirer_choices(get_runs(), name='simulation', message='Please choose a simulation to visualize'))['simulation'] 
       
-
    print(f"Visualizing simulation {simulation}")
    db_path = os.path.join(RUNS_DIR_PATH, simulation, FNAME_MODEL)
    conn = sqlite3.connect(db_path)
    dao = DAO(conn)
    
    st = time.time()
    plotter = Plotter(dao)
@@ -198,11 +173,19 @@
 
       more_plots = prompt(get_list_inquirer_choices(['yes', 'no'], name='more_plots', message='Would you like to plot more?'))['more_plots']
       if more_plots == 'no':
          break
    
    click.echo("Plotting finished!")
 
+@app.command(name='init')
+def initialize():
+   print("Initializing CESM...")
+   RUNS_DIR_PATH.mkdir(exist_ok=True)
+   if not DATA_DIR_PATH.exists():
+      DATA_DIR_PATH.mkdir()
+      data_folder_path = pkg_resources.resource_filename('cesm', 'Data')
+      copy_tree(data_folder_path, str(Path(".").joinpath("Data").absolute()))
+   print("Data files are successfully structured.")
 
 if __name__ == "__main__":
-   app()
-   pass
+   app()
```

## Comparing `cesm-0.0.2.dist-info/LICENSE.md` & `cesm-0.0.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cesm-0.0.2.dist-info/RECORD` & `cesm-0.0.3.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-cesm.py,sha256=Ae2FQMC7yN3cXG6KO6vMp7FAbwaM0Vq8M9KTc0xQJRo,7557
+cesm.py,sha256=_cVy1-xYMNl8qr8sp2KxAszZmV6wEiPe2eW5MAOJyJQ,6695
 Core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 Core/data_access.py,sha256=szVUTS3dpBSnj4OcO0T0KVkCJ-TdWMM0dNbXTNBgXlc,12046
 Core/input_parser.py,sha256=Bnxh8EllDXqMr2PecAb-RUkumFP_iSpASdmDdcEWAuI,12672
 Core/model.py,sha256=LJfduEJK-5-wEVMZSEmWWvzM_6IULdmmgZ2goXwlSRk,19682
 Core/params.py,sha256=DI8PZTfkXQDcqOlrRiMdWyvlkpDDh0XTOeVD7g_V3GY,2035
 Core/plotter.py,sha256=vEwEQLC82OvMN4dJnDufEUavaWkGg0bvs3aPaKsfaf4,12206
-cesm-0.0.2.dist-info/LICENSE.md,sha256=LV5sU4ueYgsWnKk6NuoLsuvzjUKBi9eImXu3dUbvyrA,1118
-cesm-0.0.2.dist-info/METADATA,sha256=mZOouEwd338hLYFXaTYmegclHHf7O28nsk-Oythdj9I,533
-cesm-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cesm-0.0.2.dist-info/entry_points.txt,sha256=7dUJ2Xb90-mnaZVMgeTRSB0VqIAVHdsRhr_XSwmKoHI,34
-cesm-0.0.2.dist-info/top_level.txt,sha256=lhrufen9CviFDPfab0ivOpAVDidZ_6BKtTxMrgftI20,10
-cesm-0.0.2.dist-info/RECORD,,
+cesm-0.0.3.dist-info/LICENSE.md,sha256=LV5sU4ueYgsWnKk6NuoLsuvzjUKBi9eImXu3dUbvyrA,1118
+cesm-0.0.3.dist-info/METADATA,sha256=sh8pZDbt6HjdCA6QbYiey5-YQcC78XLZuGkeATdGJ8s,1251
+cesm-0.0.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cesm-0.0.3.dist-info/entry_points.txt,sha256=7dUJ2Xb90-mnaZVMgeTRSB0VqIAVHdsRhr_XSwmKoHI,34
+cesm-0.0.3.dist-info/top_level.txt,sha256=lhrufen9CviFDPfab0ivOpAVDidZ_6BKtTxMrgftI20,10
+cesm-0.0.3.dist-info/RECORD,,
```

