# Comparing `tmp/easydock-0.3.0.tar.gz` & `tmp/easydock-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easydock-0.3.0.tar", last modified: Thu Mar 14 10:22:38 2024, max compression
+gzip compressed data, was "dist/easydock-0.3.1.tar", last modified: Thu Apr 18 19:11:26 2024, max compression
```

## Comparing `easydock-0.3.0.tar` & `easydock-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-14 10:22:38.000000 easydock-0.3.0/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2023-07-31 13:35:52.000000 easydock-0.3.0/LICENSE.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    12886 2024-03-14 10:22:38.000000 easydock-0.3.0/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2024-03-14 10:22:38.000000 easydock-0.3.0/setup.cfg
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6792 2024-03-14 09:55:57.000000 easydock-0.3.0/easydock/preparation_for_docking.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    14345 2024-03-14 09:55:57.000000 easydock-0.3.0/easydock/run_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    19025 2024-03-14 09:55:57.000000 easydock-0.3.0/easydock/database.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-07-31 13:35:52.000000 easydock-0.3.0/easydock/vina_dock_cli.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-07-31 13:35:52.000000 easydock-0.3.0/easydock/read_input.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2024-03-14 10:20:12.000000 easydock-0.3.0/easydock/__init__.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     6864 2024-03-14 09:55:57.000000 easydock-0.3.0/easydock/get_sdf_from_dock_db.py
--rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5684 2024-03-14 09:55:53.000000 easydock-0.3.0/easydock/vina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     3060 2024-03-14 09:55:53.000000 easydock-0.3.0/easydock/gnina_dock.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       91 2023-07-31 13:35:52.000000 easydock-0.3.0/easydock/auxiliary.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    10311 2024-03-14 10:20:12.000000 easydock-0.3.0/README.md
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/
--rw-r--r--   0 pavel     (1000) pavel     (1000)    12886 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/PKG-INFO
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      502 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/SOURCES.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/entry_points.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/top_level.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/requires.txt
--rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-03-14 10:22:38.000000 easydock-0.3.0/easydock.egg-info/dependency_links.txt
-drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-03-14 10:22:38.000000 easydock-0.3.0/tests/
--rw-rw-r--   0 pavel     (1000) pavel     (1000)    15418 2024-02-16 12:01:04.000000 easydock-0.3.0/tests/test_pdbqt.py
--rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-07-31 13:35:52.000000 easydock-0.3.0/setup.py
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-18 19:11:26.000000 easydock-0.3.1/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1516 2023-07-31 13:35:52.000000 easydock-0.3.1/LICENSE.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    15223 2024-04-18 19:11:26.000000 easydock-0.3.1/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       79 2024-04-18 19:11:26.000000 easydock-0.3.1/setup.cfg
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6792 2024-03-14 09:55:57.000000 easydock-0.3.1/easydock/preparation_for_docking.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    14767 2024-04-17 15:42:25.000000 easydock-0.3.1/easydock/run_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    22181 2024-04-18 18:52:16.000000 easydock-0.3.1/easydock/database.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3382 2023-07-31 13:35:52.000000 easydock-0.3.1/easydock/vina_dock_cli.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     7491 2023-07-31 13:35:52.000000 easydock-0.3.1/easydock/read_input.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       22 2024-04-18 19:01:52.000000 easydock-0.3.1/easydock/__init__.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     6685 2024-04-08 08:52:50.000000 easydock-0.3.1/easydock/get_sdf_from_dock_db.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     4801 2024-04-15 12:40:24.000000 easydock-0.3.1/easydock/protonation.py
+-rwxrwxr-x   0 pavel     (1000) pavel     (1000)     5684 2024-03-14 09:55:53.000000 easydock-0.3.1/easydock/vina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     3060 2024-03-14 09:55:53.000000 easydock-0.3.1/easydock/gnina_dock.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      263 2024-03-15 09:20:16.000000 easydock-0.3.1/easydock/auxiliary.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    12448 2024-04-18 19:08:45.000000 easydock-0.3.1/README.md
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/
+-rw-r--r--   0 pavel     (1000) pavel     (1000)    15223 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/PKG-INFO
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      526 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/SOURCES.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)      111 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/entry_points.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        9 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/top_level.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)       24 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/requires.txt
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)        1 2024-04-18 19:11:26.000000 easydock-0.3.1/easydock.egg-info/dependency_links.txt
+drwxrwxr-x   0 pavel     (1000) pavel     (1000)        0 2024-04-18 19:11:26.000000 easydock-0.3.1/tests/
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)    15418 2024-02-16 12:01:04.000000 easydock-0.3.1/tests/test_pdbqt.py
+-rw-rw-r--   0 pavel     (1000) pavel     (1000)     1155 2023-07-31 13:35:52.000000 easydock-0.3.1/setup.py
```

### Comparing `easydock-0.3.0/LICENSE.txt` & `easydock-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/PKG-INFO` & `easydock-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.3.0
+Version: 0.3.1
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # EasyDock - Python module to automate molecular docking
         
@@ -16,53 +16,60 @@
         or the latest version from github
         ```
         pip install git+https://github.com/ci-lab-cz/easydock.git
         ```
         
         ### Dependencies
         
-        from conda
+        - from conda
         ```
         conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
         ```
         
-        from pypi
-        ```
-        pip install meeko
-        ```
+        - from pypi
         
-        to use multiple servers for docking install `paramiko` (backend of `dask` if launched from the command line)
         ```
-        pip install paramiko
+        pip install paramiko meeko vina
         ```
         
-        Installation of `vina`
+        - (optional) installation of `gnina/smina` is described at https://github.com/gnina/gnina
+        
+        - (optional) installation of a `pkasolver` fork to enable protonation with this tool. We recommend to install and use CPU-based version, however, one may try a GPU supported one (look at the dependencies in `pkasolver` package).
         ```
-        pip install vina
+        pip install torch==1.13.1+cpu  --extra-index-url https://download.pytorch.org/whl/cpu
+        pip install torch-geometric==2.0.1
+        pip install torch_scatter==2.1.1+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+        pip install torch_sparse==0.6.17+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+        pip install torch_spline_conv==1.2.2+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+        pip install cairosvg svgutils
+        pip install git+https://github.com/Feriolet/dimorphite_dl.git
+        pip install git+https://github.com/DrrDom/pkasolver.git
         ```
         
-        Installation of `gnina/smina` is described at https://github.com/gnina/gnina
-        
         ### Description
         
-        Fully automatic pipeline for molecular docking.  
+        The fully automatic pipeline for molecular docking.  
         
         Features:
         - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
         - can be used as a command line utility or imported as a python module
+        - input molecules are checked for salts and attempted to fix by SaltRemover 
+        - stereoisomers can be enumerated for unspecified chiral centers and double bonds
+        - several protonation options: chemaxon and pkasolver (check notes below)
         - supports distributed computing using `dask` library
         - supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
         - all outputs are stored in an SQLite database
-        - interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
+        - interrupted calculations can be continued by invoking the same command or by supplying just a single argument - the existing output database
         - `get_sdf_from_dock_db` is used to extract data from output DB
         
         Pipeline:
         - input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
+        - compounds having salts were stripped, if this fails the whole compound will be omitted for docking reporting to STDERR 
         - up to a specified number of stereoisomers are enumerated for molecules with undefined chiral centers or double bond configurations (by default 1 random but reproducible stereoisomer is generated)
-        - ligands are protonated by Chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
+        - ligands are protonated by Chemaxon/pKasolver at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
         - molecules are converted in PDBQT format using Meeko
         - docking with `vina`/`gnina`
         - output poses are converted in MOL format and stored into output DB along with docking scores
         
         ### Example
         
         ##### Docking from command line
@@ -182,16 +189,34 @@
         1. Using `--sdf` option of the main script `run_dock` will return top poses with docking scores. If there were several enumerated stereoisomers, it will return the pose and the score of the best scoring stereoisomer only.
         2. Using `get_sdf_from_dock_db` script. it has a rich set of settings and can return SDF as well as SMILES files. The only restriction it cannot currently return the best pose among enumerated stereoisomers. In this case it is advised to use the previous option and invoke `run_dock -o database.db --sdf` on the database with docked molecules.
         
         ##### Customization
         
         To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and a yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
         
+        ### Notes
+        
+        ##### Protonation notes
+        
+        pkasolver enumerated protonation states and the closest to pH 7.4 is chosen. In some cases it may return invalid SMILES, e.g. `O=C(N1CCN(CC1)C(=O)C=2C=CC=C(C#CC3CC3)C2)C=4NN=C5CCCC45 -> O=C(c1cccc(C#CC2CC2)c1)N1CC[NH](C(=O)c2[nH]nc3c2CCC3)CC1`, which will be skipped and a corresponding warning message will appear.
+        
+        Please note, that protonation states generated with `pkasolver` were not validated. So, check protonation states.
+        
+        ##### Multiple CPUs
+        
+        Please pay attention for `--ncpu` argument if you use `--protonation pkasolver`. For `ncpu` > 1 it may result in some errors. Please report this issue. 
+        
         ### Changelog
         
+        **0.3.1**
+        - add pkasolver as a protonation tool ([@Feriolet](https://github.com/Feriolet)) [#17](https://github.com/ci-lab-cz/easydock/issues/17)
+        - add preparation step which tries to strip salts [#30](https://github.com/ci-lab-cz/easydock/issues/30)
+        - database structure was modified to store input molecules before pre-preocessing [#31](https://github.com/ci-lab-cz/easydock/pull/31)
+        - speed of database initialization was improved [#29](https://github.com/ci-lab-cz/easydock/pull/29)
+        
         **0.3.0**
         - add optional enumeration of stereoisomers. This partially breaks compatibility - docking of molecules in databases which were created by the previous version cannot be continued with this version. Everything else including API is compatible [#21](https://github.com/ci-lab-cz/easydock/pull/21)
         - fix minor errors in retrieving non-top poses by `get_sdf_from_dock_db`
         
         **0.2.9**
         - fix extraction of docking scores for gnina outputs (critial fix) [#23](https://github.com/ci-lab-cz/easydock/pull/23)
         - fix database update freezing upon errors occurred with docking individual docking programs [#22](https://github.com/ci-lab-cz/easydock/issues/22)
```

### Comparing `easydock-0.3.0/easydock/preparation_for_docking.py` & `easydock-0.3.1/easydock/preparation_for_docking.py`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/easydock/run_dock.py` & `easydock-0.3.1/easydock/run_dock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 import os
 import sqlite3
 import sys
+import time
 from functools import partial
 from multiprocessing import Pool
 
 from rdkit import Chem
 from rdkit.Chem.rdMolDescriptors import CalcNumRotatableBonds
 from easydock.database import create_db, restore_setup_from_db, init_db, update_db, save_sdf, select_mols_to_dock, \
     add_protonation
@@ -147,17 +148,16 @@
                              'protein_setup: path to a text file with coordinates of a binding site\n'
                              'exhaustiveness: 8\n'
                              'n_poses: 10\n'
                              'seed: -1\n'
                              'gnina.yml\n')
     parser.add_argument('-s', '--max_stereoisomers', metavar='INTEGER', type=int, required=False, default=1,
                         help='maximum number of isomers to enumerate. The default is set to 1.')
-    parser.add_argument('--no_protonation', action='store_true', default=False,
-                        help='disable protonation of molecules before docking. Protonation requires installed '
-                             'cxcalc chemaxon utility.')
+    parser.add_argument('--protonation', default=None, required=False, choices=['chemaxon', 'pkasolver'],
+                        help='choose a protonation program supported by EasyDock.')
     parser.add_argument('--no_tautomerization', action='store_true', default=False,
                         help='disable tautomerization of molecules during protonation.')
     parser.add_argument('--sdf', action='store_true', default=False,
                         help='save best docked poses to SDF file with the same name as output DB.')
     parser.add_argument('--hostfile', metavar='FILENAME', required=False, type=filepath_type, default=None,
                         help='text file with addresses of nodes of dask SSH cluster. The most typical, it can be '
                              'passed as $PBS_NODEFILE variable from inside a PBS script. The first line in this file '
@@ -189,27 +189,35 @@
 
     tmpfiles = []  # store text files which were saved to the setup table
 
     try:
 
         if not os.path.isfile(args.output):
             create_db(args.output, args)
-            init_db(args.output, args.input, args.max_stereoisomers, args.prefix)
+            start_init = time.time()
+            init_db(args.output, args.input, args.ncpu, args.max_stereoisomers, args.prefix)
+            end_init = time.time()
+            print(f'initializing database done in {(end_init - start_init):.2f}s', flush=True)
         else:
             args_dict, tmpfiles = restore_setup_from_db(args.output)
             # this will ignore stored values of those args which were supplied via command line
             # command line args have precedence over stored ones
             for arg in supplied_args:
                 del args_dict[arg]
             args.__dict__.update(args_dict)
 
         dask_client = create_dask_client(args.hostfile)
 
-        if not args.no_protonation:
-            add_protonation(args.output, not args.no_tautomerization)
+        if args.protonation:
+            start_protonation = time.time()
+            add_protonation(args.output, program=args.protonation, tautomerize=not args.no_tautomerization, ncpu=args.ncpu)
+            end_protonation = time.time()
+            print(f'protonation done in {(end_protonation - start_protonation):.2f}s', flush=True)
+        else:
+            print('protonation skipped')    
 
         if args.program == 'vina':
             from easydock.vina_dock import mol_dock, pred_dock_time
         elif args.program == 'gnina':
             from easydock.gnina_dock import mol_dock
             from easydock.vina_dock import pred_dock_time
         else:
```

### Comparing `easydock-0.3.0/easydock/database.py` & `easydock-0.3.1/easydock/database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 import sqlite3
-import subprocess
 import sys
 import tempfile
 from copy import deepcopy
 from functools import partial
-
+from multiprocessing import Pool
+from typing import Optional, Union
 import yaml
 from easydock import read_input
 from easydock.preparation_for_docking import mol_is_3d
-from easydock.auxiliary import take
+from easydock.auxiliary import take, mol_name_split, empty_func, empty_generator
+from easydock.protonation import protonate_chemaxon, read_protonate_chemaxon, protonate_dimorphite, read_smiles, protonate_pkasolver
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from rdkit.Chem.EnumerateStereoisomers import EnumerateStereoisomers, StereoEnumerationOptions
+from rdkit.Chem.SaltRemover import SaltRemover
 
 
 def create_db(db_fname, args, args_to_save=(), config_args_to_save=('protein', 'protein_setup'), unique_smi=False):
     """
     Create empty database structure and the setup table, which is filled with values. To setup table two fields are
     always stored: yaml file with all input args of the docking script and yaml file with docking config
     :param db_fname: file name of output DB
@@ -31,16 +33,18 @@
     os.makedirs(os.path.dirname(os.path.abspath(db_fname)), exist_ok=True)
     conn = sqlite3.connect(db_fname)
     cur = conn.cursor()
     cur.execute(f"""CREATE TABLE IF NOT EXISTS mols
                 (
                  id TEXT,
                  stereo_id TEXT,
+                 smi_input TEXT,
                  smi TEXT {'UNIQUE' if unique_smi else ''},
                  smi_protonated TEXT,
+                 source_mol_block_input TEXT,
                  source_mol_block TEXT,
                  source_mol_block_protonated TEXT,
                  docking_score REAL,
                  pdb_block TEXT,
                  mol_block TEXT,
                  dock_time REAL,
                  time TEXT,
@@ -150,44 +154,82 @@
         for bond in mol.GetBonds():
             if bond.GetStereo() == Chem.BondStereo.STEREOANY:
                 bond.SetStereo(Chem.BondStereo.STEREONONE)
         isomers = tuple(EnumerateStereoisomers(mol,options=opts))
     return isomers
 
 
-def init_db(db_fname, input_fname, max_stereoisomers=1, prefix=None):
+MolBlock = str
+Smi = str
+def generate_init_data(mol_input: tuple[Chem.Mol, str], max_stereoisomers: int, prefix: str) -> list[list[str, tuple[str, int, Union[Smi, MolBlock], Smi, Optional[MolBlock]]]]:
+    salt_remover = SaltRemover()
+    mol, mol_name = mol_input
+
+    if prefix:
+        mol_name = f'{prefix}-{mol_name}'
+
+    mol_input = mol
+    smi_input = Chem.MolToSmiles(mol, isomericSmiles=True)
+
+    if len(Chem.GetMolFrags(mol, asMols=False, sanitizeFrags=False)) > 1:
+        mol = salt_remover.StripMol(mol, dontRemoveEverything=True)
+        if len(Chem.GetMolFrags(mol, asMols=False, sanitizeFrags=False)) > 1:
+            sys.stderr.write(f'EASYDOCK Warning: molecule {mol.GetProp("_Name")} will be skipped for docking, '
+                             f'because it has multiple components which could not be fixed by SaltRemover\n')
+            if mol_is_3d(mol):
+                return [['mol', (mol_name, None, None, Chem.MolToMolBlock(mol_input), None)]]
+            else:
+                return [['smi', (mol_name, None, smi_input, None)]]
+        sys.stderr.write(f'EASYDOCK Warning: molecule {mol.GetProp("_Name")}, salts were stripped\n')
+        
+    if mol_is_3d(mol):
+        smi = Chem.MolToSmiles(mol, isomericSmiles=True)
+        return [['mol', (mol_name, 0, smi, Chem.MolToMolBlock(mol_input), Chem.MolToMolBlock(mol))]]
+
+    else:
+        isomer_list = []
+        isomers = get_isomers(mol, max_stereoisomers)
+        for stereo_id, stereo_mol in enumerate(isomers):
+            smi = Chem.MolToSmiles(stereo_mol, isomericSmiles=True)
+            isomer_list.append(['smi', (mol_name, stereo_id, smi_input, smi)])
+        return isomer_list
+
 
+def init_db(db_fname: str, input_fname: str, ncpu: int, max_stereoisomers=1, prefix: str=None):
+    Chem.SetDefaultPickleProperties(Chem.PropertyPickleOptions.AllProps)
+
+    pool = Pool(processes=ncpu)
     conn = sqlite3.connect(db_fname)
     cur = conn.cursor()
     data_smi = []  # non 3D structures
     data_mol = []  # 3D structures
-    for mol, mol_name in read_input.read_input(input_fname):
-        if prefix:
-            mol_name = f'{prefix}-{mol_name}'
-        if mol_is_3d(mol):
-            smi = Chem.MolToSmiles(mol, isomericSmiles=True)
-            data_mol.append((mol_name, 0, smi, Chem.MolToMolBlock(mol)))
-        else:
-            isomers = get_isomers(mol, max_stereoisomers)
-            for stereo_id, stereo_mol in enumerate(isomers):
-                smi = Chem.MolToSmiles(stereo_mol, isomericSmiles=True)
-                data_smi.append((mol_name, stereo_id, smi))
-    cur.executemany(f'INSERT INTO mols (id, stereo_id, smi) VALUES(?, ?, ?)', data_smi)
-    cur.executemany(f'INSERT INTO mols (id, stereo_id, smi, source_mol_block) VALUES(?, ?, ?, ?)', data_mol)
+    load_data_params = partial(generate_init_data, max_stereoisomers=max_stereoisomers, prefix=prefix)
+    data_list = pool.map(load_data_params, read_input.read_input(input_fname), chunksize=1)
+
+    for item in data_list:
+        if item is not None:
+            for input_format, data in item:
+                if input_format == 'smi':
+                    data_smi.append(data)
+                elif input_format == 'mol':
+                    data_mol.append(data)
+
+    cur.executemany(f'INSERT INTO mols (id, stereo_id, smi_input, smi) VALUES(?, ?, ?, ?)', data_smi)
+    cur.executemany(f'INSERT INTO mols (id, stereo_id, smi, source_mol_block_input, source_mol_block) VALUES(?, ?, ?, ?, ?)', data_mol)
     conn.commit()
 
 
 def get_protonation_arg_value(db_conn):
     """
-    Returns True if molecules had to be protonated and False otherwise
+    Returns True if molecules have to be protonated and False otherwise
     :param db_conn:
     :return:
     """
     d = yaml.safe_load(db_conn.execute("SELECT yaml FROM setup").fetchone()[0])
-    return not d['no_protonation']
+    return d['protonation'] is not None
 
 
 def update_db(db_conn, mol_id, data, table_name='mols', commit=True):
     """
 
     :param db_conn:
     :param mol_id: is of a molecule to update values
@@ -279,97 +321,109 @@
         else:
             mol = Chem.MolFromMolBlock(mol_block, removeHs=False)
         if mol:
             mol.SetProp('_Name', mol_id + '_' + stereo_id)
             yield mol
 
 
-def add_protonation(db_fname, tautomerize=True, table_name='mols', add_sql=''):
+def add_protonation(db_fname, program='chemaxon', tautomerize=True, table_name='mols', add_sql='', ncpu=1):
     '''
     Protonate SMILES by Chemaxon cxcalc utility to get molecule ionization states at pH 7.4
     :param db_fname:
+    :param program: name of the prorgam to use
     :param tautomerize: get a major tautomer at protonation
     :param table_name: table name with molecules to protonate
     :param add_sql: additional SQL query to be appended to the SQL query to retrieve molecules for protonation,
                     e.g. "AND id IN ('MOL1', 'MOL2')" or "AND iteration=(SELECT MAX(iteration) FROM mols)".
     :return:
     '''
     conn = sqlite3.connect(db_fname)
 
     try:
         cur = conn.cursor()
 
-        sql = f"""SELECT smi, source_mol_block, id, stereo_id 
+        # SMiLES only
+        sql = f"""SELECT smi, id || '_' || stereo_id 
                   FROM {table_name} 
-                  WHERE docking_score is NULL AND smi_protonated is NULL """
+                  WHERE docking_score is NULL AND smi_protonated is NULL AND source_mol_block is NULL """
         sql += add_sql
+        data_list_smi = list(cur.execute(sql))
 
-        data_list = list(cur.execute(sql))
-        if not data_list:
+        # mol_block only
+        sql = f"""SELECT smi, id || '_' || stereo_id 
+                  FROM {table_name} 
+                  WHERE docking_score is NULL AND smi_protonated is NULL AND source_mol_block is NOT NULL """
+        sql += add_sql
+        data_list_mol = list(cur.execute(sql))
+
+        if not data_list_smi and not data_list_mol:
             sys.stderr.write(f'no molecules to protonate\n')
             return
 
-        smi_ids = []
-        mol_ids = []
-        for i, (smi, mol_block, mol_name, stereo_id) in enumerate(data_list):
-            if mol_block is None:
-                smi_ids.append(mol_name)
-                # add missing mol blocks
-                m = Chem.MolFromSmiles(data_list[i][0])
-                m.SetProp('_Name', mol_name)
-                m_block = Chem.MolToMolBlock(m)
-                data_list[i] = (smi, m_block, mol_name, stereo_id)
-            else:
-                mol_ids.append(mol_name)
-        smi_ids = set(smi_ids)
-        mol_ids = set(mol_ids)
+        smi_names = set(mol_name for smi, mol_name in data_list_smi)
+        mol_names = set(mol_name for smi, mol_name in data_list_mol)
 
         output_data_smi = []
         output_data_mol = []
+
         with tempfile.NamedTemporaryFile(suffix='.smi', mode='w', encoding='utf-8') as tmp:
+            for smi, mol_name in data_list_smi + data_list_mol:
+                tmp.write(f'{smi}\t{mol_name}\n')
+            tmp.flush()
+
             fd, output = tempfile.mkstemp()  # use output file to avoid overflow of stdout in extreme cases
+
             try:
-                for smi, _, mol_id, stereo_id in data_list:
-                    tmp.write(f'{smi}\t{mol_id}_{stereo_id}\n')
-                tmp.flush()
-                cmd_run = ['cxcalc', '-S', '--ignore-error', 'majormicrospecies', '-H', '7.4', '-K',
-                           f'{"-M" if tautomerize else ""}', tmp.name]
-                with open(output, 'w') as file:
-                    subprocess.run(cmd_run, stdout=file, text=True)
-
-                for mol in Chem.SDMolSupplier(output, sanitize=False):
-                    if mol:
-                        mol_name, stereo_id = mol.GetProp('_Name').rsplit('_', maxsplit=1)
-                        smi = mol.GetPropsAsDict().get('MAJORMS', None)
-                        if smi is not None:
-                            try:
-                                cansmi = Chem.CanonSmiles(smi)
-                            except:
-                                sys.stderr.write(f'EASYDOCK ERROR: {mol_name}, smiles {smi} obtained after protonation '
-                                                 f'could not be read by RDKit. The molecule was skipped.\n')
-                                continue
-                            if mol_name in smi_ids:
-                                output_data_smi.append((cansmi, mol_name, stereo_id))
-                            elif mol_name in mol_ids:
-                                try:
-                                    # mol block in chemaxon sdf is an input molecule but with 2d structure
-                                    # because input is SMILES
-                                    # to assign proper 3D coordinates we load 3D mol from DB,  make all bonds single,
-                                    # remove Hs and assign bond orders from SMILES
-                                    # this should work even if a generated tautomer differs from the input molecule
-                                    mol3d = get_mols(conn, [mol_name], field_name='source_mol_block')
-                                    mol3d = Chem.RemoveHs(Chem.RWMol(mol3d[0]))
-                                    for b in mol3d.GetBonds():
-                                        b.SetBondType(Chem.BondType.SINGLE)
-                                    ref_mol = Chem.RemoveHs(Chem.MolFromSmiles(smi))
-                                    mol = AllChem.AssignBondOrdersFromTemplate(ref_mol, mol3d)
-                                    Chem.AssignStereochemistryFrom3D(mol)  # not sure whether it is necessary
-                                    output_data_mol.append((cansmi, Chem.MolToMolBlock(mol), mol_name, stereo_id))
-                                except ValueError:
-                                    continue
+
+                if program == 'chemaxon':
+                    protonate_func = partial(protonate_chemaxon, tautomerize=tautomerize)
+                    read_func = read_protonate_chemaxon
+                elif program == 'dimorphite':
+                    protonate_func = partial(protonate_dimorphite, ncpu=ncpu)
+                    read_func = read_smiles
+                elif program == 'pkasolver':
+                    protonate_func = partial(protonate_pkasolver, ncpu=ncpu)
+                    read_func = read_smiles
+                else:
+                    protonate_func = empty_func
+                    read_func = empty_generator
+
+                protonate_func(input_fname=tmp.name, output_fname=output)
+
+                for smi, mol_name in read_func(output):
+
+                    try:
+                        cansmi = Chem.CanonSmiles(smi)
+                    except:
+                        sys.stderr.write(f'EASYDOCK ERROR: {mol_name}, smiles {smi} obtained after protonation '
+                                         f'could not be read by RDKit. The molecule was skipped.\n')
+                        continue
+
+                    mol_id, stereo_id = mol_name_split(mol_name)
+
+                    if mol_name in smi_names:
+                        output_data_smi.append((cansmi, mol_id, stereo_id))
+                    elif mol_name in mol_names:
+                        try:
+                            # mol block in chemaxon sdf is an input molecule but with 2D structure
+                            # because input is SMILES
+                            # to assign proper 3D coordinates we load 3D mol from DB, make all bonds single,
+                            # remove Hs and assign bond orders from SMILES
+                            # this should work even if a generated tautomer differs from the input molecule
+                            mol3d = get_mol(conn, mol_id, stereo_id, field_name='source_mol_block')
+                            mol3d = Chem.RemoveHs(Chem.RWMol(mol3d))
+                            for b in mol3d.GetBonds():
+                                b.SetBondType(Chem.BondType.SINGLE)
+                            ref_mol = Chem.RemoveHs(Chem.MolFromSmiles(cansmi))
+                            mol = AllChem.AssignBondOrdersFromTemplate(ref_mol, mol3d)
+                            Chem.AssignStereochemistryFrom3D(mol)  # not sure whether it is necessary
+                            output_data_mol.append((cansmi, Chem.MolToMolBlock(mol), mol_id, stereo_id))
+                        except ValueError:
+                            continue
+
             finally:
                 os.remove(output)
                 os.close(fd)
 
         cur.executemany(f"""UPDATE {table_name}
                        SET 
                            smi_protonated = ?
@@ -392,15 +446,15 @@
 
 
 def select_from_db(cur, sql, values):
     """
     It makes SELECTs by chunks and works if too many values should be returned from DB.
     Workaround of the limitation of SQLite3 on the number of values in a query (https://www.sqlite.org/limits.html,
     section 9).
-    :param cur: curson or connection to db
+    :param cur: cursor or connection to db
     :param sql: SQL query, where a single question mark identify position where to insert multiple values, e.g.
                 "SELECT smi FROM mols WHERE id IN (?)". This question mark will be replaced with multiple ones.
                 So, only one such a symbol should be present in the query.
     :param values: list of values which will substitute the question mark in the query
     :return: generator over results retrieved from DB
     """
     if sql.count('?') > 1:
@@ -411,17 +465,17 @@
             yield item
 
 
 def get_mols(conn, mol_ids, field_name='mol_block'):
     """
     Returns list of Mol objects from docking DB, order is arbitrary, molecules with errors will be silently skipped
     :param conn: connection to docking DB
-    :param mol_ids: list of molecules to retrieve
+    :param mol_ids: list of molecule ids (ignores stereo_id)
     :param field_name: name of the field from which a molecule should be retrieved
-    :return:
+    :return: list of RDKit Mol objects
     """
     if field_name in ['mol_block', 'source_mol_block']:
         func = partial(Chem.MolFromMolBlock, removeHs=False)
     elif field_name in ['smi']:
         func = Chem.MolFromSmiles
     else:
         raise AttributeError(f'Wrong field name was specified for a get_mols functions. '
@@ -435,7 +489,31 @@
     for items in select_from_db(cur, sql, mol_ids):
         m = func(items[0])
         if m:
             Chem.AssignStereochemistryFrom3D(m)
             mols.append(m)
     cur.close()
     return mols
+
+
+def get_mol(conn, mol_id, stereo_id, field_name='mol_block'):
+    """
+    Returns a single molecule from database
+    :param conn: connection to docking DB
+    :param mol_id: id of a molecule
+    :param stereo_id: stereo_id of a molecule
+    :param field_name: name of the field from which a molecule should be retrieved
+    :return:
+    """
+    if field_name in ['mol_block', 'source_mol_block']:
+        func = partial(Chem.MolFromMolBlock, removeHs=False)
+    elif field_name in ['smi']:
+        func = Chem.MolFromSmiles
+    else:
+        raise AttributeError(f'Wrong field name was specified for a get_mols functions. '
+                             f'Allowed: mol_block, source_mol_block, smi. Supplied: {field_name}')
+
+    cur = conn.cursor()
+    sql = f'SELECT {field_name} FROM mols WHERE id = ? AND stereo_id = ? AND {field_name} IS NOT NULL'
+    res = cur.execute(sql, (mol_id, stereo_id))
+    mol = func(res.fetchone()[0])
+    return mol
```

### Comparing `easydock-0.3.0/easydock/vina_dock_cli.py` & `easydock-0.3.1/easydock/vina_dock_cli.py`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/easydock/read_input.py` & `easydock-0.3.1/easydock/read_input.py`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/easydock/get_sdf_from_dock_db.py` & `easydock-0.3.1/easydock/get_sdf_from_dock_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,15 @@
                         if prop_name != 'pdb_block':
                             f.write(f'>  <{prop_name}>\n')
                             f.write(f'{str(prop_value)}\n\n')
                     f.write('$$$$\n')
                     if poses:
                         poses.remove(1)
                 if poses:
-                    # print(item[1:][args.fields.index('pdb_block')])
-                    # print('=======================================')
-                    pdb_block_list = item[1:][args.fields.index('pdb_block')].split('ENDMDL\n')
-                    # print(pdb_block_list)
+                    pdb_block_list = item[1:][args.fields.index('pdb_block')].strip().split('ENDMDL')
                     mol = Chem.MolFromMolBlock(mol_block)
                     for i in poses:  # 1-based
                         try:
                             pose_mol_block = pdbqt2molblock(pdb_block_list[i-1] + 'ENDMDL\n', mol, mol_id + f'_{i}')
                         except IndexError:
                             sys.stderr.write(f'Pose number {i} is not in the PDB block of {mol_id}. '
                                              f'It will be skipped.\n')
```

### Comparing `easydock-0.3.0/easydock/vina_dock.py` & `easydock-0.3.1/easydock/vina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/easydock/gnina_dock.py` & `easydock-0.3.1/easydock/gnina_dock.py`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/README.md` & `easydock-0.3.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,53 +8,60 @@
 or the latest version from github
 ```
 pip install git+https://github.com/ci-lab-cz/easydock.git
 ```
 
 ### Dependencies
 
-from conda
+- from conda
 ```
 conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
 ```
 
-from pypi
-```
-pip install meeko
-```
+- from pypi
 
-to use multiple servers for docking install `paramiko` (backend of `dask` if launched from the command line)
 ```
-pip install paramiko
+pip install paramiko meeko vina
 ```
 
-Installation of `vina`
+- (optional) installation of `gnina/smina` is described at https://github.com/gnina/gnina
+
+- (optional) installation of a `pkasolver` fork to enable protonation with this tool. We recommend to install and use CPU-based version, however, one may try a GPU supported one (look at the dependencies in `pkasolver` package).
 ```
-pip install vina
+pip install torch==1.13.1+cpu  --extra-index-url https://download.pytorch.org/whl/cpu
+pip install torch-geometric==2.0.1
+pip install torch_scatter==2.1.1+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+pip install torch_sparse==0.6.17+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+pip install torch_spline_conv==1.2.2+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+pip install cairosvg svgutils
+pip install git+https://github.com/Feriolet/dimorphite_dl.git
+pip install git+https://github.com/DrrDom/pkasolver.git
 ```
 
-Installation of `gnina/smina` is described at https://github.com/gnina/gnina
-
 ### Description
 
-Fully automatic pipeline for molecular docking.  
+The fully automatic pipeline for molecular docking.  
 
 Features:
 - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
 - can be used as a command line utility or imported as a python module
+- input molecules are checked for salts and attempted to fix by SaltRemover 
+- stereoisomers can be enumerated for unspecified chiral centers and double bonds
+- several protonation options: chemaxon and pkasolver (check notes below)
 - supports distributed computing using `dask` library
 - supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
 - all outputs are stored in an SQLite database
-- interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
+- interrupted calculations can be continued by invoking the same command or by supplying just a single argument - the existing output database
 - `get_sdf_from_dock_db` is used to extract data from output DB
 
 Pipeline:
 - input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
+- compounds having salts were stripped, if this fails the whole compound will be omitted for docking reporting to STDERR 
 - up to a specified number of stereoisomers are enumerated for molecules with undefined chiral centers or double bond configurations (by default 1 random but reproducible stereoisomer is generated)
-- ligands are protonated by Chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
+- ligands are protonated by Chemaxon/pKasolver at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
 - molecules are converted in PDBQT format using Meeko
 - docking with `vina`/`gnina`
 - output poses are converted in MOL format and stored into output DB along with docking scores
 
 ### Example
 
 ##### Docking from command line
@@ -174,16 +181,34 @@
 1. Using `--sdf` option of the main script `run_dock` will return top poses with docking scores. If there were several enumerated stereoisomers, it will return the pose and the score of the best scoring stereoisomer only.
 2. Using `get_sdf_from_dock_db` script. it has a rich set of settings and can return SDF as well as SMILES files. The only restriction it cannot currently return the best pose among enumerated stereoisomers. In this case it is advised to use the previous option and invoke `run_dock -o database.db --sdf` on the database with docked molecules.
 
 ##### Customization
 
 To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and a yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
 
+### Notes
+
+##### Protonation notes
+
+pkasolver enumerated protonation states and the closest to pH 7.4 is chosen. In some cases it may return invalid SMILES, e.g. `O=C(N1CCN(CC1)C(=O)C=2C=CC=C(C#CC3CC3)C2)C=4NN=C5CCCC45 -> O=C(c1cccc(C#CC2CC2)c1)N1CC[NH](C(=O)c2[nH]nc3c2CCC3)CC1`, which will be skipped and a corresponding warning message will appear.
+
+Please note, that protonation states generated with `pkasolver` were not validated. So, check protonation states.
+
+##### Multiple CPUs
+
+Please pay attention for `--ncpu` argument if you use `--protonation pkasolver`. For `ncpu` > 1 it may result in some errors. Please report this issue. 
+
 ### Changelog
 
+**0.3.1**
+- add pkasolver as a protonation tool ([@Feriolet](https://github.com/Feriolet)) [#17](https://github.com/ci-lab-cz/easydock/issues/17)
+- add preparation step which tries to strip salts [#30](https://github.com/ci-lab-cz/easydock/issues/30)
+- database structure was modified to store input molecules before pre-preocessing [#31](https://github.com/ci-lab-cz/easydock/pull/31)
+- speed of database initialization was improved [#29](https://github.com/ci-lab-cz/easydock/pull/29)
+
 **0.3.0**
 - add optional enumeration of stereoisomers. This partially breaks compatibility - docking of molecules in databases which were created by the previous version cannot be continued with this version. Everything else including API is compatible [#21](https://github.com/ci-lab-cz/easydock/pull/21)
 - fix minor errors in retrieving non-top poses by `get_sdf_from_dock_db`
 
 **0.2.9**
 - fix extraction of docking scores for gnina outputs (critial fix) [#23](https://github.com/ci-lab-cz/easydock/pull/23)
 - fix database update freezing upon errors occurred with docking individual docking programs [#22](https://github.com/ci-lab-cz/easydock/issues/22)
```

### Comparing `easydock-0.3.0/easydock.egg-info/PKG-INFO` & `easydock-0.3.1/easydock.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easydock
-Version: 0.3.0
+Version: 0.3.1
 Summary: EasyDock Python module to facilitate molecular docking
 Home-page: https://github.com/ci-lab-cz/easydock
 Author: Pavel Polishchuk, Guzel Minibaeva, Aleksandra Ivanova
 Author-email: pavel_polishchuk@ukr.net
 License: UNKNOWN
 Description: # EasyDock - Python module to automate molecular docking
         
@@ -16,53 +16,60 @@
         or the latest version from github
         ```
         pip install git+https://github.com/ci-lab-cz/easydock.git
         ```
         
         ### Dependencies
         
-        from conda
+        - from conda
         ```
         conda install -c conda-forge python=3.9 numpy=1.20 rdkit scipy dask distributed
         ```
         
-        from pypi
-        ```
-        pip install meeko
-        ```
+        - from pypi
         
-        to use multiple servers for docking install `paramiko` (backend of `dask` if launched from the command line)
         ```
-        pip install paramiko
+        pip install paramiko meeko vina
         ```
         
-        Installation of `vina`
+        - (optional) installation of `gnina/smina` is described at https://github.com/gnina/gnina
+        
+        - (optional) installation of a `pkasolver` fork to enable protonation with this tool. We recommend to install and use CPU-based version, however, one may try a GPU supported one (look at the dependencies in `pkasolver` package).
         ```
-        pip install vina
+        pip install torch==1.13.1+cpu  --extra-index-url https://download.pytorch.org/whl/cpu
+        pip install torch-geometric==2.0.1
+        pip install torch_scatter==2.1.1+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+        pip install torch_sparse==0.6.17+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+        pip install torch_spline_conv==1.2.2+pt113cpu -f https://data.pyg.org/whl/torch-1.13.1%2Bcpu.html
+        pip install cairosvg svgutils
+        pip install git+https://github.com/Feriolet/dimorphite_dl.git
+        pip install git+https://github.com/DrrDom/pkasolver.git
         ```
         
-        Installation of `gnina/smina` is described at https://github.com/gnina/gnina
-        
         ### Description
         
-        Fully automatic pipeline for molecular docking.  
+        The fully automatic pipeline for molecular docking.  
         
         Features:
         - the major script `run_dock` supports docking with `vina` and `gnina` (`gnina` also supports `smina` and its custom scoring functions)
         - can be used as a command line utility or imported as a python module
+        - input molecules are checked for salts and attempted to fix by SaltRemover 
+        - stereoisomers can be enumerated for unspecified chiral centers and double bonds
+        - several protonation options: chemaxon and pkasolver (check notes below)
         - supports distributed computing using `dask` library
         - supports docking of boron-containing compounds using `vina` and `smina` (boron is replaced with carbon before docking and returned back)
         - all outputs are stored in an SQLite database
-        - interrupted calculations can be restarted by invoking the same command or by supplying just a single argument - the existing output database
+        - interrupted calculations can be continued by invoking the same command or by supplying just a single argument - the existing output database
         - `get_sdf_from_dock_db` is used to extract data from output DB
         
         Pipeline:
         - input SMILES are converted in 3D by RDKit, if input is 3D structures in SDF their conformations wil be taken as starting without changes.
+        - compounds having salts were stripped, if this fails the whole compound will be omitted for docking reporting to STDERR 
         - up to a specified number of stereoisomers are enumerated for molecules with undefined chiral centers or double bond configurations (by default 1 random but reproducible stereoisomer is generated)
-        - ligands are protonated by Chemaxon at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
+        - ligands are protonated by Chemaxon/pKasolver at pH 7.4 and the most stable tautomers are generated (optional, requires a Chemaxon license)
         - molecules are converted in PDBQT format using Meeko
         - docking with `vina`/`gnina`
         - output poses are converted in MOL format and stored into output DB along with docking scores
         
         ### Example
         
         ##### Docking from command line
@@ -182,16 +189,34 @@
         1. Using `--sdf` option of the main script `run_dock` will return top poses with docking scores. If there were several enumerated stereoisomers, it will return the pose and the score of the best scoring stereoisomer only.
         2. Using `get_sdf_from_dock_db` script. it has a rich set of settings and can return SDF as well as SMILES files. The only restriction it cannot currently return the best pose among enumerated stereoisomers. In this case it is advised to use the previous option and invoke `run_dock -o database.db --sdf` on the database with docked molecules.
         
         ##### Customization
         
         To implement support of a custom docking program one should implement a function like `mol_dock` which will take as input an RDKit mol object (named molecule) and a yml-file with all docking parameters. The function should run a command line script/utility and return back a tuple of a molecule name and a dictionary of parameters and their values which should be stored in DB (parameter names should be exactly the same as corresponding field names in DB). For examples, please look at `mol_dock` functions in `vina_dock` or `gnina_dock`.
         
+        ### Notes
+        
+        ##### Protonation notes
+        
+        pkasolver enumerated protonation states and the closest to pH 7.4 is chosen. In some cases it may return invalid SMILES, e.g. `O=C(N1CCN(CC1)C(=O)C=2C=CC=C(C#CC3CC3)C2)C=4NN=C5CCCC45 -> O=C(c1cccc(C#CC2CC2)c1)N1CC[NH](C(=O)c2[nH]nc3c2CCC3)CC1`, which will be skipped and a corresponding warning message will appear.
+        
+        Please note, that protonation states generated with `pkasolver` were not validated. So, check protonation states.
+        
+        ##### Multiple CPUs
+        
+        Please pay attention for `--ncpu` argument if you use `--protonation pkasolver`. For `ncpu` > 1 it may result in some errors. Please report this issue. 
+        
         ### Changelog
         
+        **0.3.1**
+        - add pkasolver as a protonation tool ([@Feriolet](https://github.com/Feriolet)) [#17](https://github.com/ci-lab-cz/easydock/issues/17)
+        - add preparation step which tries to strip salts [#30](https://github.com/ci-lab-cz/easydock/issues/30)
+        - database structure was modified to store input molecules before pre-preocessing [#31](https://github.com/ci-lab-cz/easydock/pull/31)
+        - speed of database initialization was improved [#29](https://github.com/ci-lab-cz/easydock/pull/29)
+        
         **0.3.0**
         - add optional enumeration of stereoisomers. This partially breaks compatibility - docking of molecules in databases which were created by the previous version cannot be continued with this version. Everything else including API is compatible [#21](https://github.com/ci-lab-cz/easydock/pull/21)
         - fix minor errors in retrieving non-top poses by `get_sdf_from_dock_db`
         
         **0.2.9**
         - fix extraction of docking scores for gnina outputs (critial fix) [#23](https://github.com/ci-lab-cz/easydock/pull/23)
         - fix database update freezing upon errors occurred with docking individual docking programs [#22](https://github.com/ci-lab-cz/easydock/issues/22)
```

### Comparing `easydock-0.3.0/tests/test_pdbqt.py` & `easydock-0.3.1/tests/test_pdbqt.py`

 * *Files identical despite different names*

### Comparing `easydock-0.3.0/setup.py` & `easydock-0.3.1/setup.py`

 * *Files identical despite different names*

